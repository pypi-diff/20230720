# Comparing `tmp/lamindb_setup-0.48.8.tar.gz` & `tmp/lamindb_setup-0.49.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lamindb_setup-0.48.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "lamindb_setup-0.49.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `lamindb_setup-0.48.8.tar` & `lamindb_setup-0.49.0.tar`

### file list

```diff
@@ -1,99 +1,101 @@
--rw-r--r--   0        0        0     4010 2023-06-21 19:39:29.494297 lamindb_setup-0.48.8/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.48.8/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.48.8/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.48.8/.gitignore
--rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.48.8/.gitmodules
--rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.48.8/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.48.8/LICENSE
--rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.48.8/README.md
--rw-r--r--   0        0        0    57606 2023-07-17 14:59:34.334852 lamindb_setup-0.48.8/docs/changelog.md
--rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.48.8/docs/faq/edge-cases-login-init.ipynb
--rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.48.8/docs/faq/index.md
--rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.48.8/docs/faq/multi-session.ipynb
--rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.48.8/docs/faq/switch-environment.ipynb
--rw-r--r--   0        0        0     6590 2023-06-07 14:57:12.963250 lamindb_setup-0.48.8/docs/faq/test-sqlite-sync.ipynb
--rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.48.8/docs/guide/01-init-instance.ipynb
--rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.48.8/docs/guide/02-load-instance.ipynb
--rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.48.8/docs/guide/03-set-storage.ipynb
--rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.48.8/docs/guide/04-schema-modules.ipynb
--rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.48.8/docs/guide/index.md
--rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.48.8/docs/guide/migrate.md
--rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.48.8/docs/guide/setup-user.md
--rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.48.8/docs/index.md
--rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.48.8/docs/reference.md
--rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.48.8/docs/test_notebooks.py
--rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.48.8/lamin-project.yaml
--rw-r--r--   0        0        0     2757 2023-07-17 14:59:23.981072 lamindb_setup-0.48.8/lamindb_setup/__init__.py
--rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.48.8/lamindb_setup/__main__.py
--rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.48.8/lamindb_setup/_check_instance_setup.py
--rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.48.8/lamindb_setup/_close.py
--rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.48.8/lamindb_setup/_delete.py
--rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.48.8/lamindb_setup/_docstrings.py
--rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.48.8/lamindb_setup/_info.py
--rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.48.8/lamindb_setup/_init_instance.py
--rw-r--r--   0        0        0     6599 2023-07-17 14:58:45.055228 lamindb_setup-0.48.8/lamindb_setup/_load_instance.py
--rw-r--r--   0        0        0     1413 2023-07-03 19:06:33.505992 lamindb_setup-0.48.8/lamindb_setup/_migrate.py
--rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.48.8/lamindb_setup/_notebook.py
--rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.48.8/lamindb_setup/_register_instance.py
--rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.48.8/lamindb_setup/_schema.py
--rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.48.8/lamindb_setup/_set.py
--rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.48.8/lamindb_setup/_settings.py
--rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.48.8/lamindb_setup/_settings_load.py
--rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.48.8/lamindb_setup/_settings_store.py
--rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.48.8/lamindb_setup/_setup_user.py
--rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.48.8/lamindb_setup/_silence_loggers.py
--rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.48.8/lamindb_setup/dev/__init__.py
--rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.48.8/lamindb_setup/dev/_cloud_sqlite_locker.py
--rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.48.8/lamindb_setup/dev/_deprecated.py
--rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.48.8/lamindb_setup/dev/_django.py
--rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.48.8/lamindb_setup/dev/_docs.py
--rw-r--r--   0        0        0     3456 2023-06-18 07:46:49.405332 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_client.py
--rw-r--r--   0        0        0     9074 2023-06-20 11:14:24.335109 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_core.py
--rw-r--r--   0        0        0     3310 2023-06-18 07:46:49.405673 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_crud.py
--rw-r--r--   0        0        0     4129 2023-06-27 14:15:46.405828 lamindb_setup-0.48.8/lamindb_setup/dev/_hub_utils.py
--rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_instance.py
--rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_load.py
--rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_save.py
--rw-r--r--   0        0        0     2318 2023-06-04 20:49:27.328010 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_store.py
--rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.48.8/lamindb_setup/dev/_settings_user.py
--rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.48.8/lamindb_setup/dev/_setup_bionty_sources.py
--rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.48.8/lamindb_setup/dev/_setup_schema.py
--rw-r--r--   0        0        0     4583 2023-07-17 14:58:45.055809 lamindb_setup-0.48.8/lamindb_setup/dev/_storage.py
--rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.48.8/lamindb_setup/dev/upath.py
--rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.48.8/lnschema-core/.github/workflows/build.yml
--rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.48.8/lnschema-core/.gitignore
--rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.48.8/lnschema-core/.pre-commit-config.yaml
--rw-r--r--   0        0        0    29416 2023-06-29 19:17:30.194449 lamindb_setup-0.48.8/lnschema-core/CHANGELOG.md
--rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.48.8/lnschema-core/LICENSE
--rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.48.8/lnschema-core/README.md
--rw-r--r--   0        0        0      617 2023-06-30 11:14:16.252662 lamindb_setup-0.48.8/lnschema-core/lnschema_core/__init__.py
--rw-r--r--   0        0        0     1395 2023-06-12 10:24:01.839707 lamindb_setup-0.48.8/lnschema-core/lnschema_core/_queryset.py
--rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.48.8/lnschema-core/lnschema_core/ids.py
--rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0001_initial.py
--rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
--rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
--rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
--rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
--rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
--rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/__init__.py
--rw-r--r--   0        0        0    23909 2023-06-29 19:17:30.196117 lamindb_setup-0.48.8/lnschema-core/lnschema_core/models.py
--rw-r--r--   0        0        0      951 2023-06-29 19:17:30.196374 lamindb_setup-0.48.8/lnschema-core/lnschema_core/types.py
--rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.48.8/lnschema-core/lnschema_core/users.py
--rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.48.8/lnschema-core/noxfile.py
--rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.48.8/lnschema-core/pyproject.toml
--rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.48.8/lnschema-core/tests/test_integrity.py
--rw-r--r--   0        0        0     1821 2023-06-27 14:15:46.405994 lamindb_setup-0.48.8/noxfile.py
--rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.48.8/pyproject.toml
--rw-r--r--   0        0        0     1169 2023-06-27 14:15:46.406331 lamindb_setup-0.48.8/tests/hub/test_instance.py
--rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.48.8/tests/hub/test_signup_signin.py
--rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.48.8/tests/hub/test_storage.py
--rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.48.8/tests/test_bionty.py
--rw-r--r--   0        0        0     2974 2023-07-17 14:58:45.056044 lamindb_setup-0.48.8/tests/test_init_instance.py
--rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.48.8/tests/test_load_instance.py
--rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.48.8/tests/test_login.py
--rw-r--r--   0        0        0      457 2023-07-03 19:06:33.506543 lamindb_setup-0.48.8/tests/test_migrate.py
--rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.48.8/tests/test_set_storage.py
--rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.48.8/tests/test_signup.py
--rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.48.8/PKG-INFO
+-rw-r--r--   0        0        0     4107 2023-07-19 05:09:05.886717 lamindb_setup-0.49.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-26 12:29:21.559431 lamindb_setup-0.49.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2023-05-26 12:29:21.559519 lamindb_setup-0.49.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1204 2023-05-26 12:29:21.559614 lamindb_setup-0.49.0/.gitignore
+-rw-r--r--   0        0        0      100 2023-05-31 13:45:54.309833 lamindb_setup-0.49.0/.gitmodules
+-rw-r--r--   0        0        0     1798 2023-06-04 10:03:32.189000 lamindb_setup-0.49.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2023-05-26 12:29:21.559824 lamindb_setup-0.49.0/LICENSE
+-rw-r--r--   0        0        0      318 2023-06-04 10:03:32.189263 lamindb_setup-0.49.0/README.md
+-rw-r--r--   0        0        0    58121 2023-07-20 09:34:12.354036 lamindb_setup-0.49.0/docs/changelog.md
+-rw-r--r--   0        0        0     6341 2023-06-04 20:49:27.327815 lamindb_setup-0.49.0/docs/faq/edge-cases-login-init.ipynb
+-rw-r--r--   0        0        0      110 2023-07-03 19:06:33.504162 lamindb_setup-0.49.0/docs/faq/index.md
+-rw-r--r--   0        0        0     1920 2023-07-03 19:06:33.504443 lamindb_setup-0.49.0/docs/faq/multi-session.ipynb
+-rw-r--r--   0        0        0     3323 2023-06-01 11:33:10.499233 lamindb_setup-0.49.0/docs/faq/switch-environment.ipynb
+-rw-r--r--   0        0        0     6645 2023-07-19 05:41:47.618199 lamindb_setup-0.49.0/docs/faq/test-sqlite-sync.ipynb
+-rw-r--r--   0        0        0     7739 2023-07-17 14:58:45.054311 lamindb_setup-0.49.0/docs/guide/01-init-instance.ipynb
+-rw-r--r--   0        0        0     4349 2023-07-17 14:58:45.054634 lamindb_setup-0.49.0/docs/guide/02-load-instance.ipynb
+-rw-r--r--   0        0        0     5640 2023-06-27 14:15:46.405054 lamindb_setup-0.49.0/docs/guide/03-set-storage.ipynb
+-rw-r--r--   0        0        0     2585 2023-07-03 19:06:33.505056 lamindb_setup-0.49.0/docs/guide/04-schema-modules.ipynb
+-rw-r--r--   0        0        0      114 2023-06-08 16:08:38.507384 lamindb_setup-0.49.0/docs/guide/index.md
+-rw-r--r--   0        0        0      409 2023-06-08 16:11:46.528420 lamindb_setup-0.49.0/docs/guide/migrate.md
+-rw-r--r--   0        0        0     1250 2023-06-08 11:34:59.767355 lamindb_setup-0.49.0/docs/guide/setup-user.md
+-rw-r--r--   0        0        0      132 2023-06-08 11:34:59.767485 lamindb_setup-0.49.0/docs/index.md
+-rw-r--r--   0        0        0       61 2023-06-08 11:34:59.767572 lamindb_setup-0.49.0/docs/reference.md
+-rw-r--r--   0        0        0      365 2023-05-31 19:23:44.384942 lamindb_setup-0.49.0/docs/test_notebooks.py
+-rw-r--r--   0        0        0      142 2023-06-04 07:52:11.614112 lamindb_setup-0.49.0/lamin-project.yaml
+-rw-r--r--   0        0        0     2757 2023-07-20 09:34:05.410170 lamindb_setup-0.49.0/lamindb_setup/__init__.py
+-rw-r--r--   0        0        0     5346 2023-06-08 07:33:18.804610 lamindb_setup-0.49.0/lamindb_setup/__main__.py
+-rw-r--r--   0        0        0     2073 2023-07-06 15:56:17.785707 lamindb_setup-0.49.0/lamindb_setup/_check_instance_setup.py
+-rw-r--r--   0        0        0      825 2023-07-03 19:06:33.505307 lamindb_setup-0.49.0/lamindb_setup/_close.py
+-rw-r--r--   0        0        0     2006 2023-06-07 14:57:12.963567 lamindb_setup-0.49.0/lamindb_setup/_delete.py
+-rw-r--r--   0        0        0      585 2023-06-04 19:41:00.163095 lamindb_setup-0.49.0/lamindb_setup/_docstrings.py
+-rw-r--r--   0        0        0      329 2023-06-04 20:17:47.260552 lamindb_setup-0.49.0/lamindb_setup/_info.py
+-rw-r--r--   0        0        0     7485 2023-07-17 14:58:45.054935 lamindb_setup-0.49.0/lamindb_setup/_init_instance.py
+-rw-r--r--   0        0        0     6600 2023-07-20 09:33:22.825129 lamindb_setup-0.49.0/lamindb_setup/_load_instance.py
+-rw-r--r--   0        0        0     1413 2023-07-03 19:06:33.505992 lamindb_setup-0.49.0/lamindb_setup/_migrate.py
+-rw-r--r--   0        0        0     1686 2023-07-02 08:22:26.164664 lamindb_setup-0.49.0/lamindb_setup/_notebook.py
+-rw-r--r--   0        0        0      783 2023-06-18 07:46:49.404472 lamindb_setup-0.49.0/lamindb_setup/_register_instance.py
+-rw-r--r--   0        0        0     1057 2023-06-04 19:41:00.163987 lamindb_setup-0.49.0/lamindb_setup/_schema.py
+-rw-r--r--   0        0        0     2189 2023-06-28 12:29:27.548961 lamindb_setup-0.49.0/lamindb_setup/_set.py
+-rw-r--r--   0        0        0     2247 2023-06-04 20:17:47.260720 lamindb_setup-0.49.0/lamindb_setup/_settings.py
+-rw-r--r--   0        0        0       87 2023-06-01 11:33:10.504660 lamindb_setup-0.49.0/lamindb_setup/_settings_load.py
+-rw-r--r--   0        0        0       72 2023-06-01 11:33:10.504736 lamindb_setup-0.49.0/lamindb_setup/_settings_store.py
+-rw-r--r--   0        0        0     3500 2023-06-18 07:46:49.404887 lamindb_setup-0.49.0/lamindb_setup/_setup_user.py
+-rw-r--r--   0        0        0      785 2023-07-03 12:53:17.048276 lamindb_setup-0.49.0/lamindb_setup/_silence_loggers.py
+-rw-r--r--   0        0        0      456 2023-06-04 20:17:47.260896 lamindb_setup-0.49.0/lamindb_setup/dev/__init__.py
+-rw-r--r--   0        0        0     5999 2023-07-08 22:27:16.811101 lamindb_setup-0.49.0/lamindb_setup/dev/_cloud_sqlite_locker.py
+-rw-r--r--   0        0        0     2491 2023-06-01 11:33:10.505290 lamindb_setup-0.49.0/lamindb_setup/dev/_deprecated.py
+-rw-r--r--   0        0        0    10929 2023-07-06 13:59:07.010192 lamindb_setup-0.49.0/lamindb_setup/dev/_django.py
+-rw-r--r--   0        0        0      240 2023-06-01 11:33:10.505462 lamindb_setup-0.49.0/lamindb_setup/dev/_docs.py
+-rw-r--r--   0        0        0     3652 2023-07-19 05:09:05.887280 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_client.py
+-rw-r--r--   0        0        0    11191 2023-07-20 09:33:22.825771 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_core.py
+-rw-r--r--   0        0        0     4153 2023-07-20 09:33:22.826619 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_crud.py
+-rw-r--r--   0        0        0     4854 2023-07-20 09:33:22.827427 lamindb_setup-0.49.0/lamindb_setup/dev/_hub_utils.py
+-rw-r--r--   0        0        0     9341 2023-07-17 14:58:45.055527 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_instance.py
+-rw-r--r--   0        0        0     2597 2023-06-01 11:33:10.505847 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_load.py
+-rw-r--r--   0        0        0     2061 2023-06-01 11:33:10.505931 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_save.py
+-rw-r--r--   0        0        0     2318 2023-07-18 04:17:11.571437 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_store.py
+-rw-r--r--   0        0        0     1088 2023-06-01 11:33:10.506112 lamindb_setup-0.49.0/lamindb_setup/dev/_settings_user.py
+-rw-r--r--   0        0        0     2338 2023-06-15 12:55:27.026063 lamindb_setup-0.49.0/lamindb_setup/dev/_setup_bionty_sources.py
+-rw-r--r--   0        0        0     2175 2023-06-19 15:23:54.026636 lamindb_setup-0.49.0/lamindb_setup/dev/_setup_schema.py
+-rw-r--r--   0        0        0     4583 2023-07-17 14:58:45.055809 lamindb_setup-0.49.0/lamindb_setup/dev/_storage.py
+-rw-r--r--   0        0        0     2704 2023-06-13 20:05:14.115984 lamindb_setup-0.49.0/lamindb_setup/dev/upath.py
+-rw-r--r--   0        0        0      841 2023-06-29 19:17:30.193448 lamindb_setup-0.49.0/lnschema-core/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2023-05-30 14:21:30.384240 lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      592 2023-06-12 10:24:01.838671 lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1381 2023-05-30 14:21:30.384442 lamindb_setup-0.49.0/lnschema-core/.gitignore
+-rw-r--r--   0        0        0     1843 2023-06-29 19:17:30.194142 lamindb_setup-0.49.0/lnschema-core/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    31175 2023-07-17 17:14:39.802147 lamindb_setup-0.49.0/lnschema-core/CHANGELOG.md
+-rw-r--r--   0        0        0    11324 2023-05-30 14:21:30.384784 lamindb_setup-0.49.0/lnschema-core/LICENSE
+-rw-r--r--   0        0        0      295 2023-06-29 19:17:30.195186 lamindb_setup-0.49.0/lnschema-core/README.md
+-rw-r--r--   0        0        0      508 2023-07-17 17:14:39.802828 lamindb_setup-0.49.0/lnschema-core/lnschema_core/__init__.py
+-rw-r--r--   0        0        0     1639 2023-06-29 19:17:30.195527 lamindb_setup-0.49.0/lnschema-core/lnschema_core/ids.py
+-rw-r--r--   0        0        0    11062 2023-06-29 19:17:30.195668 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0001_initial.py
+-rw-r--r--   0        0        0      417 2023-06-29 19:17:30.195747 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0002_alter_user_name.py
+-rw-r--r--   0        0        0      630 2023-06-29 19:17:30.195803 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py
+-rw-r--r--   0        0        0     1940 2023-06-29 19:17:30.195868 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py
+-rw-r--r--   0        0        0      620 2023-06-29 19:17:30.195921 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py
+-rw-r--r--   0        0        0     3113 2023-06-29 19:17:30.195965 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py
+-rw-r--r--   0        0        0      948 2023-07-17 17:14:39.802921 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0007_feature_synonyms_featureset_field_and_more.py
+-rw-r--r--   0        0        0      655 2023-07-17 17:14:39.802992 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0008_file_hash_type_transform_parents.py
+-rw-r--r--   0        0        0        0 2023-05-30 14:21:30.387900 lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/__init__.py
+-rw-r--r--   0        0        0       92 2023-07-17 17:14:39.803051 lamindb_setup-0.49.0/lnschema-core/lnschema_core/mocks.py
+-rw-r--r--   0        0        0    33218 2023-07-17 17:14:39.803249 lamindb_setup-0.49.0/lnschema-core/lnschema_core/models.py
+-rw-r--r--   0        0        0      969 2023-07-17 17:14:39.803366 lamindb_setup-0.49.0/lnschema-core/lnschema_core/types.py
+-rw-r--r--   0        0        0      218 2023-06-12 10:24:01.840812 lamindb_setup-0.49.0/lnschema-core/lnschema_core/users.py
+-rw-r--r--   0        0        0      387 2023-06-29 19:17:30.196558 lamindb_setup-0.49.0/lnschema-core/noxfile.py
+-rw-r--r--   0        0        0      932 2023-06-29 19:17:30.196644 lamindb_setup-0.49.0/lnschema-core/pyproject.toml
+-rw-r--r--   0        0        0      243 2023-06-29 19:17:30.196726 lamindb_setup-0.49.0/lnschema-core/tests/test_integrity.py
+-rw-r--r--   0        0        0     2055 2023-07-19 05:09:05.887435 lamindb_setup-0.49.0/noxfile.py
+-rw-r--r--   0        0        0     1101 2023-06-27 14:15:46.406161 lamindb_setup-0.49.0/pyproject.toml
+-rw-r--r--   0        0        0     1170 2023-07-20 09:33:22.827762 lamindb_setup-0.49.0/tests/hub/test_instance.py
+-rw-r--r--   0        0        0      351 2023-06-27 14:15:46.406460 lamindb_setup-0.49.0/tests/hub/test_signup_signin.py
+-rw-r--r--   0        0        0      874 2023-06-27 14:15:46.406593 lamindb_setup-0.49.0/tests/hub/test_storage.py
+-rw-r--r--   0        0        0       45 2023-06-18 07:46:49.406456 lamindb_setup-0.49.0/tests/test_bionty.py
+-rw-r--r--   0        0        0     2974 2023-07-17 14:58:45.056044 lamindb_setup-0.49.0/tests/test_init_instance.py
+-rw-r--r--   0        0        0      694 2023-06-15 00:10:45.075741 lamindb_setup-0.49.0/tests/test_load_instance.py
+-rw-r--r--   0        0        0      501 2023-06-08 11:34:59.767695 lamindb_setup-0.49.0/tests/test_login.py
+-rw-r--r--   0        0        0      457 2023-07-03 19:06:33.506543 lamindb_setup-0.49.0/tests/test_migrate.py
+-rw-r--r--   0        0        0      243 2023-06-01 11:33:10.508784 lamindb_setup-0.49.0/tests/test_set_storage.py
+-rw-r--r--   0        0        0      125 2023-06-08 11:34:59.767783 lamindb_setup-0.49.0/tests/test_signup.py
+-rw-r--r--   0        0        0     1460 1970-01-01 00:00:00.000000 lamindb_setup-0.49.0/PKG-INFO
```

