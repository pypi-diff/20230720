# Comparing `tmp/preset-cli-0.2.3.tar.gz` & `tmp/preset-cli-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "preset-cli-0.2.3.tar", last modified: Fri Jul 14 22:32:32 2023, max compression
+gzip compressed data, was "preset-cli-0.2.4.tar", last modified: Thu Jul 20 16:14:06 2023, max compression
```

## Comparing `preset-cli-0.2.3.tar` & `preset-cli-0.2.4.tar`

### file list

```diff
@@ -1,150 +1,150 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.536189 preset-cli-0.2.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-package-daily.yml
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-14 22:32:20.000000 preset-cli-0.2.3/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-14 22:32:20.000000 preset-cli-0.2.3/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10494 2023-07-14 22:32:20.000000 preset-cli-0.2.3/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-14 22:32:20.000000 preset-cli-0.2.3/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-14 22:32:20.000000 preset-cli-0.2.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-14 22:32:20.000000 preset-cli-0.2.3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-14 22:32:32.552189 preset-cli-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-14 22:32:20.000000 preset-cli-0.2.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-14 22:32:20.000000 preset-cli-0.2.3/dev-requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-14 22:32:20.000000 preset-cli-0.2.3/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/contributing.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/images/export_dashboards.png
--rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-14 22:32:20.000000 preset-cli-0.2.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/charts/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/charts/Total_count_134.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/dashboards/
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/dashboards/White_label_test.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/databases/
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/databases/Google_Sheets.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/examples/exports/datasets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/country_cnt.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/examples/exports/functions/
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/functions/demo.py
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-14 22:32:20.000000 preset-cli-0.2.3/examples/exports/metadata.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-14 22:32:20.000000 preset-cli-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-14 22:32:20.000000 preset-cli-0.2.3/requirements.in
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-14 22:32:20.000000 preset-cli-0.2.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-14 22:32:32.552189 preset-cli-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-14 22:32:20.000000 preset-cli-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.532189 preset-cli-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli/
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20803 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/dbt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)    35569 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/clients/superset.py
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/api/operators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/password.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/preset.py
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/auth/token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7872 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/export.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/import_.py
--rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sql.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/exposures.py
--rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.544189 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-14 22:32:20.000000 preset-cli-0.2.3/src/preset_cli/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.540189 preset-cli-0.2.3/src/preset_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-14 22:32:32.000000 preset-cli-0.2.3/src/preset_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/api/clients/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    53266 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/dbt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/preset_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    90501 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/api/clients/superset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/auth/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/jwt_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/password_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/auth/preset_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/superset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/import_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/main_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sql_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.548189 preset-cli-0.2.3/tests/cli/superset/sync/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/tests/cli/superset/sync/dbt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/databases_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/datasets_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/exposures_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/dbt/metrics_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:32.552189 preset-cli-0.2.3/tests/cli/superset/sync/native/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/native/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/cli/superset/sync/native/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tests/lib_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-14 22:32:20.000000 preset-cli-0.2.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-package-daily.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      984 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2261 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-07-20 16:13:55.000000 preset-cli-0.2.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-07-20 16:13:55.000000 preset-cli-0.2.4/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-07-20 16:13:55.000000 preset-cli-0.2.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    13862 2023-07-20 16:13:55.000000 preset-cli-0.2.4/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 16:13:55.000000 preset-cli-0.2.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-07-20 16:13:55.000000 preset-cli-0.2.4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-20 16:14:06.496666 preset-cli-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    24105 2023-07-20 16:13:55.000000 preset-cli-0.2.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-07-20 16:13:55.000000 preset-cli-0.2.4/dev-requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-07-20 16:13:55.000000 preset-cli-0.2.4/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9753 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/contributing.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.484666 preset-cli-0.2.4/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   271378 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/images/export_dashboards.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-07-20 16:13:55.000000 preset-cli-0.2.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/charts/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/charts/Total_count_134.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/dashboards/
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/dashboards/White_label_test.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/databases/
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/databases/Google_Sheets.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.468665 preset-cli-0.2.4/examples/exports/datasets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      943 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/country_cnt.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/examples/exports/functions/
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/functions/demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-07-20 16:13:55.000000 preset-cli-0.2.4/examples/exports/metadata.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 16:13:55.000000 preset-cli-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-07-20 16:13:55.000000 preset-cli-0.2.4/requirements.in
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-07-20 16:13:55.000000 preset-cli-0.2.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-07-20 16:14:06.496666 preset-cli-0.2.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-07-20 16:13:55.000000 preset-cli-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.472666 preset-cli-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20818 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/dbt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8520 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37259 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/clients/superset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      454 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/api/operators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/preset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/auth/token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20191 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/import_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3607 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5136 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sql.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11602 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7336 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5541 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/exposures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13561 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3554 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11573 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3282 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-07-20 16:13:55.000000 preset-cli-0.2.4/src/preset_cli/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.488666 preset-cli-0.2.4/src/preset_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    24916 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 16:14:06.000000 preset-cli-0.2.4/src/preset_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.492666 preset-cli-0.2.4/tests/api/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53266 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/dbt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14306 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/preset_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    95330 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/api/clients/superset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/auth/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/jwt_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2198 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1576 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/password_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/auth/preset_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52383 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17864 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/import_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3702 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/main_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11781 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sql_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/dbt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34503 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12832 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/databases_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34788 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/datasets_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28144 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/exposures_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16342 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/dbt/metrics_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 16:14:06.496666 preset-cli-0.2.4/tests/cli/superset/sync/native/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/native/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26997 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/cli/superset/sync/native/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tests/lib_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2007 2023-07-20 16:13:55.000000 preset-cli-0.2.4/tox.ini
```

### Comparing `preset-cli-0.2.3/.coveragerc` & `preset-cli-0.2.4/.coveragerc`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/.github/workflows/python-package-daily.yml` & `preset-cli-0.2.4/.github/workflows/python-package-daily.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/.github/workflows/python-package.yml` & `preset-cli-0.2.4/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/.github/workflows/python-publish.yml` & `preset-cli-0.2.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/.gitignore` & `preset-cli-0.2.4/.gitignore`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/.pre-commit-config.yaml` & `preset-cli-0.2.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/CHANGELOG.rst` & `preset-cli-0.2.4/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,20 @@
 =========
 Changelog
 =========
 
 Next
 ====
 
