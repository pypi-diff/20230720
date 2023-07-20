# Comparing `tmp/ansible-compat-4.1.2.tar.gz` & `tmp/ansible-compat-4.1.4.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansible-compat-4.1.2.tar", last modified: Thu Jun  1 12:54:10 2023, max compression
+gzip compressed data, was "ansible-compat-4.1.4.dev0.tar", last modified: Thu Jul 20 10:38:52 2023, max compression
```

## Comparing `ansible-compat-4.1.2.tar` & `ansible-compat-4.1.4.dev0.tar`

### file list

```diff
@@ -1,118 +1,122 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.930106 ansible-compat-4.1.2/.github/
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.934106 ansible-compat-4.1.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/workflows/ack.yml
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/workflows/push.yml
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.github/workflows/tox.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3807 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.prettierignore
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.prettierrc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.readthedocs.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.934106 ansible-compat-4.1.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      458 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.vscode/extensions.json
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/.yamllint
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.934106 ansible-compat-4.1.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/docs/api.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.934106 ansible-compat-4.1.2/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/docs/images/logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/docs/images/logo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.914106 ansible-compat-4.1.2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.938107 ansible-compat-4.1.2/examples/reqs_broken/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/examples/reqs_broken/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.938107 ansible-compat-4.1.2/examples/reqs_v1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/examples/reqs_v1/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.938107 ansible-compat-4.1.2/examples/reqs_v2/
--rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/examples/reqs_v2/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4298 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.914106 ansible-compat-4.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.942107 ansible-compat-4.1.2/src/ansible_compat/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/ports.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    34629 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/src/ansible_compat/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.946107 ansible-compat-4.1.2/src/ansible_compat.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2244 2023-06-01 12:54:10.000000 ansible-compat-4.1.2/src/ansible_compat.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2342 2023-06-01 12:54:10.000000 ansible-compat-4.1.2/src/ansible_compat.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-01 12:54:10.000000 ansible-compat-4.1.2/src/ansible_compat.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-01 12:54:10.000000 ansible-compat-4.1.2/src/ansible_compat.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-06-01 12:54:10.000000 ansible-compat-4.1.2/src/ansible_compat.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.950107 ansible-compat-4.1.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.950107 ansible-compat-4.1.2/test/assets/
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/assets/requirements-invalid-collection.yml
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/assets/requirements-invalid-role.yml
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/assets/validate0_data.json
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/assets/validate0_expected.json
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/assets/validate0_schema.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.914106 ansible-compat-4.1.2/test/collections/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.broken/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.broken/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.goodies/
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/galaxy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.918106 ansible-compat-4.1.2/test/collections/acme.goodies/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.goodies/molecule/default/
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/molecule/default/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/molecule/default/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.918106 ansible-compat-4.1.2/test/collections/acme.goodies/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.918106 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.918106 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/molecule/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
--rw-r--r--   0 runner    (1001) docker     (123)      156 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/tasks/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/roles/baz/tasks/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/collections/acme.goodies/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/collections/acme.goodies/tests/requirements.yml
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.922106 ansible-compat-4.1.2/test/roles/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.954107 ansible-compat-4.1.2/test/roles/acme.missing_deps/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/test/roles/acme.missing_deps/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/acme.missing_deps/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/acme.missing_deps/requirements.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.918106 ansible-compat-4.1.2/test/roles/acme.sample2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/test/roles/acme.sample2/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/acme.sample2/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.922106 ansible-compat-4.1.2/test/roles/ansible-role-sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/test/roles/ansible-role-sample/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/ansible-role-sample/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.922106 ansible-compat-4.1.2/test/roles/sample3/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/test/roles/sample3/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/sample3/meta/main.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.922106 ansible-compat-4.1.2/test/roles/sample4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-01 12:54:10.958107 ansible-compat-4.1.2/test/roles/sample4/meta/
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/roles/sample4/meta/main.yml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_configuration_example.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_loaders.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_prerun.py
--rw-r--r--   0 runner    (1001) docker     (123)    27639 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_runtime_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/test/test_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-01 12:53:53.000000 ansible-compat-4.1.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/ack.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/push.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3085 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.github/workflows/tox.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.packit.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3999 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.prettierignore
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.prettierrc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.readthedocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      458 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/.yamllint
+-rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/api.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)    10993 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/images/logo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.573446 ansible-compat-4.1.4.dev0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_broken/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_broken/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_v1/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v1/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.581446 ansible-compat-4.1.4.dev0/examples/reqs_v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     7615 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v2/community-molecule-0.1.0.tar.gz
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/examples/reqs_v2/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2265 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4322 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     6305 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.573446 ansible-compat-4.1.4.dev0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/src/ansible_compat/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16108 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/ports.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    35618 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/src/ansible_compat/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-07-20 10:38:52.000000 ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/assets/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/requirements-invalid-collection.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/requirements-invalid-role.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_data.json
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_expected.json
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/assets/validate0_schema.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.broken/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.broken/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/galaxy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/molecule/default/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/molecule/deep_scenario/molecule.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/tasks/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/roles/baz/tasks/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.585446 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/collections/acme.goodies/tests/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.missing_deps/requirements.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/acme.sample2/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/ansible-role-sample/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/sample3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/sample3/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/sample3/meta/main.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.577446 ansible-compat-4.1.4.dev0/test/roles/sample4/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/test/roles/sample4/meta/
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/roles/sample4/meta/main.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2897 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_configuration_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_loaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_prerun.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27640 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_runtime_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/test/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 10:38:52.589446 ansible-compat-4.1.4.dev0/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      248 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tools/get-version.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      240 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tools/update-version.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4431 2023-07-20 10:38:33.000000 ansible-compat-4.1.4.dev0/tox.ini
```

### Comparing `ansible-compat-4.1.2/.github/dependabot.yml` & `ansible-compat-4.1.4.dev0/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/.github/workflows/release.yml` & `ansible-compat-4.1.4.dev0/.github/workflows/release.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/.github/workflows/tox.yml` & `ansible-compat-4.1.4.dev0/.github/workflows/tox.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/.gitignore` & `ansible-compat-4.1.4.dev0/.gitignore`

 * *Files 4% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 # C extensions
 *.so
 
 # Distribution / packaging
 .Python
 build/
 develop-eggs/
-dist/
 downloads/
 eggs/
 .eggs/
 lib/
 lib64/
 parts/
 sdist/
@@ -28,14 +27,16 @@
 MANIFEST
 
 # PyInstaller
 #  Usually these files are written by a python script from a template
 #  before PyInstaller builds the exe, so as to inject date/other infos into it.
 *.manifest
 *.spec
+rpm/*.spec
+*.rpm
 
 # Installer logs
 pip-log.txt
 pip-delete-this-directory.txt
 
 # Unit test / coverage reports
 htmlcov/
```

