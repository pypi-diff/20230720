# Comparing `tmp/auto-labeling-pipeline-0.1.8.tar.gz` & `tmp/auto-labeling-pipeline-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-labeling-pipeline-0.1.8.tar", last modified: Tue Feb  2 07:21:28 2021, max compression
+gzip compressed data, was "auto-labeling-pipeline-0.1.9.tar", last modified: Mon Feb 15 06:43:31 2021, max compression
```

## Comparing `auto-labeling-pipeline-0.1.8.tar` & `auto-labeling-pipeline-0.1.9.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (117)       31 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.026059 auto-labeling-pipeline-0.1.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.030059 auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (117)      631 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/01-question.md
--rw-r--r--   0 runner    (1001) docker     (117)      539 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/02-bug.md
--rw-r--r--   0 runner    (1001) docker     (117)      602 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/03-install.md
--rw-r--r--   0 runner    (1001) docker     (117)      255 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/04-request.md
--rw-r--r--   0 runner    (1001) docker     (117)     1303 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.030059 auto-labeling-pipeline-0.1.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (117)      657 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (117)     2364 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (117)      633 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/workflows/package-installation.yml
--rw-r--r--   0 runner    (1001) docker     (117)      696 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (117)     2826 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (117)       27 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (117)     3372 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (117)     1670 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (117)     1072 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (117)     2129 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      509 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/Pipfile
--rw-r--r--   0 runner    (1001) docker     (117)    32830 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (117)     1219 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.030059 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)     1300 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/label.py
--rw-r--r--   0 runner    (1001) docker     (117)     1142 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/labels.py
--rw-r--r--   0 runner    (1001) docker     (117)     1455 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/mappings.py
--rw-r--r--   0 runner    (1001) docker     (117)     2092 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/menu.py
--rw-r--r--   0 runner    (1001) docker     (117)     2352 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/models.py
--rw-r--r--   0 runner    (1001) docker     (117)      590 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (117)      738 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (117)     1712 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/request.py
--rw-r--r--   0 runner    (1001) docker     (117)     1212 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/task.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/templates/
--rw-r--r--   0 runner    (1001) docker     (117)       49 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/templates/amazon_comprehend_sentiment.jinja2
--rw-r--r--   0 runner    (1001) docker     (117)      538 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/templates/gcp_entities.jinja2
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.030059 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     2129 2021-02-02 07:21:27.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     1517 2021-02-02 07:21:28.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-02 07:21:27.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       31 2021-02-02 07:21:27.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)       23 2021-02-02 07:21:27.000000 auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)       34 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (117)       38 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)     1478 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/tests/
--rw-r--r--   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)      219 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/tests/data/
--rw-r--r--   0 runner    (1001) docker     (117)      201 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/data/amazon_comprehend_sentiment.json
--rw-r--r--   0 runner    (1001) docker     (117)     3326 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/data/gcp_entities.json
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.026059 auto-labeling-pipeline-0.1.8/tests/fixtures/
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-02 07:21:28.034060 auto-labeling-pipeline-0.1.8/tests/fixtures/cassettes/
--rw-r--r--   0 runner    (1001) docker     (117)     1061 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/fixtures/cassettes/amazon_comprehend_sentiment.yaml
--rw-r--r--   0 runner    (1001) docker     (117)     1708 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/fixtures/cassettes/gcp_entities.yaml
--rw-r--r--   0 runner    (1001) docker     (117)     3636 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_labels.py
--rw-r--r--   0 runner    (1001) docker     (117)     1703 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_mappings.py
--rw-r--r--   0 runner    (1001) docker     (117)      847 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_menu.py
--rw-r--r--   0 runner    (1001) docker     (117)     1838 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (117)     1227 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_pipeline.py
--rw-r--r--   0 runner    (1001) docker     (117)      972 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_postprocessing.py
--rw-r--r--   0 runner    (1001) docker     (117)     1206 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_request.py
--rw-r--r--   0 runner    (1001) docker     (117)      876 2021-02-02 07:21:20.000000 auto-labeling-pipeline-0.1.8/tests/test_task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.216430 auto-labeling-pipeline-0.1.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (121)      631 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/01-question.md
+-rw-r--r--   0 runner    (1001) docker     (121)      539 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/02-bug.md
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/03-install.md
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/04-request.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1303 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)      657 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2364 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      633 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/workflows/package-installation.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      696 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     2826 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)       27 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     3372 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1670 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1072 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      509 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (121)    32830 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (121)     1219 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1300 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/label.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1354 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/mappings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2092 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/menu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2352 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      590 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)      738 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1712 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      753 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/task.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/templates/amazon_comprehend_sentiment.jinja2
+-rw-r--r--   0 runner    (1001) docker     (121)      538 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/templates/gcp_entities.jinja2
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2129 2021-02-15 06:43:30.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1517 2021-02-15 06:43:31.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-02-15 06:43:30.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2021-02-15 06:43:30.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-02-15 06:43:30.000000 auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1478 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (121)      201 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/data/amazon_comprehend_sentiment.json
+-rw-r--r--   0 runner    (1001) docker     (121)     3326 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/data/gcp_entities.json
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.216430 auto-labeling-pipeline-0.1.9/tests/fixtures/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-02-15 06:43:31.220430 auto-labeling-pipeline-0.1.9/tests/fixtures/cassettes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1061 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/fixtures/cassettes/amazon_comprehend_sentiment.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1708 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/fixtures/cassettes/gcp_entities.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3367 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_labels.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1703 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_menu.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1838 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (121)      847 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_postprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1206 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_request.py
+-rw-r--r--   0 runner    (1001) docker     (121)      499 2021-02-15 06:43:25.000000 auto-labeling-pipeline-0.1.9/tests/test_task.py
```

### Comparing `auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/01-question.md` & `auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/01-question.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/02-bug.md` & `auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/02-bug.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/ISSUE_TEMPLATE/03-install.md` & `auto-labeling-pipeline-0.1.9/.github/ISSUE_TEMPLATE/03-install.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/PULL_REQUEST_TEMPLATE.md` & `auto-labeling-pipeline-0.1.9/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/workflows/ci.yml` & `auto-labeling-pipeline-0.1.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/workflows/codeql-analysis.yml` & `auto-labeling-pipeline-0.1.9/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/workflows/package-installation.yml` & `auto-labeling-pipeline-0.1.9/.github/workflows/package-installation.yml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.github/workflows/pypi-publish.yml` & `auto-labeling-pipeline-0.1.9/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/.gitignore` & `auto-labeling-pipeline-0.1.9/.gitignore`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/CODE_OF_CONDUCT.md` & `auto-labeling-pipeline-0.1.9/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/CONTRIBUTING.md` & `auto-labeling-pipeline-0.1.9/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/LICENSE` & `auto-labeling-pipeline-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/PKG-INFO` & `auto-labeling-pipeline-0.1.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-labeling-pipeline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Auto labeling pipeline for doccano
 Home-page: https://github.com/doccano/auto-labeling-pipeline
 Author: Hironsan
 Author-email: hiroki.nakayama.py@gmail.com
 License: MIT
 Description: 
         # Auto labeling pipeline
```

