# Comparing `tmp/bitsmiths-fura-2.2.2.tar.gz` & `tmp/bitsmiths-fura-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitsmiths-fura-2.2.2.tar", last modified: Wed Sep 28 11:55:23 2022, max compression
+gzip compressed data, was "bitsmiths-fura-2.2.3.tar", last modified: Thu Jul 20 08:03:44 2023, max compression
```

## Comparing `bitsmiths-fura-2.2.2.tar` & `bitsmiths-fura-2.2.3.tar`

### file list

```diff
@@ -1,406 +1,406 @@
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.798199 bitsmiths-fura-2.2.2/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      227 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/.gitignore
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1145 2022-09-28 11:55:18.000000 bitsmiths-fura-2.2.2/LICENCE
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       26 2021-03-23 12:16:22.000000 bitsmiths-fura-2.2.2/MANIFEST.in
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5659 2022-09-28 11:55:23.798199 bitsmiths-fura-2.2.2/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4449 2022-09-28 09:58:23.000000 bitsmiths-fura-2.2.2/README.md
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.674201 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5659 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/PKG-INFO
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    16374 2022-09-28 11:55:23.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/SOURCES.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/dependency_links.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       41 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/entry_points.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        1 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/not-zip-safe
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      131 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/requires.txt
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)        8 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/top_level.txt
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.742200 bitsmiths-fura-2.2.2/bs_fura/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4557 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2174 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/__main__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9127 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/access.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9213 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/access_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5762 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/audit.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.754199 bitsmiths-fura-2.2.2/bs_fura/auth/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2106 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9600 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10057 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3676 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth_password.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3712 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth_password_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3413 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3445 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/auth_token_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4917 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/base_auth.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3128 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/auth/factory.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3166 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/base_access.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3034 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/base_config.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.754199 bitsmiths-fura-2.2.2/bs_fura/braze/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      723 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      817 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/auth_type_couplet.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3379 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/bauth_policy.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3876 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/brole_func_rel.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4427 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/buser_login.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    15558 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_async_server_interface.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    60500 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_async_server_marshaler.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    14796 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_interface.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    31714 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_marshaler.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7874 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_server_impl.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    14875 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_server_interface.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    58931 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/fura_server_marshaler.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      594 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/braze/reset_method_couplet.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4619 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/config.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4694 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/config_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    21097 2022-09-28 09:57:27.000000 bitsmiths-fura-2.2.2/bs_fura/dao.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    23022 2022-09-28 09:57:27.000000 bitsmiths-fura-2.2.2/bs_fura/dao_async.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.754199 bitsmiths-fura-2.2.2/bs_fura/db/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       93 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.670201 bitsmiths-fura-2.2.2/bs_fura/db/dao/
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.770199 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5604 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2295 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3564 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4818 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2202 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3383 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4716 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10013 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1860 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2702 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3725 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3670 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3032 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3676 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2604 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11116 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1963 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1849 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1891 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_incr_usage.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3637 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4286 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3413 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4237 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3598 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10529 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1842 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9891 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1870 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2538 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3632 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3782 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2933 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3583 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2441 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3276 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4045 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4074 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_role_func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4149 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3996 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3175 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10919 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3952 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1954 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2031 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10141 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3954 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2212 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2020 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2327 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3758 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_exists.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2818 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4248 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4802 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4199 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3274 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4232 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4129 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3371 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4183 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3176 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10509 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3988 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10653 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1982 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2059 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2898 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4043 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3966 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3166 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3994 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2802 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1840 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3259 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_id_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3320 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4093 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3412 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4044 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3198 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11072 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4184 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2039 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4247 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2129 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_hist.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3378 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_hist_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3341 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4255 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4206 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6010 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3614 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2371 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3580 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2360 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3243 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2319 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3604 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4822 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    14240 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    12535 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4937 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_by_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1980 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2296 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4221 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5030 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3933 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4981 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4122 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5803 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1945 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2022 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6487 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6068 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10676 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3681 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4519 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3619 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4470 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3581 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5756 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5212 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6019 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9891 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1869 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2537 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3630 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3585 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2932 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3581 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2440 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6374 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_update.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.770199 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)       93 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/__init__.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.782199 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5604 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2386 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3693 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4947 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2287 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3506 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4845 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10365 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1935 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2807 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3842 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3781 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3125 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3787 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2703 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11534 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2038 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1924 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1966 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_incr_usage.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3772 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4403 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3530 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4348 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3727 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10917 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1917 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10231 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1945 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2637 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3749 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3899 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3026 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3694 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2534 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3399 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4162 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4197 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_role_func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4266 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4107 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3292 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11331 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4063 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2029 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2112 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10487 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4071 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2293 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2095 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2414 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3881 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_exists.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2923 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4377 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4925 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4322 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3397 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4355 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4246 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3464 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4300 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3293 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10903 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4099 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11041 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2057 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2140 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3009 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4166 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4083 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3259 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4111 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2907 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1915 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3370 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_id_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3455 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4210 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3505 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4155 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3321 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11484 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4301 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2120 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4364 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2202 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_hist.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3501 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_hist_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3464 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4378 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4323 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6227 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3725 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2458 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3691 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2447 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3360 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2410 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3733 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4951 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    14832 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    13019 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5060 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_by_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2055 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2383 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4368 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5159 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4026 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5104 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4263 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5920 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2020 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2103 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6700 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6191 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11070 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3816 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4642 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3712 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4587 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3710 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5873 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5305 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6136 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10231 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1944 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_delete_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2636 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_insert.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3747 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_lock_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3696 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3025 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_select_all.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3692 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_select_one.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2533 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_update.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6581 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_update.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.790199 bitsmiths-fura-2.2.2/bs_fura/db/tables/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2810 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7100 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ada.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6724 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/aga.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7011 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/config.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4144 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/config_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     8803 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/eatok.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4113 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/eatok_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11468 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/func.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6739 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/func_grp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4151 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/func_grp_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4130 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/func_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4295 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iada_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4295 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iaga_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3468 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iconfig_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3487 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3497 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_incr_usage.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3713 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3774 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_grp_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4094 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_role_func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3753 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3521 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3563 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4127 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4169 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_delete_by_role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3785 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4511 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_exists.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4440 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3834 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3416 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3584 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_cfg_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3855 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_cfg_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3430 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_id_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3808 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3894 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3485 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_sentry_expired.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4295 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iula_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4719 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_auth_by_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3932 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_auth_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3817 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3556 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_delete_by_site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3827 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3474 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_type_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2679 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/oeatok_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2758 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ofunc_role_func_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2749 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/orole_func_rel_exists.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3769 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/orole_func_rel_search.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2724 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/osite_id_by_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9344 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/role.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7577 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/role_func_rel.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5158 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/role_func_rel_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4536 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/role_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     8895 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/site.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     7504 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/site_cfg.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4557 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/site_cfg_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4106 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/site_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     8094 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6135 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/token_hist.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4542 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/token_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6392 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/token_sentry.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4135 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/token_sentry_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10932 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/ula.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    14500 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    10641 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_auth.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5313 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_auth_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4529 2022-09-28 11:55:04.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9532 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_otp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4606 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_otp_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6738 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_type.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     4150 2022-09-28 11:55:05.000000 bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_type_key.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3427 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/err_code.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2431 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/fura_davcache.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5198 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/fura_server.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    38469 2022-09-28 09:57:27.000000 bitsmiths-fura-2.2.2/bs_fura/fura_server_impl.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    41459 2022-09-28 09:57:27.000000 bitsmiths-fura-2.2.2/bs_fura/fura_server_impl_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     3531 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/fura_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     6160 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/jw_token.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9027 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/otp.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     9188 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/otp_async.py
-drwxrwxr-x   0 nicolas   (1000) nicolas   (1000)        0 2022-09-28 11:55:23.798199 bitsmiths-fura-2.2.2/bs_fura/sql/
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2106 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/sql/__init__.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    32543 2022-09-28 11:55:21.000000 bitsmiths-fura-2.2.2/bs_fura/sql/postgresql.sql
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    11127 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/token_manager.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5783 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/token_sentry_pluggin.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    27579 2022-08-11 10:23:32.000000 bitsmiths-fura-2.2.2/bs_fura/user_login.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)    28736 2022-08-11 10:23:32.000000 bitsmiths-fura-2.2.2/bs_fura/user_login_async.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     5067 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/util.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     2820 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/bs_fura/xfura.py
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      106 2021-03-23 12:16:22.000000 bitsmiths-fura-2.2.2/pyproject.toml
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)     1713 2022-09-28 11:55:23.798199 bitsmiths-fura-2.2.2/setup.cfg
--rw-rw-r--   0 nicolas   (1000) nicolas   (1000)      996 2022-05-11 09:08:35.000000 bitsmiths-fura-2.2.2/setup.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.883129 bitsmiths-fura-2.2.3/
+-rw-rw-r--   0 steven     (501) staff       (20)      227 2022-02-25 10:17:23.000000 bitsmiths-fura-2.2.3/.gitignore
+-rw-rw-r--   0 steven     (501) staff       (20)     1145 2023-07-20 08:03:35.000000 bitsmiths-fura-2.2.3/LICENCE
+-rw-rw-r--   0 steven     (501) staff       (20)       26 2022-02-25 10:17:23.000000 bitsmiths-fura-2.2.3/MANIFEST.in
+-rw-r--r--   0 steven     (501) staff       (20)     5572 2023-07-20 08:03:44.883518 bitsmiths-fura-2.2.3/PKG-INFO
+-rw-r--r--   0 steven     (501) staff       (20)     4362 2023-07-20 08:03:04.000000 bitsmiths-fura-2.2.3/README.md
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.101463 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/
+-rw-r--r--   0 steven     (501) staff       (20)     5572 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/PKG-INFO
+-rw-r--r--   0 steven     (501) staff       (20)    16374 2023-07-20 08:03:44.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/SOURCES.txt
+-rw-r--r--   0 steven     (501) staff       (20)        1 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/dependency_links.txt
+-rw-r--r--   0 steven     (501) staff       (20)       41 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/entry_points.txt
+-rw-r--r--   0 steven     (501) staff       (20)        1 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/not-zip-safe
+-rw-r--r--   0 steven     (501) staff       (20)      131 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/requires.txt
+-rw-r--r--   0 steven     (501) staff       (20)        8 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/top_level.txt
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.129002 bitsmiths-fura-2.2.3/bs_fura/
+-rw-rw-r--   0 steven     (501) staff       (20)     4557 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2174 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/__main__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9127 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/access.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9213 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/access_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5762 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/audit.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.136354 bitsmiths-fura-2.2.3/bs_fura/auth/
+-rw-rw-r--   0 steven     (501) staff       (20)     2106 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9600 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10057 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3676 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth_password.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3712 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth_password_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3413 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth_token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3445 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/auth_token_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4917 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/base_auth.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3128 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/auth/factory.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3166 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/base_access.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3034 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/base_config.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.158200 bitsmiths-fura-2.2.3/bs_fura/braze/
+-rw-rw-r--   0 steven     (501) staff       (20)      723 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)      817 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/auth_type_couplet.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3379 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/bauth_policy.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3876 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/brole_func_rel.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4427 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/buser_login.py
+-rw-rw-r--   0 steven     (501) staff       (20)    15558 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_async_server_interface.py
+-rw-rw-r--   0 steven     (501) staff       (20)    60500 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_async_server_marshaler.py
+-rw-rw-r--   0 steven     (501) staff       (20)    14796 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_interface.py
+-rw-rw-r--   0 steven     (501) staff       (20)    31714 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_marshaler.py
+-rw-rw-r--   0 steven     (501) staff       (20)     7874 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_server_impl.py
+-rw-rw-r--   0 steven     (501) staff       (20)    14875 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_server_interface.py
+-rw-rw-r--   0 steven     (501) staff       (20)    58931 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/fura_server_marshaler.py
+-rw-rw-r--   0 steven     (501) staff       (20)      594 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/braze/reset_method_couplet.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4619 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/config.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4694 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/config_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)    21104 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/dao.py
+-rw-rw-r--   0 steven     (501) staff       (20)    23029 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/dao_async.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.159132 bitsmiths-fura-2.2.3/bs_fura/db/
+-rw-rw-r--   0 steven     (501) staff       (20)       93 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/__init__.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.091157 bitsmiths-fura-2.2.3/bs_fura/db/dao/
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.402702 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/
+-rw-rw-r--   0 steven     (501) staff       (20)     5604 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2295 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3564 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4818 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2202 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3383 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4716 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10013 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1860 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2702 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3725 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3670 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3032 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3676 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2604 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11116 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1963 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1849 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1891 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_incr_usage.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3637 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4286 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3413 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4237 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3598 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10529 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1842 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9891 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1870 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2538 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3632 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3782 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2933 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3583 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2441 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3276 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4045 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4074 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_role_func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4149 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3996 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3175 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10919 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3952 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1954 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2031 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10141 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3954 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2212 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2020 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2327 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3758 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_exists.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2818 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4248 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4802 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4199 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3274 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4232 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4129 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3371 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4183 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3176 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10509 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3988 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10653 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1982 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2059 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2898 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4043 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3966 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3166 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3994 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2802 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1840 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3259 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_id_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3320 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4093 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3412 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4044 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3198 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11072 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4184 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2039 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4247 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2129 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_hist.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3378 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_hist_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3341 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4255 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4206 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6010 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3614 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2371 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3580 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2360 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3243 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2319 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3604 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4822 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)    14240 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr.py
+-rw-rw-r--   0 steven     (501) staff       (20)    12535 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4937 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_by_token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1980 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2296 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4221 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5030 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3933 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4981 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4122 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5803 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1945 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2022 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6487 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6068 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10676 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3681 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4519 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3619 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4470 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3581 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5756 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5212 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6019 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9891 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1869 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2537 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3630 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3585 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2932 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3581 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2440 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6374 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_update.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.403761 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/
+-rw-rw-r--   0 steven     (501) staff       (20)       93 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/__init__.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.729691 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/
+-rw-rw-r--   0 steven     (501) staff       (20)     5604 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2386 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3693 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4947 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2287 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3506 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4845 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10365 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1935 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2807 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3842 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3781 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3125 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3787 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2703 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11534 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2038 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1924 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1966 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_incr_usage.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3772 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4403 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3530 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4348 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3727 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10917 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1917 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10231 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1945 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2637 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3749 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3899 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3026 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3694 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2534 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3399 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4162 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4197 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_role_func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4266 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4107 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3292 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11331 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4063 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2029 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2112 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10487 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4071 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2293 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2095 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2414 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3881 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_exists.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2923 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4377 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4925 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4322 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3397 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4355 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4246 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3464 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4300 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3293 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10903 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4099 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11041 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2057 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2140 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3009 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4166 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4083 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3259 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4111 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2907 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1915 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3370 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_id_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3455 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4210 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3505 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4155 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3321 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11484 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4301 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2120 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4364 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2202 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_hist.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3501 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_hist_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3464 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4378 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4323 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6227 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3725 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2458 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3691 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2447 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3360 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2410 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3733 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4951 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)    14832 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr.py
+-rw-rw-r--   0 steven     (501) staff       (20)    13019 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5060 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_by_token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2055 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2383 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4368 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5159 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4026 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5104 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4263 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5920 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2020 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2103 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6700 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6191 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11070 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3816 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4642 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3712 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4587 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3710 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5873 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5305 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6136 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10231 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type.py
+-rw-rw-r--   0 steven     (501) staff       (20)     1944 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_delete_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2636 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_insert.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3747 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_lock_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3696 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3025 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_select_all.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3692 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_select_one.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2533 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_update.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6581 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_update.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.842719 bitsmiths-fura-2.2.3/bs_fura/db/tables/
+-rw-rw-r--   0 steven     (501) staff       (20)     2810 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)     7100 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ada.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6724 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/aga.py
+-rw-rw-r--   0 steven     (501) staff       (20)     7011 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/config.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4144 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/config_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     8803 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/eatok.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4113 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/eatok_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)    11468 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/func.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6739 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/func_grp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4151 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/func_grp_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4130 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/func_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4295 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iada_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4295 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iaga_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3468 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iconfig_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3487 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3497 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_incr_usage.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3713 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3774 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_grp_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4094 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_role_func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3753 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3521 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3563 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4127 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4169 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_delete_by_role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3785 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4511 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_exists.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4440 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3834 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3416 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3584 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_cfg_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3855 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_cfg_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3430 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_id_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3808 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3894 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3485 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_sentry_expired.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4295 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iula_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4719 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_auth_by_token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3932 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_auth_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3817 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3556 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_delete_by_site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3827 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3474 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_type_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2679 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/oeatok_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2758 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ofunc_role_func_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2749 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/orole_func_rel_exists.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3769 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/orole_func_rel_search.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2724 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/osite_id_by_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9344 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/role.py
+-rw-rw-r--   0 steven     (501) staff       (20)     7577 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/role_func_rel.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5158 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/role_func_rel_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4536 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/role_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     8895 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/site.py
+-rw-rw-r--   0 steven     (501) staff       (20)     7504 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/site_cfg.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4557 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/site_cfg_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4106 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/site_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     8094 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6135 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/token_hist.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4542 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/token_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6392 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/token_sentry.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4135 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/token_sentry_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10932 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/ula.py
+-rw-rw-r--   0 steven     (501) staff       (20)    14500 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr.py
+-rw-rw-r--   0 steven     (501) staff       (20)    10641 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_auth.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5313 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_auth_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4529 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9532 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_otp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4606 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_otp_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     6738 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_type.py
+-rw-rw-r--   0 steven     (501) staff       (20)     4150 2023-07-20 07:12:34.000000 bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_type_key.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3427 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/err_code.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2431 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/fura_davcache.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5198 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/fura_server.py
+-rw-rw-r--   0 steven     (501) staff       (20)    38477 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/fura_server_impl.py
+-rw-rw-r--   0 steven     (501) staff       (20)    41466 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/fura_server_impl_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     3531 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/fura_token.py
+-rw-r--r--   0 steven     (501) staff       (20)     6177 2023-07-20 08:03:11.000000 bitsmiths-fura-2.2.3/bs_fura/jw_token.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9027 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/otp.py
+-rw-rw-r--   0 steven     (501) staff       (20)     9188 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/otp_async.py
+drwxr-xr-x   0 steven     (501) staff       (20)        0 2023-07-20 08:03:44.882244 bitsmiths-fura-2.2.3/bs_fura/sql/
+-rw-rw-r--   0 steven     (501) staff       (20)     2106 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/sql/__init__.py
+-rw-rw-r--   0 steven     (501) staff       (20)    35297 2023-07-20 08:03:43.000000 bitsmiths-fura-2.2.3/bs_fura/sql/postgresql.sql
+-rw-rw-r--   0 steven     (501) staff       (20)    11127 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/token_manager.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5783 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/token_sentry_pluggin.py
+-rw-r--r--   0 steven     (501) staff       (20)    27579 2022-09-22 16:55:48.000000 bitsmiths-fura-2.2.3/bs_fura/user_login.py
+-rw-r--r--   0 steven     (501) staff       (20)    28736 2022-09-22 16:55:48.000000 bitsmiths-fura-2.2.3/bs_fura/user_login_async.py
+-rw-rw-r--   0 steven     (501) staff       (20)     5067 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/util.py
+-rw-rw-r--   0 steven     (501) staff       (20)     2820 2022-05-16 10:58:03.000000 bitsmiths-fura-2.2.3/bs_fura/xfura.py
+-rw-rw-r--   0 steven     (501) staff       (20)      106 2022-02-25 10:17:23.000000 bitsmiths-fura-2.2.3/pyproject.toml
+-rw-r--r--   0 steven     (501) staff       (20)     1713 2023-07-20 08:03:44.885349 bitsmiths-fura-2.2.3/setup.cfg
+-rw-rw-r--   0 steven     (501) staff       (20)      996 2022-02-25 10:17:23.000000 bitsmiths-fura-2.2.3/setup.py
```

### Comparing `bitsmiths-fura-2.2.2/LICENCE` & `bitsmiths-fura-2.2.3/LICENCE`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/PKG-INFO` & `bitsmiths-fura-2.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsmiths-fura
-Version: 2.2.2
+Version: 2.2.3
 Summary: The Bitsmiths Function-User-Role-Authenticator Package
 Home-page: https://bitbucket.org/bitsmiths_za/bitsmiths
 Author: Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 Author-email: nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
 License: MIT
 Project-URL: Source, https://bitbucket.org/bitsmiths_za/bitsmiths
 Keywords: libraries
@@ -89,19 +89,19 @@
 
 TODO - Complete this section.
 
 
 ## Change History ##
 
 
-### 2.2.2 ###
+### 2.2.3 ###
 
 | Type | Description |
 | ---- | ----------- |
-| New | Changed the auth lock timeout to be 20 miliseconds at 500 attempts instead of 500 miliseconds at 5 attempts. This should prevent massive user logins from timing out. |
+| New | Upgraded `jwcrypto` to version >= 1.5.0 and catered for their breaking changes |
 
 
 ### 2.2.1 ###
 
 | Type | Description |
 | ---- | ----------- |
 | New | Upgraded to use `bitsmiths-mettle` version 2.2.3 |
```