### Comparing `lamindb_setup-0.48.8/.github/workflows/build.yml` & `lamindb_setup-0.49.0/.github/workflows/build.yml`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,17 @@
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9"]
         group:
           - "unit"
           - "docs"
+        lamin_env:
+          - "staging"
+          - "prod"
     timeout-minutes: 20
 
     steps:
       - name: Checkout main
         uses: actions/checkout@v3
         with:
           fetch-depth: 0
@@ -70,15 +73,15 @@
           aws-secret-access-key: ${{ secrets.AWS_SECRET_ACCESS_KEY }}
           aws-region: eu-central-1
       # - uses: "google-github-actions/auth@v0"
       #   with:
       #     credentials_json: "${{ secrets.GCP_CREDENTIALS }}"
       # - uses: "google-github-actions/setup-gcloud@v0"
       - run: nox -s "install(group='${{ matrix.group }}')"
-      - run: nox -s "build(group='${{ matrix.group }}')"
+      - run: nox -s "build(lamin_env='${{ matrix.lamin_env }}', group='${{ matrix.group }}')"
         env:
           SUPABASE_STAGING_URL: ${{ secrets.SUPABASE_STAGING_URL }}
           SUPABASE_STAGING_ANON_KEY: ${{ secrets.SUPABASE_STAGING_ANON_KEY }}
       - name: upload coverage
         uses: actions/upload-artifact@v2
         with:
           name: coverage--${{ matrix.group }}