### Comparing `auto-labeling-pipeline-0.1.8/Pipfile.lock` & `auto-labeling-pipeline-0.1.9/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/README.md` & `auto-labeling-pipeline-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/label.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/label.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/labels.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/labels.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 import abc
-from typing import Dict, Iterable, List, Optional
+from typing import Dict, Iterable, List, Optional, Type
 
-from auto_labeling_pipeline.label import Label
+from auto_labeling_pipeline.label import ClassificationLabel, Label, Seq2seqLabel, SequenceLabel
 
 
 class Labels(metaclass=abc.ABCMeta):
+    label_class: Type[Label]
 
-    def __init__(self, labels: List[Label]):
-        self.labels = labels
+    def __init__(self, labels: List[Dict]):
+        self.labels = [self.label_class(**label) for label in labels]
 
     def filter_by_name(self, vocabulary: Optional[Iterable[str]] = None) -> 'Labels':
         if not vocabulary:
             return self
-        labels = [label for label in self.labels if label.included(vocabulary)]
+        labels = [label.dict() for label in self.labels if label.included(vocabulary)]
         return self.__class__(labels)
 
     def replace_label(self, mapping: Optional[Dict[str, str]] = None) -> 'Labels':
         if not mapping:
             return self
-        self.labels = [label.replace(mapping) for label in self.labels]
-        return self.__class__(self.labels)
+        labels = [label.replace(mapping).dict() for label in self.labels]
+        return self.__class__(labels)
 
     def dict(self) -> List[dict]:
         return [label.dict() for label in self.labels]
 
 
 class ClassificationLabels(Labels):
