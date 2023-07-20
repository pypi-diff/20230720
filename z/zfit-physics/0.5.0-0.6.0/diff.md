# Comparing `tmp/zfit_physics-0.5.0.tar.gz` & `tmp/zfit_physics-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zfit_physics-0.5.0.tar", last modified: Fri Jan 27 15:47:47 2023, max compression
+gzip compressed data, was "zfit_physics-0.6.0.tar", last modified: Thu Jul 20 20:59:26 2023, max compression
```

## Comparing `zfit_physics-0.5.0.tar` & `zfit_physics-0.6.0.tar`

### file list

```diff
@@ -1,79 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.all-contributorsrc
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.codeclimate.yml
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.635923 zfit_physics-0.5.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.639923 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/other.md
--rw-r--r--   0 runner    (1001) docker     (123)      313 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/physics-specific-question.md
--rw-r--r--   0 runner    (1001) docker     (123)      531 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.639923 zfit_physics-0.5.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      933 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/workflows/cd.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.landscape.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/.scrutinizer.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.639923 zfit_physics-0.5.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.631923 zfit_physics-0.5.0/docs/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.639923 zfit_physics-0.5.0/docs/api/tools/
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/api/tools/change_headline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.639923 zfit_physics-0.5.0/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   127528 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/images/scikit-hep-logo_168x168.png
--rw-r--r--   0 runner    (1001) docker     (123)   274482 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/images/zfit-fin_400x168.png
--rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/images/zfit-fin_57x24.png
--rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/images/zfit_workflow_v1.png
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/index.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/docs/make_docs.sh
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-27 15:47:47.647923 zfit_physics-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      899 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/test_pdf_argus.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/test_pdf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/test_pdf_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/test_pdf_kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/tests/test_pdf_relbw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.631923 zfit_physics-0.5.0/utils/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/utils/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/utils/ci/test_examples.sh
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/utils/ci/testbuild_docs.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/zfit_physics/
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/zfit_physics/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/pdf_argus.py
--rw-r--r--   0 runner    (1001) docker     (123)     5025 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/pdf_conv.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/pdf_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/pdf_kde.py
--rw-r--r--   0 runner    (1001) docker     (123)     4116 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/models/pdf_relbw.py
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/pdf.py
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/plot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/zfit_physics/unstable/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/unstable/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-01-27 15:47:37.000000 zfit_physics-0.5.0/zfit_physics/unstable/pdf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-27 15:47:47.643923 zfit_physics-0.5.0/zfit_physics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-01-27 15:47:47.000000 zfit_physics-0.5.0/zfit_physics.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.065346 zfit_physics-0.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.all-contributorsrc
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.codeclimate.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.053346 zfit_physics-0.6.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.053346 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      737 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/other.md
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/physics-specific-question.md
+-rw-r--r--   0 runner    (1001) docker     (123)      531 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.053346 zfit_physics-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      933 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/workflows/cd.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/.scrutinizer.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 20:59:26.065346 zfit_physics-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1473 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.053346 zfit_physics-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.045346 zfit_physics-0.6.0/docs/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.057346 zfit_physics-0.6.0/docs/api/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/api/tools/change_headline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9505 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.057346 zfit_physics-0.6.0/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   127528 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/images/scikit-hep-logo_168x168.png
+-rw-r--r--   0 runner    (1001) docker     (123)   274482 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/images/zfit-fin_400x168.png
+-rw-r--r--   0 runner    (1001) docker     (123)    10989 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/images/zfit-fin_57x24.png
+-rw-r--r--   0 runner    (1001) docker     (123)    42170 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/images/zfit_workflow_v1.png
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/index.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)      632 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/docs/make_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-07-20 20:59:26.065346 zfit_physics-0.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.057346 zfit_physics-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/test_pdf_argus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/test_pdf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/test_pdf_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/test_pdf_kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2037 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/tests/test_pdf_relbw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.045346 zfit_physics-0.6.0/utils/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.061346 zfit_physics-0.6.0/utils/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/utils/ci/test_examples.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/utils/ci/testbuild_docs.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.061346 zfit_physics-0.6.0/zfit_physics/
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.065346 zfit_physics-0.6.0/zfit_physics/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/pdf_argus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5210 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/pdf_conv.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/pdf_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3188 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/pdf_kde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/models/pdf_relbw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/pdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/plot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.065346 zfit_physics-0.6.0/zfit_physics/unstable/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/unstable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-07-20 20:59:16.000000 zfit_physics-0.6.0/zfit_physics/unstable/pdf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 20:59:26.061346 zfit_physics-0.6.0/zfit_physics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-07-20 20:59:26.000000 zfit_physics-0.6.0/zfit_physics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-07-20 20:59:26.000000 zfit_physics-0.6.0/zfit_physics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:59:26.000000 zfit_physics-0.6.0/zfit_physics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 20:59:25.000000 zfit_physics-0.6.0/zfit_physics.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 20:59:26.000000 zfit_physics-0.6.0/zfit_physics.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 20:59:26.000000 zfit_physics-0.6.0/zfit_physics.egg-info/top_level.txt
```

### Comparing `zfit_physics-0.5.0/.all-contributorsrc` & `zfit_physics-0.6.0/.all-contributorsrc`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md` & `zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/behaviorunderdiscussion.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/bug_report.md` & `zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/feature-request.md` & `zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md` & `zfit_physics-0.6.0/.github/ISSUE_TEMPLATE/zfit-usage-question.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/ISSUE_TEMPLATE.md` & `zfit_physics-0.6.0/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.github/workflows/cd.yml` & `zfit_physics-0.6.0/.github/workflows/cd.yml`

 * *Files 14% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 jobs:
   dist:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
         with:
           fetch-depth: 0