```

### Comparing `lamindb_setup-0.48.8/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/.gitignore` & `lamindb_setup-0.49.0/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/.pre-commit-config.yaml` & `lamindb_setup-0.49.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/LICENSE` & `lamindb_setup-0.49.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/changelog.md` & `lamindb_setup-0.49.0/docs/changelog.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🗃️ Enable multiple DB access roles in instances (decompose connection string) | [431](https://github.com/laminlabs/lamindb-setup/pull/431) | [bpenteado](https://github.com/bpenteado) | 2023-07-19 | 0.49.0
+💚 Fix instability | [441](https://github.com/laminlabs/lamindb-setup/pull/441) | [falexwolf](https://github.com/falexwolf) | 2023-07-19 |
+👷 Run CI against the staging environment | [440](https://github.com/laminlabs/lamindb-setup/pull/440) | [bpenteado](https://github.com/bpenteado) | 2023-07-18 |
 ♻️ Simplify `StorageSettings` | [439](https://github.com/laminlabs/lamindb-setup/pull/439) | [falexwolf](https://github.com/falexwolf) | 2023-07-17 | 0.48.8
 🔒️ Increase locker expiration time to 1 week | [437](https://github.com/laminlabs/lamindb-setup/pull/437) | [Koncopd](https://github.com/Koncopd) | 2023-07-08 | 0.48.7
 🚸 Import order of schema modules shouldn't matter | [436](https://github.com/laminlabs/lamindb-setup/pull/436) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.6
 🚸 Deal with legacy instances | [435](https://github.com/laminlabs/lamindb-setup/pull/435) | [falexwolf](https://github.com/falexwolf) | 2023-07-06 | 0.48.5
 🚸 Raise more errors in API when instance is setup | [434](https://github.com/laminlabs/lamindb-setup/pull/434) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.48.3
 🚸 Silence loggers and close instance during init & load | [433](https://github.com/laminlabs/lamindb-setup/pull/433) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.48.2
 🐛 Fix sqlite file not existing in the bucket error | [432](https://github.com/laminlabs/lamindb-setup/pull/432) | [Koncopd](https://github.com/Koncopd) | 2023-06-28 | 0.48.1
```

### Comparing `lamindb_setup-0.48.8/docs/faq/edge-cases-login-init.ipynb` & `lamindb_setup-0.49.0/docs/faq/edge-cases-login-init.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/faq/multi-session.ipynb` & `lamindb_setup-0.49.0/docs/faq/multi-session.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/faq/switch-environment.ipynb` & `lamindb_setup-0.49.0/docs/faq/switch-environment.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/faq/test-sqlite-sync.ipynb` & `lamindb_setup-0.49.0/docs/faq/test-sqlite-sync.ipynb`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9982878904249872%*

 * *Differences: {"'cells'": "{1: {'source': {insert: [(0, 'import os\\n'), (1, '\\n'), (2, 'instance_name = "*

 * *            'f"lamindb-setup-ci-test-sqlite-sync-{os.environ[\\\'LAMIN_ENV\\\']}"\\n\')], delete: '*

 * *            '[0]}}}',*

 * * "'metadata'": "{'language_info': {'version': '3.9.16'}}"}*

```diff
@@ -12,15 +12,17 @@
         {
             "cell_type": "code",
             "execution_count": null,
             "id": "6e685a68",
             "metadata": {},
             "outputs": [],
             "source": [
-                "instance_name = f\"lamindb-setup-ci-test-sqlite-sync\"\n",
+                "import os\n",
+                "\n",
+                "instance_name = f\"lamindb-setup-ci-test-sqlite-sync-{os.environ['LAMIN_ENV']}\"\n",
                 "!lamin load {instance_name}\n",
                 "!lamin delete {instance_name}"
             ]
         },
         {
             "cell_type": "code",
             "execution_count": null,
@@ -324,15 +326,15 @@
                 "version": 3
             },
             "file_extension": ".py",
             "mimetype": "text/x-python",
             "name": "python",
             "nbconvert_exporter": "python",
             "pygments_lexer": "ipython3",
-            "version": "3.9.15"
+            "version": "3.9.16"
         },
         "vscode": {
             "interpreter": {
                 "hash": "b0fa6594d8f4cbf19f97940f81e996739fb7646882a419484c72d19e05852a7e"
             }
         }
     },
```

### Comparing `lamindb_setup-0.48.8/docs/guide/01-init-instance.ipynb` & `lamindb_setup-0.49.0/docs/guide/01-init-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/guide/02-load-instance.ipynb` & `lamindb_setup-0.49.0/docs/guide/02-load-instance.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/guide/03-set-storage.ipynb` & `lamindb_setup-0.49.0/docs/guide/03-set-storage.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/guide/04-schema-modules.ipynb` & `lamindb_setup-0.49.0/docs/guide/04-schema-modules.ipynb`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/docs/guide/setup-user.md` & `lamindb_setup-0.49.0/docs/guide/setup-user.md`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/__init__.py` & `lamindb_setup-0.49.0/lamindb_setup/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -48,15 +48,15 @@
 .. autosummary::
    :toctree:
 
    dev
 """
 
 
-__version__ = "0.48.8"  # denote a release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.49.0"  # denote a release candidate for 0.1.0 with 0.1rc1
 
 import builtins
 import sys
 from os import name as _os_name
 
 from . import dev
 from ._check_instance_setup import check_instance_setup as _check_instance_setup  # noqa
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/__main__.py` & `lamindb_setup-0.49.0/lamindb_setup/__main__.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_check_instance_setup.py` & `lamindb_setup-0.49.0/lamindb_setup/_check_instance_setup.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_close.py` & `lamindb_setup-0.49.0/lamindb_setup/_close.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_delete.py` & `lamindb_setup-0.49.0/lamindb_setup/_delete.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_docstrings.py` & `lamindb_setup-0.49.0/lamindb_setup/_docstrings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_init_instance.py` & `lamindb_setup-0.49.0/lamindb_setup/_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_load_instance.py` & `lamindb_setup-0.49.0/lamindb_setup/_load_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,14 +49,15 @@
             close_instance(mute=True)
 
     from .dev._hub_core import load_instance as load_instance_from_hub
 
     hub_result = load_instance_from_hub(
         owner=owner, name=name, _access_token=_access_token
     )
+
     # if hub_result is not a string, it means it made a request
     # that successfully returned metadata
     if not isinstance(hub_result, str):
         instance_result, storage_result = hub_result
         isettings = InstanceSettings(
             owner=owner,
             name=name,
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_migrate.py` & `lamindb_setup-0.49.0/lamindb_setup/_migrate.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_notebook.py` & `lamindb_setup-0.49.0/lamindb_setup/_notebook.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_register_instance.py` & `lamindb_setup-0.49.0/lamindb_setup/_register_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_schema.py` & `lamindb_setup-0.49.0/lamindb_setup/_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_set.py` & `lamindb_setup-0.49.0/lamindb_setup/_set.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_settings.py` & `lamindb_setup-0.49.0/lamindb_setup/_settings.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_setup_user.py` & `lamindb_setup-0.49.0/lamindb_setup/_setup_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/_silence_loggers.py` & `lamindb_setup-0.49.0/lamindb_setup/_silence_loggers.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_cloud_sqlite_locker.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_cloud_sqlite_locker.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_deprecated.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_deprecated.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_django.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_django.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_client.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,17 +85,21 @@
         )
         return auth_response.session.access_token
     finally:
         hub.auth.sign_out()
 
 
 def lamindb_client_config_settings(settings: BaseSettings) -> Dict[str, Any]:
-    connector_file, _ = urlretrieve(
-        "https://lamin-site-assets.s3.amazonaws.com/connector.env"
-    )
+    if os.getenv("LAMIN_ENV") == "staging":
+        connector_path = (
+            "https://lamin-site-assets.s3.amazonaws.com/connector_staging.env"
+        )
+    else:
+        connector_path = "https://lamin-site-assets.s3.amazonaws.com/connector.env"
+    connector_file, _ = urlretrieve(connector_path)
     connector = Connector(_env_file=connector_file)
     return dict(
         lamin_env="client",
         supabase_api_url=connector.url,
         supabase_anon_key=connector.key,
     )
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_core.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_core.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,22 +4,26 @@
 
 from lamin_logger import logger
 from postgrest.exceptions import APIError
 
 from ._hub_client import connect_hub, connect_hub_with_auth, get_lamin_site_base_url
 from ._hub_crud import (
     sb_insert_collaborator,
+    sb_insert_db_user,
     sb_insert_instance,
     sb_insert_storage,
     sb_select_account_by_handle,
+    sb_select_db_user_by_instance,
     sb_select_instance_by_name,
     sb_select_storage,
     sb_select_storage_by_root,
 )
 from ._hub_utils import (
+    LaminDsn,
+    LaminDsnModel,
     base62,
     get_storage_region,
     get_storage_type,
     secret,
     validate_db_arg,
     validate_schema_arg,
     validate_storage_root_arg,
@@ -95,14 +99,17 @@
     )
     try:
         # validate input arguments
         schema_str = validate_schema_arg(schema)
         # storage is validated in add_storage
         validate_db_arg(db)
 
+        if db:
+            db_dsn = LaminDsnModel(db=db)
+
         # get account
         account = sb_select_account_by_handle(owner, hub)
         if account is None:
             return "account-not-exists"
 
         # get storage and add if not yet there
         storage_root = storage.rstrip("/")  # current fix because of upath migration
@@ -118,37 +125,68 @@
             return "instance-exists-already"
 
         validate_unique_sqlite(
             hub=hub, db=db, storage_id=storage_id, name=name, account=account
         )
 
         instance_id = uuid4().hex
+        db_user_id = uuid4().hex
 
-        sb_insert_instance(
-            {
-                "id": instance_id,
-                "account_id": account["id"],
-                "name": name,
-                "storage_id": storage_id,
-                "db": db,
-                "schema_str": schema_str,
-                "public": False if public is None else public,
-                "description": description,
-            },
-            hub,
-        )
-
-        sb_insert_collaborator(
-            {
-                "instance_id": instance_id,
-                "account_id": account["id"],
-                "role": "admin",
-            },
-            hub,
-        )
+        if db_dsn:
+            instance = sb_insert_instance(  # noqa
+                {
+                    "id": instance_id,
+                    "account_id": account["id"],
+                    "name": name,
+                    "storage_id": storage_id,
+                    "db": db,
+                    "db_scheme": db_dsn.db.scheme,
+                    "db_host": db_dsn.db.host,
+                    "db_port": db_dsn.db.port,
+                    "db_database": db_dsn.db.database,
+                    "schema_str": schema_str,
+                    "public": False if public is None else public,
+                    "description": description,
+                },
+                hub,
+            )
+
+            db_user = sb_insert_db_user(  # noqa
+                {
+                    "id": db_user_id,
+                    "instance_id": instance_id,
+                    "db_user_name": db_dsn.db.user,
+                    "db_user_password": db_dsn.db.password,
+                },
+                hub,
+            )
+        else:
+            sb_insert_instance(
+                {
+                    "id": instance_id,
+                    "account_id": account["id"],
+                    "name": name,
+                    "storage_id": storage_id,
+                    "db": db,
+                    "schema_str": schema_str,
+                    "public": False if public is None else public,
+                    "description": description,
+                },
+                hub,
+            )
+
+            sb_insert_collaborator(
+                {
+                    "instance_id": instance_id,
+                    "account_id": account["user_id"],
+                    "db_user_id": db_user_id,
+                    "role": "admin",
+                },
+                hub,
+            )
 
         # upon successful insert of a new row in the instance table
         # (and all associated tables), return None
         # clients test for this return value, hence, don't change it
         return None
     except APIError as api_error:
         uq_instance_db_error = (
@@ -180,14 +218,33 @@
         if account is None:
             return "account-not-exists"
 
         instance = sb_select_instance_by_name(account["id"], name, hub)
         if instance is None:
             return "instance-not-reachable"
 
+        if not (instance["db"] is None or instance["db"].startswith("sqlite://")):
+            # get db_account
+            db_user = sb_select_db_user_by_instance(instance["id"], hub)
+            if db_user is None:
+                return "db-user-not-reachable"
+
+            # construct dsn from instance and db_account fields
+            db_dsn = LaminDsn.build(
+                scheme=instance["db_scheme"],
+                user=db_user["db_user_name"],
+                password=db_user["db_user_password"],
+                host=instance["db_host"],
+                port=str(instance["db_port"]),
+                database=instance["db_database"],
+            )
+
+            # override the db string with the constructed dsn
+            instance["db"] = db_dsn
+
         # get default storage
         storage = sb_select_storage(instance["storage_id"], hub)
         if storage is None:
             return "storage-does-not-exist-on-hub"
 
         return instance, storage
     except Exception:
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_crud.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_crud.py`

 * *Files 10% similar despite different names*

```diff
@@ -114,7 +114,37 @@
 
 
 def sb_select_storage_by_root(root: str, supabase_client: Client):
     data = supabase_client.table("storage").select("*").eq("root", root).execute().data
     if len(data) == 0:
         return None
     return data[0]
+
+
+# --------------- DBUser ----------------------
+def sb_insert_db_user(instance_fields: dict, supabase_client: Client):
+    try:
+        data = supabase_client.table("db_user").insert(instance_fields).execute().data
+    except Exception as e:
+        if str(e) == str("Expecting value: line 1 column 1 (char 0)"):
+            pass
+        else:
+            raise e
+    return data[0]
+
+
+def sb_select_db_user_by_instance(instance_id: str, supabase_client: Client):
+    """Get the DBAccount directly associated with Instance.
+
+    By contrast this is not the DBAccount that is linked through the
+    UserInstance table.
+    """
+    data = (
+        supabase_client.table("db_user")
+        .select("*")
+        .eq("instance_id", instance_id)
+        .execute()
+        .data
+    )
+    if len(data) == 0:
+        return None
+    return data[0]
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_hub_utils.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_hub_utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,13 +1,16 @@
 import secrets
 import string
 from pathlib import Path
 from typing import Mapping, Optional, Union
 from uuid import UUID
 
+from pydantic import BaseModel, validator
+from pydantic.networks import MultiHostDsn
+
 from .upath import UPath
 
 
 def base62(n_char: int) -> str:
     """Like nanoid without hyphen and underscore."""
     alphabet = string.digits + string.ascii_letters.swapcase()
     id = "".join(secrets.choice(alphabet) for i in range(n_char))
@@ -25,27 +28,16 @@
     # currently no actual validation, can add back if we see a need
     # the following just strips white spaces
     to_be_validated = [s.strip() for s in schema.split(",")]
     return ",".join(to_be_validated)
 
 
 def validate_db_arg(db: Optional[str]) -> None:
-    if db is not None:
-        if db.startswith("postgres") and not db.startswith("postgresql"):
-            raise ValueError(
-                "Please follow the SQLAlchemy convention of prefixing the connection"
-                " string with 'postgresql://' instead of 'postgres://'"
-            )
-        if not db.startswith("postgresql"):
-            raise ValueError("Only postgres connection strings are allowed.")
-        if not len(db.split("://")) == 2:
-            raise ValueError("Your postgres URI does not contain '://'")
-        remainder = db.split("://")[1]
-        if not len(remainder.split("/")) == 2:
-            raise ValueError("Your postgres URI does not end with a database '/dbname'")
+    if db:
+        LaminDsnModel(db=db)
 
 
 def validate_unique_sqlite(
     *, hub, db: Optional[str], storage_id: UUID, name: str, account: Mapping
 ) -> None:
     # if a remote sqlite instance, make sure there is no other instance
     # that has the same name and storage location
@@ -114,7 +106,63 @@
 def get_storage_type(storage_root: str):
     if str(storage_root).startswith("s3://"):
         return "s3"
     elif str(storage_root).startswith("gs://"):
         return "gs"
     else:
         return "local"
+
+
+class LaminDsn(MultiHostDsn):
+    """Custom DSN Type for Lamin.
+
+    This class allows us to customize the allowed schemes for databases
+    and also handles the parsing and building of DSN strings with the
+    database name instead of URL path.
+    """
+
+    allowed_schemes = {
+        "postgresql",
+        # future enabled schemes
+        # "snowflake",
+        # "bigquery"
+    }
+    user_required = True
+    __slots__ = ()
+
+    @property
+    def database(self):
+        return self.path[1:]
+
+    @classmethod
+    def build(
+        cls,
+        *,
+        scheme: str,
+        user: Optional[str] = None,
+        password: Optional[str] = None,
+        host: str,
+        port: Optional[str] = None,
+        database: Optional[str] = None,
+        query: Optional[str] = None,
+        fragment: Optional[str] = None,
+        **_kwargs: str,
+    ) -> str:
+        return super().build(
+            scheme=scheme,
+            user=user,
+            password=password,
+            host=host,
+            port=port,
+            path=f"/{database}",
+            query=query,
+            fragment=fragment,
+        )
+
+
+class LaminDsnModel(BaseModel):
+    db: LaminDsn
+
+    @validator("db")
+    def check_db_name(cls, v):
+        assert v.path and len(v.path) > 1, "database must be provided"
+        return v
```

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_instance.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_load.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_load.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_save.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_save.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_store.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_store.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_settings_user.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_settings_user.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_setup_bionty_sources.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_setup_bionty_sources.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_setup_schema.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_setup_schema.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/_storage.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lamindb_setup/dev/upath.py` & `lamindb_setup-0.49.0/lamindb_setup/dev/upath.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/.github/workflows/build.yml` & `lamindb_setup-0.49.0/lnschema-core/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/.github/workflows/latest-changes.yml` & `lamindb_setup-0.49.0/lnschema-core/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/.gitignore` & `lamindb_setup-0.49.0/lnschema-core/.gitignore`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/.pre-commit-config.yaml` & `lamindb_setup-0.49.0/lnschema-core/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/CHANGELOG.md` & `lamindb_setup-0.49.0/lnschema-core/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🍱 Added more methods for signature | [224](https://github.com/laminlabs/lnschema-core/pull/224) | [sunnyosun](https://github.com/sunnyosun) | 2023-07-17 |
+🚚 Add `Transform.parents` and `File.hash_type` | [223](https://github.com/laminlabs/lnschema-core/pull/223) | [falexwolf](https://github.com/falexwolf) | 2023-07-07 | 0.38.3
+✨ Add `from_df` and `from_anndata` to `File` | [222](https://github.com/laminlabs/lnschema-core/pull/222) | [falexwolf](https://github.com/falexwolf) | 2023-07-05 | 0.38.2
+💄 Do not show None fields | [221](https://github.com/laminlabs/lnschema-core/pull/221) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 | 0.38.1
+🚚 Move `QuerySet` to lamindb | [220](https://github.com/laminlabs/lnschema-core/pull/220) | [falexwolf](https://github.com/falexwolf) | 2023-07-03 |
+✨ Allow for annotate in `.df()` | [219](https://github.com/laminlabs/lnschema-core/pull/219) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 |
+🚚 Rename `File.name` to `File.description` | [218](https://github.com/laminlabs/lnschema-core/pull/218) | [falexwolf](https://github.com/falexwolf) | 2023-07-02 | 0.38.0
+🚚 Update `Feature` and `FeatureSet` | [217](https://github.com/laminlabs/lnschema-core/pull/217) | [falexwolf](https://github.com/falexwolf) | 2023-07-01 |
+💄 Prettify dataframe display | [216](https://github.com/laminlabs/lnschema-core/pull/216) | [falexwolf](https://github.com/falexwolf) | 2023-06-30 |
+📝 Fix docs | [215](https://github.com/laminlabs/lnschema-core/pull/215) | [falexwolf](https://github.com/falexwolf) | 2023-06-30 | 0.37.0
+🚚 Move `File` docstrings and signatures | [214](https://github.com/laminlabs/lnschema-core/pull/214) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
 🚚 Rename `BaseORM` to `ORM`, move `ORM` signatures here | [213](https://github.com/laminlabs/lnschema-core/pull/213) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 |
 ✨ Add `Dataset` & `Feature` ORMs | [212](https://github.com/laminlabs/lnschema-core/pull/212) | [falexwolf](https://github.com/falexwolf) | 2023-06-29 | 0.37a1
 💄 Denoise display of timestamps | [211](https://github.com/laminlabs/lnschema-core/pull/211) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 |
 🎨 Auto-manage `RunInput` relationship | [210](https://github.com/laminlabs/lnschema-core/pull/210) | [falexwolf](https://github.com/falexwolf) | 2023-06-26 | 0.36.1
 🚚 Repurpose `Folder` to `Tag` | [209](https://github.com/laminlabs/lnschema-core/pull/209) | [falexwolf](https://github.com/falexwolf) | 2023-06-22 | 0.36.0
 🚚 Move `BaseORM.__init__` to lamindb | [208](https://github.com/laminlabs/lnschema-core/pull/208) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 | 0.35.10
 🚚 Expand field length `short_name` in transform | [207](https://github.com/laminlabs/lnschema-core/pull/207) | [falexwolf](https://github.com/falexwolf) | 2023-06-19 |
```

### Comparing `lamindb_setup-0.48.8/lnschema-core/LICENSE` & `lamindb_setup-0.49.0/lnschema-core/LICENSE`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/ids.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/ids.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0001_initial.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0003_alter_storage_region_alter_transform_short_name.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0004_rename_folder_tag_alter_project_folders.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0005_alter_run_inputs_delete_runinput.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/migrations/0006_feature_dataset.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/models.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,84 +1,107 @@
 import builtins
+from datetime import datetime
+from pathlib import Path
 from typing import (  # noqa
     TYPE_CHECKING,
     Any,
     Dict,
     Iterable,
     List,
     Literal,
     NamedTuple,
     Optional,
     Union,
     overload,
 )
 
 from django.db import models
-from django.db.models import PROTECT, CharField, Manager, TextField
+from django.db.models import PROTECT
+from django.db.models.query_utils import DeferredAttribute as Field
+from upath import UPath
 
-from lnschema_core.types import ListLike, StrField
+from lnschema_core.mocks import AnnDataAccessor, BackedAccessor, QuerySet
+from lnschema_core.types import AnnDataLike, DataLike, ListLike, PathLike, StrField
 
-from ._queryset import QuerySet
 from .ids import base62_8, base62_12, base62_20
 from .types import TransformType
 from .users import current_user_id
 
 if TYPE_CHECKING:
     import pandas as pd
 
-is_run_from_ipython = getattr(builtins, "__IPYTHON__", False)
-TRANSFORM_TYPE_DEFAULT = TransformType.notebook if is_run_from_ipython else TransformType.pipeline
+IPYTHON = getattr(builtins, "__IPYTHON__", False)
+TRANSFORM_TYPE_DEFAULT = TransformType.notebook if IPYTHON else TransformType.pipeline
 
 
 class ORM(models.Model):
     """LaminDB's base ORM.
 
     Is based on `django.db.models.Model`.
+
+    Why does LaminDB call it `ORM` and not `Model`? The term "ORM" can't lead to
+    confusion with statistical, machine learning or biological models.
     """
 
-    def add_synonym(self, synonym: Union[str, ListLike], force: bool = False):
+    def add_synonym(
+        self,
+        synonym: Union[str, ListLike],
+        force: bool = False,
+        save: Optional[bool] = None,
+    ):
         """Add synonyms to a record."""
         pass
 
     def remove_synonym(self, synonym: Union[str, ListLike]):
         """Remove synonyms from a record."""
         pass
 
+    def describe(self):
+        """Rich representation of a record with relationships."""
+        pass
+
+    def view_parents(self, field: Optional[StrField] = None, distance: int = 100):
+        """View parents of a record in a graph."""
+        pass
+
+    def set_abbr(self, value: str):
+        """Set value for abbr field."""
+        pass
+
     @classmethod
-    def from_values(cls, identifiers: ListLike, field: StrField, **kwargs):
+    def from_values(cls, identifiers: ListLike, field: StrField, **kwargs) -> List["ORM"]:
         """Parse values for an identifier (a name, an id, etc.) and create records.
 
         This method helps avoid problems around duplication of entries,
         violation of idempotency, and performance when creating records in bulk.
 
         Guide: :doc:`/biology/registries`.
 
         Args:
-            identifiers: `ListLike` A list of values for an identifier, e.g.
-                `["name1", "name2"]`.
-            field: `StrField` If `iterable` is `ListLike`, an `ORM` field to look
-                up, e.g. `lb.CellMarker.name`.
-            **kwargs: Can contain `species`. Either `"human"`, `"mouse"`, or any other
-                `name` of `Bionty.Species`. If `None`, will use default species in
+            identifiers: ``ListLike`` A list of values for an identifier, e.g.
+                ``["name1", "name2"]``.
+            field: ``StrField`` An ``ORM`` field to look up, e.g., ``lb.CellMarker.name``.
+            **kwargs: Can contain ``species``. Either ``"human"``, ``"mouse"``, or any other
+                `name` of `Bionty.Species`. If ``None``, will use default species in
                 bionty for each entity.
 
         Returns:
             A list of records.
 
-        For every `value` in an iterable of identifiers and a given `ORM.field`,
+        For every ``value`` in a list-like of identifiers and a given `ORM.field`,
         this function performs:
 
         1. It checks whether the value already exists in the database
-        (`ORM.select(field=value)`). If so, it adds the queried record to
-        the returned list and skips step 2. Otherwise, proceed with 2.
-        2. If the `ORM` is from `lnschema_bionty`, it checks whether there is an
-        exact match in the underlying ontology (`Bionty.inspect(value, field)`).
-        If so, it creates a record from Bionty and adds it to the returned list.
-        Otherwise, it creates a record that populates a single field using `value`
-        and adds the record to the returned list.
+           (``ORM.select(field=value)``). If so, it adds the queried record to
+           the returned list and skips step 2. Otherwise, proceed with 2.
+        2. If the ``ORM`` is from ``lnschema_bionty``, it checks whether there is an
+           exact match in the underlying ontology (``Bionty.inspect(value, field)``).
+           If so, it creates a record from Bionty and adds it to the returned list.
+           Otherwise, it creates a record that populates a single field using `value`
+           and adds the record to the returned list.
         """
         pass
 
     @classmethod
     def inspect(
         cls,
         identifiers: ListLike,
@@ -140,15 +163,14 @@
         cls,
         synonyms: Iterable,
         *,
         return_mapper: bool = False,
         case_sensitive: bool = False,
         keep: Literal["first", "last", False] = "first",
         synonyms_field: str = "synonyms",
-        synonyms_sep: str = "|",
         field: Optional[str] = None,
         **kwargs,
     ) -> Union[List[str], Dict[str, str]]:
         """Maps input synonyms to standardized names.
 
         Args:
             synonyms: `Iterable` Synonyms that will be standardized.
@@ -160,77 +182,76 @@
                 multiple names, determines which duplicates to mark as
                 `pd.DataFrame.duplicated`
 
                     - "first": returns the first mapped standardized name
                     - "last": returns the last mapped standardized name
                     - `False`: returns all mapped standardized name
             synonyms_field: `str = "synonyms"` A field containing the concatenated synonyms.
-            synonyms_sep: `str = "|"` Which separator is used to separate synonyms.
             field: `Optional[str]` The field representing the standardized names.
 
         Returns:
             If `return_mapper` is `False`: a list of standardized names. Otherwise,
             a dictionary of mapped values with mappable synonyms as keys and
             standardized names as values.
 
         Examples:
             >>> import lnschema_bionty as lb
             >>> gene_synonyms = ["A1CF", "A1BG", "FANCD1", "FANCD20"]
             >>> standardized_names = lb.Gene.map_synonyms(gene_synonyms, species="human")
         """
 
     @classmethod
-    def select(cls, **expressions) -> Union[QuerySet, Manager]:
+    def select(cls, **expressions) -> QuerySet:
         """Query records.
 
         Guide: :doc:`/guide/select`.
 
         Args:
-            ORM: An ORM class.
             expressions: Fields and values passed as Django query expressions.
 
         Returns:
-            A `QuerySet` or Django `Manager`.
+            A :class:`~lamindb.dev.QuerySet`.
         """
         from lamindb._select import select
 
         return select(cls, **expressions)
 
     @classmethod
     def search(
         cls,
         string: str,
         *,
         field: Optional[StrField] = None,
         top_hit: bool = False,
-        case_sensitive: bool = True,
-        synonyms_field: Optional[Union[str, TextField, CharField]] = "synonyms",
-        synonyms_sep: str = "|",
+        case_sensitive: bool = False,
+        synonyms_field: Optional[StrField] = "synonyms",
     ) -> Union["pd.DataFrame", "ORM"]:
         """Search the table.
 
         Args:
             string: `str` The input string to match against the field ontology values.
             field: `Optional[StrField] = None` The field
                 against which the input string is matching.
             top_hit: `bool = False` If `True`, return only the top hit or hits (in
                 case of equal scores).
             case_sensitive: `bool = False` Whether the match is case sensitive.
-            synonyms_field: `bool = True` Also search synonyms. If `None`, is ignored.
+            synonyms_field: `Optional[StrField] = "synonyms"` Search synonyms if
+                column is available. If `None`, is ignored.
 
         Returns:
             A sorted `DataFrame` of search results with a score in column
             `__ratio__`. If `top_hit` is `True`, the best match.
         """
         pass
 
     class Meta:
         abstract = True
 
 
+# -------------------------------------------------------------------------------------
 # A note on required fields at the ORM level
 #
 # As Django does most of its validation on the Form-level, it doesn't offer functionality
 # for validating the integrity of an ORM object upon instantation (similar to pydantic)
 #
 # For required fields, we define them as commonly done on the SQL level together
 # with a validator in ORM (validate_required_fields)
@@ -238,14 +259,15 @@
 # This goes against the Django convention, but goes with the SQLModel convention
 # (Optional fields can be null on the SQL level, non-optional fields cannot)
 #
 # Due to Django's convention where CharField has pre-configured (null=False, default=""), marking
 # a required field necessitates passing `default=None`. Without the validator it would trigger
 # an error at the SQL-level, with it, it triggers it at instantiation
 
+# -------------------------------------------------------------------------------------
 # A note on class and instance methods of core ORM
 #
 # All of these are defined and tested within lamindb, in files starting with _{orm_name}.py
 
 
 class User(ORM):
     """Users.
@@ -367,14 +389,19 @@
     Defaults to `notebook` if run from ipython and to `pipeline` if run from python.
 
     If run from the app, it defaults to `app`.
     """
     reference = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Reference for the transform, e.g., a URL.
     """
+    parents = models.ManyToManyField("self", symmetrical=False, related_name="children")
+    """Parent transforms (predecessors) in data lineage.
+
+    These are auto-populated whenever a transform loads a file as run input.
+    """
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_transforms")
     """Creator of record, a :class:`~lamindb.User`."""
 
@@ -473,17 +500,19 @@
     """
 
     id = models.CharField(max_length=12, default=base62_12, primary_key=True)
     """Universal id, valid across DB instances."""
     name = models.CharField(max_length=255, db_index=True, default=None)
     """Name or title of feature (required)."""
     type = models.CharField(max_length=96, null=True, default=None)
-    """A way of grouping features of same type."""
+    """Type (a mere string description)."""
     description = models.TextField(null=True, default=None)
     """A description."""
+    synonyms = models.TextField(null=True, default=None)
+    """Bar-separated (|) synonyms."""
     feature_sets = models.ManyToManyField("FeatureSet", related_name="features")
     """Feature sets linked to this gene."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of run execution."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_features")
@@ -501,71 +530,336 @@
     Guides:
 
     - :doc:`/biology/scrna`
     - :doc:`/biology/flow`
 
     Examples:
 
-    >>> import lnschema_bionty as bt
-    >>> reference = bt.Gene(species="mouse")
-    >>> feature_set = ln.FeatureSet.from_values(adata.var["ensemble_id"], Gene.ensembl_gene_id)
-    >>> feature_set.save()
-    >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq")
-    >>> file.save()
-    >>> file.featuresets.add(featureset)
+        >>> features = ln.Feature.from_values(["feat1", "feat2"])
+        >>> ln.FeatureSet(features)
+
+        >>> import lnschema_bionty as bt
+        >>> reference = bt.Gene(species="mouse")
+        >>> feature_set = ln.FeatureSet.from_values(adata.var["ensemble_id"], Gene.ensembl_gene_id)
+        >>> feature_set.save()
+        >>> file = ln.File(adata, name="Mouse Lymph Node scRNA-seq")
+        >>> file.save()
+        >>> file.feature_sets.add(feature_set)
 
     """
 
-    id = models.CharField(max_length=64, primary_key=True, default=None)
-    """A universal id, valid across DB instances, a hash of the linked set of features."""
+    id = models.CharField(max_length=20, primary_key=True, default=None)
+    """A universal id (hash of the set of feature identifiers)."""
     type = models.CharField(max_length=64)
-    """A feature entity type."""
+    """Type formatted as ``"{schema_name}{ORM.__name__}"``."""
+    field = models.CharField(max_length=32)
+    """Field of ORM that was hashed."""
     files = models.ManyToManyField("File", related_name="feature_sets")
     """Files linked to the feature set."""
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_featuresets")
     """Creator of record, a :class:`~lamindb.User`."""
 
+    @overload
+    def __init__(
+        self,
+        features: List[ORM],
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        pass
+
+    @classmethod  # type:ignore
+    def from_values(cls, values: ListLike, field: Field = Feature.name, **kwargs) -> "FeatureSet":  # type: ignore
+        """Create feature set from identifier values.
+
+        Args:
+           values: ``ListLike`` A list of identifiers, like feature names or ids.
+           field: ``Field = Feature.name`` The field of a reference ORM to
+               map values.
+           **kwargs: Can contain ``species`` or other context to interpret values.
+
+        Example:
+
+            >>> features = ["feat1", "feat2"]
+            >>> feature_set = ln.FeatureSet.from_values(features)
+
+            >>> genes = ["ENS980983409", "ENS980983410"]
+            >>> feature_set = ln.FeatureSet.from_values(features, lb.Gene.ensembl_gene_id)
+        """
+        pass
+
+    def save(self, *args, **kwargs) -> None:
+        """Save."""
+
 
 class File(ORM):
-    """Test."""
+    """Files.
+
+    Args:
+        data: `Union[PathLike, DataLike]` A file path or an in-memory data
+            object (`DataFrame`, `AnnData`) to serialize. Can be a cloud path, e.g.,
+            `"s3://my-bucket/my_samples/my_file.fcs"`.
+        key: `Optional[str] = None` A storage key: a relative filepath within the
+            current default storage, e.g., `"my_samples/my_file.fcs"`.
+        name: `Optional[str] = None` A description.
+        run: `Optional[Run] = None` The run that created the file, gets auto-linked
+            if `ln.track()` was called.
+        feature_sets: `Optional[List[FeatureSet]] = None` A list of `FeatureSet`
+            records describing the features measured in the file.
+
+    Track where files come from by passing the generating :class:`~lamindb.Run`.
+
+    Often, files store jointly measured observations of features: track them
+    with :class:`~lamindb.FeatureSet`.
+
+    If files have corresponding representations in storage and memory, LaminDB
+    makes some configurable default choices (e.g., serialize a `DataFrame` as a
+    `.parquet` file).
+
+    .. admonition:: Formats in storage & their API access
+
+        Listed are typical `suffix` values & in memory data objects.
+
+        - Table: `.csv`, `.tsv`, `.parquet`, `.ipc` ⟷ `DataFrame`, `pyarrow.Table`
+        - Annotated matrix: `.h5ad`, `.h5mu`, `.zrad` ⟷ `AnnData`, `MuData`
+        - Image: `.jpg`, `.png` ⟷ `np.ndarray`, ...
+        - Arrays: HDF5 group, zarr group, TileDB store ⟷ HDF5, zarr, TileDB loaders
+        - Fastq: `.fastq` ⟷ /
+        - VCF: `.vcf` ⟷ /
+        - QC: `.html` ⟷ /
+
+    .. note::
+
+        In some cases, e.g. for zarr-based storage, a `File` object is stored as
+        many small objects in what appears to be a "folder" in storage.
+
+    """
 
     id = models.CharField(max_length=20, primary_key=True)
     """A universal random id (20-char base62), valid across DB instances."""
-    name = models.CharField(max_length=255, db_index=True, null=True, default=None)
-    """A name or title for the file, mostly useful if no key is provided."""
+    storage: "Storage" = models.ForeignKey(Storage, PROTECT, related_name="files")
+    """Storage location (:class:`~lamindb.Storage`), e.g., an S3 bucket, local folder or network location."""
     key = models.CharField(max_length=255, db_index=True, null=True, default=None)
     """Storage key, the relative path within the storage location."""
     suffix = models.CharField(max_length=30, db_index=True, null=True, default=None)
     """File suffix.
 
     This is a file extension if the `file` is stored in a file format.
     It's `None` if the storage format doesn't have a canonical extension.
     """
+    description = models.CharField(max_length=255, db_index=True, null=True, default=None)
+    """A description."""
     size = models.BigIntegerField(null=True, db_index=True)
     """Size in bytes.
 
     Examples: 1KB is 1e3 bytes, 1MB is 1e6, 1GB is 1e9, 1TB is 1e12 etc.
     """
-    hash = models.CharField(max_length=86, db_index=True, null=True, default=None)
-    """Hash of file content. 86 base64 chars allow to store 64 bytes, 512 bits."""
-    run = models.ForeignKey(Run, PROTECT, related_name="outputs", null=True)
-    """:class:`~lamindb.Run` that created the `file`."""
+    hash = models.CharField(max_length=86, db_index=True, null=True, default=None)  # 86 base64 chars allow to store 64 bytes, 512 bits
+    """Hash or pseudo-hash of file content.
+
+    Useful to ascertain integrity and avoid duplication.
+    """
+    hash_type = models.CharField(max_length=30, db_index=True, null=True, default=None)
+    """Type of hash."""
     transform = models.ForeignKey(Transform, PROTECT, related_name="files", null=True)
     """:class:`~lamindb.Transform` whose run created the `file`."""
-    storage: "Storage" = models.ForeignKey(Storage, PROTECT, related_name="files")
-    """:class:`~lamindb.Storage` location of `file`, see `.path()` for full path."""
+    run = models.ForeignKey(Run, PROTECT, related_name="outputs", null=True)
+    """:class:`~lamindb.Run` that created the `file`."""
     # tags from Tags.files
     # features from Features.files
     # input_of from Run.inputs
     created_at = models.DateTimeField(auto_now_add=True, db_index=True)
     """Time of creation of record."""
     updated_at = models.DateTimeField(auto_now=True, db_index=True)
     """Time of last update to record."""
     created_by = models.ForeignKey(User, PROTECT, default=current_user_id, related_name="created_files")
     """Creator of record, a :class:`~lamindb.User`."""
 
     class Meta:
         unique_together = (("storage", "key"),)
+
+    @overload
+    def __init__(
+        self,
+        data: Union[PathLike, DataLike],
+        key: Optional[str] = None,
+        run: Optional[Run] = None,
+        name: Optional[str] = None,
+        feature_sets: Optional[List[FeatureSet]] = None,
+    ):
+        ...
+
+    @overload
+    def __init__(
+        self,
+        *db_args,
+    ):
+        ...
+
+    def __init__(
+        self,
+        *args,
+        **kwargs,
+    ):
+        pass
+
+    @classmethod
+    def from_df(
+        cls,
+        df: "pd.DataFrame",
+        columns_ref: Field = Feature.name,
+        key: Optional[str] = None,
+        description: Optional[str] = None,
+        run: Optional[Run] = None,
+    ) -> "File":
+        """Create from ``DataFrame``, link column names as features."""
+        pass
+
+    @classmethod
+    def from_anndata(
+        cls,
+        adata: "AnnDataLike",
+        var_ref: Optional[Field],
+        obs_columns_ref: Optional[Field] = Feature.name,
+        key: Optional[str] = None,
+        description: Optional[str] = None,
+        run: Optional[Run] = None,
+    ) -> "File":
+        """Create from ``AnnData`` or ``.h5ad`` file, link ``var_names`` and ``obs.columns`` as features."""
+        pass
+
+    @classmethod
+    def from_dir(
+        cls,
+        path: PathLike,
+        *,
+        run: Optional[Run] = None,
+    ) -> List["File"]:
+        """Create a list of file objects from a directory."""
+        pass
+
+    def replace(
+        self,
+        data: Union[PathLike, DataLike],
+        run: Optional[Run] = None,
+        format: Optional[str] = None,
+    ) -> None:
+        """Replace file content.
+
+        Args:
+            data: ``Union[PathLike, DataLike]`` A file path or an in-memory data
+                object (`DataFrame`, `AnnData`).
+            run: ``Optional[Run] = None`` The run that created the file gets
+                auto-linked if ``ln.track()`` was called.
+
+        Examples:
+
+            Say we made a change to the content of a file (e.g., edited the image
+            `paradisi05_laminopathic_nuclei.jpg`).
+
+            This is how we replace the old file in storage with the new file:
+
+            >>> file.replace("paradisi05_laminopathic_nuclei.jpg")
+            >>> file.save()
+
+            Note that this neither changes the storage key nor the filename.
+
+            However, it will update the suffix if the file type changes.
+        """
+        pass
+
+    def backed(self, is_run_input: Optional[bool] = None) -> Union["AnnDataAccessor", "BackedAccessor"]:
+        """Return a cloud-backed data object to stream."""
+        pass
+
+    @classmethod
+    def tree(
+        cls,
+        prefix: Optional[str] = None,
+        *,
+        level: int = -1,
+        limit_to_directories: bool = False,
+        length_limit: int = 1000,
+    ):
+        """Given a prefix, print a visual tree structure of files."""
+        pass
+
+    def path(self) -> Union[Path, UPath]:
+        """Path in storage."""
+
+    def load(self, is_run_input: Optional[bool] = None, stream: bool = False) -> DataLike:
+        """Stage and load to memory.
+
+        Returns in-memory representation if possible, e.g., an `AnnData` object
+        for an `h5ad` file.
+        """
+        pass
+
+    def stage(self, is_run_input: Optional[bool] = None) -> Path:
+        """Update cache from cloud storage if outdated.
+
+        Returns a path to a locally cached on-disk object (say, a
+        `.jpg` file).
+        """
+        pass
+
+    def delete(self, storage: Optional[bool] = None) -> None:
+        """Delete file, optionally from storage.
+
+        Args:
+            storage: `Optional[bool] = None` Indicate whether you want to delete the
+            file in storage.
+
+        Example:
+
+            For any `File` object `file`, call:
+
+            >>> file.delete()
+
+        """
+        pass
+
+    def save(self, *args, **kwargs) -> None:
+        """Save the file to database & storage."""
+        pass
+
+
+# -------------------------------------------------------------------------------------
+# Low-level logic needed in lamindb-setup
+
+# Below is needed within lnschema-core because lamindb-setup already performs
+# some logging
+
+
+def format_datetime(dt: Union[datetime, Any]) -> str:
+    if not isinstance(dt, datetime):
+        return dt
+    else:
+        return dt.strftime("%Y-%m-%d %H:%M:%S")
+
+
+def __repr__(self: ORM) -> str:
+    field_names = [field.name for field in self._meta.fields if (not isinstance(field, models.ForeignKey) and field.name != "created_at")]
+    field_names += [f"{field.name}_id" for field in self._meta.fields if isinstance(field, models.ForeignKey)]
+    fields_str = {k: format_datetime(getattr(self, k)) for k in field_names if hasattr(self, k)}
+    fields_joined_str = ", ".join([f"{k}={fields_str[k]}" for k in fields_str if fields_str[k] is not None])
+    return f"{self.__class__.__name__}({fields_joined_str})"
+
+
+ORM.__repr__ = __repr__  # type: ignore
+ORM.__str__ = __repr__  # type: ignore
```

### Comparing `lamindb_setup-0.48.8/lnschema-core/lnschema_core/types.py` & `lamindb_setup-0.49.0/lnschema-core/lnschema_core/types.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     import numpy as np
     import pandas as pd
 
 PathLike = TypeVar("PathLike", str, Path, UPath)
 # statically typing the following is hard because these are all heavy
 # dependencies, even DataFrame is heavy & slow to import
 DataLike = Any
+AnnDataLike = Any
 ListLike = TypeVar("ListLike", "pd.Series", list, "np.array")
 StrField = TypeVar("StrField", str, CharField, TextField)
 
 
 class ChoicesMixin:
     @classmethod
     def choices(cls):
```

### Comparing `lamindb_setup-0.48.8/lnschema-core/pyproject.toml` & `lamindb_setup-0.49.0/lnschema-core/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/pyproject.toml` & `lamindb_setup-0.49.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/tests/hub/test_instance.py` & `lamindb_setup-0.49.0/tests/hub/test_instance.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,10 +32,11 @@
 
 def test_load_instance(auth_1, instance_1):
     result = load_instance(
         owner=auth_1["handle"],
         name=instance_1["name"],
         _access_token=auth_1["access_token"],
     )
+
     loaded_instance, _ = result
     assert loaded_instance["name"] == instance_1["name"]
     assert loaded_instance["db"]
```

### Comparing `lamindb_setup-0.48.8/tests/hub/test_storage.py` & `lamindb_setup-0.49.0/tests/hub/test_storage.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/tests/test_init_instance.py` & `lamindb_setup-0.49.0/tests/test_init_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/tests/test_load_instance.py` & `lamindb_setup-0.49.0/tests/test_load_instance.py`

 * *Files identical despite different names*

### Comparing `lamindb_setup-0.48.8/PKG-INFO` & `lamindb_setup-0.49.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lamindb_setup
-Version: 0.48.8
+Version: 0.49.0
 Summary: LaminDB setup.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lnschema_core>=0.35.4
 Requires-Dist: lamin_logger>=0.3.3
 Requires-Dist: django
 Requires-Dist: dj_database_url
```