### Comparing `bitsmiths-fura-2.2.2/README.md` & `bitsmiths-fura-2.2.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,19 +58,19 @@
 
 TODO - Complete this section.
 
 
 ## Change History ##
 
 
-### 2.2.2 ###
+### 2.2.3 ###
 
 | Type | Description |
 | ---- | ----------- |
-| New | Changed the auth lock timeout to be 20 miliseconds at 500 attempts instead of 500 miliseconds at 5 attempts. This should prevent massive user logins from timing out. |
+| New | Upgraded `jwcrypto` to version >= 1.5.0 and catered for their breaking changes |
 
 
 ### 2.2.1 ###
 
 | Type | Description |
 | ---- | ----------- |
 | New | Upgraded to use `bitsmiths-mettle` version 2.2.3 |
```

### Comparing `bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/PKG-INFO` & `bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitsmiths-fura
-Version: 2.2.2
+Version: 2.2.3
 Summary: The Bitsmiths Function-User-Role-Authenticator Package
 Home-page: https://bitbucket.org/bitsmiths_za/bitsmiths
 Author: Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 Author-email: nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
 License: MIT
 Project-URL: Source, https://bitbucket.org/bitsmiths_za/bitsmiths
 Keywords: libraries
@@ -89,19 +89,19 @@
 
 TODO - Complete this section.
 
 
 ## Change History ##
 
 
-### 2.2.2 ###
+### 2.2.3 ###
 
 | Type | Description |
 | ---- | ----------- |
-| New | Changed the auth lock timeout to be 20 miliseconds at 500 attempts instead of 500 miliseconds at 5 attempts. This should prevent massive user logins from timing out. |
+| New | Upgraded `jwcrypto` to version >= 1.5.0 and catered for their breaking changes |
 
 
 ### 2.2.1 ###
 
 | Type | Description |
 | ---- | ----------- |
 | New | Upgraded to use `bitsmiths-mettle` version 2.2.3 |
```

### Comparing `bitsmiths-fura-2.2.2/bitsmiths_fura.egg-info/SOURCES.txt` & `bitsmiths-fura-2.2.3/bitsmiths_fura.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/__main__.py` & `bitsmiths-fura-2.2.3/bs_fura/__main__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/access.py` & `bitsmiths-fura-2.2.3/bs_fura/access.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/access_async.py` & `bitsmiths-fura-2.2.3/bs_fura/access_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/audit.py` & `bitsmiths-fura-2.2.3/bs_fura/audit.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth_async.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth_password.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth_password.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth_password_async.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth_password_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth_token.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth_token.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/auth_token_async.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/auth_token_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/base_auth.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/base_auth.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/auth/factory.py` & `bitsmiths-fura-2.2.3/bs_fura/auth/factory.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/base_access.py` & `bitsmiths-fura-2.2.3/bs_fura/base_access.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/base_config.py` & `bitsmiths-fura-2.2.3/bs_fura/base_config.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 from .auth_type_couplet import AuthType_Couplet
 from .reset_method_couplet import ResetMethod_Couplet
 from .bauth_policy import bAuthPolicy
 from .buser_login import bUserLogin
 from .brole_func_rel import bRoleFuncRel
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/bauth_policy.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/bauth_policy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/brole_func_rel.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/brole_func_rel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/buser_login.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/buser_login.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_async_server_interface.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_async_server_interface.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_async_server_marshaler.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_async_server_marshaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_interface.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_marshaler.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_marshaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_client_server_impl.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_client_server_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_server_interface.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_server_interface.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/fura_server_marshaler.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/fura_server_marshaler.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import dataclasses
 import typing
 import mettle.braze
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/braze/reset_method_couplet.py` & `bitsmiths-fura-2.2.3/bs_fura/braze/reset_method_couplet.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.braze.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 class ResetMethod_Couplet(dict):
 
     key_email = "E"
     key_sms = "S"
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/config.py` & `bitsmiths-fura-2.2.3/bs_fura/config.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/config_async.py` & `bitsmiths-fura-2.2.3/bs_fura/config_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/dao.py` & `bitsmiths-fura-2.2.3/bs_fura/dao.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
 
         :param site_id: The site id.
         :param usr_id: The user id.
         :return: (tUser) The site record, or None if not found.
         """
         u = self.db_dao.dUsr(self.pod.dbcon)
 
-        u.lock_one_deft(site_id, usr_id, self.std_db_lock())
+        u.lock_one_deft(site_id, usr_id, self.pod.std_db_lock())
 
         return u.rec
 
 
     def usr_create(self, audit: BsAudit, rec: tUsr) -> tUsr:
         """
         Create a new user.
@@ -326,15 +326,15 @@
         :param audit: The audit object to use.
         :param rec: The user record to update.
         :param internal: This is an internal safe update.
         :return: The user record updated.
         """
         du = self.db_dao.dUsr(self.pod.dbcon)
 
-        du.lock_one_deft(rec.site_id, rec.id, self.std_db_lock())
+        du.lock_one_deft(rec.site_id, rec.id, self.pod.std_db_lock())
 
         if du.rec.tm_stamp.replace(microsecond=0) != rec.tm_stamp.replace(microsecond=0):
             raise xMettle("Stale data. Please refresh and try again.")
 
         bef = copy.copy(du.rec)
 
         if bef.date_activate and bef.date_activate <= datetime.date.today():
@@ -381,17 +381,17 @@
 
         if not urr.exec_deft(site_id, usr_id).fetch():
             return None
 
         return urr.orec.role_id
 
 
-    def std_db_lock(self, mili_seconds: int = 20, retrys: int = 500) -> mettle.db.DBLock:
+    def std_db_lock(self, mili_seconds: int = 500, retrys: int = 10) -> mettle.db.DBLock:
         """
-        Gets a lock that retries for 10 seconds before raising an exception.
+        Gets a lock that retries for 5 seconds before raising an exception.
 
         :param mili_seconds: Miliseconds between retrys
         :param retrys: Number of retrys
         :return: The db lock record.
         """
         return mettle.db.DBLock(mili_seconds, retrys)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/dao_async.py` & `bitsmiths-fura-2.2.3/bs_fura/dao_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -305,15 +305,15 @@
 
         :param site_id: The site id.
         :param usr_id: The user id.
         :return: (tUser) The site record, or None if not found.
         """
         u = self.db_dao.dUsr(self.pod.dbcon)
 
-        await u.lock_one_deft(site_id, usr_id, self.std_db_lock())
+        await u.lock_one_deft(site_id, usr_id, self.pod.std_db_lock())
 
         return u.rec
 
 
     async def usr_create(self, audit: BsAudit, rec: tUsr) -> tUsr:
         """
         Create a new user.
@@ -341,15 +341,15 @@
         :param audit: The audit object to use.
         :param rec: The user record to update.
         :param internal: This is an internal safe update.
         :return: The user record updated.
         """
         du = self.db_dao.dUsr(self.pod.dbcon)
 
-        await du.lock_one_deft(rec.site_id, rec.id, self.std_db_lock())
+        await du.lock_one_deft(rec.site_id, rec.id, self.pod.std_db_lock())
 
         if du.rec.tm_stamp.replace(microsecond=0) != rec.tm_stamp.replace(microsecond=0):
             raise xMettle("Stale data. Please refresh and try again.")
 
         bef = copy.copy(du.rec)
 
         if bef.date_activate and bef.date_activate <= datetime.date.today():
@@ -396,17 +396,17 @@
 
         if not await (await urr.exec_deft(site_id, usr_id)).fetch():
             return None
 
         return urr.orec.role_id
 
 
-    def std_db_lock(self, mili_seconds: int = 20, retrys: int = 500) -> mettle.db.DBLock:
+    def std_db_lock(self, mili_seconds: int = 500, retrys: int = 10) -> mettle.db.DBLock:
         """
-        Gets a lock that retries for 10 seconds before raising an exception.
+        Gets a lock that retries for 5 seconds before raising an exception.
 
         :param mili_seconds: Miliseconds between retrys
         :param retrys: Number of retrys
         :return: The db lock record.
         """
         return mettle.db.DBLock(mili_seconds, retrys)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 from .ada import dAda
 from .ada_insert import dAdaInsert
 from .ada_search import dAdaSearch
 from .aga import dAga
 from .aga_insert import dAgaInsert
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ada_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ada_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/aga_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/aga_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_select_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_select_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/config_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/config_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_delete_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_incr_usage.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_incr_usage.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_insert.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/eatok_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/eatok_update.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_delete_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_delete_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_lock_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_grp_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_grp_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_role_func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_role_func_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_select_one.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/func_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/func_update.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_delete_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.role_key import tRoleKey
+from bs_fura.db.tables.usr_key import tUsrKey
 
-class dRoleDeleteOne:
+class dUsrDeleteOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tRoleKey()
+        self.irec     = tUsrKey()
 
     def __enter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -38,43 +38,43 @@
     def _destroy(self):
         if self._dbstmnt:
             self._dbstmnt.destroy()
             self._dbstmnt = None
 
     def exec_deft(self,
                   site_id: int,
-                  id: str) -> "dRoleDeleteOne":
+                  id: str) -> "dUsrDeleteOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
 
         return self.exec()
 