-      - uses: actions/setup-python@v4.4.0
+      - uses: actions/setup-python@v4.6.1
 
       - name: Build SDist and wheel
         run: pipx run --spec build pyproject-build
 
       - name: Check metadata
         run: pipx run twine check dist/*
 
@@ -37,10 +37,10 @@
 
     steps:
       - uses: actions/download-artifact@v3
         with:
           name: artifact
           path: dist
 
-      - uses: pypa/gh-action-pypi-publish@v1.6.4
+      - uses: pypa/gh-action-pypi-publish@v1.8.7
         with:
           password: ${{ secrets.PYPI_ZFIT_PHYSICS_TOKEN }}
```

### Comparing `zfit_physics-0.5.0/.github/workflows/ci.yml` & `zfit_physics-0.6.0/.github/workflows/ci.yml`

 * *Files 12% similar despite different names*

```diff
@@ -15,51 +15,51 @@
   tests_graph:
     runs-on: ubuntu-latest
     timeout-minutes: 150
     strategy:
       max-parallel: 4
       fail-fast: False
       matrix:
-        python-version: [ "3.7", "3.8", "3.10" ]
+        python-version: [ "3.8", "3.9", "3.10", "3.11" ]
     name: JIT compiled tests for Python ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4.4.0
+      - uses: actions/setup-python@v4.6.1
         name: Set up Python ${{ matrix.python-version }}
 
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
+          pip install .[dev]
       - name: Test with pytest
         run: |
-          pip install .[dev]
           coverage run --source=. --omit=".tox/*" --branch -m pytest .
           coverage report
 
 
   tests_eager:
     runs-on: ubuntu-latest
     timeout-minutes: 150
     strategy:
       max-parallel: 4
       fail-fast: False
       matrix:
-        python-version: [ "3.7", "3.8", "3.10" ]
+        python-version: [ "3.8", "3.9", "3.10", "3.11" ]
     name: Eager mode tests for Python ${{ matrix.python-version }}
     steps:
       - uses: actions/checkout@v3
-      - uses: actions/setup-python@v4.4.0
+      - uses: actions/setup-python@v4.6.1
         name: Set up Python ${{ matrix.python-version }}
 
         with:
           python-version: ${{ matrix.python-version }}
       - name: Install dependencies
         run: |
           python -m pip install --upgrade pip
+          pip install .[dev]
       - name: Test with pytest
         run: |
-          pip install .[dev]
           ZFIT_DO_JIT=0
           coverage run --source=. --omit=".tox/*,*/test*," --branch -m pytest .
           coverage report