+Version 0.2.4 - 2023-07-20
+==========================
+
+- Further adjustments to dbt marshmallow schemas to avoid integration errors (`#228 <https://github.com/preset-io/backend-sdk/pull/228>_`).
+- Export RLS rules is now compatible with Preset Cloud and older Superset installations (`#227 <https://github.com/preset-io/backend-sdk/pull/227>_`)
+
 Version 0.2.3 - 2023-07-14
 ==========================
 
 - Adjustments to dbt marshmallow schemas to avoid integration errors (`#225 <https://github.com/preset-io/backend-sdk/pull/225>_`).
 
 Version 0.2.2 - 2023-07-05
 ==========================
```

### Comparing `preset-cli-0.2.3/CONTRIBUTING.rst` & `preset-cli-0.2.4/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/Makefile` & `preset-cli-0.2.4/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/PKG-INFO` & `preset-cli-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.3/README.rst` & `preset-cli-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/dev-requirements.txt` & `preset-cli-0.2.4/dev-requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/docs/Makefile` & `preset-cli-0.2.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/docs/conf.py` & `preset-cli-0.2.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/docs/images/export_dashboards.png` & `preset-cli-0.2.4/docs/images/export_dashboards.png`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/docs/index.rst` & `preset-cli-0.2.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/examples/exports/charts/Total_count_134.yaml` & `preset-cli-0.2.4/examples/exports/charts/Total_count_134.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/examples/exports/dashboards/White_label_test.yaml` & `preset-cli-0.2.4/examples/exports/dashboards/White_label_test.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/examples/exports/datasets/Google_Sheets/country_cnt.yaml` & `preset-cli-0.2.4/examples/exports/datasets/Google_Sheets/country_cnt.yaml`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/requirements.txt` & `preset-cli-0.2.4/requirements.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/setup.cfg` & `preset-cli-0.2.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/setup.py` & `preset-cli-0.2.4/setup.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/api/clients/dbt.py` & `preset-cli-0.2.4/src/preset_cli/api/clients/dbt.py`

 * *Files 0% similar despite different names*

```diff
@@ -371,15 +371,15 @@
 
     # not present in the spec
     full_name = fields.String(allow_none=True)
     repository_credentials_id = fields.Integer(allow_none=True)
     gitlab = fields.String(allow_none=True)
     name = fields.String()
     pull_request_url_template = fields.String(allow_none=True)