### Comparing `ansible-compat-4.1.2/.pre-commit-config.yaml` & `ansible-compat-4.1.4.dev0/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -6,30 +6,32 @@
   autofix_commit_msg: |
     chore: auto fixes from pre-commit.com hooks
 
     for more information, see https://pre-commit.ci
   skip:
     # https://github.com/pre-commit-ci/issues/issues/55
     - pip-compile
+    # No docker on pre-commit.ci
+    - validate-config-in-container
 default_language_version:
   # Needed in order to make pip-compile output predictable.
   python: python3.9
 exclude: |
   (?x)^(
     test/assets/.*
   )$
 repos:
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: "v0.0.267"
+    rev: "v0.0.277"
     hooks:
       - id: ruff
         args: [--fix, --exit-non-zero-on-fix]
   - repo: https://github.com/pre-commit/mirrors-prettier
     # keep it before yamllint
-    rev: "v3.0.0-alpha.9-for-vscode"
+    rev: "v3.0.0"
     hooks:
       - id: prettier
         additional_dependencies:
           - prettier
           - prettier-plugin-toml
           - prettier-plugin-sort-json
   - repo: https://github.com/pre-commit/pre-commit-hooks.git
@@ -45,31 +47,31 @@
       - id: mixed-line-ending
       - id: check-byte-order-marker
       - id: check-executables-have-shebangs
       - id: check-merge-conflict
       - id: debug-statements
         language_version: python3
   - repo: https://github.com/codespell-project/codespell
-    rev: v2.2.4
+    rev: v2.2.5
     hooks:
       - id: codespell
   - repo: https://github.com/adrienverge/yamllint.git
-    rev: v1.31.0
+    rev: v1.32.0
     hooks:
       - id: yamllint
         files: \.(yaml|yml)$
         types: [file, yaml]
         entry: yamllint --strict
   - repo: https://github.com/psf/black
     rev: 23.3.0
     hooks:
       - id: black
         language_version: python3
   - repo: https://github.com/pre-commit/mirrors-mypy
