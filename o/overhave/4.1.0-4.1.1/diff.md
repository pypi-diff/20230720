# Comparing `tmp/overhave-4.1.0.tar.gz` & `tmp/overhave-4.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "overhave-4.1.0.tar", max compression
+gzip compressed data, was "overhave-4.1.1.tar", max compression
```

## Comparing `overhave-4.1.0.tar` & `overhave-4.1.1.tar`

### file list

```diff
@@ -1,245 +1,245 @@
--rw-r--r--   0        0        0    23136 2023-07-10 05:49:29.631843 overhave-4.1.0/README.rst
--rw-r--r--   0        0        0     3193 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/__init__.py
--rw-r--r--   0        0        0       63 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/admin/__init__.py
--rw-r--r--   0        0        0     5172 2023-07-10 05:49:29.647843 overhave-4.1.0/overhave/admin/app.py
--rw-r--r--   0        0        0   735118 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/ace-src/ace.js
--rw-r--r--   0        0        0     5426 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/ace-src/mode-gherkin.js
--rw-r--r--   0        0        0     1263 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/css/overhave.css
--rw-r--r--   0        0        0    38062 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/files/favicon.ico
--rw-r--r--   0        0        0      138 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/__init__.py
--rw-r--r--   0        0        0     1819 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/flask_admin.py
--rw-r--r--   0        0        0      287 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/flask_app.py
--rw-r--r--   0        0        0     2112 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/flask/login_manager.py
--rw-r--r--   0        0        0      187 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/draft_detail.html
--rw-r--r--   0        0        0      405 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation.html
--rw-r--r--   0        0        0      194 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_create.html
--rw-r--r--   0        0        0      190 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_edit.html
--rw-r--r--   0        0        0      860 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/emulation_run_detail.html
--rw-r--r--   0        0        0    10071 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature.html
--rw-r--r--   0        0        0      404 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature_create.html
--rw-r--r--   0        0        0      465 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/feature_edit.html
--rw-r--r--   0        0        0      177 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/index.html
--rw-r--r--   0        0        0     2414 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/login.html
--rw-r--r--   0        0        0      149 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/overhave_master.html
--rw-r--r--   0        0        0     1696 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run.html
--rw-r--r--   0        0        0     1535 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run_detail.html
--rw-r--r--   0        0        0      189 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_run_list.html
--rw-r--r--   0        0        0      606 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user.html
--rw-r--r--   0        0        0      210 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user_create.html
--rw-r--r--   0        0        0      208 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/templates/test_user_edit.html
--rw-r--r--   0        0        0      451 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/__init__.py
--rw-r--r--   0        0        0     1386 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/access.py
--rw-r--r--   0        0        0     2914 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/base.py
--rw-r--r--   0        0        0     1105 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/draft.py
--rw-r--r--   0        0        0     3407 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/emulation.py
--rw-r--r--   0        0        0     1620 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/emulation_run.py
--rw-r--r--   0        0        0    10257 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/feature.py
--rw-r--r--   0        0        0      306 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/__init__.py
--rw-r--r--   0        0        0     4997 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/formatters.py
--rw-r--r--   0        0        0      631 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/helpers.py
--rw-r--r--   0        0        0     1404 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/formatters/safe_formatter.py
--rw-r--r--   0        0        0       51 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/__init__.py
--rw-r--r--   0        0        0     1648 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/custom_page.py
--rw-r--r--   0        0        0     1578 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/login_form.py
--rw-r--r--   0        0        0     2645 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/index/view.py
--rw-r--r--   0        0        0     1794 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/scenario_test_run.py
--rw-r--r--   0        0        0     1329 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/tag.py
--rw-r--r--   0        0        0     3665 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/admin/views/testing_users.py
--rw-r--r--   0        0        0       52 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/__init__.py
--rw-r--r--   0        0        0     5970 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/app.py
--rw-r--r--   0        0        0      216 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/asgi.py
--rw-r--r--   0        0        0      143 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/__init__.py
--rw-r--r--   0        0        0      348 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/models.py
--rw-r--r--   0        0        0     1395 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/regular.py
--rw-r--r--   0        0        0      867 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/auth/token.py
--rw-r--r--   0        0        0     2422 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/deps.py
--rw-r--r--   0        0        0      848 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/settings.py
--rw-r--r--   0        0        0      580 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/__init__.py
--rw-r--r--   0        0        0     1416 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/auth_views.py
--rw-r--r--   0        0        0      550 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/emulation_views.py
--rw-r--r--   0        0        0      586 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/extra_views.py
--rw-r--r--   0        0        0      461 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/feature_type_views.py
--rw-r--r--   0        0        0     1184 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/feature_views.py
--rw-r--r--   0        0        0      969 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/tags_views.py
--rw-r--r--   0        0        0     2041 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/testrun_views.py
--rw-r--r--   0        0        0     4486 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/api/views/testuser_views.py
--rw-r--r--   0        0        0     4047 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/base_settings.py
--rw-r--r--   0        0        0      164 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/__init__.py
--rw-r--r--   0        0        0      557 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/admin.py
--rw-r--r--   0        0        0      534 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/api.py
--rw-r--r--   0        0        0      647 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/consumers.py
--rw-r--r--   0        0        0       84 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/__init__.py
--rw-r--r--   0        0        0      830 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/group.py
--rw-r--r--   0        0        0     1755 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/db_cmds/regular.py
--rw-r--r--   0        0        0      358 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/group.py
--rw-r--r--   0        0        0     3048 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/s3.py
--rw-r--r--   0        0        0     1573 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/cli/synchronizer.py
--rw-r--r--   0        0        0      455 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/__init__.py
--rw-r--r--   0        0        0     3283 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/base.py
--rw-r--r--   0        0        0     1349 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/statuses.py
--rw-r--r--   0        0        0     8141 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/tables.py
--rw-r--r--   0        0        0      795 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/users.py
--rw-r--r--   0        0        0     1249 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/db/utils.py
--rw-r--r--   0        0        0       46 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/emulation/__init__.py
--rw-r--r--   0        0        0     4103 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/emulation/emulator.py
--rw-r--r--   0        0        0      897 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/__init__.py
--rw-r--r--   0        0        0     1231 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/archiver.py
--rw-r--r--   0        0        0      247 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/__init__.py
--rw-r--r--   0        0        0      316 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/abstract.py
--rw-r--r--   0        0        0      497 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/base.py
--rw-r--r--   0        0        0      754 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/default.py
--rw-r--r--   0        0        0      116 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/__init__.py
--rw-r--r--   0        0        0     3493 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/manager.py
--rw-r--r--   0        0        0      198 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/ldap/settings.py
--rw-r--r--   0        0        0     1487 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/secret_mixin.py
--rw-r--r--   0        0        0     1396 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/auth_managers/simple.py
--rw-r--r--   0        0        0      169 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/__init__.py
--rw-r--r--   0        0        0      425 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/abstract.py
--rw-r--r--   0        0        0      221 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/errors.py
--rw-r--r--   0        0        0     2748 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/feature/extractor.py
--rw-r--r--   0        0        0     1098 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/file_extractor.py
--rw-r--r--   0        0        0     1760 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/git_initializer.py
--rw-r--r--   0        0        0       55 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/language/__init__.py
--rw-r--r--   0        0        0     1198 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/language/prefixes.py
--rw-r--r--   0        0        0      102 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/__init__.py
--rw-r--r--   0        0        0      415 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/models.py
--rw-r--r--   0        0        0     5825 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/report_manager/report_manager.py
--rw-r--r--   0        0        0     6633 2023-07-10 05:49:29.651843 overhave-4.1.0/overhave/entities/settings.py
--rw-r--r--   0        0        0       54 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/extra/__init__.py
--rw-r--r--   0        0        0      386 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/extra/prefixes.py
--rw-r--r--   0        0        0      739 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/__init__.py
--rw-r--r--   0        0        0     7209 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/base_factory.py
--rw-r--r--   0        0        0      418 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/__init__.py
--rw-r--r--   0        0        0      306 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/abstract_consumer.py
--rw-r--r--   0        0        0     4555 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/admin_factory.py
--rw-r--r--   0        0        0     1312 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/emulation_factory.py
--rw-r--r--   0        0        0     3956 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/publication_factory.py
--rw-r--r--   0        0        0      486 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/s3_init_factory.py
--rw-r--r--   0        0        0     2184 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/synchronizer_factory.py
--rw-r--r--   0        0        0     1888 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/components/test_execution_factory.py
--rw-r--r--   0        0        0     2045 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/consumer_factory.py
--rw-r--r--   0        0        0      550 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/__init__.py
--rw-r--r--   0        0        0     2950 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/admin_context.py
--rw-r--r--   0        0        0     4028 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/base_context.py
--rw-r--r--   0        0        0      506 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/emulation_context.py
--rw-r--r--   0        0        0     2032 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/publication_context.py
--rw-r--r--   0        0        0     1288 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/synchronizer_context.py
--rw-r--r--   0        0        0     2519 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/context/test_execution_context.py
--rw-r--r--   0        0        0      769 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/factory/getters.py
--rw-r--r--   0        0        0      353 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/__init__.py
--rw-r--r--   0        0        0      193 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/client/__init__.py
--rw-r--r--   0        0        0     3162 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/client/container.py
--rw-r--r--   0        0        0      983 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/metrics/getters.py
--rw-r--r--   0        0        0      342 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/__init__.py
--rw-r--r--   0        0        0      399 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/abstract_publisher.py
--rw-r--r--   0        0        0     4015 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/base_publisher.py
--rw-r--r--   0        0        0      532 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/errors.py
--rw-r--r--   0        0        0     4928 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/git_publisher.py
--rw-r--r--   0        0        0      224 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/__init__.py
--rw-r--r--   0        0        0     4208 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/gitlab_publisher.py
--rw-r--r--   0        0        0     1408 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/settings.py
--rw-r--r--   0        0        0      171 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/__init__.py
--rw-r--r--   0        0        0     2157 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/client.py
--rw-r--r--   0        0        0     1015 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/gitlab/tokenizer/settings.py
--rw-r--r--   0        0        0      178 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/objects.py
--rw-r--r--   0        0        0      877 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/settings.py
--rw-r--r--   0        0        0      119 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/__init__.py
--rw-r--r--   0        0        0     1672 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/settings.py
--rw-r--r--   0        0        0     4323 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/publication/stash/stash_publisher.py
--rw-r--r--   0        0        0      371 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/__init__.py
--rw-r--r--   0        0        0     3538 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/config_injector.py
--rw-r--r--   0        0        0      827 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/deps.py
--rw-r--r--   0        0        0      530 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/__init__.py
--rw-r--r--   0        0        0      305 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/__init__.py
--rw-r--r--   0        0        0      927 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
--rw-r--r--   0        0        0     1102 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/links.py
--rw-r--r--   0        0        0     1260 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/severity.py
--rw-r--r--   0        0        0     2452 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
--rw-r--r--   0        0        0     1638 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/bdd_item.py
--rw-r--r--   0        0        0      981 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/parsed_info.py
--rw-r--r--   0        0        0     2874 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/helpers/tag_controller.py
--rw-r--r--   0        0        0     6192 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/plugin.py
--rw-r--r--   0        0        0     2223 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/plugin_resolver.py
--rw-r--r--   0        0        0     3945 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/pytest_plugin/proxy_manager.py
--rw-r--r--   0        0        0      517 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/__init__.py
--rw-r--r--   0        0        0      157 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/__init__.py
--rw-r--r--   0        0        0     5100 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/compiler.py
--rw-r--r--   0        0        0      631 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/compiler/settings.py
--rw-r--r--   0        0        0      150 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/__init__.py
--rw-r--r--   0        0        0     3495 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/file_manager.py
--rw-r--r--   0        0        0     2820 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/file_manager/settings.py
--rw-r--r--   0        0        0      230 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/__init__.py
--rw-r--r--   0        0        0      854 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/models.py
--rw-r--r--   0        0        0     8442 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/parser.py
--rw-r--r--   0        0        0      263 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/parser/settings.py
--rw-r--r--   0        0        0      235 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/prefix_mixin.py
--rw-r--r--   0        0        0       95 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/__init__.py
--rw-r--r--   0        0        0      229 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/abstract.py
--rw-r--r--   0        0        0     1441 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/duplicate_id_mixin.py
--rw-r--r--   0        0        0      510 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/errors.py
--rw-r--r--   0        0        0     2827 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/scenario/validator/validator.py
--rw-r--r--   0        0        0     1226 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/__init__.py
--rw-r--r--   0        0        0     1180 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/api_auth_storage.py
--rw-r--r--   0        0        0     3271 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/converters.py
--rw-r--r--   0        0        0     6178 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/draft_storage.py
--rw-r--r--   0        0        0     5323 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/emulation_storage.py
--rw-r--r--   0        0        0     4947 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_storage.py
--rw-r--r--   0        0        0     1566 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_tag_storage.py
--rw-r--r--   0        0        0     2176 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/feature_type_storage.py
--rw-r--r--   0        0        0     1902 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/scenario_storage.py
--rw-r--r--   0        0        0      589 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/system_user_group_storage.py
--rw-r--r--   0        0        0     1930 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/system_user_storage.py
--rw-r--r--   0        0        0     3054 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/test_run_storage.py
--rw-r--r--   0        0        0     4451 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/storage/test_user_storage.py
--rw-r--r--   0        0        0      192 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/__init__.py
--rw-r--r--   0        0        0      260 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/abstract.py
--rw-r--r--   0        0        0     3728 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/storage_manager.py
--rw-r--r--   0        0        0     7025 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/synchronization/synchronizer.py
--rw-r--r--   0        0        0      307 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/__init__.py
--rw-r--r--   0        0        0     4256 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/executor.py
--rw-r--r--   0        0        0     1056 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/objects.py
--rw-r--r--   0        0        0     1750 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/settings.py
--rw-r--r--   0        0        0     4106 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/step_collector.py
--rw-r--r--   0        0        0     1617 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/test_execution/test_runner.py
--rw-r--r--   0        0        0      983 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/__init__.py
--rw-r--r--   0        0        0      623 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/__init__.py
--rw-r--r--   0        0        0      122 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/__init__.py
--rw-r--r--   0        0        0     1810 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/authenticator.py
--rw-r--r--   0        0        0      237 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/models.py
--rw-r--r--   0        0        0      499 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/api_client/settings.py
--rw-r--r--   0        0        0      208 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/__init__.py
--rw-r--r--   0        0        0      590 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/auth.py
--rw-r--r--   0        0        0     2139 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/client.py
--rw-r--r--   0        0        0      110 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/objects.py
--rw-r--r--   0        0        0     1287 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/base_client/settings.py
--rw-r--r--   0        0        0      258 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/__init__.py
--rw-r--r--   0        0        0     2003 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/client.py
--rw-r--r--   0        0        0      609 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/models.py
--rw-r--r--   0        0        0      144 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/objects.py
--rw-r--r--   0        0        0      377 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/settings.py
--rw-r--r--   0        0        0      741 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/gitlab_client/utils.py
--rw-r--r--   0        0        0      326 2023-07-10 05:49:29.655843 overhave-4.1.0/overhave/transport/http/stash_client/__init__.py
--rw-r--r--   0        0        0     2115 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/client.py
--rw-r--r--   0        0        0     2757 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/models.py
--rw-r--r--   0        0        0      569 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/http/stash_client/settings.py
--rw-r--r--   0        0        0      109 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/__init__.py
--rw-r--r--   0        0        0     1896 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/authenticator.py
--rw-r--r--   0        0        0      420 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/ldap/settings.py
--rw-r--r--   0        0        0      430 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/__init__.py
--rw-r--r--   0        0        0     2937 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/consumer.py
--rw-r--r--   0        0        0     1661 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/deps.py
--rw-r--r--   0        0        0     2439 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/objects.py
--rw-r--r--   0        0        0     1319 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/producer.py
--rw-r--r--   0        0        0     1384 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/runner.py
--rw-r--r--   0        0        0     1674 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/redis/settings.py
--rw-r--r--   0        0        0      132 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/__init__.py
--rw-r--r--   0        0        0     8494 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/manager.py
--rw-r--r--   0        0        0     2082 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/models.py
--rw-r--r--   0        0        0      181 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/objects.py
--rw-r--r--   0        0        0      885 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/transport/s3/settings.py
--rw-r--r--   0        0        0      103 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/__init__.py
--rw-r--r--   0        0        0       84 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/mocks.py
--rw-r--r--   0        0        0      139 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/time.py
--rw-r--r--   0        0        0      148 2023-07-10 05:49:29.659843 overhave-4.1.0/overhave/utils/url.py
--rw-r--r--   0        0        0     3522 2023-07-10 05:49:29.659843 overhave-4.1.0/pyproject.toml
--rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.1.0/PKG-INFO
+-rw-r--r--   0        0        0    23136 2023-07-20 08:50:59.794347 overhave-4.1.1/README.rst
+-rw-r--r--   0        0        0     3193 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/__init__.py
+-rw-r--r--   0        0        0       63 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/admin/__init__.py
+-rw-r--r--   0        0        0     5172 2023-07-20 08:50:59.806347 overhave-4.1.1/overhave/admin/app.py
+-rw-r--r--   0        0        0   735118 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/ace-src/ace.js
+-rw-r--r--   0        0        0     5426 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/ace-src/mode-gherkin.js
+-rw-r--r--   0        0        0     1263 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/css/overhave.css
+-rw-r--r--   0        0        0    38062 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/files/favicon.ico
+-rw-r--r--   0        0        0      138 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/__init__.py
+-rw-r--r--   0        0        0     1893 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/flask_admin.py
+-rw-r--r--   0        0        0      287 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/flask_app.py
+-rw-r--r--   0        0        0     2112 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/flask/login_manager.py
+-rw-r--r--   0        0        0      187 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/draft_detail.html
+-rw-r--r--   0        0        0      405 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/emulation.html
+-rw-r--r--   0        0        0      194 2023-07-20 08:50:59.810347 overhave-4.1.1/overhave/admin/templates/emulation_create.html
+-rw-r--r--   0        0        0      190 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/emulation_edit.html
+-rw-r--r--   0        0        0      860 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/emulation_run_detail.html
+-rw-r--r--   0        0        0    10071 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature.html
+-rw-r--r--   0        0        0      404 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature_create.html
+-rw-r--r--   0        0        0      465 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/feature_edit.html
+-rw-r--r--   0        0        0      177 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/index.html
+-rw-r--r--   0        0        0     2414 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/login.html
+-rw-r--r--   0        0        0      149 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/overhave_master.html
+-rw-r--r--   0        0        0     1696 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run.html
+-rw-r--r--   0        0        0     1535 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run_detail.html
+-rw-r--r--   0        0        0      189 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_run_list.html
+-rw-r--r--   0        0        0      606 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user.html
+-rw-r--r--   0        0        0      210 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user_create.html
+-rw-r--r--   0        0        0      208 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/templates/test_user_edit.html
+-rw-r--r--   0        0        0      451 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/__init__.py
+-rw-r--r--   0        0        0     1386 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/access.py
+-rw-r--r--   0        0        0     2914 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/base.py
+-rw-r--r--   0        0        0     1105 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/draft.py
+-rw-r--r--   0        0        0     3407 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/emulation.py
+-rw-r--r--   0        0        0     1620 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/emulation_run.py
+-rw-r--r--   0        0        0    10257 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/feature.py
+-rw-r--r--   0        0        0      306 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/__init__.py
+-rw-r--r--   0        0        0     4997 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/formatters.py
+-rw-r--r--   0        0        0      631 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/helpers.py
+-rw-r--r--   0        0        0     1404 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/formatters/safe_formatter.py
+-rw-r--r--   0        0        0       51 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/__init__.py
+-rw-r--r--   0        0        0     1648 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/custom_page.py
+-rw-r--r--   0        0        0     1578 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/login_form.py
+-rw-r--r--   0        0        0     3023 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/index/view.py
+-rw-r--r--   0        0        0     1794 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/scenario_test_run.py
+-rw-r--r--   0        0        0     1329 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/tag.py
+-rw-r--r--   0        0        0     3665 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/admin/views/testing_users.py
+-rw-r--r--   0        0        0       52 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/__init__.py
+-rw-r--r--   0        0        0     5970 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/app.py
+-rw-r--r--   0        0        0      216 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/asgi.py
+-rw-r--r--   0        0        0      143 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/__init__.py
+-rw-r--r--   0        0        0      348 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/models.py
+-rw-r--r--   0        0        0     1395 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/regular.py
+-rw-r--r--   0        0        0      867 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/auth/token.py
+-rw-r--r--   0        0        0     2422 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/deps.py
+-rw-r--r--   0        0        0      848 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/settings.py
+-rw-r--r--   0        0        0      580 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/__init__.py
+-rw-r--r--   0        0        0     1416 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/auth_views.py
+-rw-r--r--   0        0        0      550 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/emulation_views.py
+-rw-r--r--   0        0        0      586 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/extra_views.py
+-rw-r--r--   0        0        0      461 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/feature_type_views.py
+-rw-r--r--   0        0        0     1184 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/feature_views.py
+-rw-r--r--   0        0        0      969 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/tags_views.py
+-rw-r--r--   0        0        0     2041 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/testrun_views.py
+-rw-r--r--   0        0        0     4496 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/api/views/testuser_views.py
+-rw-r--r--   0        0        0     4047 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/base_settings.py
+-rw-r--r--   0        0        0      164 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/__init__.py
+-rw-r--r--   0        0        0      557 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/admin.py
+-rw-r--r--   0        0        0      534 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/api.py
+-rw-r--r--   0        0        0      647 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/consumers.py
+-rw-r--r--   0        0        0       84 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/__init__.py
+-rw-r--r--   0        0        0      830 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/group.py
+-rw-r--r--   0        0        0     1755 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/db_cmds/regular.py
+-rw-r--r--   0        0        0      358 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/group.py
+-rw-r--r--   0        0        0     3048 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/s3.py
+-rw-r--r--   0        0        0     1573 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/cli/synchronizer.py
+-rw-r--r--   0        0        0      455 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/__init__.py
+-rw-r--r--   0        0        0     3283 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/base.py
+-rw-r--r--   0        0        0     1349 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/statuses.py
+-rw-r--r--   0        0        0     8141 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/tables.py
+-rw-r--r--   0        0        0      795 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/users.py
+-rw-r--r--   0        0        0     1249 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/db/utils.py
+-rw-r--r--   0        0        0       46 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/emulation/__init__.py
+-rw-r--r--   0        0        0     4103 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/emulation/emulator.py
+-rw-r--r--   0        0        0      897 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/__init__.py
+-rw-r--r--   0        0        0     1231 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/archiver.py
+-rw-r--r--   0        0        0      247 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/__init__.py
+-rw-r--r--   0        0        0      316 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/abstract.py
+-rw-r--r--   0        0        0      497 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/base.py
+-rw-r--r--   0        0        0      754 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/default.py
+-rw-r--r--   0        0        0      116 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/__init__.py
+-rw-r--r--   0        0        0     3493 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/manager.py
+-rw-r--r--   0        0        0      198 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/ldap/settings.py
+-rw-r--r--   0        0        0     1487 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/secret_mixin.py
+-rw-r--r--   0        0        0     1396 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/auth_managers/simple.py
+-rw-r--r--   0        0        0      169 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/__init__.py
+-rw-r--r--   0        0        0      425 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/abstract.py
+-rw-r--r--   0        0        0      221 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/errors.py
+-rw-r--r--   0        0        0     2748 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/feature/extractor.py
+-rw-r--r--   0        0        0     1098 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/file_extractor.py
+-rw-r--r--   0        0        0     1760 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/git_initializer.py
+-rw-r--r--   0        0        0       55 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/language/__init__.py
+-rw-r--r--   0        0        0     1198 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/language/prefixes.py
+-rw-r--r--   0        0        0      102 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/__init__.py
+-rw-r--r--   0        0        0      415 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/models.py
+-rw-r--r--   0        0        0     5825 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/report_manager/report_manager.py
+-rw-r--r--   0        0        0     6700 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/entities/settings.py
+-rw-r--r--   0        0        0       54 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/extra/__init__.py
+-rw-r--r--   0        0        0      386 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/extra/prefixes.py
+-rw-r--r--   0        0        0      739 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/__init__.py
+-rw-r--r--   0        0        0     7209 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/base_factory.py
+-rw-r--r--   0        0        0      418 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/__init__.py
+-rw-r--r--   0        0        0      306 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/abstract_consumer.py
+-rw-r--r--   0        0        0     4555 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/admin_factory.py
+-rw-r--r--   0        0        0     1312 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/emulation_factory.py
+-rw-r--r--   0        0        0     3956 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/publication_factory.py
+-rw-r--r--   0        0        0      486 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/s3_init_factory.py
+-rw-r--r--   0        0        0     2184 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/synchronizer_factory.py
+-rw-r--r--   0        0        0     1888 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/components/test_execution_factory.py
+-rw-r--r--   0        0        0     2045 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/consumer_factory.py
+-rw-r--r--   0        0        0      550 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/__init__.py
+-rw-r--r--   0        0        0     2950 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/admin_context.py
+-rw-r--r--   0        0        0     4028 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/base_context.py
+-rw-r--r--   0        0        0      506 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/emulation_context.py
+-rw-r--r--   0        0        0     2032 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/publication_context.py
+-rw-r--r--   0        0        0     1288 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/synchronizer_context.py
+-rw-r--r--   0        0        0     2519 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/context/test_execution_context.py
+-rw-r--r--   0        0        0      769 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/factory/getters.py
+-rw-r--r--   0        0        0      353 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/metrics/__init__.py
+-rw-r--r--   0        0        0      193 2023-07-20 08:50:59.814347 overhave-4.1.1/overhave/metrics/client/__init__.py
+-rw-r--r--   0        0        0     3162 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/metrics/client/container.py
+-rw-r--r--   0        0        0      983 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/metrics/getters.py
+-rw-r--r--   0        0        0      342 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/__init__.py
+-rw-r--r--   0        0        0      399 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/abstract_publisher.py
+-rw-r--r--   0        0        0     4015 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/base_publisher.py
+-rw-r--r--   0        0        0      532 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/errors.py
+-rw-r--r--   0        0        0     4928 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/git_publisher.py
+-rw-r--r--   0        0        0      224 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/__init__.py
+-rw-r--r--   0        0        0     4208 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/gitlab_publisher.py
+-rw-r--r--   0        0        0     1408 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/settings.py
+-rw-r--r--   0        0        0      171 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/__init__.py
+-rw-r--r--   0        0        0     2157 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/client.py
+-rw-r--r--   0        0        0     1015 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/gitlab/tokenizer/settings.py
+-rw-r--r--   0        0        0      178 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/objects.py
+-rw-r--r--   0        0        0      877 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/settings.py
+-rw-r--r--   0        0        0      119 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/__init__.py
+-rw-r--r--   0        0        0     1672 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/settings.py
+-rw-r--r--   0        0        0     4323 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/publication/stash/stash_publisher.py
+-rw-r--r--   0        0        0      371 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/__init__.py
+-rw-r--r--   0        0        0     3538 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/config_injector.py
+-rw-r--r--   0        0        0      827 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/deps.py
+-rw-r--r--   0        0        0      530 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/__init__.py
+-rw-r--r--   0        0        0      305 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/__init__.py
+-rw-r--r--   0        0        0      927 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/description_manager.py
+-rw-r--r--   0        0        0     1102 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/links.py
+-rw-r--r--   0        0        0     1260 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/severity.py
+-rw-r--r--   0        0        0     2452 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py
+-rw-r--r--   0        0        0     1638 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/bdd_item.py
+-rw-r--r--   0        0        0      981 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/parsed_info.py
+-rw-r--r--   0        0        0     2874 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/helpers/tag_controller.py
+-rw-r--r--   0        0        0     6192 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/plugin.py
+-rw-r--r--   0        0        0     2223 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/plugin_resolver.py
+-rw-r--r--   0        0        0     3945 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/pytest_plugin/proxy_manager.py
+-rw-r--r--   0        0        0      517 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/__init__.py
+-rw-r--r--   0        0        0      157 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/__init__.py
+-rw-r--r--   0        0        0     5100 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/compiler.py
+-rw-r--r--   0        0        0      631 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/compiler/settings.py
+-rw-r--r--   0        0        0      150 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/__init__.py
+-rw-r--r--   0        0        0     3495 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/file_manager.py
+-rw-r--r--   0        0        0     2820 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/file_manager/settings.py
+-rw-r--r--   0        0        0      230 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/__init__.py
+-rw-r--r--   0        0        0      854 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/models.py
+-rw-r--r--   0        0        0     8442 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/parser.py
+-rw-r--r--   0        0        0      263 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/parser/settings.py
+-rw-r--r--   0        0        0      235 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/prefix_mixin.py
+-rw-r--r--   0        0        0       95 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/__init__.py
+-rw-r--r--   0        0        0      229 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/abstract.py
+-rw-r--r--   0        0        0     1441 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/duplicate_id_mixin.py
+-rw-r--r--   0        0        0      510 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/errors.py
+-rw-r--r--   0        0        0     2827 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/scenario/validator/validator.py
+-rw-r--r--   0        0        0     1226 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/__init__.py
+-rw-r--r--   0        0        0     1180 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/api_auth_storage.py
+-rw-r--r--   0        0        0     3271 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/converters.py
+-rw-r--r--   0        0        0     6178 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/draft_storage.py
+-rw-r--r--   0        0        0     5323 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/emulation_storage.py
+-rw-r--r--   0        0        0     4947 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_storage.py
+-rw-r--r--   0        0        0     1566 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_tag_storage.py
+-rw-r--r--   0        0        0     2176 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/feature_type_storage.py
+-rw-r--r--   0        0        0     1902 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/scenario_storage.py
+-rw-r--r--   0        0        0      589 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/system_user_group_storage.py
+-rw-r--r--   0        0        0     1930 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/system_user_storage.py
+-rw-r--r--   0        0        0     3054 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/test_run_storage.py
+-rw-r--r--   0        0        0     3616 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/storage/test_user_storage.py
+-rw-r--r--   0        0        0      192 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/__init__.py
+-rw-r--r--   0        0        0      260 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/abstract.py
+-rw-r--r--   0        0        0     3728 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/storage_manager.py
+-rw-r--r--   0        0        0     7025 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/synchronization/synchronizer.py
+-rw-r--r--   0        0        0      307 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/__init__.py
+-rw-r--r--   0        0        0     4256 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/executor.py
+-rw-r--r--   0        0        0     1056 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/objects.py
+-rw-r--r--   0        0        0     1750 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/settings.py
+-rw-r--r--   0        0        0     4106 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/step_collector.py
+-rw-r--r--   0        0        0     1617 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/test_execution/test_runner.py
+-rw-r--r--   0        0        0      983 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/__init__.py
+-rw-r--r--   0        0        0      623 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/__init__.py
+-rw-r--r--   0        0        0      122 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/__init__.py
+-rw-r--r--   0        0        0     1810 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/authenticator.py
+-rw-r--r--   0        0        0      237 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/models.py
+-rw-r--r--   0        0        0      499 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/api_client/settings.py
+-rw-r--r--   0        0        0      208 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/__init__.py
+-rw-r--r--   0        0        0      590 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/auth.py
+-rw-r--r--   0        0        0     2139 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/client.py
+-rw-r--r--   0        0        0      110 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/objects.py
+-rw-r--r--   0        0        0     1287 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/base_client/settings.py
+-rw-r--r--   0        0        0      258 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/__init__.py
+-rw-r--r--   0        0        0     2003 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/client.py
+-rw-r--r--   0        0        0      609 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/models.py
+-rw-r--r--   0        0        0      144 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/objects.py
+-rw-r--r--   0        0        0      377 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/settings.py
+-rw-r--r--   0        0        0      741 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/gitlab_client/utils.py
+-rw-r--r--   0        0        0      326 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/__init__.py
+-rw-r--r--   0        0        0     2115 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/client.py
+-rw-r--r--   0        0        0     2757 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/models.py
+-rw-r--r--   0        0        0      569 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/http/stash_client/settings.py
+-rw-r--r--   0        0        0      109 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/__init__.py
+-rw-r--r--   0        0        0     1896 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/authenticator.py
+-rw-r--r--   0        0        0      420 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/ldap/settings.py
+-rw-r--r--   0        0        0      430 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/__init__.py
+-rw-r--r--   0        0        0     2937 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/consumer.py
+-rw-r--r--   0        0        0     1661 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/deps.py
+-rw-r--r--   0        0        0     2439 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/objects.py
+-rw-r--r--   0        0        0     1319 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/producer.py
+-rw-r--r--   0        0        0     1384 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/runner.py
+-rw-r--r--   0        0        0     1674 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/redis/settings.py
+-rw-r--r--   0        0        0      132 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/__init__.py
+-rw-r--r--   0        0        0     8494 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/manager.py
+-rw-r--r--   0        0        0     2082 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/models.py
+-rw-r--r--   0        0        0      181 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/objects.py
+-rw-r--r--   0        0        0      885 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/transport/s3/settings.py
+-rw-r--r--   0        0        0      103 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/__init__.py
+-rw-r--r--   0        0        0       84 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/mocks.py
+-rw-r--r--   0        0        0      139 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/time.py
+-rw-r--r--   0        0        0      148 2023-07-20 08:50:59.818347 overhave-4.1.1/overhave/utils/url.py
+-rw-r--r--   0        0        0     3522 2023-07-20 08:50:59.822347 overhave-4.1.1/pyproject.toml
+-rw-r--r--   0        0        0    25392 1970-01-01 00:00:00.000000 overhave-4.1.1/PKG-INFO
```

### Comparing `overhave-4.1.0/README.rst` & `overhave-4.1.1/README.rst`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/__init__.py` & `overhave-4.1.1/overhave/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/app.py` & `overhave-4.1.1/overhave/admin/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/files/ace-src/ace.js` & `overhave-4.1.1/overhave/admin/files/ace-src/ace.js`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/files/ace-src/mode-gherkin.js` & `overhave-4.1.1/overhave/admin/files/ace-src/mode-gherkin.js`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/files/css/overhave.css` & `overhave-4.1.1/overhave/admin/files/css/overhave.css`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/files/favicon.ico` & `overhave-4.1.1/overhave/admin/files/favicon.ico`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/flask/flask_admin.py` & `overhave-4.1.1/overhave/admin/flask/flask_admin.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 
 def get_flask_admin(factory: IAdminFactory) -> Admin:
     index_view = OverhaveIndexView(
         name="Info",
         url="/",
         auth_manager=factory.auth_manager,
         index_template_path=factory.context.admin_settings.index_template_path,
+        support_chat_url=factory.context.admin_settings.support_chat_url,
     )
     admin = Admin(
         name="Overhave", template_mode="bootstrap4", index_view=index_view, base_template="overhave_master.html"
     )
     admin.add_link(MenuLink(name="Log out", url="/logout"))
     views_list = [
         FeatureView(db.Feature, db.current_session, category="Scenarios", name="Features"),
```