```

### Comparing `zfit_physics-0.5.0/.gitignore` & `zfit_physics-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/.pre-commit-config.yaml` & `zfit_physics-0.6.0/.pre-commit-config.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -17,67 +17,64 @@
       - id: requirements-txt-fixer
       - id: trailing-whitespace
       - id: detect-private-key
       - id: fix-byte-order-marker
       - id: check-ast
 
   - repo: https://github.com/PyCQA/docformatter
-    rev: v1.5.1
+    rev: v1.7.5
     hooks:
       - id: docformatter
         args: [ -r, --in-place, --wrap-descriptions, '120', --wrap-summaries, '120', -- ]
 
-
-  - repo: https://github.com/mattlqx/pre-commit-sign
-    rev: v1.1.3
-    hooks:
-      - id: sign-commit
   - repo: https://github.com/pre-commit/pygrep-hooks
-    rev: v1.9.0
+    rev: v1.10.0
     hooks:
       - id: python-use-type-annotations
       - id: python-check-mock-methods
       - id: python-no-eval
       - id: rst-directive-colons
 
   - repo: https://github.com/PyCQA/isort
-    rev: 5.11.4
+    rev: 5.12.0
     hooks:
       - id: isort
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.3.1
+    rev: v3.9.0
     hooks:
       - id: pyupgrade
-        args: [ --py37-plus ]
+        args: [ --py38-plus ]
 
   - repo: https://github.com/asottile/setup-cfg-fmt
-    rev: v2.2.0
+    rev: v2.4.0
     hooks:
       - id: setup-cfg-fmt
+        args: [ --max-py-version=3.10, --include-version-classifiers ]
+
 
   # Notebook formatting
   - repo: https://github.com/nbQA-dev/nbQA
-    rev: 1.6.0
+    rev: 1.7.0
     hooks:
       - id: nbqa-isort
-        additional_dependencies: [ isort==5.6.4 ]
+        additional_dependencies: [ isort ]
 
       - id: nbqa-pyupgrade
-        additional_dependencies: [ pyupgrade==2.7.4 ]
-        args: [ --py37-plus ]
+        additional_dependencies: [ pyupgrade ]
+        args: [ --py38-plus ]
 
   - repo: https://github.com/mgedmin/check-manifest
     rev: '0.49'
     hooks:
       - id: check-manifest
         stages: [ manual ]
   - repo: https://github.com/sondrelg/pep585-upgrade
     rev: 'v1.0'
     hooks:
     - id: upgrade-type-hints
       args: [ '--futures=true' ]
 
   - repo: https://github.com/psf/black
-    rev: 22.12.0
+    rev: 23.7.0
     hooks:
       - id: black
```

### Comparing `zfit_physics-0.5.0/.scrutinizer.yml` & `zfit_physics-0.6.0/.scrutinizer.yml`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/CHANGELOG.rst` & `zfit_physics-0.6.0/CHANGELOG.rst`

 * *Files 15% similar despite different names*

```diff
@@ -22,15 +22,18 @@
 ------------
 
 Requirement changes
 -------------------
 
 Thanks
 ------
+0.6.0 (20 Jul 2023)
+===================
 
+Upgrade to zfit >= 0.12, support Python 3.8-3.11
 
 0.4.0 (27 Jan 2023)
 ===================
 
 Compability with zfit >= 0.11, < 0.13
 
 0.3.0 (26 Jan 2023)
```

### Comparing `zfit_physics-0.5.0/LICENSE` & `zfit_physics-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/PKG-INFO` & `zfit_physics-0.6.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfit_physics
-Version: 0.5.0
+Version: 0.6.0
 Summary: Physics extension to zfit
 Home-page: https://github.com/zfit/zfit-physics
 Author: zfit
 Author-email: zfit@physik.uzh.ch
 Maintainer: zfit
 Maintainer-email: zfit@physik.uzh.ch
 License: BSD-3-Clause
@@ -13,17 +13,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 ************
 zfit physics
 ************