-    git_provider_id = fields.Integer()
+    git_provider_id = fields.Integer(allow_none=True)
     git_provider = fields.String(allow_none=True)
     project_id = fields.Integer()
     deploy_key = fields.Nested(DeployKeySchema)
     github_repo = fields.String(allow_none=True)
 
 
 class ProjectSchema(PostelSchema):
```

### Comparing `preset-cli-0.2.3/src/preset_cli/api/clients/preset.py` & `preset-cli-0.2.4/src/preset_cli/api/clients/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/api/clients/superset.py` & `preset-cli-0.2.4/src/preset_cli/api/clients/superset.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,15 +187,15 @@
 
 
 class RuleType(TypedDict):
     """
     Schema for an RLS rule.
     """
 
-    name: str
+    name: Optional[str]
     description: Optional[str]
     filter_type: str
     tables: List[str]
     roles: List[str]
     group_key: str
     clause: str
 
@@ -686,14 +686,20 @@
         )
         validate_response(response)
 
         payload = response.json()
 
         return payload["message"] == "OK"
 
+    def get_rls(self, **kwargs: str) -> List[Any]:
+        """
+        Return RLS rules, possibly filtered.
+        """
+        return self.get_resources("rowlevelsecurity", **kwargs)
+
     def export_users(self) -> Iterator[UserType]:
         """
         Return all users.
         """
         # For on-premise OSS Superset we can fetch the list of users by crawling the
         # ``/users/list/`` page. For a Preset workspace we need custom logic to talk
         # to Manager.
@@ -804,17 +810,17 @@
 
                 yield {
                     "name": name,
                     "permissions": permissions,
                     "users": users,
                 }
 
-    def export_rls(self) -> Iterator[RuleType]:
+    def export_rls_legacy(self) -> Iterator[RuleType]:
         """
-        Return all RLS rules.
+        Return all RLS rules from legacy endpoint.
         """
         page = 0
         while True:
             params = {
                 "psize_RowLevelSecurityFiltersModelView": MAX_PAGE_SIZE,
                 "page_RowLevelSecurityFiltersModelView": page,
             }
@@ -853,22 +859,63 @@
                     ("description", str),
                     ("filter_type", str),
                     ("tables", parse_html_array),
                     ("roles", parse_html_array),
                     ("group_key", str),
                     ("clause", str),
                 ]
+
+                # Before Superset 2.1.0, RLS dont have name and description
+                if table.find("th").text.strip() == "Filter Type":
+                    keys.remove(("name", str))
+                    keys.remove(("description", str))
+
                 yield cast(
                     RuleType,
                     {
                         key: parse(tr.find("td").text.strip())
                         for (key, parse), tr in zip(keys, table.find_all("tr"))
                     },
                 )
 