### Comparing `overhave-4.1.0/overhave/admin/flask/login_manager.py` & `overhave-4.1.1/overhave/admin/flask/login_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/emulation_run_detail.html` & `overhave-4.1.1/overhave/admin/templates/emulation_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/feature.html` & `overhave-4.1.1/overhave/admin/templates/feature.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/login.html` & `overhave-4.1.1/overhave/admin/templates/login.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/test_run.html` & `overhave-4.1.1/overhave/admin/templates/test_run.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/test_run_detail.html` & `overhave-4.1.1/overhave/admin/templates/test_run_detail.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/templates/test_user.html` & `overhave-4.1.1/overhave/admin/templates/test_user.html`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/access.py` & `overhave-4.1.1/overhave/admin/views/access.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/base.py` & `overhave-4.1.1/overhave/admin/views/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/draft.py` & `overhave-4.1.1/overhave/admin/views/draft.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/emulation.py` & `overhave-4.1.1/overhave/admin/views/emulation.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/emulation_run.py` & `overhave-4.1.1/overhave/admin/views/emulation_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/feature.py` & `overhave-4.1.1/overhave/admin/views/feature.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/formatters/formatters.py` & `overhave-4.1.1/overhave/admin/views/formatters/formatters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/formatters/helpers.py` & `overhave-4.1.1/overhave/admin/views/formatters/helpers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/formatters/safe_formatter.py` & `overhave-4.1.1/overhave/admin/views/formatters/safe_formatter.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/index/custom_page.py` & `overhave-4.1.1/overhave/admin/views/index/custom_page.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/index/login_form.py` & `overhave-4.1.1/overhave/admin/views/index/login_form.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/index/view.py` & `overhave-4.1.1/overhave/admin/views/index/view.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 from pathlib import Path
 from typing import Any
 
 import flask