```

### Comparing `zfit_physics-0.5.0/README.rst` & `zfit_physics-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/Makefile` & `zfit_physics-0.6.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/api/tools/change_headline.py` & `zfit_physics-0.6.0/docs/api/tools/change_headline.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/conf.py` & `zfit_physics-0.6.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/images/scikit-hep-logo_168x168.png` & `zfit_physics-0.6.0/docs/images/scikit-hep-logo_168x168.png`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/images/zfit-fin_400x168.png` & `zfit_physics-0.6.0/docs/images/zfit-fin_400x168.png`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/images/zfit-fin_57x24.png` & `zfit_physics-0.6.0/docs/images/zfit-fin_57x24.png`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/images/zfit_workflow_v1.png` & `zfit_physics-0.6.0/docs/images/zfit_workflow_v1.png`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/docs/make_docs.sh` & `zfit_physics-0.6.0/docs/make_docs.sh`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/setup.cfg` & `zfit_physics-0.6.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -5,44 +5,47 @@
 long_description_content_type = text/x-rst
 url = https://github.com/zfit/zfit-physics
 author = zfit
 author_email = zfit@physik.uzh.ch
 maintainer = zfit
 maintainer_email = zfit@physik.uzh.ch
 license = BSD-3-Clause
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 3 - Alpha
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: BSD License
 	Natural Language :: English
 	Operating System :: MacOS
 	Operating System :: Unix
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
+	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: Implementation :: CPython
 	Topic :: Scientific/Engineering :: Physics
 keywords = TensorFlow, model, fitting, scalable, HEP, physics
 
 [options]
-python_requires = >=3.7
+python_requires = >=3.8
 
 [bdist_wheel]
 universal = 1
 
 [flake8]
 exclude = 
 	docs,
 	examples,
 	dist,
 	building,
 	build,
 	legacy,
 	utils
-max-line-length = 110
+max-line-length = 120
 statistics = True
 max-complexity = 30
 
 [aliases]
 test = pytest
 
 [tool:pytest]
@@ -50,13 +53,13 @@
 
 [isort]
 multi_line_output = 3
 include_trailing_comma = True
 force_grid_wrap = 0
 use_parentheses = True
 ensure_newline_before_comments = True
-line_length = 88
+line_length = 120
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `zfit_physics-0.5.0/setup.py` & `zfit_physics-0.6.0/setup.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/conftest.py` & `zfit_physics-0.6.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/test_pdf_argus.py` & `zfit_physics-0.6.0/tests/test_pdf_argus.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/test_pdf_conv.py` & `zfit_physics-0.6.0/tests/test_pdf_conv.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/test_pdf_example.py` & `zfit_physics-0.6.0/tests/test_pdf_example.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/test_pdf_kde.py` & `zfit_physics-0.6.0/tests/test_pdf_kde.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/tests/test_pdf_relbw.py` & `zfit_physics-0.6.0/tests/test_pdf_relbw.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/zfit_physics/__init__.py` & `zfit_physics-0.6.0/zfit_physics/__init__.py`

 * *Files identical despite different names*

### Comparing `zfit_physics-0.5.0/zfit_physics/models/pdf_argus.py` & `zfit_physics-0.6.0/zfit_physics/models/pdf_argus.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 """ARGUS PDF (https://en.wikipedia.org/wiki/ARGUS_distribution)"""
+from typing import Optional
+
 import numpy as np
 import tensorflow as tf
 import tensorflow_probability as tfp
 import zfit
 from zfit import z
 from zfit.util import ztyping
 
@@ -40,15 +42,23 @@
 
     m_factor = 1 - z.square(m_frac)
     argus = m * z.pow(m_factor, p) * (z.exp(c * m_factor))
     return argus
 
 
 class Argus(zfit.pdf.BasePDF):
-    def __init__(self, obs: ztyping.ObsTypeInput, m0, c, p, name: str = "ArgusPDF"):
+    def __init__(
+        self,
+        obs: ztyping.ObsTypeInput,
+        m0,
+        c,
+        p,
+        name: str = "ArgusPDF",
+        extended: Optional[ztyping.ParamTypeInput] = None,
+    ):
         r"""`ARGUS shape <https://en.wikipedia.org/wiki/ARGUS_distribution>`_ describing the invariant mass of a particle
         in a continuous background.
 
         The ARGUS shaped function describes the reconstructed invariant mass of a decayed particle, especially at the
         kinematic boundaries of the maximum beam energy. It is defined as
 
         .. math::
@@ -57,23 +67,24 @@
             \cdot \exp\left[ c \cdot \left(1 - \left(\frac{m}{m_0}\right)^2 \right) \right]
 
         and normalized to one over the `norm_range` (which defaults to `obs`).
 
         The implementation follows the `RooFit version <https://root.cern.ch/doc/master/classRooArgusBG.html>`_
 
         Args:
+            obs: Observable the PDF is defined on
             m0: Maximal energetically allowed mass, cutoff
             c: Shape parameter; "peakiness" of the distribution
             p: Generalization of the ARGUS shape, for p = 0.5, the normal ARGUS shape is recovered
 
         Returns:
             `tf.Tensor`: the values matching the (broadcasted) shapes of the input
         """
         params = {"m0": m0, "c": c, "p": p}