-    def exec(self, irec: tRoleKey = None) -> "dRoleDeleteOne":
+    def exec(self, irec: tUsrKey = None) -> "dUsrDeleteOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("RoleDeleteOne", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("UsrDeleteOne", self._dbcon.STMNT_TYPE_CUD)
 
         self._dbstmnt.sql("""delete from
-  fura.Role
+  fura.Usr
 where
   site_id = :site_id and
   id = :id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 128)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_by_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_by_role.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_by_site.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_delete_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_exists.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_exists.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_func_rel_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_func_rel_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_lock_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_search.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
@@ -10,70 +10,70 @@
 
 from bs_fura.db.tables.irole_search import iRoleSearch
 from bs_fura.db.tables.role import tRole
 
 class dRoleSearch:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
-    def __init__(self, dbcon: mettle.db.IConnect):
+    def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
         self.irec     = iRoleSearch()
         self.orec     = None
 
-    def __enter__(self):
+    async def __aenter__(self):
         """
         With statement enter.
         """
         return self
 
-    def __exit__(self, type, value, traceback):
+    async def __aexit__(self, type, value, traceback):
         """
         With statement exit.
         """
-        self._destroy()
+        await self._destroy()
 
-    def _destroy(self):
+    async def _destroy(self):
         if self._dbstmnt:
-            self._dbstmnt.destroy()
+            await self._dbstmnt.destroy()
             self._dbstmnt = None
 
-    def exec_deft(self,
-                  site_id: int,
-                  criteria: str) -> "dRoleSearch":
+    async def exec_deft(self,
+                        site_id: int,
+                        criteria: str) -> "dRoleSearch":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param criteria: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.criteria = criteria
 
-        return self.exec()
+        return await self.exec()
 
-    def exec(self, irec: iRoleSearch = None) -> "dRoleSearch":
+    async def exec(self, irec: iRoleSearch = None) -> "dRoleSearch":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
-        self._destroy()
+        await self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("RoleSearch", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("RoleSearch", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   r.*
 from
   fura.role r
 where
   r.site_id = :siteId
@@ -88,29 +88,29 @@
         self._dbstmnt.bind_out("descr", str, 256)
         self._dbstmnt.bind_out("status", str, 1)
         self._dbstmnt.bind_out("level", int, 4)
         self._dbstmnt.bind_out("sess_timeout", int, 4)
         self._dbstmnt.bind_out("modified_by", str, 128)
         self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
 
-        self._dbcon.execute(self._dbstmnt)
+        await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
 
-    def fetch(self, must_exist: bool = False) -> bool:
+    async def fetch(self, must_exist: bool = False) -> bool:
         """
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
-        if not self._dbcon.fetch(self._dbstmnt):
+        if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
                 raise mettle.lib.xMettle(f"Record not found: [table:Role, proc:Search, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tRole()
 
         self.orec.site_id = self._dbstmnt.result[0]
@@ -120,32 +120,32 @@
         self.orec.level = self._dbstmnt.result[4]
         self.orec.sess_timeout = self._dbstmnt.result[5]
         self.orec.modified_by = self._dbstmnt.result[6]
         self.orec.tm_stamp = self._dbstmnt.result[7]
 
         return True
 
-    def fetch_iter(self) -> tRole:
+    async def fetch_iter(self) -> tRole:
         """
         Yield all the rows one at a time.
 
         :return: Iterator for output rows
         """
-        while self.fetch():
+        while await self.fetch():
             yield self.orec
 
-    def fetch_all(self, out_list: tRole.List, clear_list: bool = True) -> int:
+    async def fetch_all(self, out_list: tRole.List, clear_list: bool = True) -> int:
         """
         Fetch all the rows into the specified list and return the list count.
 
         :param out_list:
         :param clear_list:
         :return: Number of rows fetched.
         """
         if clear_list:
             out_list.clear()
 
-        while self.fetch():
+        while await self.fetch():
             out_list.append(self.orec)
 
         return len(out_list)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/role_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_delete_by_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_delete_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.site_cfg_key import tSiteCfgKey
+from bs_fura.db.tables.token_key import tTokenKey
 
-class dSiteCfgDeleteOne:
+class dTokenDeleteOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tSiteCfgKey()
+        self.irec     = tTokenKey()
 
     def __enter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -38,49 +38,49 @@
     def _destroy(self):
         if self._dbstmnt:
             self._dbstmnt.destroy()
             self._dbstmnt = None
 
     def exec_deft(self,
                   site_id: int,
-                  id: str) -> "dSiteCfgDeleteOne":
+                  id: str) -> "dTokenDeleteOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
 
         return self.exec()
 
-    def exec(self, irec: tSiteCfgKey = None) -> "dSiteCfgDeleteOne":
+    def exec(self, irec: tTokenKey = None) -> "dTokenDeleteOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("SiteCfgDeleteOne", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("TokenDeleteOne", self._dbcon.STMNT_TYPE_CUD)
 
         self._dbstmnt.sql("""delete from
-  fura.SiteCfg
+  fura.Token
 where
   site_id = :site_id and
   id = :id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("id", self.irec.id, str, 256)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 64)
 
         self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_select_all.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_cfg_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_delete_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_id_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_id_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_select_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/site_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/role_delete_one.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.token_key import tTokenKey
+from bs_fura.db.tables.role_key import tRoleKey
 
-class dTokenDeleteOne:
+class dRoleDeleteOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tTokenKey()
+        self.irec     = tRoleKey()
 
     def __enter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -38,49 +38,49 @@
     def _destroy(self):
         if self._dbstmnt:
             self._dbstmnt.destroy()
             self._dbstmnt = None
 
     def exec_deft(self,
                   site_id: int,
-                  id: str) -> "dTokenDeleteOne":
+                  id: str) -> "dRoleDeleteOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
 
         return self.exec()
 
-    def exec(self, irec: tTokenKey = None) -> "dTokenDeleteOne":
+    def exec(self, irec: tRoleKey = None) -> "dRoleDeleteOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("TokenDeleteOne", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("RoleDeleteOne", self._dbcon.STMNT_TYPE_CUD)
 
         self._dbstmnt.sql("""delete from
-  fura.Token
+  fura.Role
 where
   site_id = :site_id and
   id = :id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("id", self.irec.id, str, 64)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
         self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_expired.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_hist.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_hist.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_hist_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.token_hist import tTokenHist
+from bs_fura.db.tables.token import tToken
 
-class dTokenHistInsert:
+class dTokenInsert:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tTokenHist()
+        self.irec     = tToken()
 
     def __enter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -44,15 +44,15 @@
                   site_id: int,
                   id: str,
                   usr_id: str,
                   date_created: datetime.datetime,
                   expires: datetime.datetime,
                   use_cnt: int,
                   aud_id: str,
-                  tm_stamp: datetime.datetime) -> "dTokenHistInsert":
+                  tm_stamp: datetime.datetime) -> "dTokenInsert":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :param usr_id: str
         :param date_created: datetime.datetime
@@ -69,29 +69,29 @@
         self.irec.expires = expires
         self.irec.use_cnt = use_cnt
         self.irec.aud_id = aud_id
         self.irec.tm_stamp = tm_stamp
 
         return self.exec()
 
-    def exec(self, irec: tTokenHist = None) -> "dTokenHistInsert":
+    def exec(self, irec: tToken = None) -> "dTokenInsert":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("TokenHistInsert", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("TokenInsert", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""insert into fura.TokenHist (
+        self._dbstmnt.sql("""insert into fura.Token (
   site_id,
   id,
   usr_id,
   date_created,
   expires,
   use_cnt,
   audId,
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.token import tToken
 
-class dTokenInsert:
+class dTokenUpdate:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
@@ -43,16 +43,15 @@
     def exec_deft(self,
                   site_id: int,
                   id: str,
                   usr_id: str,
                   date_created: datetime.datetime,
                   expires: datetime.datetime,
                   use_cnt: int,
-                  aud_id: str,
-                  tm_stamp: datetime.datetime) -> "dTokenInsert":
+                  aud_id: str) -> "dTokenUpdate":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :param usr_id: str
         :param date_created: datetime.datetime
@@ -65,51 +64,43 @@
         self.irec.site_id = site_id
         self.irec.id = id
         self.irec.usr_id = usr_id
         self.irec.date_created = date_created
         self.irec.expires = expires
         self.irec.use_cnt = use_cnt
         self.irec.aud_id = aud_id
-        self.irec.tm_stamp = tm_stamp
 
         return self.exec()
 
-    def exec(self, irec: tToken = None) -> "dTokenInsert":
+    def exec(self, irec: tToken = None) -> "dTokenUpdate":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("TokenInsert", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("TokenUpdate", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""insert into fura.Token (
-  site_id,
-  id,
-  usr_id,
-  date_created,
-  expires,
-  use_cnt,
-  audId,
-  tmStamp
-) values (
-  :site_id,
-  :id,
-  :usr_id,
-  :date_created,
-  :expires,
-  :use_cnt,
-  :audId,
-  :tmStamp
-)""")
+        self._dbstmnt.sql("""update
+  fura.Token
+set
+  usr_id = :usr_id,
+  date_created = :date_created,
+  expires = :expires,
+  use_cnt = :use_cnt,
+  audId = :audId,
+  tmStamp = :tmStamp
+where
+  site_id = :site_id and
+  id = :id""")
 
         self.irec.tm_stamp = self._dbcon.get_timestamp()
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 64)
         self._dbstmnt.bind_in("usr_id", self.irec.usr_id, str, 128)
         self._dbstmnt.bind_in("date_created", self.irec.date_created, datetime.datetime)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_expired.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_select_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_sentry_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_sentry_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/token_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/token_hist_insert.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.token import tToken
+from bs_fura.db.tables.token_hist import tTokenHist
 
-class dTokenUpdate:
+class dTokenHistInsert:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tToken()
+        self.irec     = tTokenHist()
 
     def __enter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -43,15 +43,16 @@
     def exec_deft(self,
                   site_id: int,
                   id: str,
                   usr_id: str,
                   date_created: datetime.datetime,
                   expires: datetime.datetime,
                   use_cnt: int,
-                  aud_id: str) -> "dTokenUpdate":
+                  aud_id: str,
+                  tm_stamp: datetime.datetime) -> "dTokenHistInsert":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :param usr_id: str
         :param date_created: datetime.datetime
@@ -64,43 +65,51 @@
         self.irec.site_id = site_id
         self.irec.id = id
         self.irec.usr_id = usr_id
         self.irec.date_created = date_created
         self.irec.expires = expires
         self.irec.use_cnt = use_cnt
         self.irec.aud_id = aud_id
+        self.irec.tm_stamp = tm_stamp
 
         return self.exec()
 
-    def exec(self, irec: tToken = None) -> "dTokenUpdate":
+    def exec(self, irec: tTokenHist = None) -> "dTokenHistInsert":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("TokenUpdate", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("TokenHistInsert", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""update
-  fura.Token
-set
-  usr_id = :usr_id,
-  date_created = :date_created,
-  expires = :expires,
-  use_cnt = :use_cnt,
-  audId = :audId,
-  tmStamp = :tmStamp
-where
-  site_id = :site_id and
-  id = :id""")
+        self._dbstmnt.sql("""insert into fura.TokenHist (
+  site_id,
+  id,
+  usr_id,
+  date_created,
+  expires,
+  use_cnt,
+  audId,
+  tmStamp
+) values (
+  :site_id,
+  :id,
+  :usr_id,
+  :date_created,
+  :expires,
+  :use_cnt,
+  :audId,
+  :tmStamp
+)""")
 
         self.irec.tm_stamp = self._dbcon.get_timestamp()
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 64)
         self._dbstmnt.bind_in("usr_id", self.irec.usr_id, str, 128)
         self._dbstmnt.bind_in("date_created", self.irec.date_created, datetime.datetime)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/ula_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/ula_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_by_token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_by_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_delete_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_select_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_auth_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_auth_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_delete_by_site.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_delete_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,87 +1,87 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.usr_key import tUsrKey
 
 class dUsrDeleteOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
-    def __init__(self, dbcon: mettle.db.IConnect):
+    def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
         self.irec     = tUsrKey()
 
-    def __enter__(self):
+    async def __aenter__(self):
         """
         With statement enter.
         """
         return self
 
-    def __exit__(self, type, value, traceback):
+    async def __aexit__(self, type, value, traceback):
         """
         With statement exit.
         """
-        self._destroy()
+        await self._destroy()
 
-    def _destroy(self):
+    async def _destroy(self):
         if self._dbstmnt:
-            self._dbstmnt.destroy()
+            await self._dbstmnt.destroy()
             self._dbstmnt = None
 
-    def exec_deft(self,
-                  site_id: int,
-                  id: str) -> "dUsrDeleteOne":
+    async def exec_deft(self,
+                        site_id: int,
+                        id: str) -> "dUsrDeleteOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
 
-        return self.exec()
+        return await self.exec()
 
-    def exec(self, irec: tUsrKey = None) -> "dUsrDeleteOne":
+    async def exec(self, irec: tUsrKey = None) -> "dUsrDeleteOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
-        self._destroy()
+        await self._destroy()
 
-        self._dbstmnt = self._dbcon.statement("UsrDeleteOne", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = await self._dbcon.statement("UsrDeleteOne", self._dbcon.STMNT_TYPE_CUD)
 
         self._dbstmnt.sql("""delete from
   fura.Usr
 where
   site_id = :site_id and
   id = :id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
-        self._dbcon.execute(self._dbstmnt)
+        await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_select_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_otp_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_otp_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_select_all.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_delete_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_lock_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_select_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_type_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_type_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao/postgresql/usr_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/usr_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 from .ada import dAda
 from .ada_insert import dAdaInsert
 from .ada_search import dAdaSearch
 from .aga import dAga
 from .aga_insert import dAgaInsert
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ada_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ada_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/aga_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/aga_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_delete_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_insert.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/config_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/config_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_delete_by_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_incr_usage.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_incr_usage.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_search.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/eatok_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/eatok_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_delete_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_select_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.func_grp_key import tFuncGrpKey
 from bs_fura.db.tables.func_grp import tFuncGrp
 
-class dFuncGrpLockOne:
+class dFuncGrpSelectOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
@@ -39,58 +39,56 @@
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
-                        id: str) -> "dFuncGrpLockOne":
+                        id: str) -> "dFuncGrpSelectOne":
         """
         Execute the query by setting all the inputs.
 
         :param id: str
         :return: Self for convenience.
         """
         self.irec.id = id
 
         return await self.exec()
 
-    async def exec(self, irec: tFuncGrpKey = None) -> "dFuncGrpLockOne":
+    async def exec(self, irec: tFuncGrpKey = None) -> "dFuncGrpSelectOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("FuncGrpLockOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("FuncGrpSelectOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   id,
   descr,
   modified_by,
   tm_stamp
 from
   fura.FuncGrp
 where
-  id = :id for update nowait""")
+  id = :id""")
 
         self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
         self._dbstmnt.bind_out("id", str, 128)
         self._dbstmnt.bind_out("descr", str, 256)
         self._dbstmnt.bind_out("modified_by", str, 128)
         self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
 
-        await self._dbcon.lock(self._dbstmnt)
-
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
 
@@ -99,15 +97,15 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:FuncGrp, proc:LockOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:FuncGrp, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tFuncGrp()
 
         self.orec.id = self._dbstmnt.result[0]
         self.orec.descr = self._dbstmnt.result[1]
         self.orec.modified_by = self._dbstmnt.result[2]
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_select_all.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_lock_one.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.func_grp_key import tFuncGrpKey
 from bs_fura.db.tables.func_grp import tFuncGrp
 
-class dFuncGrpSelectOne:
+class dFuncGrpLockOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
@@ -39,56 +39,58 @@
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
-                        id: str) -> "dFuncGrpSelectOne":
+                        id: str) -> "dFuncGrpLockOne":
         """
         Execute the query by setting all the inputs.
 
         :param id: str
         :return: Self for convenience.
         """
         self.irec.id = id
 
         return await self.exec()
 
-    async def exec(self, irec: tFuncGrpKey = None) -> "dFuncGrpSelectOne":
+    async def exec(self, irec: tFuncGrpKey = None) -> "dFuncGrpLockOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("FuncGrpSelectOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("FuncGrpLockOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   id,
   descr,
   modified_by,
   tm_stamp
 from
   fura.FuncGrp
 where
-  id = :id""")
+  id = :id for update nowait""")
 
         self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
         self._dbstmnt.bind_out("id", str, 128)
         self._dbstmnt.bind_out("descr", str, 256)
         self._dbstmnt.bind_out("modified_by", str, 128)
         self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
 
+        await self._dbcon.lock(self._dbstmnt)
+
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
 
@@ -97,15 +99,15 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:FuncGrp, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:FuncGrp, proc:LockOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tFuncGrp()
 
         self.orec.id = self._dbstmnt.result[0]
         self.orec.descr = self._dbstmnt.result[1]
         self.orec.modified_by = self._dbstmnt.result[2]
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_grp_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_grp_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_role_func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_role_func_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/func_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/func_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_by_site.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_delete_by_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_delete_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_by_role.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_by_site.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_exists.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_exists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_insert.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_func_rel_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_func_rel_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_select_one.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.irole_search import iRoleSearch
+from bs_fura.db.tables.role_key import tRoleKey
 from bs_fura.db.tables.role import tRole
 
-class dRoleSearch:
+class dRoleSelectOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = iRoleSearch()
+        self.irec     = tRoleKey()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -40,52 +40,58 @@
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
                         site_id: int,