+import httpx
 import ldap
 from flask_admin import AdminIndexView, expose
 from flask_login import login_required, login_user, logout_user
+from markupsafe import Markup
 from sqlalchemy.exc import OperationalError, ProgrammingError
 from werkzeug.wrappers import Response
 from wtforms.validators import ValidationError
 
 from overhave.admin.views.index.custom_page import CustomPageForm
 from overhave.admin.views.index.login_form import LoginForm
 from overhave.entities import IAdminAuthorizationManager
@@ -17,33 +19,43 @@
 logger = logging.getLogger(__name__)
 
 
 class OverhaveIndexView(AdminIndexView):
     """View for index."""
 
     def __init__(
-        self, name: str, url: str, auth_manager: IAdminAuthorizationManager, index_template_path: Path | None
+        self,
+        name: str,
+        url: str,
+        auth_manager: IAdminAuthorizationManager,
+        index_template_path: Path | None,
+        support_chat_url: httpx.URL | None,
     ) -> None:
         super().__init__(
             name=name,
             url=url,
         )
         self._auth_manager = auth_manager
         self._index_template_path = index_template_path
+        self._support_chat_url = support_chat_url
 
     @expose("/login", methods=["GET", "POST"])
     def login(self) -> Any:  # noqa: C901
         form = LoginForm(auth_manager=self._auth_manager)
         if not form.validate_on_submit():
             return self.render("login.html", form=form)
         try:
             user = form.get_user()
             login_user(user)
         except ValidationError:
-            return form.flash_and_redirect("Incorrect username/password pair!")
+            flash_msg = f"Username '{form.username.data}' is not registered!"
+            if self._support_chat_url:
+                flash_msg += f" Please contact the <a href='{self._support_chat_url}'>support channel</a>!"
+
+            return form.flash_and_redirect(Markup(flash_msg))
         except ldap.SERVER_DOWN:
             return form.flash_and_redirect("LDAP auth_managers service is unreachable!")
         except OperationalError:
             logger.exception("DataBase is unreachable!")
             return form.flash_and_redirect("DataBase is unreachable!")
         except ProgrammingError:
             logger.exception("Error while trying to operate with DataBase")
```

### Comparing `overhave-4.1.0/overhave/admin/views/scenario_test_run.py` & `overhave-4.1.1/overhave/admin/views/scenario_test_run.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/tag.py` & `overhave-4.1.1/overhave/admin/views/tag.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/admin/views/testing_users.py` & `overhave-4.1.1/overhave/admin/views/testing_users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/app.py` & `overhave-4.1.1/overhave/api/app.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/auth/regular.py` & `overhave-4.1.1/overhave/api/auth/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/auth/token.py` & `overhave-4.1.1/overhave/api/auth/token.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/deps.py` & `overhave-4.1.1/overhave/api/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/settings.py` & `overhave-4.1.1/overhave/api/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/__init__.py` & `overhave-4.1.1/overhave/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/auth_views.py` & `overhave-4.1.1/overhave/api/views/auth_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/emulation_views.py` & `overhave-4.1.1/overhave/api/views/emulation_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/extra_views.py` & `overhave-4.1.1/overhave/api/views/extra_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/feature_views.py` & `overhave-4.1.1/overhave/api/views/feature_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/tags_views.py` & `overhave-4.1.1/overhave/api/views/tags_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/testrun_views.py` & `overhave-4.1.1/overhave/api/views/testrun_views.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/api/views/testuser_views.py` & `overhave-4.1.1/overhave/api/views/testuser_views.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,25 +17,25 @@
 )
 
 logger = logging.getLogger(__name__)
 
 
 def _get_test_user_by_id_handler(user_id: int, test_user_storage: ITestUserStorage) -> TestUserModel:
     logger.info("Getting %s with user_id=%s...", TestUserModel.__name__, user_id)