-        super().__init__(obs=obs, name=name, params=params)
+        super().__init__(obs=obs, name=name, params=params, extended=extended)
 
     _N_OBS = 1
 
     def _unnormalized_pdf(self, x):
         """
         Calculation of ARGUS PDF value
         (Docs: https://docs.scipy.org/doc/scipy/reference/generated/scipy.stats.argus.html)
```

### Comparing `zfit_physics-0.5.0/zfit_physics/models/pdf_conv.py` & `zfit_physics-0.6.0/zfit_physics/models/pdf_conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import tensorflow as tf
 import tensorflow_probability as tfp
 import zfit
 import zfit.models.functor
 from zfit import z
 from zfit.exception import FunctionNotImplementedError
 from zfit.util import exception, ztyping
@@ -12,30 +14,33 @@
     def __init__(
         self,
         func: zfit.pdf.BasePDF,
         kernel: zfit.pdf.BasePDF,
         limits: ztyping.ObsTypeInput,
         obs: ztyping.ObsTypeInput,
         ndraws: int = 20000,
+        *,
+        extended: Optional[ztyping.ParamTypeInput] = None,
         name: str = "Convolution",
         experimental_pdf_normalized=False,
     ):
         """Numerical Convolution pdf of *func* convoluted with *kernel*.
 
         Args:
             func (:py:class:`zfit.pdf.BasePDF`): PDF  with `pdf` method that takes x and returns the function value.
                 Here x is a `Data` with the obs and limits of *limits*.
             kernel (:py:class:`zfit.pdf.BasePDF`): PDF with `pdf` method that takes x acting as the kernel.
                 Here x is a `Data` with the obs and limits of *limits*.
             limits (:py:class:`zfit.Space`): Limits for the numerical integration.
             obs (:py:class:`zfit.Space`): Observables of the class