-                        criteria: str) -> "dRoleSearch":
+                        id: str) -> "dRoleSelectOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
-        :param criteria: str
+        :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
-        self.irec.criteria = criteria
+        self.irec.id = id
 
         return await self.exec()
 
-    async def exec(self, irec: iRoleSearch = None) -> "dRoleSearch":
+    async def exec(self, irec: tRoleKey = None) -> "dRoleSelectOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("RoleSearch", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("RoleSelectOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
-  r.*
+  site_id,
+  id,
+  descr,
+  status,
+  level,
+  sess_timeout,
+  modified_by,
+  tm_stamp
 from
-  fura.role r
+  fura.Role
 where
-  r.site_id = :siteId
-  [criteria]""")
+  site_id = :site_id and
+  id = :id""")
 
-        self._dbstmnt.dynamic("[criteria]", self.irec.criteria)
-
-        self._dbstmnt.bind_in("siteId", self.irec.site_id, int, 4)
+        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
         self._dbstmnt.bind_out("site_id", int, 4)
         self._dbstmnt.bind_out("id", str, 128)
         self._dbstmnt.bind_out("descr", str, 256)
         self._dbstmnt.bind_out("status", str, 1)
         self._dbstmnt.bind_out("level", int, 4)
         self._dbstmnt.bind_out("sess_timeout", int, 4)
@@ -104,15 +110,15 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Role, proc:Search, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Role, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tRole()
 
         self.orec.site_id = self._dbstmnt.result[0]
         self.orec.id = self._dbstmnt.result[1]
         self.orec.descr = self._dbstmnt.result[2]
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_select_all.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_by_code.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.role_key import tRoleKey
-from bs_fura.db.tables.role import tRole
+from bs_fura.db.tables.isite_by_code import iSiteByCode
+from bs_fura.db.tables.site import tSite
 
-class dRoleSelectOne:
+class dSiteByCode:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tRoleKey()
+        self.irec     = iSiteByCode()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -39,66 +39,55 @@
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
-                        site_id: int,
-                        id: str) -> "dRoleSelectOne":
+                        code: str) -> "dSiteByCode":
         """
         Execute the query by setting all the inputs.
 
-        :param site_id: int
-        :param id: str
+        :param code: str
         :return: Self for convenience.
         """
-        self.irec.site_id = site_id
-        self.irec.id = id
+        self.irec.code = code
 
         return await self.exec()
 
-    async def exec(self, irec: tRoleKey = None) -> "dRoleSelectOne":
+    async def exec(self, irec: iSiteByCode = None) -> "dSiteByCode":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("RoleSelectOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("SiteByCode", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
-  site_id,
-  id,
-  descr,
-  status,
-  level,
-  sess_timeout,
-  modified_by,
-  tm_stamp
+  s.*
 from
-  fura.Role
+  fura.site s
 where
-  site_id = :site_id and
-  id = :id""")
+  s.code = :code""")
 
-        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("id", self.irec.id, str, 128)
+        self._dbstmnt.bind_in("code", self.irec.code, str)
 
-        self._dbstmnt.bind_out("site_id", int, 4)
-        self._dbstmnt.bind_out("id", str, 128)
+        self._dbstmnt.bind_out("id", int, 4)
+        self._dbstmnt.bind_out("code", str, 32)
         self._dbstmnt.bind_out("descr", str, 256)
         self._dbstmnt.bind_out("status", str, 1)
-        self._dbstmnt.bind_out("level", int, 4)
-        self._dbstmnt.bind_out("sess_timeout", int, 4)
+        self._dbstmnt.bind_out("cc", str, 2)
+        self._dbstmnt.bind_out("ccy", str, 3)
+        self._dbstmnt.bind_out("dc", str, 3)
         self._dbstmnt.bind_out("modified_by", str, 128)
         self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
 
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
@@ -110,40 +99,41 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Role, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Site, proc:ByCode, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
-        self.orec = tRole()
+        self.orec = tSite()
 
-        self.orec.site_id = self._dbstmnt.result[0]
-        self.orec.id = self._dbstmnt.result[1]
+        self.orec.id = self._dbstmnt.result[0]
+        self.orec.code = self._dbstmnt.result[1]
         self.orec.descr = self._dbstmnt.result[2]
         self.orec.status = self._dbstmnt.result[3]
-        self.orec.level = self._dbstmnt.result[4]
-        self.orec.sess_timeout = self._dbstmnt.result[5]
-        self.orec.modified_by = self._dbstmnt.result[6]
-        self.orec.tm_stamp = self._dbstmnt.result[7]
+        self.orec.cc = self._dbstmnt.result[4]
+        self.orec.ccy = self._dbstmnt.result[5]
+        self.orec.dc = self._dbstmnt.result[6]
+        self.orec.modified_by = self._dbstmnt.result[7]
+        self.orec.tm_stamp = self._dbstmnt.result[8]
 
         return True
 
-    async def fetch_iter(self) -> tRole:
+    async def fetch_iter(self) -> tSite:
         """
         Yield all the rows one at a time.
 
         :return: Iterator for output rows
         """
         while await self.fetch():
             yield self.orec
 
-    async def fetch_all(self, out_list: tRole.List, clear_list: bool = True) -> int:
+    async def fetch_all(self, out_list: tSite.List, clear_list: bool = True) -> int:
         """
         Fetch all the rows into the specified list and return the list count.
 
         :param out_list:
         :param clear_list:
         :return: Number of rows fetched.
         """
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/role_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/role_update.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_lock_one.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.isite_by_code import iSiteByCode
-from bs_fura.db.tables.site import tSite
+from bs_fura.db.tables.token_key import tTokenKey
+from bs_fura.db.tables.token import tToken
 
-class dSiteByCode:
+class dTokenLockOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = iSiteByCode()
+        self.irec     = tTokenKey()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -39,57 +39,70 @@
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
-                        code: str) -> "dSiteByCode":
+                        site_id: int,
+                        id: str) -> "dTokenLockOne":
         """
         Execute the query by setting all the inputs.
 
-        :param code: str
+        :param site_id: int
+        :param id: str
         :return: Self for convenience.
         """
-        self.irec.code = code
+        self.irec.site_id = site_id
+        self.irec.id = id
 
         return await self.exec()
 
-    async def exec(self, irec: iSiteByCode = None) -> "dSiteByCode":
+    async def exec(self, irec: tTokenKey = None) -> "dTokenLockOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("SiteByCode", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("TokenLockOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
-  s.*
+  site_id,
+  id,
+  usr_id,
+  date_created,
+  expires,
+  use_cnt,
+  audId,
+  tmStamp
 from
-  fura.site s
+  fura.Token
 where
-  s.code = :code""")
+  site_id = :site_id and
+  id = :id for update nowait""")
 
-        self._dbstmnt.bind_in("code", self.irec.code, str)
+        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 64)
 
-        self._dbstmnt.bind_out("id", int, 4)
-        self._dbstmnt.bind_out("code", str, 32)
-        self._dbstmnt.bind_out("descr", str, 256)
-        self._dbstmnt.bind_out("status", str, 1)
-        self._dbstmnt.bind_out("cc", str, 2)
-        self._dbstmnt.bind_out("ccy", str, 3)
-        self._dbstmnt.bind_out("dc", str, 3)
-        self._dbstmnt.bind_out("modified_by", str, 128)
-        self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
+        self._dbstmnt.bind_out("site_id", int, 4)
+        self._dbstmnt.bind_out("id", str, 64)
+        self._dbstmnt.bind_out("usr_id", str, 128)
+        self._dbstmnt.bind_out("date_created", datetime.datetime)
+        self._dbstmnt.bind_out("expires", datetime.datetime)
+        self._dbstmnt.bind_out("use_cnt", int, 4)
+        self._dbstmnt.bind_out("audId", str)
+        self._dbstmnt.bind_out("tmStamp", datetime.datetime)
+
+        await self._dbcon.lock(self._dbstmnt)
 
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
@@ -99,41 +112,40 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Site, proc:ByCode, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Token, proc:LockOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
-        self.orec = tSite()
+        self.orec = tToken()
 
-        self.orec.id = self._dbstmnt.result[0]
-        self.orec.code = self._dbstmnt.result[1]
-        self.orec.descr = self._dbstmnt.result[2]
-        self.orec.status = self._dbstmnt.result[3]
-        self.orec.cc = self._dbstmnt.result[4]
-        self.orec.ccy = self._dbstmnt.result[5]
-        self.orec.dc = self._dbstmnt.result[6]
-        self.orec.modified_by = self._dbstmnt.result[7]
-        self.orec.tm_stamp = self._dbstmnt.result[8]
+        self.orec.site_id = self._dbstmnt.result[0]
+        self.orec.id = self._dbstmnt.result[1]
+        self.orec.usr_id = self._dbstmnt.result[2]
+        self.orec.date_created = self._dbstmnt.result[3]
+        self.orec.expires = self._dbstmnt.result[4]
+        self.orec.use_cnt = self._dbstmnt.result[5]
+        self.orec.aud_id = self._dbstmnt.result[6]
+        self.orec.tm_stamp = self._dbstmnt.result[7]
 
         return True
 
-    async def fetch_iter(self) -> tSite:
+    async def fetch_iter(self) -> tToken:
         """
         Yield all the rows one at a time.
 
         :return: Iterator for output rows
         """
         while await self.fetch():
             yield self.orec
 
-    async def fetch_all(self, out_list: tSite.List, clear_list: bool = True) -> int:
+    async def fetch_all(self, out_list: tToken.List, clear_list: bool = True) -> int:
         """
         Fetch all the rows into the specified list and return the list count.
 
         :param out_list:
         :param clear_list:
         :return: Number of rows fetched.
         """
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_delete_by_site.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_cfg_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_cfg_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_delete_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_id_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_id_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/site_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/site_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_delete_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_expired.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_hist.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_hist.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_hist_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_hist_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_select_one.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.token_key import tTokenKey
 from bs_fura.db.tables.token import tToken
 
-class dTokenLockOne:
+class dTokenSelectOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
@@ -40,70 +40,68 @@
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
                         site_id: int,
-                        id: str) -> "dTokenLockOne":
+                        id: str) -> "dTokenSelectOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
 
         return await self.exec()
 
-    async def exec(self, irec: tTokenKey = None) -> "dTokenLockOne":
+    async def exec(self, irec: tTokenKey = None) -> "dTokenSelectOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("TokenLockOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("TokenSelectOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   site_id,
   id,
   usr_id,
   date_created,
   expires,
   use_cnt,
   audId,
   tmStamp
 from
   fura.Token
 where
   site_id = :site_id and
-  id = :id for update nowait""")
+  id = :id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 64)
 
         self._dbstmnt.bind_out("site_id", int, 4)
         self._dbstmnt.bind_out("id", str, 64)
         self._dbstmnt.bind_out("usr_id", str, 128)
         self._dbstmnt.bind_out("date_created", datetime.datetime)
         self._dbstmnt.bind_out("expires", datetime.datetime)
         self._dbstmnt.bind_out("use_cnt", int, 4)
         self._dbstmnt.bind_out("audId", str)
         self._dbstmnt.bind_out("tmStamp", datetime.datetime)
 
-        await self._dbcon.lock(self._dbstmnt)
-
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
 
@@ -112,15 +110,15 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Token, proc:LockOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Token, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tToken()
 
         self.orec.site_id = self._dbstmnt.result[0]
         self.orec.id = self._dbstmnt.result[1]
         self.orec.usr_id = self._dbstmnt.result[2]
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_select_one.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.token_key import tTokenKey
-from bs_fura.db.tables.token import tToken
+from bs_fura.db.tables.usr_otp_key import tUsrOtpKey
+from bs_fura.db.tables.usr_otp import tUsrOtp
 
-class dTokenSelectOne:
+class dUsrOtpSelectOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tTokenKey()
+        self.irec     = tUsrOtpKey()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -40,67 +40,71 @@
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
                         site_id: int,
-                        id: str) -> "dTokenSelectOne":
+                        usr_id: str) -> "dUsrOtpSelectOne":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
-        :param id: str
+        :param usr_id: str
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
-        self.irec.id = id
+        self.irec.usr_id = usr_id
 
         return await self.exec()
 
-    async def exec(self, irec: tTokenKey = None) -> "dTokenSelectOne":
+    async def exec(self, irec: tUsrOtpKey = None) -> "dUsrOtpSelectOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("TokenSelectOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("UsrOtpSelectOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   site_id,
-  id,
   usr_id,
-  date_created,
-  expires,
-  use_cnt,
-  audId,
-  tmStamp
+  otp_method,
+  otp,
+  expire,
+  used,
+  target,
+  fail_cnt,
+  meta_data,
+  tm_stamp
 from
-  fura.Token
+  fura.UsrOtp
 where
   site_id = :site_id and
-  id = :id""")
+  usr_id = :usr_id""")
 
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("id", self.irec.id, str, 64)
+        self._dbstmnt.bind_in("usr_id", self.irec.usr_id, str, 128)
 
         self._dbstmnt.bind_out("site_id", int, 4)
-        self._dbstmnt.bind_out("id", str, 64)
         self._dbstmnt.bind_out("usr_id", str, 128)
-        self._dbstmnt.bind_out("date_created", datetime.datetime)
-        self._dbstmnt.bind_out("expires", datetime.datetime)
-        self._dbstmnt.bind_out("use_cnt", int, 4)
-        self._dbstmnt.bind_out("audId", str)
-        self._dbstmnt.bind_out("tmStamp", datetime.datetime)
+        self._dbstmnt.bind_out("otp_method", str, 1)
+        self._dbstmnt.bind_out("otp", str, 128)
+        self._dbstmnt.bind_out("expire", datetime.datetime)
+        self._dbstmnt.bind_out("used", bool)
+        self._dbstmnt.bind_out("target", str, 64)
+        self._dbstmnt.bind_out("fail_cnt", int, 4)
+        self._dbstmnt.bind_out("meta_data", dict)
+        self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
 
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
@@ -110,40 +114,42 @@
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Token, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:UsrOtp, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
-        self.orec = tToken()
+        self.orec = tUsrOtp()
 
         self.orec.site_id = self._dbstmnt.result[0]
-        self.orec.id = self._dbstmnt.result[1]
-        self.orec.usr_id = self._dbstmnt.result[2]
-        self.orec.date_created = self._dbstmnt.result[3]
-        self.orec.expires = self._dbstmnt.result[4]
-        self.orec.use_cnt = self._dbstmnt.result[5]
-        self.orec.aud_id = self._dbstmnt.result[6]
-        self.orec.tm_stamp = self._dbstmnt.result[7]
+        self.orec.usr_id = self._dbstmnt.result[1]
+        self.orec.otp_method = self._dbstmnt.result[2]
+        self.orec.otp = self._dbstmnt.result[3]
+        self.orec.expire = self._dbstmnt.result[4]
+        self.orec.used = self._dbstmnt.result[5]
+        self.orec.target = self._dbstmnt.result[6]
+        self.orec.fail_cnt = self._dbstmnt.result[7]
+        self.orec.meta_data = self._dbstmnt.result[8]
+        self.orec.tm_stamp = self._dbstmnt.result[9]
 
         return True
 
-    async def fetch_iter(self) -> tToken:
+    async def fetch_iter(self) -> tUsrOtp:
         """
         Yield all the rows one at a time.
 
         :return: Iterator for output rows
         """
         while await self.fetch():
             yield self.orec
 
-    async def fetch_all(self, out_list: tToken.List, clear_list: bool = True) -> int:
+    async def fetch_all(self, out_list: tUsrOtp.List, clear_list: bool = True) -> int:
         """
         Fetch all the rows into the specified list and return the list count.
 
         :param out_list:
         :param clear_list:
         :return: Number of rows fetched.
         """
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_expired.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_select_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_sentry_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_sentry_update.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/token_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/token_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula_insert.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/ula_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/ula_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_by_token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_by_token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_delete_by_site.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_delete_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_lock_one.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_select_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_auth_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_auth_update.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_delete_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_insert.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.usr_key import tUsrKey
+from bs_fura.db.tables.usr_type import tUsrType
 
-class dUsrDeleteOne:
+class dUsrTypeInsert:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tUsrKey()
+        self.irec     = tUsrType()
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -37,50 +37,66 @@
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
-                        site_id: int,
-                        id: str) -> "dUsrDeleteOne":
+                        id: str,
+                        descr: str,
+                        modified_by: str,
+                        tm_stamp: datetime.datetime) -> "dUsrTypeInsert":
         """
         Execute the query by setting all the inputs.
 