-    test_user = test_user_storage.get_test_user_by_id(user_id)
+    test_user = test_user_storage.get_testuser_model_by_id(user_id)
     if test_user is None:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with id={user_id} does not exist!"
         )
     return test_user
 
 
 def _get_test_user_by_key_handler(user_key: str, test_user_storage: ITestUserStorage) -> TestUserModel:
     logger.info("Getting %s with user_key='%s'...", TestUserModel.__name__, user_key)
-    test_user = test_user_storage.get_test_user_by_key(user_key)
+    test_user = test_user_storage.get_testuser_model_by_key(user_key)
     if test_user is None:
         raise fastapi.HTTPException(
             status_code=HTTPStatus.BAD_REQUEST, detail=f"User with key='{user_key}' does not exist!"
         )
     return test_user
```

### Comparing `overhave-4.1.0/overhave/base_settings.py` & `overhave-4.1.1/overhave/base_settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/admin.py` & `overhave-4.1.1/overhave/cli/admin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/api.py` & `overhave-4.1.1/overhave/cli/api.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/consumers.py` & `overhave-4.1.1/overhave/cli/consumers.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/db_cmds/group.py` & `overhave-4.1.1/overhave/cli/db_cmds/group.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/db_cmds/regular.py` & `overhave-4.1.1/overhave/cli/db_cmds/regular.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/s3.py` & `overhave-4.1.1/overhave/cli/s3.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/cli/synchronizer.py` & `overhave-4.1.1/overhave/cli/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/db/base.py` & `overhave-4.1.1/overhave/db/base.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/db/statuses.py` & `overhave-4.1.1/overhave/db/statuses.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/db/tables.py` & `overhave-4.1.1/overhave/db/tables.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/db/users.py` & `overhave-4.1.1/overhave/db/users.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/db/utils.py` & `overhave-4.1.1/overhave/db/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/emulation/emulator.py` & `overhave-4.1.1/overhave/emulation/emulator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/__init__.py` & `overhave-4.1.1/overhave/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/archiver.py` & `overhave-4.1.1/overhave/entities/archiver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/auth_managers/default.py` & `overhave-4.1.1/overhave/entities/auth_managers/default.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/auth_managers/ldap/manager.py` & `overhave-4.1.1/overhave/entities/auth_managers/ldap/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/auth_managers/secret_mixin.py` & `overhave-4.1.1/overhave/entities/auth_managers/secret_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/auth_managers/simple.py` & `overhave-4.1.1/overhave/entities/auth_managers/simple.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/feature/extractor.py` & `overhave-4.1.1/overhave/entities/feature/extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/file_extractor.py` & `overhave-4.1.1/overhave/entities/file_extractor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/git_initializer.py` & `overhave-4.1.1/overhave/entities/git_initializer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/language/prefixes.py` & `overhave-4.1.1/overhave/entities/language/prefixes.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/report_manager/report_manager.py` & `overhave-4.1.1/overhave/entities/report_manager/report_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/entities/settings.py` & `overhave-4.1.1/overhave/entities/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
     # Threadpool size for admin service
     threadpool_process_num: int = 5
 
     # Force filling the tasks field in feature creation
     strict_feature_tasks: bool = False
 