-    rev: v1.3.0
+    rev: v1.4.1
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
         args: ["--strict"]
         additional_dependencies:
           - ansible-core
           - cached_property
@@ -107,7 +109,12 @@
         name: Check constraints files and requirements
         files: ^(pyproject\.toml|requirements\.txt)$
         language: python
         entry: python -m piptools compile --resolver=backtracking -q --strip-extras --extra docs --extra test --output-file=requirements.txt pyproject.toml --unsafe-package ansible-core --unsafe-package resolvelib --unsafe-package typing_extensions
         pass_filenames: false
         additional_dependencies:
           - pip-tools>=6.11.0
+  - repo: https://github.com/packit/pre-commit-hooks
+    rev: v1.2.0
+    hooks:
+      - id: validate-config-in-container
+        alias: packit
```

### Comparing `ansible-compat-4.1.2/.readthedocs.yml` & `ansible-compat-4.1.4.dev0/.readthedocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/.vscode/settings.json` & `ansible-compat-4.1.4.dev0/.vscode/settings.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/LICENSE` & `ansible-compat-4.1.4.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/PKG-INFO` & `ansible-compat-4.1.4.dev0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.2
+Version: 4.1.4.dev0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.2/README.md` & `ansible-compat-4.1.4.dev0/README.md`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/docs/images/favicon.ico` & `ansible-compat-4.1.4.dev0/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/docs/images/logo.png` & `ansible-compat-4.1.4.dev0/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/docs/images/logo.svg` & `ansible-compat-4.1.4.dev0/docs/images/logo.svg`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/examples/reqs_v2/community-molecule-0.1.0.tar.gz` & `ansible-compat-4.1.4.dev0/examples/reqs_v2/community-molecule-0.1.0.tar.gz`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/mkdocs.yml` & `ansible-compat-4.1.4.dev0/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/pyproject.toml` & `ansible-compat-4.1.4.dev0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,16 @@
   "D213", # incompatible with D212
   "E501", # we use black
   "RET504", # Unnecessary variable assignment before `return` statement
   # Temporary disabled during adoption:
   "S607", # Starting a process with a partial executable path
   "PLR0912", # Bug https://github.com/charliermarsh/ruff/issues/4244
   "PLR0913", # Bug https://github.com/charliermarsh/ruff/issues/4244
-
+  "RUF012",
+  "PERF203",
 ]
 target-version = "py39"
 
 [tool.ruff.pydocstyle]
 convention = "pep257"
 
 [tool.ruff.flake8-pytest-style]
```

### Comparing `ansible-compat-4.1.2/requirements.txt` & `ansible-compat-4.1.4.dev0/requirements.txt`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/config.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/constants.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/constants.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/errors.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/errors.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/loaders.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/loaders.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/prerun.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/prerun.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/runtime.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/runtime.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,25 @@
 """Ansible runtime environment manager."""
+from __future__ import annotations
+
 import contextlib