-        :param site_id: int
         :param id: str
+        :param descr: str
+        :param modified_by: str
+        :param tm_stamp: datetime.datetime
         :return: Self for convenience.
         """
-        self.irec.site_id = site_id
         self.irec.id = id
+        self.irec.descr = descr
+        self.irec.modified_by = modified_by
+        self.irec.tm_stamp = tm_stamp
 
         return await self.exec()
 
-    async def exec(self, irec: tUsrKey = None) -> "dUsrDeleteOne":
+    async def exec(self, irec: tUsrType = None) -> "dUsrTypeInsert":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrDeleteOne", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = await self._dbcon.statement("UsrTypeInsert", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""delete from
-  fura.Usr
-where
-  site_id = :site_id and
-  id = :id""")
-
-        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("id", self.irec.id, str, 128)
+        self._dbstmnt.sql("""insert into fura.UsrType (
+  id,
+  descr,
+  modified_by,
+  tm_stamp
+) values (
+  :id,
+  :descr,
+  :modified_by,
+  :tm_stamp
+)""")
+
+        self.irec.tm_stamp = await self._dbcon.get_timestamp()
+
+        self._dbstmnt.bind_in("id", self.irec.id, str, 32)
+        self._dbstmnt.bind_in("descr", self.irec.descr, str, 128)
+        self._dbstmnt.bind_in("modified_by", self.irec.modified_by, str, 128)
+        self._dbstmnt.bind_in("tm_stamp", self.irec.tm_stamp, datetime.datetime)
 
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_lock_one.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_insert.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_select_all.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_select_all.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,30 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.usr_otp_key import tUsrOtpKey
-from bs_fura.db.tables.usr_otp import tUsrOtp
+from bs_fura.db.tables.usr import tUsr
 
-class dUsrOtpSelectOne:
-    __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
+class dUsrSelectAll:
+    __slots__ = ("_dbcon", "_dbstmnt", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tUsrOtpKey()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -38,118 +36,132 @@
         await self._destroy()
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
-    async def exec_deft(self,
-                        site_id: int,
-                        usr_id: str) -> "dUsrOtpSelectOne":
+    async def exec(self) -> "dUsrSelectAll":
         """
-        Execute the query by setting all the inputs.
+        Execute the query.
 
-        :param site_id: int
-        :param usr_id: str
         :return: Self for convenience.
         """
-        self.irec.site_id = site_id
-        self.irec.usr_id = usr_id
-
-        return await self.exec()
-
-    async def exec(self, irec: tUsrOtpKey = None) -> "dUsrOtpSelectOne":
-        """
-        Execute the query, optionally passing in the input rec.
-
-        :param irec:
-        :return: Self for convenience.
-        """
-        if irec:
-            self.irec._copy_from(irec)
-
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrOtpSelectOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("UsrSelectAll", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   site_id,
-  usr_id,
-  otp_method,
-  otp,
-  expire,
-  used,
-  target,
-  fail_cnt,
-  meta_data,
-  tm_stamp
+  id,
+  role_id,
+  status,
+  name_first,
+  name_last,
+  title,
+  date_activate,
+  date_expire,
+  email1,
+  email2,
+  cellno1,
+  cellno2,
+  modified_by,
+  tm_stamp,
+  usrtype_id,
+  email1_conf,
+  email2_conf,
+  cellno1_conf,
+  cellno2_conf,
+  opt_system,
+  opt_market,
+  opt_fail_login
 from
-  fura.UsrOtp
-where
-  site_id = :site_id and
-  usr_id = :usr_id""")
-
-        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
-        self._dbstmnt.bind_in("usr_id", self.irec.usr_id, str, 128)
+  fura.Usr
+order by
+  site_id,
+  id""")
 
         self._dbstmnt.bind_out("site_id", int, 4)
-        self._dbstmnt.bind_out("usr_id", str, 128)
-        self._dbstmnt.bind_out("otp_method", str, 1)
-        self._dbstmnt.bind_out("otp", str, 128)
-        self._dbstmnt.bind_out("expire", datetime.datetime)
-        self._dbstmnt.bind_out("used", bool)
-        self._dbstmnt.bind_out("target", str, 64)
-        self._dbstmnt.bind_out("fail_cnt", int, 4)
-        self._dbstmnt.bind_out("meta_data", dict)
+        self._dbstmnt.bind_out("id", str, 128)
+        self._dbstmnt.bind_out("role_id", str, 128)
+        self._dbstmnt.bind_out("status", str, 1)
+        self._dbstmnt.bind_out("name_first", str, 128)
+        self._dbstmnt.bind_out("name_last", str, 128)
+        self._dbstmnt.bind_out("title", str, 5)
+        self._dbstmnt.bind_out("date_activate", datetime.date)
+        self._dbstmnt.bind_out("date_expire", datetime.date)
+        self._dbstmnt.bind_out("email1", str, 256)
+        self._dbstmnt.bind_out("email2", str, 256)
+        self._dbstmnt.bind_out("cellno1", str, 32)
+        self._dbstmnt.bind_out("cellno2", str, 32)
+        self._dbstmnt.bind_out("modified_by", str, 128)
         self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
+        self._dbstmnt.bind_out("usrtype_id", str, 32)
+        self._dbstmnt.bind_out("email1_conf", bool)
+        self._dbstmnt.bind_out("email2_conf", bool)
+        self._dbstmnt.bind_out("cellno1_conf", bool)
+        self._dbstmnt.bind_out("cellno2_conf", bool)
+        self._dbstmnt.bind_out("opt_system", bool)
+        self._dbstmnt.bind_out("opt_market", bool)
+        self._dbstmnt.bind_out("opt_fail_login", bool)
 
         await self._dbcon.execute(self._dbstmnt)
 
-        if irec:
-            irec._copy_from(self.irec)
-
         return self
 
     async def fetch(self, must_exist: bool = False) -> bool:
         """
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:UsrOtp, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Usr, proc:SelectAll]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
-        self.orec = tUsrOtp()
+        self.orec = tUsr()
 
         self.orec.site_id = self._dbstmnt.result[0]
-        self.orec.usr_id = self._dbstmnt.result[1]
-        self.orec.otp_method = self._dbstmnt.result[2]
-        self.orec.otp = self._dbstmnt.result[3]
-        self.orec.expire = self._dbstmnt.result[4]
-        self.orec.used = self._dbstmnt.result[5]
-        self.orec.target = self._dbstmnt.result[6]
-        self.orec.fail_cnt = self._dbstmnt.result[7]
-        self.orec.meta_data = self._dbstmnt.result[8]
-        self.orec.tm_stamp = self._dbstmnt.result[9]
+        self.orec.id = self._dbstmnt.result[1]
+        self.orec.role_id = self._dbstmnt.result[2]
+        self.orec.status = self._dbstmnt.result[3]
+        self.orec.name_first = self._dbstmnt.result[4]
+        self.orec.name_last = self._dbstmnt.result[5]
+        self.orec.title = self._dbstmnt.result[6]
+        self.orec.date_activate = self._dbstmnt.result[7]
+        self.orec.date_expire = self._dbstmnt.result[8]
+        self.orec.email1 = self._dbstmnt.result[9]
+        self.orec.email2 = self._dbstmnt.result[10]
+        self.orec.cellno1 = self._dbstmnt.result[11]
+        self.orec.cellno2 = self._dbstmnt.result[12]
+        self.orec.modified_by = self._dbstmnt.result[13]
+        self.orec.tm_stamp = self._dbstmnt.result[14]
+        self.orec.usrtype_id = self._dbstmnt.result[15]
+        self.orec.email1_conf = self._dbstmnt.result[16]
+        self.orec.email2_conf = self._dbstmnt.result[17]
+        self.orec.cellno1_conf = self._dbstmnt.result[18]
+        self.orec.cellno2_conf = self._dbstmnt.result[19]
+        self.orec.opt_system = self._dbstmnt.result[20]
+        self.orec.opt_market = self._dbstmnt.result[21]
+        self.orec.opt_fail_login = self._dbstmnt.result[22]
 
         return True
 
-    async def fetch_iter(self) -> tUsrOtp:
+    async def fetch_iter(self) -> tUsr:
         """
         Yield all the rows one at a time.
 
         :return: Iterator for output rows
         """
         while await self.fetch():
             yield self.orec
 
-    async def fetch_all(self, out_list: tUsrOtp.List, clear_list: bool = True) -> int:
+    async def fetch_all(self, out_list: tUsr.List, clear_list: bool = True) -> int:
         """
         Fetch all the rows into the specified list and return the list count.
 
         :param out_list:
         :param clear_list:
         :return: Number of rows fetched.
         """
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_otp_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_otp_update.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_select_one.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,32 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
+from bs_fura.db.tables.usr_key import tUsrKey
 from bs_fura.db.tables.usr import tUsr
 
-class dUsrSelectAll:
-    __slots__ = ("_dbcon", "_dbstmnt", "orec")
+class dUsrSelectOne:
+    __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
+        self.irec     = tUsrKey()
         self.orec     = None
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
@@ -36,23 +38,42 @@
         await self._destroy()
 
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
-    async def exec(self) -> "dUsrSelectAll":
+    async def exec_deft(self,
+                        site_id: int,
+                        id: str) -> "dUsrSelectOne":
         """
-        Execute the query.
+        Execute the query by setting all the inputs.
 
+        :param site_id: int
+        :param id: str
         :return: Self for convenience.
         """
+        self.irec.site_id = site_id
+        self.irec.id = id
+
+        return await self.exec()
+
+    async def exec(self, irec: tUsrKey = None) -> "dUsrSelectOne":
+        """
+        Execute the query, optionally passing in the input rec.
+
+        :param irec:
+        :return: Self for convenience.
+        """
+        if irec:
+            self.irec._copy_from(irec)
+
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrSelectAll", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("UsrSelectOne", self._dbcon.STMNT_TYPE_READ)
 
         self._dbstmnt.sql("""select
   site_id,
   id,
   role_id,
   status,
   name_first,
@@ -72,17 +93,20 @@
   cellno1_conf,
   cellno2_conf,
   opt_system,
   opt_market,
   opt_fail_login
 from
   fura.Usr
-order by
-  site_id,
-  id""")
+where
+  site_id = :site_id and
+  id = :id""")
+
+        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 128)
 
         self._dbstmnt.bind_out("site_id", int, 4)
         self._dbstmnt.bind_out("id", str, 128)
         self._dbstmnt.bind_out("role_id", str, 128)
         self._dbstmnt.bind_out("status", str, 1)
         self._dbstmnt.bind_out("name_first", str, 128)
         self._dbstmnt.bind_out("name_last", str, 128)
@@ -102,26 +126,29 @@
         self._dbstmnt.bind_out("cellno2_conf", bool)
         self._dbstmnt.bind_out("opt_system", bool)
         self._dbstmnt.bind_out("opt_market", bool)
         self._dbstmnt.bind_out("opt_fail_login", bool)
 
         await self._dbcon.execute(self._dbstmnt)
 
+        if irec:
+            irec._copy_from(self.irec)
+
         return self
 
     async def fetch(self, must_exist: bool = False) -> bool:
         """
         Fetches the next row from the executed query.
 
         :param must_exist:
         :return: True if a row was fetched, else False.
         """
         if not await self._dbcon.fetch(self._dbstmnt):
             if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Usr, proc:SelectAll]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
+                raise mettle.lib.xMettle(f"Record not found: [table:Usr, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
             return False
 
         self.orec = tUsr()
 
         self.orec.site_id = self._dbstmnt.result[0]
         self.orec.id = self._dbstmnt.result[1]
         self.orec.role_id = self._dbstmnt.result[2]
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_update.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,33 +1,31 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.usr_key import tUsrKey
 from bs_fura.db.tables.usr import tUsr
 
-class dUsrSelectOne:
-    __slots__ = ("_dbcon", "_dbstmnt", "irec", "orec")
+class dUsrUpdate:
+    __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tUsrKey()
-        self.orec     = None
+        self.irec     = tUsr()
 
     async def __aenter__(self):
         """
         With statement enter.
         """
         return self
 
@@ -40,163 +38,156 @@
     async def _destroy(self):
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
                         site_id: int,
-                        id: str) -> "dUsrSelectOne":
+                        id: str,
+                        role_id: str,
+                        status: str,
+                        name_first: str,
+                        name_last: str,
+                        title: str,
+                        date_activate: datetime.date,
+                        date_expire: datetime.date,
+                        email1: str,
+                        email2: str,
+                        cellno1: str,
+                        cellno2: str,
+                        modified_by: str,
+                        usrtype_id: str,
+                        email1_conf: bool,
+                        email2_conf: bool,
+                        cellno1_conf: bool,
+                        cellno2_conf: bool,
+                        opt_system: bool,
+                        opt_market: bool,
+                        opt_fail_login: bool) -> "dUsrUpdate":
         """
         Execute the query by setting all the inputs.
 
         :param site_id: int
         :param id: str
+        :param role_id: str
+        :param status: str
+        :param name_first: str
+        :param name_last: str
+        :param title: str
+        :param date_activate: datetime.date
+        :param date_expire: datetime.date
+        :param email1: str
+        :param email2: str
+        :param cellno1: str
+        :param cellno2: str
+        :param modified_by: str
+        :param tm_stamp: datetime.datetime
+        :param usrtype_id: str
+        :param email1_conf: bool
+        :param email2_conf: bool
+        :param cellno1_conf: bool
+        :param cellno2_conf: bool
+        :param opt_system: bool
+        :param opt_market: bool
+        :param opt_fail_login: bool
         :return: Self for convenience.
         """
         self.irec.site_id = site_id
         self.irec.id = id
+        self.irec.role_id = role_id
+        self.irec.status = status
+        self.irec.name_first = name_first
+        self.irec.name_last = name_last
+        self.irec.title = title
+        self.irec.date_activate = date_activate
+        self.irec.date_expire = date_expire
+        self.irec.email1 = email1
+        self.irec.email2 = email2
+        self.irec.cellno1 = cellno1
+        self.irec.cellno2 = cellno2
+        self.irec.modified_by = modified_by
+        self.irec.usrtype_id = usrtype_id
+        self.irec.email1_conf = email1_conf
+        self.irec.email2_conf = email2_conf
+        self.irec.cellno1_conf = cellno1_conf
+        self.irec.cellno2_conf = cellno2_conf
+        self.irec.opt_system = opt_system
+        self.irec.opt_market = opt_market
+        self.irec.opt_fail_login = opt_fail_login
 
         return await self.exec()
 