+    # Link to support chat
+    support_chat_url: httpx.URL | None
+
 
 class OverhaveLanguageSettings(BaseOverhavePrefix):
     """Settings for language definitions."""
 
     step_prefixes: StepPrefixesModel | None
```

### Comparing `overhave-4.1.0/overhave/factory/__init__.py` & `overhave-4.1.1/overhave/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/base_factory.py` & `overhave-4.1.1/overhave/factory/base_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/components/admin_factory.py` & `overhave-4.1.1/overhave/factory/components/admin_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/components/emulation_factory.py` & `overhave-4.1.1/overhave/factory/components/emulation_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/components/publication_factory.py` & `overhave-4.1.1/overhave/factory/components/publication_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/components/synchronizer_factory.py` & `overhave-4.1.1/overhave/factory/components/synchronizer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/components/test_execution_factory.py` & `overhave-4.1.1/overhave/factory/components/test_execution_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/consumer_factory.py` & `overhave-4.1.1/overhave/factory/consumer_factory.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/__init__.py` & `overhave-4.1.1/overhave/factory/context/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/admin_context.py` & `overhave-4.1.1/overhave/factory/context/admin_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/base_context.py` & `overhave-4.1.1/overhave/factory/context/base_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/publication_context.py` & `overhave-4.1.1/overhave/factory/context/publication_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/synchronizer_context.py` & `overhave-4.1.1/overhave/factory/context/synchronizer_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/context/test_execution_context.py` & `overhave-4.1.1/overhave/factory/context/test_execution_context.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/factory/getters.py` & `overhave-4.1.1/overhave/factory/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/metrics/client/container.py` & `overhave-4.1.1/overhave/metrics/client/container.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/metrics/getters.py` & `overhave-4.1.1/overhave/metrics/getters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/base_publisher.py` & `overhave-4.1.1/overhave/publication/base_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/errors.py` & `overhave-4.1.1/overhave/publication/errors.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/git_publisher.py` & `overhave-4.1.1/overhave/publication/git_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/gitlab/gitlab_publisher.py` & `overhave-4.1.1/overhave/publication/gitlab/gitlab_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/gitlab/settings.py` & `overhave-4.1.1/overhave/publication/gitlab/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/gitlab/tokenizer/client.py` & `overhave-4.1.1/overhave/publication/gitlab/tokenizer/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/gitlab/tokenizer/settings.py` & `overhave-4.1.1/overhave/publication/gitlab/tokenizer/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/settings.py` & `overhave-4.1.1/overhave/publication/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/stash/settings.py` & `overhave-4.1.1/overhave/publication/stash/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/publication/stash/stash_publisher.py` & `overhave-4.1.1/overhave/publication/stash/stash_publisher.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/config_injector.py` & `overhave-4.1.1/overhave/pytest_plugin/config_injector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/deps.py` & `overhave-4.1.1/overhave/pytest_plugin/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/__init__.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/description_manager.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/description_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/links.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/links.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/severity.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/severity.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/allure_utils/step_context_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/bdd_item.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/bdd_item.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/parsed_info.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/parsed_info.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/helpers/tag_controller.py` & `overhave-4.1.1/overhave/pytest_plugin/helpers/tag_controller.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/plugin.py` & `overhave-4.1.1/overhave/pytest_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/plugin_resolver.py` & `overhave-4.1.1/overhave/pytest_plugin/plugin_resolver.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/pytest_plugin/proxy_manager.py` & `overhave-4.1.1/overhave/pytest_plugin/proxy_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/__init__.py` & `overhave-4.1.1/overhave/scenario/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/compiler/compiler.py` & `overhave-4.1.1/overhave/scenario/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/compiler/settings.py` & `overhave-4.1.1/overhave/scenario/compiler/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/file_manager/file_manager.py` & `overhave-4.1.1/overhave/scenario/file_manager/file_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/file_manager/settings.py` & `overhave-4.1.1/overhave/scenario/file_manager/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/parser/models.py` & `overhave-4.1.1/overhave/scenario/parser/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/parser/parser.py` & `overhave-4.1.1/overhave/scenario/parser/parser.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/validator/duplicate_id_mixin.py` & `overhave-4.1.1/overhave/scenario/validator/duplicate_id_mixin.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/scenario/validator/validator.py` & `overhave-4.1.1/overhave/scenario/validator/validator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/__init__.py` & `overhave-4.1.1/overhave/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/api_auth_storage.py` & `overhave-4.1.1/overhave/storage/api_auth_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/converters.py` & `overhave-4.1.1/overhave/storage/converters.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/draft_storage.py` & `overhave-4.1.1/overhave/storage/draft_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/emulation_storage.py` & `overhave-4.1.1/overhave/storage/emulation_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/feature_storage.py` & `overhave-4.1.1/overhave/storage/feature_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/feature_tag_storage.py` & `overhave-4.1.1/overhave/storage/feature_tag_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/feature_type_storage.py` & `overhave-4.1.1/overhave/storage/feature_type_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/scenario_storage.py` & `overhave-4.1.1/overhave/storage/scenario_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/system_user_group_storage.py` & `overhave-4.1.1/overhave/storage/system_user_group_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/system_user_storage.py` & `overhave-4.1.1/overhave/storage/system_user_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/test_run_storage.py` & `overhave-4.1.1/overhave/storage/test_run_storage.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/storage/test_user_storage.py` & `overhave-4.1.1/overhave/storage/test_user_storage.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import abc
 