+            extended: If the PDF should be extended, i.e. a yield.
             ndraws (int): Number of draws for the mc integration
             name (str): Human readable name of the pdf
         """
-        super().__init__(obs=obs, pdfs=[func, kernel], params={}, name=name)
+        super().__init__(obs=obs, pdfs=[func, kernel], params={}, name=name, extended=extended)
         limits = self._check_input_limits(limits=limits)
         if limits.n_limits == 0:
             raise exception.LimitsNotSpecifiedError("obs have to have limits to define where to integrate over.")
         if limits.n_limits > 1:
             raise WorkInProgressError("Multiple Limits not implemented")
 
         #        if not isinstance(func, zfit.pdf.BasePDF):
```

### Comparing `zfit_physics-0.5.0/zfit_physics/models/pdf_kde.py` & `zfit_physics-0.6.0/zfit_physics/models/pdf_kde.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 from collections import OrderedDict
+from typing import Optional
 
 import tensorflow as tf
 import tensorflow_probability.python.distributions as tfd
 import zfit
 from zfit import z
 from zfit.models.dist_tfp import WrapDistribution
 from zfit.util import ztyping
 from zfit.util.container import convert_to_container
-from zfit.util.exception import AnalyticIntegralNotImplemented, WorkInProgressError
+from zfit.util.exception import WorkInProgressError
 
 
 class GaussianKDE(WrapDistribution):  # multidimensional kde with gaussian kernel
     def __init__(
         self,
         data: tf.Tensor,
         bandwidth: ztyping.ParamTypeInput,
         obs: ztyping.ObsTypeInput,
         name: str = "GaussianKDE",
+        *,
+        extended: Optional[ztyping.ParamTypeInput] = None,
     ):
         """Gaussian Kernel Density Estimation using Silverman's rule of thumb.
 
         Args:
             data: Data points to build a kernel around
             bandwidth: sigmas for the covariance matrix of the multivariate gaussian
             obs:
             name: Name of the PDF
         """
         dtype = zfit.settings.ztypes.float
         if isinstance(data, zfit.core.interfaces.ZfitData):
-
             raise WorkInProgressError("Currently, no dataset supported yet")
             # size = data.nevents
             # dims = data.n_obs
             # with data.
             # data = data.value()
             # if data.weights is not None:
 
@@ -73,12 +75,13 @@
         super().__init__(
             distribution=distribution,
             dist_params={},
             dist_kwargs=dist_kwargs,
             params=params,
             obs=obs,
             name=name,
+            extended=extended,
         )
 
     # @zfit.supports()
     # def _analytic_integrate(self, limits, norm_range):
     #     raise AnalyticIntegralNotImplementedError
```

### Comparing `zfit_physics-0.5.0/zfit_physics/models/pdf_relbw.py` & `zfit_physics-0.6.0/zfit_physics/models/pdf_relbw.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+from typing import Optional
+
 import numpy as np
 import tensorflow as tf
 import zfit
 from zfit import z
 from zfit.core.space import ANY_LOWER, ANY_UPPER, Space
 from zfit.util import ztyping
 
@@ -25,26 +27,35 @@
     alpha = gamma / m
     gamma2 = m**2 * (1.0 + alpha**2) ** 0.5
     k = 2.0 ** (3.0 / 2.0) * m**2 * alpha * gamma2 / (np.pi * (m**2 + gamma2) ** 0.5)
 
     return k / ((x**2 - m**2) ** 2 + m**4 * alpha**2)
 
 
-class RelativisticBreitWigner(zfit.pdf.ZPDF):
-    """Relativistic Breit-Wigner distribution.
+class RelativisticBreitWigner(zfit.pdf.BasePDF):
+    _N_OBS = 1
 
-    Formula for PDF and CDF are based on https://gist.github.com/andrewfowlie/cd0ed7e6c96f7c9e88f85eb3b9665b97
+    def __init__(
+        self,
+        m: ztyping.ParamTypeInput,
+        gamma: ztyping.ParamTypeInput,
+        obs: ztyping.ObsTypeInput,
+        name: str = "RelativisticBreitWigner",
+        extended: Optional[ztyping.ParamTypeInput] = None,
+    ):
+        """Relativistic Breit-Wigner distribution.
 
-    Args:
-        m: the average value
-        gamma: the width of the distribution
-    """
+        Formula for PDF and CDF are based on https://gist.github.com/andrewfowlie/cd0ed7e6c96f7c9e88f85eb3b9665b97
 
-    _N_OBS = 1
-    _PARAMS = ["m", "gamma"]
+        Args:
+            m: the average value
+            gamma: the width of the distribution
+        """
+        params = dict(m=m, gamma=gamma)
+        super().__init__(obs=obs, params=params, name=name, extended=extended)
 
     def _unnormalized_pdf(self, x: tf.Tensor) -> tf.Tensor:
         """Calculate the PDF at value(s) x.
 
         Args:
             x : Either one value or an array
```

### Comparing `zfit_physics-0.5.0/zfit_physics.egg-info/PKG-INFO` & `zfit_physics-0.6.0/zfit_physics.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zfit-physics
-Version: 0.5.0
+Version: 0.6.0
 Summary: Physics extension to zfit
 Home-page: https://github.com/zfit/zfit-physics
 Author: zfit
 Author-email: zfit@physik.uzh.ch
 Maintainer: zfit
 Maintainer-email: zfit@physik.uzh.ch
 License: BSD-3-Clause
@@ -13,17 +13,20 @@
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
 
 ************
 zfit physics
 ************
```

### Comparing `zfit_physics-0.5.0/zfit_physics.egg-info/SOURCES.txt` & `zfit_physics-0.6.0/zfit_physics.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 .all-contributorsrc
 .codeclimate.yml
 .git_archival.txt
 .gitattributes
 .gitignore
-.landscape.yml
 .pre-commit-config.yaml
 .scrutinizer.yml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
```