-    async def exec(self, irec: tUsrKey = None) -> "dUsrSelectOne":
+    async def exec(self, irec: tUsr = None) -> "dUsrUpdate":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrSelectOne", self._dbcon.STMNT_TYPE_READ)
+        self._dbstmnt = await self._dbcon.statement("UsrUpdate", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""select
-  site_id,
-  id,
-  role_id,
-  status,
-  name_first,
-  name_last,
-  title,
-  date_activate,
-  date_expire,
-  email1,
-  email2,
-  cellno1,
-  cellno2,
-  modified_by,
-  tm_stamp,
-  usrtype_id,
-  email1_conf,
-  email2_conf,
-  cellno1_conf,
-  cellno2_conf,
-  opt_system,
-  opt_market,
-  opt_fail_login
-from
+        self._dbstmnt.sql("""update
   fura.Usr
+set
+  role_id = :role_id,
+  status = :status,
+  name_first = :name_first,
+  name_last = :name_last,
+  title = :title,
+  date_activate = :date_activate,
+  date_expire = :date_expire,
+  email1 = :email1,
+  email2 = :email2,
+  cellno1 = :cellno1,
+  cellno2 = :cellno2,
+  modified_by = :modified_by,
+  tm_stamp = :tm_stamp,
+  usrtype_id = :usrtype_id,
+  email1_conf = :email1_conf,
+  email2_conf = :email2_conf,
+  cellno1_conf = :cellno1_conf,
+  cellno2_conf = :cellno2_conf,
+  opt_system = :opt_system,
+  opt_market = :opt_market,
+  opt_fail_login = :opt_fail_login
 where
   site_id = :site_id and
   id = :id""")
 
+        self.irec.tm_stamp = await self._dbcon.get_timestamp()
+
         self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
         self._dbstmnt.bind_in("id", self.irec.id, str, 128)
-
-        self._dbstmnt.bind_out("site_id", int, 4)
-        self._dbstmnt.bind_out("id", str, 128)
-        self._dbstmnt.bind_out("role_id", str, 128)
-        self._dbstmnt.bind_out("status", str, 1)
-        self._dbstmnt.bind_out("name_first", str, 128)
-        self._dbstmnt.bind_out("name_last", str, 128)
-        self._dbstmnt.bind_out("title", str, 5)
-        self._dbstmnt.bind_out("date_activate", datetime.date)
-        self._dbstmnt.bind_out("date_expire", datetime.date)
-        self._dbstmnt.bind_out("email1", str, 256)
-        self._dbstmnt.bind_out("email2", str, 256)
-        self._dbstmnt.bind_out("cellno1", str, 32)
-        self._dbstmnt.bind_out("cellno2", str, 32)
-        self._dbstmnt.bind_out("modified_by", str, 128)
-        self._dbstmnt.bind_out("tm_stamp", datetime.datetime)
-        self._dbstmnt.bind_out("usrtype_id", str, 32)
-        self._dbstmnt.bind_out("email1_conf", bool)
-        self._dbstmnt.bind_out("email2_conf", bool)
-        self._dbstmnt.bind_out("cellno1_conf", bool)
-        self._dbstmnt.bind_out("cellno2_conf", bool)
-        self._dbstmnt.bind_out("opt_system", bool)
-        self._dbstmnt.bind_out("opt_market", bool)
-        self._dbstmnt.bind_out("opt_fail_login", bool)
+        self._dbstmnt.bind_in("role_id", self.irec.role_id, str, 128)
+        self._dbstmnt.bind_in("status", self.irec.status, str, 1)
+        self._dbstmnt.bind_in("name_first", self.irec.name_first, str, 128)
+        self._dbstmnt.bind_in("name_last", self.irec.name_last, str, 128)
+        self._dbstmnt.bind_in("title", self.irec.title, str, 5)
+        self._dbstmnt.bind_in("date_activate", self.irec.date_activate, datetime.date)
+        self._dbstmnt.bind_in("date_expire", self.irec.date_expire, datetime.date)
+        self._dbstmnt.bind_in("email1", self.irec.email1, str, 256)
+        self._dbstmnt.bind_in("email2", self.irec.email2, str, 256)
+        self._dbstmnt.bind_in("cellno1", self.irec.cellno1, str, 32)
+        self._dbstmnt.bind_in("cellno2", self.irec.cellno2, str, 32)
+        self._dbstmnt.bind_in("modified_by", self.irec.modified_by, str, 128)
+        self._dbstmnt.bind_in("tm_stamp", self.irec.tm_stamp, datetime.datetime)
+        self._dbstmnt.bind_in("usrtype_id", self.irec.usrtype_id, str, 32)
+        self._dbstmnt.bind_in("email1_conf", self.irec.email1_conf, bool)
+        self._dbstmnt.bind_in("email2_conf", self.irec.email2_conf, bool)
+        self._dbstmnt.bind_in("cellno1_conf", self.irec.cellno1_conf, bool)
+        self._dbstmnt.bind_in("cellno2_conf", self.irec.cellno2_conf, bool)
+        self._dbstmnt.bind_in("opt_system", self.irec.opt_system, bool)
+        self._dbstmnt.bind_in("opt_market", self.irec.opt_market, bool)
+        self._dbstmnt.bind_in("opt_fail_login", self.irec.opt_fail_login, bool)
 
         await self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
 
-    async def fetch(self, must_exist: bool = False) -> bool:
-        """
-        Fetches the next row from the executed query.
-
-        :param must_exist:
-        :return: True if a row was fetched, else False.
-        """
-        if not await self._dbcon.fetch(self._dbstmnt):
-            if must_exist:
-                raise mettle.lib.xMettle(f"Record not found: [table:Usr, proc:SelectOne, row:{self.irec}]", err_code=mettle.lib.xMettle.eCode.DBNotFound)
-            return False
-
-        self.orec = tUsr()
-
-        self.orec.site_id = self._dbstmnt.result[0]
-        self.orec.id = self._dbstmnt.result[1]
-        self.orec.role_id = self._dbstmnt.result[2]
-        self.orec.status = self._dbstmnt.result[3]
-        self.orec.name_first = self._dbstmnt.result[4]
-        self.orec.name_last = self._dbstmnt.result[5]
-        self.orec.title = self._dbstmnt.result[6]
-        self.orec.date_activate = self._dbstmnt.result[7]
-        self.orec.date_expire = self._dbstmnt.result[8]
-        self.orec.email1 = self._dbstmnt.result[9]
-        self.orec.email2 = self._dbstmnt.result[10]
-        self.orec.cellno1 = self._dbstmnt.result[11]
-        self.orec.cellno2 = self._dbstmnt.result[12]
-        self.orec.modified_by = self._dbstmnt.result[13]
-        self.orec.tm_stamp = self._dbstmnt.result[14]
-        self.orec.usrtype_id = self._dbstmnt.result[15]
-        self.orec.email1_conf = self._dbstmnt.result[16]
-        self.orec.email2_conf = self._dbstmnt.result[17]
-        self.orec.cellno1_conf = self._dbstmnt.result[18]
-        self.orec.cellno2_conf = self._dbstmnt.result[19]
-        self.orec.opt_system = self._dbstmnt.result[20]
-        self.orec.opt_market = self._dbstmnt.result[21]
-        self.orec.opt_fail_login = self._dbstmnt.result[22]
-
-        return True
-
-    async def fetch_iter(self) -> tUsr:
-        """
-        Yield all the rows one at a time.
-
-        :return: Iterator for output rows
-        """
-        while await self.fetch():
-            yield self.orec
-
-    async def fetch_all(self, out_list: tUsr.List, clear_list: bool = True) -> int:
-        """
-        Fetch all the rows into the specified list and return the list count.
-
-        :param out_list:
-        :param clear_list:
-        :return: Number of rows fetched.
-        """
-        if clear_list:
-            out_list.clear()
-
-        while await self.fetch():
-            out_list.append(self.orec)
-
-        return len(out_list)
-
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import asyncio
 import datetime
 import uuid
 import time
 import mettle.lib
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_delete_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_delete_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_insert.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_update.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
 from bs_fura.db.tables.usr_type import tUsrType
 
-class dUsrTypeInsert:
+class dUsrTypeUpdate:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
     def __init__(self, dbcon: mettle.db.IAConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
@@ -39,57 +39,52 @@
         if self._dbstmnt:
             await self._dbstmnt.destroy()
             self._dbstmnt = None
 
     async def exec_deft(self,
                         id: str,
                         descr: str,
-                        modified_by: str,
-                        tm_stamp: datetime.datetime) -> "dUsrTypeInsert":
+                        modified_by: str) -> "dUsrTypeUpdate":
         """
         Execute the query by setting all the inputs.
 
         :param id: str
         :param descr: str
         :param modified_by: str
         :param tm_stamp: datetime.datetime
         :return: Self for convenience.
         """
         self.irec.id = id
         self.irec.descr = descr
         self.irec.modified_by = modified_by
-        self.irec.tm_stamp = tm_stamp
 
         return await self.exec()
 
-    async def exec(self, irec: tUsrType = None) -> "dUsrTypeInsert":
+    async def exec(self, irec: tUsrType = None) -> "dUsrTypeUpdate":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
         await self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrTypeInsert", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = await self._dbcon.statement("UsrTypeUpdate", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""insert into fura.UsrType (
-  id,
-  descr,
-  modified_by,
-  tm_stamp
-) values (
-  :id,
-  :descr,
-  :modified_by,
-  :tm_stamp
-)""")
+        self._dbstmnt.sql("""update
+  fura.UsrType
+set
+  descr = :descr,
+  modified_by = :modified_by,
+  tm_stamp = :tm_stamp
+where
+  id = :id""")
 
         self.irec.tm_stamp = await self._dbcon.get_timestamp()
 
         self._dbstmnt.bind_in("id", self.irec.id, str, 32)
         self._dbstmnt.bind_in("descr", self.irec.descr, str, 128)
         self._dbstmnt.bind_in("modified_by", self.irec.modified_by, str, 128)
         self._dbstmnt.bind_in("tm_stamp", self.irec.tm_stamp, datetime.datetime)
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_lock_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_lock_one.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_select_all.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_select_all.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_select_one.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao_async/postgresql/usr_type_select_one.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/dao_async/postgresql/usr_type_update.py` & `bitsmiths-fura-2.2.3/bs_fura/db/dao/postgresql/site_cfg_delete_one.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,98 +1,87 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #  Target Database = postgresql
 #
 import datetime
 import uuid
 import time
 import mettle.lib
 import mettle.io
 import mettle.db
 
-from bs_fura.db.tables.usr_type import tUsrType
+from bs_fura.db.tables.site_cfg_key import tSiteCfgKey
 
-class dUsrTypeUpdate:
+class dSiteCfgDeleteOne:
     __slots__ = ("_dbcon", "_dbstmnt", "irec")
 
-    def __init__(self, dbcon: mettle.db.IAConnect):
+    def __init__(self, dbcon: mettle.db.IConnect):
         """
         Constructor.
 
         :param dbcon: Mettle database connection object.
         """
         self._dbcon   = dbcon
         self._dbstmnt = None
-        self.irec     = tUsrType()
+        self.irec     = tSiteCfgKey()
 
-    async def __aenter__(self):
+    def __enter__(self):
         """
         With statement enter.
         """
         return self
 
-    async def __aexit__(self, type, value, traceback):
+    def __exit__(self, type, value, traceback):
         """
         With statement exit.
         """
-        await self._destroy()
+        self._destroy()
 
-    async def _destroy(self):
+    def _destroy(self):
         if self._dbstmnt:
-            await self._dbstmnt.destroy()
+            self._dbstmnt.destroy()
             self._dbstmnt = None
 
-    async def exec_deft(self,
-                        id: str,
-                        descr: str,
-                        modified_by: str) -> "dUsrTypeUpdate":
+    def exec_deft(self,
+                  site_id: int,
+                  id: str) -> "dSiteCfgDeleteOne":
         """
         Execute the query by setting all the inputs.
 
+        :param site_id: int
         :param id: str
-        :param descr: str
-        :param modified_by: str
-        :param tm_stamp: datetime.datetime
         :return: Self for convenience.
         """
+        self.irec.site_id = site_id
         self.irec.id = id
-        self.irec.descr = descr
-        self.irec.modified_by = modified_by
 
-        return await self.exec()
+        return self.exec()
 
-    async def exec(self, irec: tUsrType = None) -> "dUsrTypeUpdate":
+    def exec(self, irec: tSiteCfgKey = None) -> "dSiteCfgDeleteOne":
         """
         Execute the query, optionally passing in the input rec.
 
         :param irec:
         :return: Self for convenience.
         """
         if irec:
             self.irec._copy_from(irec)
 
-        await self._destroy()
+        self._destroy()
 
-        self._dbstmnt = await self._dbcon.statement("UsrTypeUpdate", self._dbcon.STMNT_TYPE_CUD)
+        self._dbstmnt = self._dbcon.statement("SiteCfgDeleteOne", self._dbcon.STMNT_TYPE_CUD)
 
-        self._dbstmnt.sql("""update
-  fura.UsrType
-set
-  descr = :descr,
-  modified_by = :modified_by,
-  tm_stamp = :tm_stamp
+        self._dbstmnt.sql("""delete from
+  fura.SiteCfg
 where
+  site_id = :site_id and
   id = :id""")
 
-        self.irec.tm_stamp = await self._dbcon.get_timestamp()
+        self._dbstmnt.bind_in("site_id", self.irec.site_id, int, 4)
+        self._dbstmnt.bind_in("id", self.irec.id, str, 256)
 
-        self._dbstmnt.bind_in("id", self.irec.id, str, 32)
-        self._dbstmnt.bind_in("descr", self.irec.descr, str, 128)
-        self._dbstmnt.bind_in("modified_by", self.irec.modified_by, str, 128)
-        self._dbstmnt.bind_in("tm_stamp", self.irec.tm_stamp, datetime.datetime)
-
-        await self._dbcon.execute(self._dbstmnt)
+        self._dbcon.execute(self._dbstmnt)
 
         if irec:
             irec._copy_from(self.irec)
 
         return self
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 from .ada import tAda
 from .iada_search import iAdaSearch
 from .aga import tAga
 from .iaga_search import iAgaSearch
 from .config_key import tConfigKey
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ada.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ada.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/aga.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/aga.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/config.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/config_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/config_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/eatok.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/eatok.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/eatok_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/eatok_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/func.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/func.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/func_grp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/func_grp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/func_grp_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/func_grp_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/func_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/func_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iada_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iada_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iaga_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iaga_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iconfig_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iconfig_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_delete_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_incr_usage.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_incr_usage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ieatok_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ieatok_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_grp_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_grp_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_role_func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_role_func_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ifunc_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ifunc_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_by_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_delete_by_role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_delete_by_role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_exists.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_exists.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_func_rel_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_func_rel_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/irole_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/irole_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_cfg_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_cfg_delete_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_cfg_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_cfg_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/isite_id_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/isite_id_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_by_site.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_expired.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/itoken_sentry_expired.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/itoken_sentry_expired.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iula_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iula_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_auth_by_token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_auth_by_token.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_auth_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_auth_delete_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_by_site.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_delete_by_site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_delete_by_site.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_search.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/iusr_type_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/iusr_type_search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/oeatok_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/oeatok_search.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ofunc_role_func_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ofunc_role_func_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/orole_func_rel_exists.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/orole_func_rel_exists.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/orole_func_rel_search.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/orole_func_rel_search.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/osite_id_by_code.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/osite_id_by_code.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/role.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/role.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/role_func_rel.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/role_func_rel.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/role_func_rel_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/role_func_rel_key.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/role_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/role_key.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/site.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/site.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/site_cfg.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/site_cfg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/site_cfg_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/site_cfg_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/site_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/site_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/token.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/token.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/token_hist.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/token_hist.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/token_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/token_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/token_sentry.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/token_sentry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/token_sentry_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/token_sentry_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/ula.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/ula.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_auth.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_auth.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_auth_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_auth_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:04 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_otp.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_otp.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_otp_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_otp_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_type.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/db/tables/usr_type_key.py` & `bitsmiths-fura-2.2.3/bs_fura/db/tables/usr_type_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Wed Sep 28 13:55:05 2022
+# This file was generated by mettle.genes.db.GenPy3 [ver 2.2] on Thu Jul 20 09:12:34 2023
 #
 
 import datetime
 import uuid
 import time
 import dataclasses
 import typing
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/err_code.py` & `bitsmiths-fura-2.2.3/bs_fura/err_code.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/fura_davcache.py` & `bitsmiths-fura-2.2.3/bs_fura/fura_davcache.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/fura_server.py` & `bitsmiths-fura-2.2.3/bs_fura/fura_server.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/fura_server_impl.py` & `bitsmiths-fura-2.2.3/bs_fura/fura_server_impl.py`

 * *Files 1% similar despite different names*

```diff
@@ -755,15 +755,15 @@
             try:
                 with UserLogin(self._dao, ul_rec.site_code) as ul:
                     ul.login(ul_rec.user_id, ul_rec.auth_type, ul_rec.auth_data, ul_rec.ip_addr, ul_rec.geo_loc)
 
                     self._new_token = ul.gen_fura_token(self._fura_token)
 
             except xFura as xf:
-                self._log.info(f'user_login Failed: {xf}')
+                self._log.debug('userLogin Failed [%s]' % str(xf))
 
                 if xf.get_error_code() in (ErrCode.AuthMaxFailures.value, ErrCode.AuthInvalid.value):
                     return xf.get_error_code()
 
                 return ErrCode.AuthInvalid.value
 
             finally:
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/fura_server_impl_async.py` & `bitsmiths-fura-2.2.3/bs_fura/fura_server_impl_async.py`

 * *Files 0% similar despite different names*

```diff
@@ -778,15 +778,15 @@
             try:
                 async with UserLoginAsync(self._dao, ul_rec.site_code) as ul:
                     await ul.login(ul_rec.user_id, ul_rec.auth_type, ul_rec.auth_data, ul_rec.ip_addr, ul_rec.geo_loc)
 
                     self._new_token = ul.gen_fura_token(await self.get_fura_token())
 
             except xFura as xf:
-                self._log.debug(f'user_login Failed: {xf}')
+                self._log.debug('userLogin Failed [%s]' % str(xf))
 
                 if xf.get_error_code() in (ErrCode.AuthMaxFailures.value, ErrCode.AuthInvalid.value):
                     return xf.get_error_code()
 
                 return ErrCode.AuthInvalid.value
 
             finally:
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/fura_token.py` & `bitsmiths-fura-2.2.3/bs_fura/fura_token.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/jw_token.py` & `bitsmiths-fura-2.2.3/bs_fura/jw_token.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         """
         Decrypts the token back to its claim state.
 
         :param tok: The encrypted token.
         :param ignore_expirey: If true, ignore the expirey datetime check.
         :return The decrypted claim dictionary.
         """