+import sqlalchemy as sa
 import sqlalchemy.orm as so
 
 from overhave import db
 from overhave.storage import TestUserModel, TestUserSpecification
 from overhave.utils import get_current_time
 
 
@@ -24,65 +25,53 @@
 
 
 class ITestUserStorage(abc.ABC):
     """Abstract class for Test User storage."""
 
     @staticmethod
     @abc.abstractmethod
-    def get_test_user_by_id(user_id: int) -> TestUserModel | None:
+    def get_testuser_model_by_id(user_id: int) -> TestUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def get_test_user_by_key(key: str) -> TestUserModel | None:
+    def get_testuser_model_by_key(key: str) -> TestUserModel | None:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def get_test_users_by_feature_type_name(
         session: so.Session, feature_type_id: int, allow_update: bool
     ) -> list[TestUserModel]:
         pass
 
     @staticmethod
     @abc.abstractmethod
-    def create_test_user(
-        key: str,
-        name: str,
-        specification: TestUserSpecification,
-        created_by: str,
-        feature_type_id: int,
-        allow_update: bool,
-    ) -> TestUserModel:
-        pass
-
-    @staticmethod
-    @abc.abstractmethod
     def update_test_user_specification(user_id: int, specification: TestUserSpecification) -> None:
         pass
 
     @staticmethod
     @abc.abstractmethod
     def delete_test_user(user_id: int) -> None:
         pass
 
 
 class TestUserStorage(ITestUserStorage):
     """Class for Test User storage."""
 
     @staticmethod