+    def export_rls(self) -> Iterator[RuleType]:
+        """
+        Return all RLS rules.
+        """
+        url = self.baseurl / "api/v1/rowlevelsecurity/"
+        response = self.session.get(url)
+        if response.status_code == 200:
+            for rule in self.get_rls():
+                keys = [
+                    "name",
+                    "description",
+                    "filter_type",
+                    "tables",
+                    "roles",
+                    "group_key",
+                    "clause",
+                ]
+                data = {}
+                for key in keys:
+                    if key == "tables":
+                        data[key] = [
+                            f"{inner_item['schema']}.{inner_item['table_name']}"
+                            for inner_item in rule.get(key, [])
+                        ]
+                    elif key == "roles":
+                        data[key] = [
+                            inner_item["name"] for inner_item in rule.get(key, [])
+                        ]
+                    else:
+                        data[key] = rule.get(key)
+                yield cast(RuleType, data)
+
+        else:
+            yield from self.export_rls_legacy()
+
     def import_role(self, role: RoleType) -> None:  # pylint: disable=too-many-locals
         """
         Import a given role.
 
         Note: this only works with Preset workspaces for now, since it translates the
         Superset permissions to the Preset permissions.
         """
```

### Comparing `preset-cli-0.2.3/src/preset_cli/auth/jwt.py` & `preset-cli-0.2.4/src/preset_cli/auth/jwt.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/auth/lib.py` & `preset-cli-0.2.4/src/preset_cli/auth/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/auth/main.py` & `preset-cli-0.2.4/src/preset_cli/auth/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/auth/password.py` & `preset-cli-0.2.4/src/preset_cli/auth/password.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/auth/preset.py` & `preset-cli-0.2.4/src/preset_cli/auth/preset.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/main.py` & `preset-cli-0.2.4/src/preset_cli/cli/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/export.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/export.py`

 * *Files 1% similar despite different names*

```diff
@@ -237,15 +237,15 @@
     Export RLS rules to a YAML file.
     """
     auth = ctx.obj["AUTH"]
     url = URL(ctx.obj["INSTANCE"])
     client = SupersetClient(url, auth)
 
     with open(path, "w", encoding="utf-8") as output:
-        yaml.dump(list(client.export_rls()), output)
+        yaml.dump(list(client.export_rls()), output, sort_keys=False)
 
 
 @click.command()
 @click.argument(
     "path",
     type=click.Path(resolve_path=True),
     default="ownership.yaml",
```

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/import_.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/import_.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/main.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/main.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sql.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sql.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/command.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/databases.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/databases.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/datasets.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/datasets.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/exposures.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/exposures.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/lib.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/dbt/metrics.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/dbt/metrics.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/cli/superset/sync/native/command.py` & `preset-cli-0.2.4/src/preset_cli/cli/superset/sync/native/command.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/exceptions.py` & `preset-cli-0.2.4/src/preset_cli/exceptions.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli/lib.py` & `preset-cli-0.2.4/src/preset_cli/lib.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli.egg-info/PKG-INFO` & `preset-cli-0.2.4/src/preset_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: preset-cli
-Version: 0.2.3
+Version: 0.2.4
 Summary: A CLI to interact with Preset (https://preset.io/) workspaces.
 Home-page: https://github.com/preset-io/backend-sdk
 Author: Beto Dealmeida
 Author-email: beto@preset.io
 License: Other/Proprietary License
 Project-URL: Documentation, https://github.com/preset-io/backend-sdk/blob/master/README.rst
 Platform: any
```

### Comparing `preset-cli-0.2.3/src/preset_cli.egg-info/SOURCES.txt` & `preset-cli-0.2.4/src/preset_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/src/preset_cli.egg-info/requires.txt` & `preset-cli-0.2.4/src/preset_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/api/clients/dbt_test.py` & `preset-cli-0.2.4/tests/api/clients/dbt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/api/clients/preset_test.py` & `preset-cli-0.2.4/tests/api/clients/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/api/clients/superset_test.py` & `preset-cli-0.2.4/tests/api/clients/superset_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -1231,14 +1231,26 @@
         client.import_zip("database", data, overwrite=True)
     assert excinfo.value.errors == [{"message": "An error occurred"}]
     assert (
         requests_mock.last_request.headers["Referer"] == "https://superset.example.org/"
     )
 
 
+def test_get_rls(mocker: MockerFixture) -> None:
+    """
+    Test the ``get_rls`` method.
+    """
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    get_resources = mocker.patch.object(client, "get_resources")
+
+    client.get_rls()
+    get_resources.assert_called_with("rowlevelsecurity")
+
+
 def test_export_users(requests_mock: Mocker) -> None:
     """
     Test ``export_users``.
     """
     requests_mock.get("https://superset.example.org/users/list/")
     requests_mock.get(
         "https://superset.example.org/users/list/?psize_UserDBModelView=100&page_UserDBModelView=0",
@@ -1664,17 +1676,17 @@
             "name": "Public",
             "permissions": [],
             "users": [],
         },
     ]
 
 
-def test_export_rls(requests_mock: Mocker) -> None:
+def test_export_rls_legacy(requests_mock: Mocker) -> None:
     """