+import fnmatch
 import importlib
 import json
 import logging
 import os
 import re
 import shutil
 import subprocess
 import tempfile
 import warnings
 from collections import OrderedDict
 from dataclasses import dataclass, field
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Optional, Union, no_type_check
+from typing import TYPE_CHECKING, Any, Callable, no_type_check
 
 import subprocess_tee
 from packaging.version import Version
 
 from ansible_compat.config import (
     AnsibleConfig,
     ansible_collections_path,
@@ -74,15 +77,15 @@
         super().__init__(version)
 
 
 @dataclass
 class Plugins:  # pylint: disable=too-many-instance-attributes
     """Dataclass to access installed Ansible plugins, uses ansible-doc to retrieve them."""
 
-    runtime: "Runtime"
+    runtime: Runtime
     become: dict[str, str] = field(init=False)
     cache: dict[str, str] = field(init=False)
     callback: dict[str, str] = field(init=False)
     cliconf: dict[str, str] = field(init=False)
     connection: dict[str, str] = field(init=False)
     httpapi: dict[str, str] = field(init=False)
     inventory: dict[str, str] = field(init=False)
@@ -139,31 +142,31 @@
         return result
 
 
 # pylint: disable=too-many-instance-attributes
 class Runtime:
     """Ansible Runtime manager."""
 
-    _version: Optional[Version] = None
+    _version: Version | None = None
     collections: OrderedDict[str, Collection] = OrderedDict()
-    cache_dir: Optional[Path] = None
+    cache_dir: Path | None = None
     # Used to track if we have already initialized the Ansible runtime as attempts
     # to do it multiple tilmes will cause runtime warnings from within ansible-core
     initialized: bool = False
     plugins: Plugins
 
     def __init__(
         self,
-        project_dir: Optional[Path] = None,
+        project_dir: Path | None = None,
         *,
         isolated: bool = False,
-        min_required_version: Optional[str] = None,
+        min_required_version: str | None = None,
         require_module: bool = False,
         max_retries: int = 0,
-        environ: Optional[dict[str, str]] = None,
+        environ: dict[str, str] | None = None,
     ) -> None:
         """Initialize Ansible runtime environment.
 
         :param project_dir: The directory containing the Ansible project. If
                             not mentioned it will be guessed from the current
                             working directory.
         :param isolated: Assure that installation of collections or roles
@@ -307,20 +310,20 @@
     def clean(self) -> None:
         """Remove content of cache_dir."""
         if self.cache_dir:
             shutil.rmtree(self.cache_dir, ignore_errors=True)
 
     def run(  # ruff: disable=PLR0913
         self,
-        args: Union[str, list[str]],
+        args: str | list[str],
         *,
         retry: bool = False,
         tee: bool = False,
-        env: Optional[dict[str, str]] = None,
-        cwd: Optional[Path] = None,
+        env: dict[str, str] | None = None,
+        cwd: Path | None = None,
     ) -> CompletedProcess:
         """Execute a command inside an Ansible environment.
 
         :param retry: Retry network operations on failures.
         :param tee: Also pass captured stdout/stderr to system while running.
         """
         if tee:
@@ -373,32 +376,32 @@
             return self._version
 
         msg = "Unable to find a working copy of ansible executable."
         raise MissingAnsibleError(msg, proc=proc)
 
     def version_in_range(
         self,
-        lower: Optional[str] = None,
-        upper: Optional[str] = None,
+        lower: str | None = None,
+        upper: str | None = None,
     ) -> bool:
         """Check if Ansible version is inside a required range.
 
         The lower limit is inclusive and the upper one exclusive.
         """
         if lower and self.version < Version(lower):
             return False
         if upper and self.version >= Version(upper):
             return False
         return True
 
     def install_collection(
         self,
-        collection: Union[str, Path],
+        collection: str | Path,
         *,
-        destination: Optional[Path] = None,
+        destination: Path | None = None,
         force: bool = False,
     ) -> None:
         """Install an Ansible collection.
 
         Can accept version constraints like 'foo.bar:>=1.2.3'
         """
         cmd = [
@@ -435,15 +438,15 @@
             msg = f"Command returned {run.returncode} code:\n{run.stdout}\n{run.stderr}"
             _logger.error(msg)
             raise InvalidPrerequisiteError(msg)
 
     def install_collection_from_disk(
         self,
         path: Path,
-        destination: Optional[Path] = None,
+        destination: Path | None = None,
     ) -> None:
         """Build and install collection from a given disk path."""
         if not self.version_in_range(upper="2.11"):
             self.install_collection(path, destination=destination, force=True)
             return
         # older versions of ansible able unable to install without building
         with tempfile.TemporaryDirectory() as tmp_dir:
@@ -546,104 +549,124 @@
                     env={**os.environ, "ANSIBLE_COLLECTIONS_PATH": ":".join(cpaths)},
                 )
                 if result.returncode != 0:
                     _logger.error(result.stdout)
                     _logger.error(result.stderr)
                     raise AnsibleCommandError(result)
 
+    def search_galaxy_paths(self, search_dir: Path, depth: int = 0) -> list[str]:
+        """Search for galaxy paths (only one level deep)."""
+        galaxy_paths: list[str] = []
+        for file in os.listdir(search_dir):
+            file_path = Path(file)
+            if file_path.is_dir() and depth < 1:
+                galaxy_paths.extend(self.search_galaxy_paths(file_path, 1))
+            elif fnmatch.fnmatch(file, "galaxy.yml"):
+                galaxy_paths.append(str(search_dir / file))
+        if depth == 0 and not galaxy_paths:
+            return ["galaxy.yml"]
+        return galaxy_paths
+
     def prepare_environment(  # noqa: C901
         self,
-        required_collections: Optional[dict[str, str]] = None,
+        required_collections: dict[str, str] | None = None,
         *,
         retry: bool = False,
         install_local: bool = False,
         offline: bool = False,
         role_name_check: int = 0,
     ) -> None:
         """Make dependencies available if needed."""
-        destination: Optional[Path] = None
+        destination: Path | None = None
         if required_collections is None:
             required_collections = {}
 
         # first one is standard for collection layout repos and the last two
         # are part of Tower specification
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#ansible-galaxy-support
         # https://docs.ansible.com/ansible-tower/latest/html/userguide/projects.html#collections-support
         for req_file in REQUIREMENT_LOCATIONS:
             self.install_requirements(Path(req_file), retry=retry, offline=offline)
 
-        galaxy_path = Path("galaxy.yml")
-        if galaxy_path.exists():
-            data = yaml_from_file(galaxy_path)
-            if isinstance(data, dict) and "dependencies" in data:
-                for name, required_version in data["dependencies"].items():
-                    _logger.info(
-                        "Provisioning collection %s:%s from galaxy.yml",
-                        name,
-                        required_version,
-                    )
-                    self.install_collection(
-                        f"{name}:{required_version}",
-                        destination=destination,
-                    )
+        for gpath in self.search_galaxy_paths(self.project_dir):
+            galaxy_path = Path(gpath)
+            if galaxy_path.exists():
+                data = yaml_from_file(galaxy_path)
+                if isinstance(data, dict) and "dependencies" in data:
+                    for name, required_version in data["dependencies"].items():
+                        _logger.info(
+                            "Provisioning collection %s:%s from galaxy.yml",
+                            name,
+                            required_version,
+                        )
+                        self.install_collection(
+                            f"{name}:{required_version}",
+                            destination=destination,
+                        )
 
-        if self.cache_dir:
-            destination = self.cache_dir / "collections"
-        for name, min_version in required_collections.items():
-            self.install_collection(
-                f"{name}:>={min_version}",
-                destination=destination,
-            )
+            if self.cache_dir:
+                destination = self.cache_dir / "collections"
+            for name, min_version in required_collections.items():
+                self.install_collection(
+                    f"{name}:>={min_version}",
+                    destination=destination,
+                )
 
-        self._prepare_ansible_paths()
+            self._prepare_ansible_paths()
 
-        if not install_local:
-            return
+            if not install_local:
+                return
 
-        if Path("galaxy.yml").exists():
-            if destination:
-                # while function can return None, that would not break the logic
-                colpath = Path(
-                    f"{destination}/ansible_collections/{colpath_from_path(Path.cwd())}",
-                )
-                if colpath.is_symlink():
-                    if os.path.realpath(colpath) == Path.cwd():
+            if galaxy_path.exists():
+                if destination:
+                    # while function can return None, that would not break the logic
+                    colpath = Path(
+                        f"{destination}/ansible_collections/{colpath_from_path(Path.cwd())}",
+                    )
+                    if colpath.is_symlink():
+                        if os.path.realpath(colpath) == Path.cwd():
+                            _logger.warning(
+                                "Found symlinked collection, skipping its installation.",
+                            )
+                            return
                         _logger.warning(
-                            "Found symlinked collection, skipping its installation.",
+                            "Collection is symlinked, but not pointing to %s directory, so we will remove it.",
+                            Path.cwd(),
                         )
-                        return
-                    _logger.warning(
-                        "Collection is symlinked, but not pointing to %s directory, so we will remove it.",
-                        Path.cwd(),
-                    )
-                    colpath.unlink()
+                        colpath.unlink()
 
-            # molecule scenario within a collection
-            self.install_collection_from_disk(Path("."), destination=destination)
-        elif (
-            Path().resolve().parent.name == "roles"
-            and Path("../../galaxy.yml").exists()
-        ):
-            # molecule scenario located within roles/<role-name>/molecule inside
-            # a collection
-            self.install_collection_from_disk(Path("../.."), destination=destination)
-        else:
-            # no collection, try to recognize and install a standalone role
-            self._install_galaxy_role(
-                self.project_dir,
-                role_name_check=role_name_check,
-                ignore_errors=True,
-            )
+                # molecule scenario within a collection
+                self.install_collection_from_disk(
+                    galaxy_path.parent,
+                    destination=destination,
+                )
+            elif (
+                Path().resolve().parent.name == "roles"
+                and Path("../../galaxy.yml").exists()
+            ):
+                # molecule scenario located within roles/<role-name>/molecule inside
+                # a collection
+                self.install_collection_from_disk(
+                    Path("../.."),
+                    destination=destination,
+                )
+            else:
+                # no collection, try to recognize and install a standalone role
+                self._install_galaxy_role(
+                    self.project_dir,
+                    role_name_check=role_name_check,
+                    ignore_errors=True,
+                )
         # reload collections
         self.load_collections()
 
     def require_collection(
         self,
         name: str,
-        version: Optional[str] = None,
+        version: str | None = None,
         *,
         install: bool = True,
     ) -> None:
         """Check if a minimal collection version is present or exits.
 
         In the future this method may attempt to install a missing or outdated
         collection before failing.
```

### Comparing `ansible-compat-4.1.2/src/ansible_compat/schema.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat/types.py` & `ansible-compat-4.1.4.dev0/src/ansible_compat/types.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/src/ansible_compat.egg-info/PKG-INFO` & `ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansible-compat
-Version: 4.1.2
+Version: 4.1.4.dev0
 Summary: Ansible compatibility goodies
 Author-email: Sorin Sbarnea <ssbarnea@redhat.com>
 Maintainer-email: Sorin Sbarnea <ssbarnea@redhat.com>
 License: MIT
 Project-URL: homepage, https://github.com/ansible/ansible-compat
 Project-URL: documentation, https://ansible-compat.readthedocs.io/
 Project-URL: repository, https://github.com/ansible/ansible-compat
```

### Comparing `ansible-compat-4.1.2/src/ansible_compat.egg-info/SOURCES.txt` & `ansible-compat-4.1.4.dev0/src/ansible_compat.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.packit.yaml
 .pre-commit-config.yaml
 .prettierignore
 .prettierrc.yaml
 .readthedocs.yml
 .yamllint
 LICENSE
 README.md
@@ -72,8 +73,10 @@
 test/collections/acme.goodies/roles/baz/tasks/main.yml
 test/collections/acme.goodies/tests/requirements.yml
 test/roles/acme.missing_deps/requirements.yml
 test/roles/acme.missing_deps/meta/main.yml
 test/roles/acme.sample2/meta/main.yml
 test/roles/ansible-role-sample/meta/main.yml
 test/roles/sample3/meta/main.yml
-test/roles/sample4/meta/main.yml
+test/roles/sample4/meta/main.yml
+tools/get-version.sh
+tools/update-version.sh
```

### Comparing `ansible-compat-4.1.2/test/assets/validate0_expected.json` & `ansible-compat-4.1.4.dev0/test/assets/validate0_expected.json`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/test/collections/acme.goodies/galaxy.yml` & `ansible-compat-4.1.4.dev0/test/collections/acme.goodies/galaxy.yml`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/test/conftest.py` & `ansible-compat-4.1.4.dev0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/test/test_config.py` & `ansible-compat-4.1.4.dev0/test/test_config.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/test/test_runtime.py` & `ansible-compat-4.1.4.dev0/test/test_runtime.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
 )
 def test_install_collection_from_disk(
     path: str,
     scenario: str,
     expected_collections: list[str],
 ) -> None:
     """Tests ability to install a local collection."""
-    # ensure we do not have acme.google installed in user directory as it may
+    # ensure we do not have acme.goodies installed in user directory as it may
     # produce false positives
     rmtree(
         pathlib.Path(
             "~/.ansible/collections/ansible_collections/acme/goodies",
         ).expanduser(),
         ignore_errors=True,
     )
```

### Comparing `ansible-compat-4.1.2/test/test_runtime_example.py` & `ansible-compat-4.1.4.dev0/test/test_runtime_example.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/test/test_schema.py` & `ansible-compat-4.1.4.dev0/test/test_schema.py`

 * *Files identical despite different names*

### Comparing `ansible-compat-4.1.2/tox.ini` & `ansible-compat-4.1.4.dev0/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -134,13 +134,20 @@
 
 [testenv:py]
 description = Run the tests with {basepython} ansible-core 2.12+
 deps =
   {[testenv]deps}
   ansible-core>=2.12
 
+[testenv:rpm]
+description = Use packit to build RPM (requires RPM based Linux distro)
+deps =
+  packitos
+commands =
+  packit build in-mock
+
 [testenv:docs]
 description = Build docs
 commands =
   mkdocs {posargs:build} --strict
 extras = docs
 passenv = *
```