-    def get_test_user_by_id(user_id: int) -> TestUserModel | None:
+    def get_testuser_model_by_id(user_id: int) -> TestUserModel | None:
         with db.create_session() as session:
             user = session.get(db.TestUser, user_id)
             if user is not None:
                 return TestUserModel.from_orm(user)
             return None
 
     @staticmethod
-    def get_test_user_by_key(key: str) -> TestUserModel | None:
+    def get_testuser_model_by_key(key: str) -> TestUserModel | None:
         with db.create_session() as session:
             user: db.TestUser | None = session.query(db.TestUser).filter(db.TestUser.key == key).one_or_none()
             if user is not None:
                 return TestUserModel.from_orm(user)
             return None
 
     @staticmethod
@@ -93,46 +82,26 @@
             session.query(db.TestUser)
             .filter(db.TestUser.feature_type_id == feature_type_id, db.TestUser.allow_update.is_(allow_update))
             .all()
         )
         return [TestUserModel.from_orm(user) for user in db_users]
 
     @staticmethod
-    def create_test_user(
-        key: str,
-        name: str,
-        specification: TestUserSpecification,
-        created_by: str,
-        feature_type_id: int,
-        allow_update: bool,
-    ) -> TestUserModel:
-        with db.create_session() as session:
-            test_user = db.TestUser(
-                key=key,
-                name=name,
-                specification=specification,
-                feature_type_id=feature_type_id,
-                created_by=created_by,
-                allow_update=allow_update,
-                changed_at=get_current_time(),
-            )
-            session.add(test_user)
-            session.flush()
-            return TestUserModel.from_orm(test_user)
-
-    @staticmethod
     def update_test_user_specification(user_id: int, specification: TestUserSpecification) -> None:
         with db.create_session() as session:
             test_user = session.get(db.TestUser, user_id)
             if test_user is None:
                 raise TestUserDoesNotExistError(f"Test user with id {user_id} does not exist!")
             if not test_user.allow_update:
                 raise TestUserUpdatingNotAllowedError(f"Test user updating with id {user_id} not allowed!")
-            test_user.specification = specification
-            test_user.changed_at = get_current_time()
+            session.execute(
+                sa.update(db.TestUser)
+                .where(db.TestUser.id == test_user.id)
+                .values(specification=specification, changed_at=get_current_time())
+            )
 
     @staticmethod
     def delete_test_user(user_id: int) -> None:
         with db.create_session() as session:
             user = session.get(db.TestUser, user_id)
             if user is None:
                 raise TestUserDoesNotExistError(f"Test user with id {user_id} does not exist!")
```

### Comparing `overhave-4.1.0/overhave/synchronization/storage_manager.py` & `overhave-4.1.1/overhave/synchronization/storage_manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/synchronization/synchronizer.py` & `overhave-4.1.1/overhave/synchronization/synchronizer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/test_execution/executor.py` & `overhave-4.1.1/overhave/test_execution/executor.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/test_execution/objects.py` & `overhave-4.1.1/overhave/test_execution/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/test_execution/settings.py` & `overhave-4.1.1/overhave/test_execution/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/test_execution/step_collector.py` & `overhave-4.1.1/overhave/test_execution/step_collector.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/test_execution/test_runner.py` & `overhave-4.1.1/overhave/test_execution/test_runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/__init__.py` & `overhave-4.1.1/overhave/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/__init__.py` & `overhave-4.1.1/overhave/transport/http/__init__.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/api_client/authenticator.py` & `overhave-4.1.1/overhave/transport/http/api_client/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/base_client/auth.py` & `overhave-4.1.1/overhave/transport/http/base_client/auth.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/base_client/client.py` & `overhave-4.1.1/overhave/transport/http/base_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/base_client/settings.py` & `overhave-4.1.1/overhave/transport/http/base_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/gitlab_client/client.py` & `overhave-4.1.1/overhave/transport/http/gitlab_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/gitlab_client/models.py` & `overhave-4.1.1/overhave/transport/http/gitlab_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/gitlab_client/utils.py` & `overhave-4.1.1/overhave/transport/http/gitlab_client/utils.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/stash_client/client.py` & `overhave-4.1.1/overhave/transport/http/stash_client/client.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/stash_client/models.py` & `overhave-4.1.1/overhave/transport/http/stash_client/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/http/stash_client/settings.py` & `overhave-4.1.1/overhave/transport/http/stash_client/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/ldap/authenticator.py` & `overhave-4.1.1/overhave/transport/ldap/authenticator.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/consumer.py` & `overhave-4.1.1/overhave/transport/redis/consumer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/deps.py` & `overhave-4.1.1/overhave/transport/redis/deps.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/objects.py` & `overhave-4.1.1/overhave/transport/redis/objects.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/producer.py` & `overhave-4.1.1/overhave/transport/redis/producer.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/runner.py` & `overhave-4.1.1/overhave/transport/redis/runner.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/redis/settings.py` & `overhave-4.1.1/overhave/transport/redis/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/s3/manager.py` & `overhave-4.1.1/overhave/transport/s3/manager.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/s3/models.py` & `overhave-4.1.1/overhave/transport/s3/models.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/overhave/transport/s3/settings.py` & `overhave-4.1.1/overhave/transport/s3/settings.py`

 * *Files identical despite different names*

### Comparing `overhave-4.1.0/pyproject.toml` & `overhave-4.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "overhave"
-version = "4.1.0"
+version = "4.1.1"
 description = "Overhave - web-framework for BDD"
 readme = "README.rst"
 authors = [
     "Vladislav Mukhamatnurov <livestreamepidemz@yandex.ru>",
     "Tinkoff Backend Dialog System Team <bds-dev@tinkoff.ru>"
 ]
 classifiers = [
```

### Comparing `overhave-4.1.0/PKG-INFO` & `overhave-4.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overhave
-Version: 4.1.0
+Version: 4.1.1
 Summary: Overhave - web-framework for BDD
 Author: Vladislav Mukhamatnurov
 Author-email: livestreamepidemz@yandex.ru
 Requires-Python: >=3.8,<3.12
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: Flask
 Classifier: Framework :: Pytest
```