-        etoken = jwcrypto.jwt.JWT(key = self._key, jwt = tok)
+        etoken = jwcrypto.jwt.JWT(key=self._key, jwt=tok, expected_type="JWE")
         token  = jwcrypto.jwt.JWT(key = self._key, jwt = etoken.claims)
         claim  = json.loads(token.claims)
 
         if ignore_expirey:
             return claim
 
         exp = claim.get('tex')
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/otp.py` & `bitsmiths-fura-2.2.3/bs_fura/otp.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/otp_async.py` & `bitsmiths-fura-2.2.3/bs_fura/otp_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/sql/__init__.py` & `bitsmiths-fura-2.2.3/bs_fura/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/sql/postgresql.sql` & `bitsmiths-fura-2.2.3/bs_fura/sql/postgresql.sql`

 * *Files 12% similar despite different names*

```diff
@@ -1,113 +1,112 @@
-CREATE TABLE fura.sitecfg (
-   site_id INTEGER
-  ,id varchar(256)
+CREATE TABLE fura.service (
+   id varchar(96)
+  ,servicegrpid varchar(128)
   ,descr varchar(256)
-  ,value varchar(4096)
-  ,modified_by varchar(64)
-  ,tm_stamp TIMESTAMP
+  ,audid varchar(128)
+  ,tmstamp TIMESTAMP
 );
-ALTER TABLE fura.sitecfg ADD PRIMARY KEY (
-   site_id
-  ,id
+ALTER TABLE fura.service ADD PRIMARY KEY (
+   id
 );
-CREATE TABLE fura.funcgrp (
+CREATE TABLE fura.servicesiterel (
    id varchar(128)
-  ,descr varchar(256)
-  ,modified_by varchar(128)
-  ,tm_stamp TIMESTAMP
+  ,siteid INTEGER
+  ,serviceid varchar(96)
+  ,audid varchar(128)
+  ,tmstamp TIMESTAMP
 );
-ALTER TABLE fura.funcgrp ADD PRIMARY KEY (
+ALTER TABLE fura.servicesiterel ADD PRIMARY KEY (
    id
 );
-CREATE TABLE fura.eatok (
-   id SERIAL8
-  ,tok varchar(256)
-  ,site_id INTEGER
-  ,usr_id varchar(128)
-  ,func_id varchar(128)
-  ,grant_usr_id varchar(128)
-  ,created TIMESTAMP
-  ,expires TIMESTAMP
-  ,max_usages INTEGER
-  ,usages INTEGER
-);
-ALTER TABLE fura.eatok ADD PRIMARY KEY (
-   id
+CREATE TABLE fura.rssr (
+   siteid INTEGER
+  ,roleserviceid varchar(128)
+  ,rssrid varchar(128)
+);
+ALTER TABLE fura.rssr ADD PRIMARY KEY (
+   siteid
+  ,roleserviceid
+  ,rssrid
 );
-CREATE TABLE fura.token (
-   site_id INTEGER
-  ,id varchar(64)
-  ,usr_id varchar(128)
-  ,date_created TIMESTAMP
-  ,expires TIMESTAMP
-  ,use_cnt INTEGER
-  ,audid VARCHAR
+CREATE TABLE fura.roleservice (
+   siteid INTEGER
+  ,id varchar(128)
+  ,descr varchar(256)
+  ,accesstype VARCHAR
+  ,audid varchar(128)
   ,tmstamp TIMESTAMP
 );
-ALTER TABLE fura.token ADD PRIMARY KEY (
-   site_id
+ALTER TABLE fura.roleservice ADD PRIMARY KEY (
+   siteid
   ,id
 );
-CREATE TABLE fura.rolefuncrel (
-   site_id INTEGER
-  ,role_id varchar(128)
-  ,func_id varchar(128)
-  ,modified_by varchar(128)
-  ,tm_stamp TIMESTAMP
-);
-ALTER TABLE fura.rolefuncrel ADD PRIMARY KEY (
-   site_id
-  ,role_id
-  ,func_id
-);
-CREATE TABLE fura.ula (
-   site_id INTEGER
-  ,site_code varchar(32)
-  ,tm_stamp TIMESTAMP
-  ,usr_id varchar(128)
-  ,err_code INTEGER
-  ,state character(1)
-  ,action character(1)
-  ,auth_type character(1)
-  ,auth_ip varchar(32)
-  ,auth_geo varchar(64)
-);
-CREATE TABLE fura.tokensentry (
-   site_id INTEGER
-  ,token_cnt BIGINT
-  ,last_poll TIMESTAMP
-);
-ALTER TABLE fura.tokensentry ADD PRIMARY KEY (
-   site_id
-);
 CREATE TABLE fura.role (
    site_id INTEGER
   ,id varchar(128)
   ,descr varchar(256)
   ,status character(1)
   ,LEVEL INTEGER
   ,sess_timeout INTEGER
   ,modified_by varchar(128)
   ,tm_stamp TIMESTAMP
 );
 ALTER TABLE fura.role ADD PRIMARY KEY (
    site_id
   ,id
 );
-CREATE TABLE fura.aga (
+CREATE TABLE fura.ada (
    site_id INTEGER
   ,site_code varchar(32)
   ,tm_stamp TIMESTAMP
   ,usr_id varchar(128)
   ,eausr_id varchar(128)
   ,role_id varchar(128)
   ,func_id varchar(128)
   ,action character(1)
   ,src varchar(128)
+  ,reason varchar(128)
+);
+CREATE TABLE fura.rolefuncrel (
+   site_id INTEGER
+  ,role_id varchar(128)
+  ,func_id varchar(128)
+  ,modified_by varchar(128)
+  ,tm_stamp TIMESTAMP
+);
+ALTER TABLE fura.rolefuncrel ADD PRIMARY KEY (
+   site_id
+  ,role_id
+  ,func_id
+);
+CREATE TABLE fura.usrotp (
+   site_id INTEGER
+  ,usr_id varchar(128)
+  ,otp_method character(1)
+  ,otp varchar(128)
+  ,expire TIMESTAMP
+  ,used BOOLEAN
+  ,target varchar(64)
+  ,fail_cnt INTEGER
+  ,meta_data JSONB
+  ,tm_stamp TIMESTAMP
+);
+ALTER TABLE fura.usrotp ADD PRIMARY KEY (
+   site_id
+  ,usr_id
+);
+CREATE TABLE fura.config (
+   id varchar(256)
+  ,descr varchar(256)
+  ,value varchar(4096)
+  ,modified_by varchar(128)
+  ,tm_stamp TIMESTAMP
+);
+ALTER TABLE fura.config ADD PRIMARY KEY (
+   id
 );
 CREATE TABLE fura.usr (
    site_id INTEGER
   ,id varchar(128)
   ,role_id varchar(128)
   ,status character(1)
   ,name_first varchar(128)
@@ -130,51 +129,37 @@
   ,opt_market BOOLEAN
   ,opt_fail_login BOOLEAN
 );
 ALTER TABLE fura.usr ADD PRIMARY KEY (
    site_id
   ,id
 );
-CREATE TABLE fura.usrotp (
-   site_id INTEGER
-  ,usr_id varchar(128)
-  ,otp_method character(1)
-  ,otp varchar(128)
-  ,expire TIMESTAMP
-  ,used BOOLEAN
-  ,target varchar(64)
-  ,fail_cnt INTEGER
-  ,meta_data JSONB
-  ,tm_stamp TIMESTAMP
-);
-ALTER TABLE fura.usrotp ADD PRIMARY KEY (
-   site_id
-  ,usr_id
-);
-CREATE TABLE fura.ada (
+CREATE TABLE fura.ula (
    site_id INTEGER
   ,site_code varchar(32)
   ,tm_stamp TIMESTAMP
   ,usr_id varchar(128)
-  ,eausr_id varchar(128)
-  ,role_id varchar(128)
-  ,func_id varchar(128)
+  ,err_code INTEGER
+  ,state character(1)
   ,action character(1)
-  ,src varchar(128)
-  ,reason varchar(128)
+  ,auth_type character(1)
+  ,auth_ip varchar(32)
+  ,auth_geo varchar(64)
 );
-CREATE TABLE fura.config (
-   id varchar(256)
+CREATE TABLE fura.sitecfg (
+   site_id INTEGER
+  ,id varchar(256)
   ,descr varchar(256)
   ,value varchar(4096)
-  ,modified_by varchar(128)
+  ,modified_by varchar(64)
   ,tm_stamp TIMESTAMP
 );
-ALTER TABLE fura.config ADD PRIMARY KEY (
-   id
+ALTER TABLE fura.sitecfg ADD PRIMARY KEY (
+   site_id
+  ,id
 );
 CREATE TABLE fura.site (
    id serial4
   ,code varchar(32)
   ,descr varchar(256)
   ,status character(1)
   ,cc varchar(2)
@@ -182,83 +167,149 @@
   ,dc varchar(3)
   ,modified_by varchar(128)
   ,tm_stamp TIMESTAMP
 );
 ALTER TABLE fura.site ADD PRIMARY KEY (
    id
 );
-CREATE TABLE fura.usrauth (
-   site_id INTEGER
-  ,usr_id varchar(128)
-  ,auth_type character(1)
-  ,auth_data varchar(4096)
-  ,fail_cnt INTEGER
-  ,salt varchar(128)
-  ,last_ip varchar(32)
-  ,last_geo varchar(64)
-  ,last_succ TIMESTAMP
-  ,last_fail TIMESTAMP
+CREATE TABLE fura.servicegrp (
+   id varchar(128)
+  ,descr varchar(256)
+  ,audid varchar(128)
+  ,tmstamp TIMESTAMP
+);
+ALTER TABLE fura.servicegrp ADD PRIMARY KEY (
+   id
+);
+CREATE TABLE fura.funcgrp (
+   id varchar(128)
+  ,descr varchar(256)
   ,modified_by varchar(128)
   ,tm_stamp TIMESTAMP
 );
-ALTER TABLE fura.usrauth ADD PRIMARY KEY (
-   site_id
-  ,usr_id
-  ,auth_type
+ALTER TABLE fura.funcgrp ADD PRIMARY KEY (
+   id
+);
+CREATE TABLE fura.aga (
+   site_id INTEGER
+  ,site_code varchar(32)
+  ,tm_stamp TIMESTAMP
+  ,usr_id varchar(128)
+  ,eausr_id varchar(128)
+  ,role_id varchar(128)
+  ,func_id varchar(128)
+  ,action character(1)
+  ,src varchar(128)
 );
 CREATE TABLE fura.func (
    id varchar(128)
   ,funcgrp_id varchar(128)
   ,descr varchar(256)
   ,action character(1)
   ,oride character(1)
   ,audit_lvl INTEGER
   ,modified_by varchar(128)
   ,tm_stamp TIMESTAMP
 );
 ALTER TABLE fura.func ADD PRIMARY KEY (
    id
 );
-CREATE TABLE fura.tokenhist (
+CREATE TABLE fura.token (
    site_id INTEGER
   ,id varchar(64)
   ,usr_id varchar(128)
   ,date_created TIMESTAMP
   ,expires TIMESTAMP
   ,use_cnt INTEGER
   ,audid VARCHAR
   ,tmstamp TIMESTAMP
 );
+ALTER TABLE fura.token ADD PRIMARY KEY (
+   site_id
+  ,id
+);
 CREATE TABLE fura.usrtype (
    id varchar(32)
   ,descr varchar(128)
   ,modified_by varchar(128)
   ,tm_stamp TIMESTAMP
 );
 ALTER TABLE fura.usrtype ADD PRIMARY KEY (
    id
 );
-ALTER TABLE fura.tokensentry
+CREATE TABLE fura.usrauth (
+   site_id INTEGER
+  ,usr_id varchar(128)
+  ,auth_type character(1)
+  ,auth_data varchar(4096)
+  ,fail_cnt INTEGER
+  ,salt varchar(128)
+  ,last_ip varchar(32)
+  ,last_geo varchar(64)
+  ,last_succ TIMESTAMP
+  ,last_fail TIMESTAMP
+  ,modified_by varchar(128)
+  ,tm_stamp TIMESTAMP
+);
+ALTER TABLE fura.usrauth ADD PRIMARY KEY (
+   site_id
+  ,usr_id
+  ,auth_type
+);
+CREATE TABLE fura.tokensentry (
+   site_id INTEGER
+  ,token_cnt BIGINT
+  ,last_poll TIMESTAMP
+);
+ALTER TABLE fura.tokensentry ADD PRIMARY KEY (
+   site_id
+);
+CREATE TABLE fura.eatok (
+   id SERIAL8
+  ,tok varchar(256)
+  ,site_id INTEGER
+  ,usr_id varchar(128)
+  ,func_id varchar(128)
+  ,grant_usr_id varchar(128)
+  ,created TIMESTAMP
+  ,expires TIMESTAMP
+  ,max_usages INTEGER
+  ,usages INTEGER
+);
+ALTER TABLE fura.eatok ADD PRIMARY KEY (
+   id
+);
+CREATE TABLE fura.tokenhist (
+   site_id INTEGER
+  ,id varchar(64)
+  ,usr_id varchar(128)
+  ,date_created TIMESTAMP
+  ,expires TIMESTAMP
+  ,use_cnt INTEGER
+  ,audid VARCHAR
+  ,tmstamp TIMESTAMP
+);
+ALTER TABLE fura.usrotp
    ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN token_cnt SET NOT NULL
-  ,ALTER COLUMN last_poll SET NOT NULL
+  ,ALTER COLUMN usr_id SET NOT NULL
+  ,ALTER COLUMN otp_method SET NOT NULL
+  ,ALTER COLUMN used SET NOT NULL
+  ,ALTER COLUMN fail_cnt SET NOT NULL
+  ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
-ALTER TABLE fura.tokensentry ADD CONSTRAINT tokensentry_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
-ALTER TABLE fura.token
-   ALTER COLUMN site_id SET NOT NULL
+ALTER TABLE fura.usrotp ADD CONSTRAINT usrotp_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
+ALTER TABLE fura.roleservice
+   ALTER COLUMN siteid SET NOT NULL
   ,ALTER COLUMN id SET NOT NULL
-  ,ALTER COLUMN usr_id SET NOT NULL
-  ,ALTER COLUMN date_created SET NOT NULL
-  ,ALTER COLUMN expires SET NOT NULL
-  ,ALTER COLUMN use_cnt SET NOT NULL
+  ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN accesstype SET NOT NULL
   ,ALTER COLUMN audid SET NOT NULL
   ,ALTER COLUMN tmstamp SET NOT NULL
 ;
-ALTER TABLE fura.token ADD CONSTRAINT token_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
-ALTER TABLE fura.token ADD CONSTRAINT token_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
+ALTER TABLE fura.roleservice ADD CONSTRAINT roleservice_fk_st FOREIGN KEY (siteid) REFERENCES fura.site;
 ALTER TABLE fura.usrauth
    ALTER COLUMN site_id SET NOT NULL
   ,ALTER COLUMN usr_id SET NOT NULL
   ,ALTER COLUMN auth_type SET NOT NULL
   ,ALTER COLUMN fail_cnt SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
@@ -268,44 +319,14 @@
    ALTER COLUMN site_id SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
   ,ALTER COLUMN err_code SET NOT NULL
   ,ALTER COLUMN state SET NOT NULL
   ,ALTER COLUMN action SET NOT NULL
   ,ALTER COLUMN auth_type SET NOT NULL
 ;
-ALTER TABLE fura.tokenhist
-   ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN id SET NOT NULL
-  ,ALTER COLUMN usr_id SET NOT NULL
-  ,ALTER COLUMN date_created SET NOT NULL
-  ,ALTER COLUMN expires SET NOT NULL
-  ,ALTER COLUMN use_cnt SET NOT NULL
-  ,ALTER COLUMN audid SET NOT NULL
-  ,ALTER COLUMN tmstamp SET NOT NULL
-;
-ALTER TABLE fura.aga
-   ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN site_code SET NOT NULL
-  ,ALTER COLUMN tm_stamp SET NOT NULL
-  ,ALTER COLUMN usr_id SET NOT NULL
-  ,ALTER COLUMN role_id SET NOT NULL
-  ,ALTER COLUMN func_id SET NOT NULL
-  ,ALTER COLUMN action SET NOT NULL
-;
-ALTER TABLE fura.role
-   ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN id SET NOT NULL
-  ,ALTER COLUMN descr SET NOT NULL
-  ,ALTER COLUMN status SET NOT NULL
-  ,ALTER COLUMN LEVEL SET NOT NULL
-  ,ALTER COLUMN sess_timeout SET NOT NULL
-  ,ALTER COLUMN modified_by SET NOT NULL
-  ,ALTER COLUMN tm_stamp SET NOT NULL
-;
-ALTER TABLE fura.role ADD CONSTRAINT role_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
 ALTER TABLE fura.usr
    ALTER COLUMN site_id SET NOT NULL
   ,ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN status SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
   ,ALTER COLUMN usrtype_id SET NOT NULL
@@ -316,110 +337,181 @@
   ,ALTER COLUMN opt_system SET NOT NULL
   ,ALTER COLUMN opt_market SET NOT NULL
   ,ALTER COLUMN opt_fail_login SET NOT NULL
 ;
 ALTER TABLE fura.usr ADD CONSTRAINT usr_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
 ALTER TABLE fura.usr ADD CONSTRAINT usr_fk_usrtype FOREIGN KEY (usrtype_id) REFERENCES fura.usrtype;
 ALTER TABLE fura.usr ADD CONSTRAINT usr_fk_role FOREIGN KEY (site_id, role_id) REFERENCES fura.role;
+ALTER TABLE fura.funcgrp
+   ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN modified_by SET NOT NULL
+  ,ALTER COLUMN tm_stamp SET NOT NULL
+;
+ALTER TABLE fura.eatok
+   ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN tok SET NOT NULL
+  ,ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN usr_id SET NOT NULL
+  ,ALTER COLUMN func_id SET NOT NULL
+  ,ALTER COLUMN grant_usr_id SET NOT NULL
+  ,ALTER COLUMN created SET NOT NULL
+  ,ALTER COLUMN expires SET NOT NULL
+  ,ALTER COLUMN max_usages SET NOT NULL
+  ,ALTER COLUMN usages SET NOT NULL
+;
+ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
+ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_grant FOREIGN KEY (site_id, grant_usr_id) REFERENCES fura.usr;
+ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_func FOREIGN KEY (func_id) REFERENCES fura.func;
+ALTER TABLE fura.eatok ADD CONSTRAINT eatok_uk_tok UNIQUE (
+   tok
+  ,site_id
+);
 ALTER TABLE fura.rolefuncrel
    ALTER COLUMN site_id SET NOT NULL
   ,ALTER COLUMN role_id SET NOT NULL
   ,ALTER COLUMN func_id SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
-ALTER TABLE fura.sitecfg
-   ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN id SET NOT NULL
+ALTER TABLE fura.servicegrp
+   ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN descr SET NOT NULL
-  ,ALTER COLUMN modified_by SET NOT NULL
-  ,ALTER COLUMN tm_stamp SET NOT NULL
+  ,ALTER COLUMN audid SET NOT NULL
+  ,ALTER COLUMN tmstamp SET NOT NULL
 ;
-ALTER TABLE fura.usrtype
+ALTER TABLE fura.service
    ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN servicegrpid SET NOT NULL
   ,ALTER COLUMN descr SET NOT NULL
-  ,ALTER COLUMN modified_by SET NOT NULL
+  ,ALTER COLUMN audid SET NOT NULL
+  ,ALTER COLUMN tmstamp SET NOT NULL
+;
+ALTER TABLE fura.service ADD CONSTRAINT service_fk_sg FOREIGN KEY (servicegrpid) REFERENCES fura.servicegrp;
+ALTER TABLE fura.aga
+   ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN site_code SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
+  ,ALTER COLUMN usr_id SET NOT NULL
+  ,ALTER COLUMN role_id SET NOT NULL
+  ,ALTER COLUMN func_id SET NOT NULL
+  ,ALTER COLUMN action SET NOT NULL
 ;
-ALTER TABLE fura.funcgrp
+ALTER TABLE fura.rssr
+   ALTER COLUMN siteid SET NOT NULL
+  ,ALTER COLUMN roleserviceid SET NOT NULL
+  ,ALTER COLUMN rssrid SET NOT NULL
+;
+ALTER TABLE fura.rssr ADD CONSTRAINT rssr_fk_rs FOREIGN KEY (siteid, roleserviceid) REFERENCES fura.roleservice;
+ALTER TABLE fura.rssr ADD CONSTRAINT rssr_fk_rssr FOREIGN KEY (rssrid) REFERENCES fura.servicesiterel;
+ALTER TABLE fura.servicesiterel
    ALTER COLUMN id SET NOT NULL
-  ,ALTER COLUMN descr SET NOT NULL
-  ,ALTER COLUMN modified_by SET NOT NULL
-  ,ALTER COLUMN tm_stamp SET NOT NULL
+  ,ALTER COLUMN siteid SET NOT NULL
+  ,ALTER COLUMN serviceid SET NOT NULL
+  ,ALTER COLUMN audid SET NOT NULL
+  ,ALTER COLUMN tmstamp SET NOT NULL
 ;
+ALTER TABLE fura.servicesiterel ADD CONSTRAINT servicesiterel_fk_st FOREIGN KEY (siteid) REFERENCES fura.site;
+ALTER TABLE fura.servicesiterel ADD CONSTRAINT servicesiterel_fk_se FOREIGN KEY (serviceid) REFERENCES fura.service;
 ALTER TABLE fura.ada
    ALTER COLUMN site_id SET NOT NULL
   ,ALTER COLUMN site_code SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
   ,ALTER COLUMN usr_id SET NOT NULL
   ,ALTER COLUMN role_id SET NOT NULL
   ,ALTER COLUMN func_id SET NOT NULL
   ,ALTER COLUMN action SET NOT NULL
   ,ALTER COLUMN reason SET NOT NULL
 ;
-ALTER TABLE fura.config
+ALTER TABLE fura.sitecfg
+   ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN modified_by SET NOT NULL
+  ,ALTER COLUMN tm_stamp SET NOT NULL
+;
+ALTER TABLE fura.site
    ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN status SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
-ALTER TABLE fura.usrotp
+ALTER TABLE fura.site ADD CONSTRAINT site_uk_code UNIQUE (
+   code
+);
+ALTER TABLE fura.role
    ALTER COLUMN site_id SET NOT NULL
-  ,ALTER COLUMN usr_id SET NOT NULL
-  ,ALTER COLUMN otp_method SET NOT NULL
-  ,ALTER COLUMN used SET NOT NULL
-  ,ALTER COLUMN fail_cnt SET NOT NULL
+  ,ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN status SET NOT NULL
+  ,ALTER COLUMN LEVEL SET NOT NULL
+  ,ALTER COLUMN sess_timeout SET NOT NULL
+  ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
-ALTER TABLE fura.usrotp ADD CONSTRAINT usrotp_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
-ALTER TABLE fura.eatok
+ALTER TABLE fura.role ADD CONSTRAINT role_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
+ALTER TABLE fura.token
+   ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN id SET NOT NULL
+  ,ALTER COLUMN usr_id SET NOT NULL
+  ,ALTER COLUMN date_created SET NOT NULL
+  ,ALTER COLUMN expires SET NOT NULL
+  ,ALTER COLUMN use_cnt SET NOT NULL
+  ,ALTER COLUMN audid SET NOT NULL
+  ,ALTER COLUMN tmstamp SET NOT NULL
+;
+ALTER TABLE fura.token ADD CONSTRAINT token_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
+ALTER TABLE fura.token ADD CONSTRAINT token_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
+ALTER TABLE fura.tokensentry
+   ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN token_cnt SET NOT NULL
+  ,ALTER COLUMN last_poll SET NOT NULL
+;
+ALTER TABLE fura.tokensentry ADD CONSTRAINT tokensentry_fk_site FOREIGN KEY (site_id) REFERENCES fura.site;
+ALTER TABLE fura.usrtype
    ALTER COLUMN id SET NOT NULL
-  ,ALTER COLUMN tok SET NOT NULL
-  ,ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN descr SET NOT NULL
+  ,ALTER COLUMN modified_by SET NOT NULL
+  ,ALTER COLUMN tm_stamp SET NOT NULL
+;
+ALTER TABLE fura.tokenhist
+   ALTER COLUMN site_id SET NOT NULL
+  ,ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN usr_id SET NOT NULL
-  ,ALTER COLUMN func_id SET NOT NULL
-  ,ALTER COLUMN grant_usr_id SET NOT NULL
-  ,ALTER COLUMN created SET NOT NULL
+  ,ALTER COLUMN date_created SET NOT NULL
   ,ALTER COLUMN expires SET NOT NULL
-  ,ALTER COLUMN max_usages SET NOT NULL
-  ,ALTER COLUMN usages SET NOT NULL
+  ,ALTER COLUMN use_cnt SET NOT NULL
+  ,ALTER COLUMN audid SET NOT NULL
+  ,ALTER COLUMN tmstamp SET NOT NULL
 ;
-ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_usr FOREIGN KEY (site_id, usr_id) REFERENCES fura.usr;
-ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_grant FOREIGN KEY (site_id, grant_usr_id) REFERENCES fura.usr;
-ALTER TABLE fura.eatok ADD CONSTRAINT eatok_fk_func FOREIGN KEY (func_id) REFERENCES fura.func;
-ALTER TABLE fura.eatok ADD CONSTRAINT eatok_uk_tok UNIQUE (
-   tok
-  ,site_id
-);
-ALTER TABLE fura.site
+ALTER TABLE fura.config
    ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN descr SET NOT NULL
-  ,ALTER COLUMN status SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
-ALTER TABLE fura.site ADD CONSTRAINT site_uk_code UNIQUE (
-   code
-);
 ALTER TABLE fura.func
    ALTER COLUMN id SET NOT NULL
   ,ALTER COLUMN funcgrp_id SET NOT NULL
   ,ALTER COLUMN descr SET NOT NULL
   ,ALTER COLUMN action SET NOT NULL
   ,ALTER COLUMN oride SET NOT NULL
   ,ALTER COLUMN audit_lvl SET NOT NULL
   ,ALTER COLUMN modified_by SET NOT NULL
   ,ALTER COLUMN tm_stamp SET NOT NULL
 ;
 ALTER TABLE fura.func ADD CONSTRAINT func_fk_funcgrp FOREIGN KEY (funcgrp_id) REFERENCES fura.funcgrp;
-CREATE INDEX usrauth_ix_token ON fura.usrauth
+CREATE INDEX servicesiterel_ix_st ON fura.servicesiterel
 (
-   site_id
-  ,auth_type
-  ,auth_data
+   siteid
+);
+CREATE INDEX servicesiterel_ix_se ON fura.servicesiterel
+(
+   serviceid
 );
 CREATE INDEX usr_ix_role ON fura.usr
 (
    site_id
   ,role_id
 );
 CREATE INDEX usr_ix_usrtype ON fura.usr
@@ -427,14 +519,20 @@
    site_id
   ,usrtype_id
 );
 CREATE INDEX func_ix_funcgrp ON fura.func
 (
    funcgrp_id
 );
+CREATE INDEX usrauth_ix_token ON fura.usrauth
+(
+   site_id
+  ,auth_type
+  ,auth_data
+);
 INSERT INTO audit.cfg SELECT 'fura.config',        'id',                       'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.config');
 INSERT INTO audit.cfg SELECT 'fura.func',          'id',                       'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.func');
 INSERT INTO audit.cfg SELECT 'fura.site',          'id',                       'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.site');
 INSERT INTO audit.cfg SELECT 'fura.sitecfg',       'site_id|id',               'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.sitecfg');
 INSERT INTO audit.cfg SELECT 'fura.role',          'site_id|id',               'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.role');
 INSERT INTO audit.cfg SELECT 'fura.rolefuncrel',   'site_id|role_id|func_id',  'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.rolefuncrel');
 INSERT INTO audit.cfg SELECT 'fura.usr',           'site_id|id',               'modified_by|tm_stamp', NULL, NULL, NULL, 'modified_by', 'M' WHERE NOT EXISTS (SELECT id FROM audit.cfg WHERE id = 'fura.usr');
```

### Comparing `bitsmiths-fura-2.2.2/bs_fura/token_manager.py` & `bitsmiths-fura-2.2.3/bs_fura/token_manager.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/token_sentry_pluggin.py` & `bitsmiths-fura-2.2.3/bs_fura/token_sentry_pluggin.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/user_login.py` & `bitsmiths-fura-2.2.3/bs_fura/user_login.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/user_login_async.py` & `bitsmiths-fura-2.2.3/bs_fura/user_login_async.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/util.py` & `bitsmiths-fura-2.2.3/bs_fura/util.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/bs_fura/xfura.py` & `bitsmiths-fura-2.2.3/bs_fura/xfura.py`

 * *Files identical despite different names*

### Comparing `bitsmiths-fura-2.2.2/setup.cfg` & `bitsmiths-fura-2.2.3/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = bitsmiths-fura
 description = The Bitsmiths Function-User-Role-Authenticator Package
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://bitbucket.org/bitsmiths_za/bitsmiths
 author = Nicolas Milicevic, Steven van Niekerk, Darrly Daniels
 author_email = nicolas@bitsmiths.co.za, steven@bitsmiths.co.za, darryl@bitsmiths.co.za
-version = 2.2.2
+version = 2.2.3
 license = MIT
 license_files = LICENCE
 platforms = unix, linux, osx, cygwin, win32
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
```

### Comparing `bitsmiths-fura-2.2.2/setup.py` & `bitsmiths-fura-2.2.3/setup.py`

 * *Files identical despite different names*