-    Test ``export_rls``.
+    Test ``export_rls_legacy``.
     """
     requests_mock.get(
         (
             "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
             "psize_RowLevelSecurityFiltersModelView=100&"
             "page_RowLevelSecurityFiltersModelView=0"
         ),
@@ -1762,30 +1774,194 @@
   </body>
 </html>
         """,
     )
 
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
-    assert list(client.export_rls()) == [
+    assert list(client.export_rls_legacy()) == [
         {
             "name": "My Rule",
             "description": "This is a rule. There are many others like it, but this one is mine.",
             "filter_type": "Regular",
             "tables": ["main.test_table"],
             "roles": ["Gamma"],
             "group_key": "department",
             "clause": "client_id = 9",
         },
     ]
 
 
-def test_export_rls_no_rules(requests_mock: Mocker) -> None:
+def test_export_rls_legacy_older_superset(requests_mock: Mocker) -> None:
+    """
+    Test ``export_rls_legacy`` with older Superset version.
+    """
+    requests_mock.get(
+        (
+            "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
+            "psize_RowLevelSecurityFiltersModelView=100&"
+            "page_RowLevelSecurityFiltersModelView=0"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Filter Type</th>
+        <th>Tables</th>
+        <th>Roles</th>
+        <th>Clause</th>
+        <th>Creator</th>
+        <th>Modified</th>
+      </tr>
+      <tr>
+        <td><input id="1" /></td>
+        <td>Regular</td>
+        <td>[main.test_table]</td>
+        <td>client_id = 9</td>
+        <td>admin admin</td>
+        <td>35 minutes ago</td>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        (
+            "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
+            "psize_RowLevelSecurityFiltersModelView=100&"
+            "page_RowLevelSecurityFiltersModelView=1"
+        ),
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table></table>
+    <table>
+      <tr>
+        <th></th>
+        <th>Filter Type</th>
+        <th>Tables</th>
+        <th>Roles</th>
+        <th>Clause</th>
+        <th>Creator</th>
+        <th>Modified</th>
+      </tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+    requests_mock.get(
+        "https://superset.example.org/rowlevelsecurityfiltersmodelview/show/1",
+        text="""
+<!DOCTYPE html>
+<html lang="en">
+  <head>
+    <meta charset="utf-8">
+  </head>
+  <body>
+    <table>
+      <tr><th>Filter Type</th><td>Regular</td></tr>
+      <tr><th>Tables</th><td>[main.test_table]</td></tr>
+      <tr><th>Roles</th><td>[Gamma]</td></tr>
+      <tr><th>Group Key</th><td>department</td></tr>
+      <tr><th>Clause</th><td>client_id = 9</td></tr>
+    </table>
+  </body>
+</html>
+        """,
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+    assert list(client.export_rls_legacy()) == [
+        {
+            "filter_type": "Regular",
+            "tables": ["main.test_table"],
+            "roles": ["Gamma"],
+            "group_key": "department",
+            "clause": "client_id = 9",
+        },
+    ]
+
+
+def test_export_rls_legacy_route(requests_mock: Mocker, mocker: MockerFixture) -> None:
+    """
+    Test ``export_rls`` going through the legacy route
+    """
+    requests_mock.get(
+        "https://superset.example.org/api/v1/rowlevelsecurity/",
+        status_code=404,
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+
+    export_rls_legacy = mocker.patch.object(client, "export_rls_legacy")
+    list(client.export_rls())
+    export_rls_legacy.assert_called_once()
+
+
+def test_export_rls(requests_mock: Mocker, mocker: MockerFixture) -> None:
+    """
+    Test ``export_rls``
+    """
+    requests_mock.get(
+        "https://superset.example.org/api/v1/rowlevelsecurity/",
+        status_code=200,
+    )
+
+    auth = Auth()
+    client = SupersetClient("https://superset.example.org/", auth)
+
+    get_rls = mocker.patch.object(client, "get_rls")
+    get_rls.return_value = [
+        {
+            "changed_on_delta_humanized": "2 days ago",
+            "clause": "client_id = 9",
+            "description": "This is a rule. There are many others like it, but this one is mine.",
+            "filter_type": "Regular",
+            "group_key": "department",
+            "id": 9,
+            "name": "My Rule",
+            "roles": [{"id": 1, "name": "Admin"}, {"id": 2, "name": "Gamma"}],
+            "tables": [
+                {"id": 18, "schema": "main", "table_name": "test_table"},
+                {"id": 20, "schema": "main", "table_name": "second_test"},
+            ],
+        },
+    ]
+
+    assert list(client.export_rls()) == [
+        {
+            "name": "My Rule",
+            "description": "This is a rule. There are many others like it, but this one is mine.",
+            "filter_type": "Regular",
+            "tables": ["main.test_table", "main.second_test"],
+            "roles": ["Admin", "Gamma"],
+            "group_key": "department",
+            "clause": "client_id = 9",
+        },
+    ]
+
+
+def test_export_rls_legacy_no_rules(requests_mock: Mocker) -> None:
     """
-    Test ``export_rls``.
+    Test ``export_rls_legacy`` with no rows returned.
     """
     requests_mock.get(
         (
             "https://superset.example.org/rowlevelsecurityfiltersmodelview/list/?"
             "psize_RowLevelSecurityFiltersModelView=100&"
             "page_RowLevelSecurityFiltersModelView=0"
         ),
@@ -1801,15 +1977,15 @@
   </body>
 </html>
         """,
     )
 
     auth = Auth()
     client = SupersetClient("https://superset.example.org/", auth)
-    assert list(client.export_rls()) == []
+    assert list(client.export_rls_legacy()) == []
 
 
 def test_export_ownership(mocker: MockerFixture) -> None:
     """
     Test ``export_ownership``.
     """
     mocker.patch.object(
```

### Comparing `preset-cli-0.2.3/tests/auth/jwt_test.py` & `preset-cli-0.2.4/tests/auth/jwt_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/auth/lib_test.py` & `preset-cli-0.2.4/tests/auth/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/auth/main_test.py` & `preset-cli-0.2.4/tests/auth/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/auth/password_test.py` & `preset-cli-0.2.4/tests/auth/password_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/auth/preset_test.py` & `preset-cli-0.2.4/tests/auth/preset_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/main_test.py` & `preset-cli-0.2.4/tests/cli/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/export_test.py` & `preset-cli-0.2.4/tests/cli/superset/export_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/import_test.py` & `preset-cli-0.2.4/tests/cli/superset/import_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/main_test.py` & `preset-cli-0.2.4/tests/cli/superset/main_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sql_test.py` & `preset-cli-0.2.4/tests/cli/superset/sql_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/command_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/databases_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/databases_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/datasets_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/datasets_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/exposures_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/exposures_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/lib_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/manifest.json` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/manifest.json`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/dbt/metrics_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/dbt/metrics_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/cli/superset/sync/native/command_test.py` & `preset-cli-0.2.4/tests/cli/superset/sync/native/command_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tests/lib_test.py` & `preset-cli-0.2.4/tests/lib_test.py`

 * *Files identical despite different names*

### Comparing `preset-cli-0.2.3/tox.ini` & `preset-cli-0.2.4/tox.ini`

 * *Files identical despite different names*