-    pass
+    label_class = ClassificationLabel
 
 
 class SequenceLabels(Labels):
-    pass
+    label_class = SequenceLabel
 
 
 class Seq2seqLabels(Labels):
+    label_class = Seq2seqLabel
 
     def filter_by_name(self, vocabulary: Optional[Iterable[str]] = None) -> Labels:
         return self
 
     def replace_label(self, mapping: Optional[Dict[str, str]] = None) -> Labels:
         return self
```

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/mappings.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/mappings.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,49 @@
 import json
 import pathlib
 from typing import Any, Dict, Optional, Type
 
 from jinja2 import Template
 
-from auto_labeling_pipeline.labels import Labels
-from auto_labeling_pipeline.task import DocumentClassification, GenericTask, SequenceLabeling, Task
+from auto_labeling_pipeline.labels import ClassificationLabels, Labels, SequenceLabels
 
 TEMPLATE_DIR = pathlib.Path(__file__).parent / 'templates'
 
 
 class MappingTemplate:
-    task: Type[Task]
+    label_collection: Type[Labels]
     template_file: str = ''
 
-    def __init__(self, task: Type[Task] = GenericTask, template: Optional[str] = ''):
+    def __init__(self, label_collection: Type[Labels] = Labels, template: Optional[str] = ''):
         if self.template_file:
             template = self.load()
-        self.task = task if task is not GenericTask else self.task
+        if label_collection is not Labels:
+            self.label_collection = label_collection
         self.template = template
 
     def render(self, response: Dict) -> Labels:
         template = Template(self.template)
         rendered_json = template.render(input=response)
         labels = json.loads(rendered_json)
-        labels = self.task.create_label_collection(labels)
+        labels = self.label_collection(labels)
         return labels
 
     def load(self) -> str:
         filepath = TEMPLATE_DIR / self.template_file
         with open(filepath) as f:
             return f.read()
 
     def dict(self) -> Dict[str, Any]:
         return {
             'template': self.template,
-            'task': self.task
+            'collection': self.label_collection
         }
 
 
 class AmazonComprehendSentimentTemplate(MappingTemplate):
-    task = DocumentClassification
+    label_collection = ClassificationLabels
     template_file = 'amazon_comprehend_sentiment.jinja2'
 
 
 class GCPEntitiesTemplate(MappingTemplate):
-    task = SequenceLabeling
+    label_collection = SequenceLabels
     template_file = 'gcp_entities.jinja2'
```

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/menu.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/menu.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/models.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/models.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/pipeline.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/pipeline.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/postprocessing.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/postprocessing.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/request.py` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/request.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline/templates/gcp_entities.jinja2` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline/templates/gcp_entities.jinja2`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/PKG-INFO` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-labeling-pipeline
-Version: 0.1.8
+Version: 0.1.9
 Summary: Auto labeling pipeline for doccano
 Home-page: https://github.com/doccano/auto-labeling-pipeline
 Author: Hironsan
 Author-email: hiroki.nakayama.py@gmail.com
 License: MIT
 Description: 
         # Auto labeling pipeline
```

### Comparing `auto-labeling-pipeline-0.1.8/auto_labeling_pipeline.egg-info/SOURCES.txt` & `auto-labeling-pipeline-0.1.9/auto_labeling_pipeline.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/setup.py` & `auto-labeling-pipeline-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/data/gcp_entities.json` & `auto-labeling-pipeline-0.1.9/tests/data/gcp_entities.json`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/fixtures/cassettes/amazon_comprehend_sentiment.yaml` & `auto-labeling-pipeline-0.1.9/tests/fixtures/cassettes/amazon_comprehend_sentiment.yaml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/fixtures/cassettes/gcp_entities.yaml` & `auto-labeling-pipeline-0.1.9/tests/fixtures/cassettes/gcp_entities.yaml`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_labels.py` & `auto-labeling-pipeline-0.1.9/tests/test_labels.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,45 +1,41 @@
 import pytest
 
-from auto_labeling_pipeline.label import ClassificationLabel, Seq2seqLabel, SequenceLabel
 from auto_labeling_pipeline.labels import ClassificationLabels, Seq2seqLabels, SequenceLabels
 
 
 @pytest.fixture
 def example_classification_data():
     labels = [
         {'label': 'A'},
         {'label': 'B'},
         {'label': 'C'}
     ]
-    labels = [ClassificationLabel(**label) for label in labels]
     labels = ClassificationLabels(labels)
     return labels
 
 
 @pytest.fixture
 def example_sequence_data():
     labels = [
         {'label': 'A', 'start_offset': 0, 'end_offset': 1},
         {'label': 'B', 'start_offset': 1, 'end_offset': 2},
         {'label': 'C', 'start_offset': 2, 'end_offset': 3}
     ]
-    labels = [SequenceLabel(**label) for label in labels]
     labels = SequenceLabels(labels)
     return labels
 
 
 @pytest.fixture
 def example_seq2seq_data():
     labels = [
         {'text': 'A'},
         {'text': 'B'},
         {'text': 'C'}
     ]
-    labels = [Seq2seqLabel(**label) for label in labels]
     labels = Seq2seqLabels(labels)
     return labels
 
 
 class TestClassificationLabels:
 
     def test_filter_by_name(self, example_classification_data):
```

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_mappings.py` & `auto-labeling-pipeline-0.1.9/tests/test_mappings.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_menu.py` & `auto-labeling-pipeline-0.1.9/tests/test_menu.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_models.py` & `auto-labeling-pipeline-0.1.9/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_pipeline.py` & `auto-labeling-pipeline-0.1.9/tests/test_pipeline.py`

 * *Files identical despite different names*

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_postprocessing.py` & `auto-labeling-pipeline-0.1.9/tests/test_postprocessing.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,17 @@
-from auto_labeling_pipeline.label import ClassificationLabel
 from auto_labeling_pipeline.labels import ClassificationLabels
 from auto_labeling_pipeline.postprocessing import PostProcessor
 
 
 def test_postprocessor():
     labels = [
         {'label': 'PERSON'},
         {'label': 'ORG'},
         {'label': 'Facility'}
     ]
-    labels = [ClassificationLabel(**label) for label in labels]
     labels = ClassificationLabels(labels)
     mapping = {'Facility': 'ORG'}
     processor = PostProcessor(mapping=mapping)
     labels = processor.transform(labels).dict()
     expected = [
         {'label': 'ORG'},
     ]
```

### Comparing `auto-labeling-pipeline-0.1.8/tests/test_request.py` & `auto-labeling-pipeline-0.1.9/tests/test_request.py`

 * *Files identical despite different names*

