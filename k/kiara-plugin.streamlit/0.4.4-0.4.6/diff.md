# Comparing `tmp/kiara_plugin.streamlit-0.4.4.tar.gz` & `tmp/kiara_plugin.streamlit-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.streamlit-0.4.4.tar", last modified: Thu Jun 29 08:57:58 2023, max compression
+gzip compressed data, was "kiara_plugin.streamlit-0.4.6.tar", last modified: Thu Jul 20 09:47:10 2023, max compression
```

## Comparing `kiara_plugin.streamlit-0.4.4.tar` & `kiara_plugin.streamlit-0.4.6.tar`

### file list

```diff
@@ -1,153 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.330222 kiara_plugin.streamlit-0.4.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7404 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      688 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      779 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/jobs/download_journals.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      754 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/operations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/apps/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/pipelines/example_file_onboarding.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/apps/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.330222 kiara_plugin.streamlit-0.4.4/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)      849 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/pipelines/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.346223 kiara_plugin.streamlit-0.4.4/examples/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/example.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/help.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipeline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/example.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/topic_modeling.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/step_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5354 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_dynamic.py
--rw-r--r--   0 runner    (1001) docker     (123)     6535 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_static.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workflows.py
--rw-r--r--   0 runner    (1001) docker     (123)     7482 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/examples/streamlit/workshop.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4472 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      413 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.334222 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/
--rw-r--r--   0 runner    (1001) docker     (123)     7881 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/
--rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/
--rw-r--r--   0 runner    (1001) docker     (123)     4265 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5936 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/
--rw-r--r--   0 runner    (1001) docker     (123)     9266 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8539 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/container_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     7004 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/scalars.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/operations/
--rw-r--r--   0 runner    (1001) docker     (123)     2494 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/operations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/
--rw-r--r--   0 runner    (1001) docker     (123)     7566 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/assemblies.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/core_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/network_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/tabular.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/
--rw-r--r--   0 runner    (1001) docker     (123)     1983 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11223 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     6870 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      470 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/renderers/
--rw-r--r--   0 runner    (1001) docker     (123)     1868 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/renderers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.342223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/pipeline/
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
--rw-r--r--   0 runner    (1001) docker     (123)    10206 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/streamlit.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/class_loading.py
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/monkey_patches.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.350223 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5889 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:56:46.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:57:58.000000 kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.354223 kiara_plugin.streamlit-0.4.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:58.358224 kiara_plugin.streamlit-0.4.4/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-06-29 08:56:26.000000 kiara_plugin.streamlit-0.4.4/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.843371 kiara_plugin.streamlit-0.4.6/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.863373 kiara_plugin.streamlit-0.4.6/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.867374 kiara_plugin.streamlit-0.4.6/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7408 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      688 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      792 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4612 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.867374 kiara_plugin.streamlit-0.4.6/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/dev_helper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.867374 kiara_plugin.streamlit-0.4.6/apps/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/jobs/download_journals.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      710 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/operations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.867374 kiara_plugin.streamlit-0.4.6/apps/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/pipelines/example_file_onboarding.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/apps/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.843371 kiara_plugin.streamlit-0.4.6/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.867374 kiara_plugin.streamlit-0.4.6/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2650 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.847372 kiara_plugin.streamlit-0.4.6/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/pipelines/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1373 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/analyze_network_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/examples/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/pipelines/example.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/pipelines/topic_modeling.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     5308 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/workflow_dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6495 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/workflow_static.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8113 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/examples/streamlit/workshop.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.847372 kiara_plugin.streamlit-0.4.6/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.871374 kiara_plugin.streamlit-0.4.6/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1834 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-20 09:47:10.891376 kiara_plugin.streamlit-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.847372 kiara_plugin.streamlit-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.847372 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/
+-rw-r--r--   0 runner    (1001) docker     (123)     4738 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29992 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     9240 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/context/
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/context/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/data_import/
+-rw-r--r--   0 runner    (1001) docker     (123)     7522 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/data_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/data_import/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/explore/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/explore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2684 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/explore/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4476 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6273 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9005 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/
+-rw-r--r--   0 runner    (1001) docker     (123)    16095 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9874 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/container_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10725 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8663 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/scalars.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/modals/
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/modals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6107 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/operations/
+-rw-r--r--   0 runner    (1001) docker     (123)     6110 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/operations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)     3520 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/
+-rw-r--r--   0 runner    (1001) docker     (123)     9626 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/assemblies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7122 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/core_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3670 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/tabular.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11354 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12037 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6917 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      479 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.883375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/renderers/
+-rw-r--r--   0 runner    (1001) docker     (123)     7551 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/renderers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.855373 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/code_gen/
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/code_gen/kiara_streamlit_api.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/pipeline/
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)    12023 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/streamlit.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1551 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/class_loading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2636 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/monkey_patches.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.875374 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5883 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:45:59.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 09:47:10.000000 kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:47:10.887375 kiara_plugin.streamlit-0.4.6/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      233 2023-07-20 09:45:47.000000 kiara_plugin.streamlit-0.4.6/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.streamlit-0.4.4/.cruft.json` & `kiara_plugin.streamlit-0.4.6/.cruft.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'8a773724c6c0b1b6df826fcda971c185f25234c8'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
+    "commit": "8a773724c6c0b1b6df826fcda971c185f25234c8",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.streamlit-0.4.6/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.streamlit-0.4.6/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/.github/workflows/build-darwin.yaml` & `kiara_plugin.streamlit-0.4.6/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/.github/workflows/build-linux.yaml` & `kiara_plugin.streamlit-0.4.6/.github/workflows/build-linux.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -146,15 +146,15 @@
         run: python -m build
       - name: upload source package
         run: curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: upload wheel
         run: curl -F package=@$(ls dist/kiara*.whl) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/
       - name: publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: "${{ secrets.PYPI_API_TOKEN }}"
 
   conda_package_build:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
```

### Comparing `kiara_plugin.streamlit-0.4.4/.github/workflows/build-windows.yaml` & `kiara_plugin.streamlit-0.4.6/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/.gitignore` & `kiara_plugin.streamlit-0.4.6/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -60,7 +60,9 @@
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.streamlit/meta.yaml
 other_pipelines
+.pixi
+dev.py
```

### Comparing `kiara_plugin.streamlit-0.4.4/.pre-commit-config.yaml` & `kiara_plugin.streamlit-0.4.6/.pre-commit-config.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     files: "^src/"
     pass_filenames: true
     args: ["--config-file", "setup.cfg", "--ignore-missing-imports", "--explicit-package-bases"]
     additional_dependencies: [pydantic>=1.8.0, rich>=10.0.0, ruamel.yaml, anyio>=3.0.0, pyzmq>=22.0.3, bidict, sqlalchemy-stubs, types-python-slugify, types-setuptools, types-python-dateutil, dag_cbor, multiformats, textual, regex, types-pytz, types-orjson]
 
 - repo: https://github.com/charliermarsh/ruff-pre-commit
   # Ruff version.
-  rev: 'v0.0.275'
+  rev: 'v0.0.277'
   hooks:
     - id: ruff
 
 - repo: https://github.com/Kludex/no-optional
   rev: 0.4.0
   hooks:
     - id: no_optional
```

### Comparing `kiara_plugin.streamlit-0.4.4/LICENSE` & `kiara_plugin.streamlit-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/Makefile` & `kiara_plugin.streamlit-0.4.6/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/PKG-INFO` & `kiara_plugin.streamlit-0.4.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.streamlit
-Version: 0.4.4
+Version: 0.4.6
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
-Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: workflow_app
 Provides-Extra: all_plugins
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
 Provides-Extra: dev_all
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.streamlit/goto?ref=develop)
```

### Comparing `kiara_plugin.streamlit-0.4.4/README.md` & `kiara_plugin.streamlit-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/apps/components.py` & `kiara_plugin.streamlit-0.4.6/apps/operations.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,24 @@
 # -*- coding: utf-8 -*-
 import os
 
-import streamlit as st
-
 import kiara_plugin.streamlit as kst
 from kiara.interfaces.python_api import JobDesc
 
-st.set_page_config(layout="wide")
+st = kst.init(page_config={"layout": "wide"})
 
-kst.init()
-st.kiara.api.set_active_context("components_doc", create=True)
+st.kiara.api.set_active_context("_operation_doc", create=True)
 
 if "file_bundle" not in st.kiara.api.list_alias_names():
 
     with st.spinner("Downloading example data ..."):
         job_file = os.path.join(
             os.path.dirname(__file__), "jobs", "download_journals.yaml"
         )
         job_desc = JobDesc.create_from_file(path=job_file)
 
         results = st.kiara.api.run_job(job_desc)
 
         for field_name, value in results.items():
             st.kiara.api.store_value(value, field_name)
 
-
-st.kiara.component_info()
+st.kiara.operation_documentation()
```

### Comparing `kiara_plugin.streamlit-0.4.4/apps/jobs/download_journals.yaml` & `kiara_plugin.streamlit-0.4.6/apps/jobs/download_journals.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/apps/operations.py` & `kiara_plugin.streamlit-0.4.6/apps/components.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # -*- coding: utf-8 -*-
 import os
 
-import streamlit as st
-
 import kiara_plugin.streamlit as kst
 from kiara.interfaces.python_api import JobDesc
 
-st.set_page_config(layout="wide")
-kst.init()
+st = kst.init(page_config={"layout": "wide"})
 
-st.kiara.api.set_active_context("_operation_doc", create=True)
+st.kiara.api.set_active_context("components_doc", create=True)
 
 if "file_bundle" not in st.kiara.api.list_alias_names():
-    print("MISSING")
 
     with st.spinner("Downloading example data ..."):
         job_file = os.path.join(
             os.path.dirname(__file__), "jobs", "download_journals.yaml"
         )
         job_desc = JobDesc.create_from_file(path=job_file)
 
         results = st.kiara.api.run_job(job_desc)
 
         for field_name, value in results.items():
             st.kiara.api.store_value(value, field_name)
 
-st.kiara.operation_documentation()
+
+st.kiara.component_info()
```

### Comparing `kiara_plugin.streamlit-0.4.4/apps/pipelines/example_file_onboarding.yaml` & `kiara_plugin.streamlit-0.4.6/apps/pipelines/example_file_onboarding.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -19,14 +19,27 @@
     step_id: create_nodes_table
     input_links:
       file: pick_journal_nodes.file
   - module_type: create.table.from.file
     step_id: create_edges_table
     input_links:
       file: pick_journal_edges.file
+  - module_type: assemble.tables
+    step_id: assemble_tables
+    module_config:
+      constants:
+        table_name_1: "nodes"
+        table_name_2: "edges"
+    input_links:
+      table_1: create_nodes_table.table
+      table_2: create_edges_table.table
+  - module_type: create.database.from.tables
+    step_id: create_database_from_tables
+    input_links:
+      tables: assemble_tables.tables
 
 
 input_aliases:
   download_example_data.source: "example_data_source"
   download_example_data.sub_path: "sub_folder"
   download_example_data.include_files: "include_files"
   download_example_data.exclude_files: "exclude_files"
@@ -40,7 +53,9 @@
 output_aliases:
   download_example_data.file_bundle: "file_bundle"
   create_files_table.table: "files_table"
   pick_journal_nodes.file: "nodes_file"
   pick_journal_edges.file: "edges_file"
   create_nodes_table.table: "nodes_table"
   create_edges_table.table: "edges_table"
+  assemble_tables.tables: "journals_tables"
+  create_database_from_tables.database: "journals_database"
```

### Comparing `kiara_plugin.streamlit-0.4.4/docs/development.md` & `kiara_plugin.streamlit-0.4.6/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/docs/index.md` & `kiara_plugin.streamlit-0.4.6/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.streamlit-0.4.6/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.streamlit-0.4.6/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipeline.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,37 +1,26 @@
 # -*- coding: utf-8 -*-
+import os
 
 import nltk
 import streamlit as st
 
 import kiara_plugin.streamlit as kiara_streamlit
 from kiara_plugin.streamlit.components.workflow.static import WorkflowSessionStatic
 
 st.set_page_config(layout="wide")
 
-nltk.download("punkt")
-nltk.download("stopwords")
-
 kst = kiara_streamlit.init()
 
 current = kst.api.get_current_context_name()
 with st.sidebar:
     selected_context = st.kiara.context_switch_control(allow_create=True, key="xxx")
     context_changed = current != selected_context
 
-pipeline = {
-    "pipeline_name": "logic.nor",
-    "doc": "Returns 'True' if both inputs are 'False'.",
-    "steps": [
-        {"module_type": "logic.or", "step_id": "or"},
-        {"module_type": "logic.not", "step_id": "not", "input_links": {"a": "or.y"}},
-    ],
-    "input_aliases": {"or.a": "a", "or.b": "b"},
-    "output_aliases": {"not.y": "y"},
-}
+pipeline = {{ pipeline.structure.pipeline_config.get_raw_config() }}
 
 
 workflow_ref = "workflow_static"
 if workflow_ref not in st.session_state or context_changed:
     workflow = st.kiara.api.create_workflow(initial_pipeline=pipeline)
     workflow_session: WorkflowSessionStatic = WorkflowSessionStatic(workflow=workflow)
     st.session_state[workflow_ref] = workflow_session
```

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/example.yaml` & `kiara_plugin.streamlit-0.4.6/examples/streamlit/pipelines/example.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/pipelines/topic_modeling.yaml` & `kiara_plugin.streamlit-0.4.6/examples/streamlit/pipelines/topic_modeling.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_dynamic.py` & `kiara_plugin.streamlit-0.4.6/examples/streamlit/workflow_dynamic.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 # -*- coding: utf-8 -*-
-import streamlit as st
-
-import kiara_plugin.streamlit as kiara_streamlit
+import kiara_plugin.streamlit as kst
 from kiara_plugin.streamlit.components.workflow.dynamic import WorkflowSessionDynamic
 
-st.set_page_config(layout="wide")
+st = kst.init(page_config={"layout": "wide"})
 
-kst = kiara_streamlit.init()
 
 EXPLANATION = """
 This is an example of how an exploratory data-science workflow could (not should!) look like in 'pure' UI (without code), usually you'd use notebook tech like Jupyter for that. Obviously there are limitations, but there is also some 'guidance' inbuilt (which those notebooks lack), because all the possible operations for the dataset you choose are pre-filtered for you. Also, it ships with the documentation about everything it can do, which is kinda nice.
 
 An alternative to this would be a node-based approach, something like the blender node editor ( https://www.youtube.com/watch?v=moKFSMJwpmE ) or  https://gimelstudio.github.io/
 
 The prototype is a bit terse at the moment, and I haven't had time to think about guiding users through all this, so it might be that your initial experience is a bit confusing. But I figured it is probably not be a bad idea to expose you to this, because that way you can register with yourself the typical kind of problems new users would have, and that we are out to solve. I haven't implemented anything 'onboarding' yet (that's another one of the topics I plan to address with prototypes like this), so this thing has 2 datasets automatically included: 2 csv files that can be used to generate a network graph .
@@ -39,15 +36,15 @@
 - click the 'Preview' box above to see the table you are working with as input, select the inputs accordingly: 'Source', 'Target' (we don't need the 'id_column_name' in this particular instance because we don't hava a separate nodes table)
 - select the only result for the next step again, tihs is of type 'network_data'. We don't have many modules yet to work with 'network_data', but I hope you get the idea where this is going...
 """
 
 with st.expander("Notes (click to hide)", expanded=True):
     st.markdown(EXPLANATION)
 
-current = kst.api.get_current_context_name()
+current = st.kiara.api.get_current_context_name()
 with st.sidebar:
     selected_context = st.kiara.context_switch_control(allow_create=True, key="xxx")
     context_changed = current != selected_context
 
 workflow_ref = "workflow_dynamic"
 if workflow_ref not in st.session_state or context_changed:
     workflow = st.kiara.api.create_workflow()
@@ -56,23 +53,23 @@
 else:
     workflow_session = st.session_state[workflow_ref]
 
 if not st.kiara.api.list_alias_names():
     with st.spinner("Downloading example data ..."):
 
         result = st.kiara.api.run_job(
-            operation="download.file",
+            operation="import.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
+                "source": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_nodes_file")
 
         result = st.kiara.api.run_job(
-            operation="download.file",
+            operation="import.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
+                "source": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_edges_file")
 
 st.kiara.workflow(workflow_session)
```

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/workflow_static.py` & `kiara_plugin.streamlit-0.4.6/examples/streamlit/workflow_static.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # -*- coding: utf-8 -*-
 import os
 
 import nltk
-import streamlit as st
 
-import kiara_plugin.streamlit as kiara_streamlit
+import kiara_plugin.streamlit as kst
 from kiara.interfaces.python_api import OperationInfo
 from kiara_plugin.streamlit.components.workflow.static import WorkflowSessionStatic
 
-st.set_page_config(layout="wide")
+st = kst.init(page_config={"layout": "wide"})
 
 nltk.download("punkt")
 nltk.download("stopwords")
 
-kst = kiara_streamlit.init()
-
 EXPLANATION = """
 This is an example of how to render a pre-assembled pipeline as a workflow UI. All of this is rendered auto-matically, using the content of this pipeline:
 
 - https://github.com/DHARPA-Project/kiara_plugin.streamlit/blob/develop/examples/streamlit/pipelines/topic_modeling.yaml
 
 The whole experience is a bit clunky, which is par for the course for a fully-auto-rendered, interactive multi-page form like this. It'll be possible to augment the pipeline description I linked above with additional hints, which will improve the UI experience substantially (e.g. only present column names available in the selected table, instead of asking the user to input the column names free-form).
 
@@ -54,22 +51,22 @@
 
    - the final step, if you know about topic modeling, then the results will make sense, otherwise, probably not. Select to create a few topics (maybe `num_topics_min` 5 and num_topics_max 9), check `compute_coherence` and words_per_topic 3. Our production app would have a lot more explanations and documentation what any of the inputs and outputs mean, what exactly happens, what LDA is, etc.
 """
 with st.expander("Notes (click to hide)", expanded=True):
     st.markdown(EXPLANATION)
 
 
-current = kst.api.get_current_context_name()
+current = st.kiara.api.get_current_context_name()
 with st.sidebar:
     selected_context = st.kiara.context_switch_control(allow_create=True, key="xxx")
     context_changed = current != selected_context
 
 
 with st.spinner("Registering pipelines ..."):
-    if "topic_modeling" not in kst.api.list_operation_ids():
+    if "topic_modeling" not in st.kiara.api.list_operation_ids():
         pipelines_path = os.path.join(
             os.path.dirname(__file__), "pipelines", "topic_modeling.yaml"
         )
         ops = st.kiara.api.register_pipelines(pipelines_path)
 
 pipeline = None
 if "selected_pipeline" in st.session_state:
@@ -93,33 +90,33 @@
 else:
     workflow_session = st.session_state[workflow_ref]
 
 if "example_corpus" not in st.kiara.api.list_alias_names():
     with st.spinner("Downloading example data ..."):
 
         result = st.kiara.api.run_job(
-            operation="download.file",
+            operation="import.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
+                "source": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_nodes_file")
 
         result = st.kiara.api.run_job(
-            operation="download.file",
+            operation="import.file",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
+                "source": "https://github.com/DHARPA-Project/kiara.examples/raw/main/examples/data/network_analysis/journals/JournalEdges1902.csv"
             },
         )
         st.kiara.api.store_value(value=result["file"], alias="journal_edges_file")
 
         result = st.kiara.api.run_job(
-            operation="download.file_bundle",
+            operation="import.file_bundle",
             inputs={
-                "url": "https://github.com/DHARPA-Project/kiara.examples/archive/refs/heads/main.zip",
+                "source": "https://github.com/DHARPA-Project/kiara.examples/archive/refs/heads/main.zip",
                 "sub_path": "kiara.examples-main/examples/data/language_processing/text_corpus/data",
             },
         )
         st.kiara.api.store_value(value=result["file_bundle"], alias="example_corpus")
 
 
 st.kiara.workflow(workflow_session)
```

### Comparing `kiara_plugin.streamlit-0.4.4/examples/streamlit/workshop.py` & `kiara_plugin.streamlit-0.4.6/examples/streamlit/workshop.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,21 @@
 # -*- coding: utf-8 -*-
-import streamlit as st
-
 import kiara_plugin.streamlit as kst
 from kiara.api import KiaraAPI
 
 # st.set_page_config(layout="wide")
 
 # This example app introduces kiara, a data orchestration software. It will walk you through creating a simple streamilt application, and some basic but essential functions that can be built on in further notebooks.
 
 # first, we initialize the kiara streamlit integration
 # that way, we'll get access to the kiara api and some custom components
 # via the 'st' object
 # a list of components can be found here: https://kiara-doc-components.streamlit.app/
 
-
-kst.init()
+st = kst.init(page_config={"layout": "wide"})
 
 # for convenience, and for IDS to help us autocomplete, we assign the kiara api to a variable
 kiara: KiaraAPI = st.kiara.api
 
 # in most cases, we need to pick an operation we want to use. You can query the kiara api for the availble ones like:
 #
 #  st.write(kiara.list_operation_ids())
@@ -29,40 +26,40 @@
 #
 # or, go https://kiara-doc-operations.streamlit.app/ and have a look there
 
 """---"""
 
 # Downloading files
 
-# Great, now we know the different kind of operations we can use with kiara. Let’s start by introducing some files to our application, using the download.file function.  First we want to find out what this operation does, and just as importantly, what inputs it needs to work.
+# Great, now we know the different kind of operations we can use with kiara. Let’s start by introducing some files to our application, using the 'import.file' function.  First we want to find out what this operation does, and just as importantly, what inputs it needs to work.
 
 # We'll put the result in an expander, because it's a lot of text.
 
 """# Download file
 
 *kiara* will download a csv file from a url you provide, it will execute the 'download.file' operation. For details about this operation, click on the expander below.
 """
-with st.expander("Show operation info 'download.file'", expanded=False):
-    st.write(st.kiara.operation_info("download.file"))
+with st.expander("Show operation info 'import.file'", expanded=False):
+    st.write(st.kiara.operation_info("import.file"))
 
-# So from this, we know that download.file will download a single file from a remote location for us to use in kiara.  We need to give the function a url and, if we want, a file name. These are the inputs.  In return, we will get the file and metadata about the file as our outputs.
+# So from this, we know that `import.file` will download a single file from a remote location for us to use in kiara.  We need to give the function at least a source (url) and, if we want, a file name. These are the inputs.  In return, we will get the file and metadata about the file as our outputs.
 # Let’s give this a go using some kiara sample data.
-# First we define our inputs, then use kiara.run_job with our chosen operation, download.file, and save this as our outputs.
+# First we define our inputs, then use kiara.run_job with our chosen operation, `import.file`, and save this as our outputs.
 
 # For the url, we can actually ask the user, but giving them a default value in case they don't have one at hand.
 
-default_url = "https://raw.githubusercontent.com/DHARPA-Project/kiara.examples/main/examples/data/journals/JournalNodes1902.csv"
+default_url = "https://raw.githubusercontent.com/DHARPA-Project/kiara.examples/main/examples/data/network_analysis/journals/JournalNodes1902.csv"
 url = st.text_input("Please provide a url to download", value=default_url)
 
 # we want the user to kick of the download process, so we need to have a button they can use
 download_button = st.button("Download file")
 if download_button:
     # after looking at the operation info, we know that we need to provide a url and a file name
-    inputs = {"url": url, "file_name": url.split("/")[-1]}
-    outputs = kiara.run_job("download.file", inputs=inputs)
+    inputs = {"source": url, "file_name": url.split("/")[-1]}
+    outputs = kiara.run_job("import.file", inputs=inputs)
     # we need to store the download result in the session state, otherwise it would be lost after a script rerun
     st.session_state["download_result"] = outputs
 
 download_result = st.session_state.get("download_result", None)
 if not download_result:
     st.write("No file downloaded yet. Stoping now...")
     st.stop()
@@ -95,23 +92,30 @@
 
 op_id = "create.table.from.file"
 create_table_info = kiara.retrieve_operation_info(op_id)
 
 with st.expander(f"Show operation info '{op_id}'", expanded=False):
     st.kiara.operation_info(op_id)
 
+# As we can see from the operation info, in addition to the file input, we can also specify whether the files' first row is a header,
+# or not. This is important since if it's a header, we want the table names to follow it's content, and if not, we also need to know.
+# This is a simple as operation inputs go, so let's render an input widget so the user can tell us what to do (by default, without any input,
+# kiara will try to auto-determine the header status).
+
+is_header = st.kiara.input_boolean(label="Is the first row a header?", key="is_header")
+
 # Great, we have all the information we need now.
 # Let’s go again.
 # First we define our inputs, the downloaded file we saved earlier.
 # Then use kiara.run_job with our chosen operation, this time stored as op_id.
 # Once this is saved as our outputs, we can print it out."""
 
 create_table_btn = st.button("Create table")
 if create_table_btn:
-    inputs = {"file": downloaded_file}
+    inputs = {"file": downloaded_file, "first_row_is_header": is_header}
     outputs = kiara.run_job(op_id, inputs=inputs)
     st.session_state["create_table_result"] = outputs
 
 create_table_result = st.session_state.get("create_table_result", None)
 if not create_table_result:
     st.write("No table created yet. Stoping now...")
     st.stop()
```

### Comparing `kiara_plugin.streamlit-0.4.4/mkdocs.yml` & `kiara_plugin.streamlit-0.4.6/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/pyproject.toml` & `kiara_plugin.streamlit-0.4.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -13,62 +13,66 @@
     {name = "Markus Binsteiner", email = "markus@frkl.io"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["kiara", "streamlit"]
 license = {text = "MPL-2.0"}
 classifiers = [
-    "Framework :: Django",
     "Programming Language :: Python :: 3",
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11"
 ]
 dependencies = [
-    "kiara_plugin.tabular>=0.4.28",
-    "kiara_plugin.onboarding>=0.4.5",
+    "kiara>=0.4.48",
+    "kiara_plugin.tabular>=0.4.29",
+    "kiara_plugin.onboarding>=0.4.7",
+    "kiara_plugin.html>=0.4.4",
     "streamlit>=1.24.0",
     "streamlit-aggrid>=0.3.4",
+    "streamlit-option-menu>=0.3.6",
     "importlib-resources",
     "pydot>=1.4.0",
-    "pyvis>=0.3.0",
+    "pygwalker>=0.1.11",
+    "streamlit-scrollable-textbox>=0.0.3",
     "streamlit-tags>=1.2.8"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 workflow_app = [
     "PyGithub>=1.58.0",
     "githublfs>=0.1.3"
 ]
 all_plugins = [
-    "kiara_plugin.network_analysis>=0.4.9",
+    "kiara_plugin.network_analysis>=0.4.14",
     "kiara_plugin.language_processing>=0.4.10",
-    "kiara_plugin.html>=0.4.3",
-    "kiara_plugin.onboarding>=0.4.5"
 ]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
 dev_testing = [
     "kiara[dev_testing]",
     "kiara_plugin.network_analysis>=0.4.7",
 ]
 dev_utils = [
     "kiara[dev_utils]",
 ]
 dev_all = [
     "kiara[dev_all]"
 ]
+streamlit = [
+    "kiara_plugin.streamlit"
+]
 
 [project.entry-points."kiara.plugin"]
 streamlit = "kiara_plugin.streamlit"
 
 [project.entry-points."kiara.data_types"]
 streamlit = "kiara_plugin.streamlit:find_data_types"
 
@@ -142,15 +146,15 @@
     "PD",
     "PLC",
     "PLE",
     "PLR",
     "PLW",
     "PIE",
 ]
-ignore = ["E501", "S101", "SIM118", "SIM108", "PLR2004", "PLR0913", "S110", "PLR0912", "PLR0915", "PIE810", "T201", "PD011", "F405", "RUF012"]
+ignore = ["E501", "S101", "SIM118", "SIM108", "PLR2004", "PLR0913", "S110", "PLR0912", "PLR0915", "PIE810", "T201", "PD011", "F405", "RUF012", "RUF013", "F403", "PLR0911", "RUF003"]
 
 fix = true
 fixable = ["E", "F", "RUF100", "I001", "Q"]
 
 
 #fixable = ["E", "F", "RUF100", "I001"]
 # Enable Pyflakes `E` and `F` codes by default.
```

### Comparing `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_info_pages.py` & `kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/scripts/documentation/gen_module_doc.py` & `kiara_plugin.streamlit-0.4.6/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/setup.cfg` & `kiara_plugin.streamlit-0.4.6/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -103,14 +103,17 @@
 
 [mypy-orjson.*]
 ignore_missing_imports = true
 
 [mypy-pyarrow.*]
 ignore_missing_imports = true
 
+[mypy-pygwalker.*]
+ignore_missing_imports = true
+
 [mypy-pyvis.*]
 ignore_missing_imports = true
 
 [mypy-ruamel.*]
 ignore_missing_imports = true
 
 [mypy-streamlit_nested_layout.*]
@@ -118,14 +121,17 @@
 
 [mypy-st_aggrid.*]
 ignore_missing_imports = true
 
 [mypy-streamlit_tags.*]
 ignore_missing_imports = true
 
+[mypy-streamlit_scrollable_textbox.*]
+ignore_missing_imports = true
+
 [mypy-uvloop]
 ignore_missing_imports = true
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 # -*- coding: utf-8 -*-
 import abc
 import warnings
 from functools import partial
-from typing import Any, Callable, Dict, Generic, List, Type, TypeVar, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    Generic,
+    List,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 from pydantic import BaseModel, Field
 from pydantic.fields import ModelField
 
 import streamlit as st
 from kiara.interfaces.python_api.models.info import InfoItemGroup, ItemInfo
 from kiara.models.documentation import (
@@ -17,30 +28,30 @@
 from kiara.models.python_class import PythonClass
 from kiara_plugin.streamlit.defaults import AUTO_GEN_MARKER
 from streamlit.runtime.state import SessionStateProxy
 
 with warnings.catch_warnings():
     pass
 
-from typing import TYPE_CHECKING
-
 from streamlit.delta_generator import DeltaGenerator
 
 if TYPE_CHECKING:
     from kiara.api import Kiara, KiaraAPI
-    from kiara_plugin.streamlit.streamlit import KiaraStreamlit
+    from kiara_plugin.streamlit import KiaraStreamlit
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class ComponentOptions(BaseModel):
 
     key: str = Field(
         description="The (base) key to use for this component.", default=AUTO_GEN_MARKER
     )
 
     def create_key(self, *args) -> str:
+        """Create a unique key for a component."""
 
         base = ["kiara", self.key]
         base.extend(args)
         _key = "__".join(base)
         return _key
 
     def get_session_key(self, *key: str) -> str:
@@ -117,28 +128,46 @@
     def set_session_var(
         self, options: "ComponentOptions", *key: str, value: Any
     ) -> None:
 
         session_key = options.get_session_key(*key)
         self._session_state[session_key] = value
 
+    def _create_session_store_callback(
+        self, options: ComponentOptions, *key, default=None
+    ) -> Tuple[Callable, str]:
+
+        _widget_key = options.create_key(*key)
+
+        current = self.get_session_var(options, *key, default=default)
+
+        if current is not None and _widget_key not in self._session_state:
+            self._session_state[_widget_key] = current
+
+        def callback():
+            self._st.session_state[
+                options.get_session_key(*key)
+            ] = self._st.session_state[_widget_key]
+
+        return callback, _widget_key
+
     def render_func(self, st: Union[DeltaGenerator, None] = None) -> Callable:
 
         if st is None:
             st = self._st
 
         return partial(self.render, st)
 
     def get_option_names(self) -> List[str]:
 
         option_fields = list(self.__class__._options.__fields__.keys())
         option_fields.reverse()
         return option_fields
 
-    def render(self, st: DeltaGenerator, *args, **kwargs) -> Any:
+    def render(self, st: "KiaraStreamlitAPI", *args, **kwargs) -> Any:
 
         option_fields = self.get_option_names()
 
         for idx, arg in enumerate(args):
             try:
                 key = option_fields[idx]
             except Exception:
@@ -163,41 +192,59 @@
             import traceback
 
             traceback.print_exc()
             st.error(e)
             return None
 
     @abc.abstractmethod
-    def _render(self, st: DeltaGenerator, options: COMP_OPTIONS_TYPE):
+    def _render(self, st: "KiaraStreamlitAPI", options: COMP_OPTIONS_TYPE):
         pass
 
     def get_component(self, component_name: str) -> "KiaraComponent":
         result = self._kiara_streamlit.get_component(component_name)
         return result
 
 
 class ArgInfo(BaseModel):
     @classmethod
     def from_field(cls, field_info: ModelField):
 
-        python_type = str(field_info.type_)
+        python_type = field_info.outer_type_
         desc = field_info.field_info.description
         req = field_info.required
         default = field_info.default
 
-        if field_info.outer_type_ != field_info.type_:
-            python_type = str(field_info.outer_type_)
-
         if not desc:
             desc = "-- n/a --"
+
+        if (
+            not field_info.is_complex()
+            and not field_info.required
+            and "Union" not in str(python_type)
+        ):
+            python_type_string = f"Union[None, {python_type.__name__}]"
+        else:
+            python_type_string = str(python_type)
+            if python_type_string.startswith("<class"):
+                python_type_string = python_type.__name__
+
+        python_type_string = python_type_string.replace("NoneType", "None")
+        python_type_string = python_type_string.replace("typing.", "")
         return ArgInfo(
-            python_type=python_type, description=desc, required=req, default=default
+            python_type=python_type,
+            description=desc,
+            required=req,
+            default=default,
+            python_type_string=python_type_string,
         )
 
-    python_type: str = Field(description="The python type of this argument.")
+    python_type: Any = Field(description="The python type of this argument.")
+    python_type_string: str = Field(
+        description="The python type hint of this argument."
+    )
     description: str = Field(description="The description of this argument.")
     required: bool = Field(description="Whether this argument is required.")
     default: Any = Field(description="The default value for this argument.")
 
 
 class ComponentInfo(ItemInfo[KiaraComponent]):
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/context/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/context/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
-from typing import Any, Callable, ClassVar, List, Union
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, List, Union
 
 from pydantic import Field
 
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class ContextSwitchOptions(ComponentOptions):
 
     allow_create: bool = Field(
         description="Allow the user to create a new context.", default=False
     )
@@ -33,15 +35,15 @@
             "args": {
                 "switch_to_selected": False,
                 "allow_create": True,
             },
         }
     ]
 
-    def _render(self, st: DeltaGenerator, options: ContextSwitchOptions) -> bool:
+    def _render(self, st: "KiaraStreamlitAPI", options: ContextSwitchOptions) -> bool:
 
         if not options.allow_create:
             context_names = self.api.list_context_names()
             if "default" in context_names:
                 context_names.pop(context_names.index("default"))
                 context_names.insert(0, "default")
             current = self.api.get_current_context_name()
@@ -100,15 +102,15 @@
             context_names = self.api.list_context_names()
 
             if "default" in context_names:
                 context_names.pop(context_names.index("default"))
                 context_names.insert(0, "default")
 
             selected_context = self.write_selectbox(
-                st=selectbox_placeholder,
+                st=selectbox_placeholder,  # type: ignore
                 items=context_names,
                 options=options,
                 key=["kiara_context", "select_context"],
                 force=force,
                 default=current,
                 label="Select context",
                 help="Select the active context.",
@@ -117,15 +119,15 @@
             if selected_context != current and options.switch_to_selected:
                 self.api.set_active_context(selected_context)
 
             return selected_context
 
     def write_selectbox(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: ContextSwitchOptions,
         key: List[str],
         items: List[str],
         force: Any = None,
         default: Any = None,
         label: Union[str, None] = None,
         help: Union[str, None] = None,
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 # -*- coding: utf-8 -*-
 import abc
-from typing import Generic, List, Mapping, Tuple, Type, TypeVar, Union
+from typing import TYPE_CHECKING, Generic, List, Mapping, Tuple, Type, TypeVar, Union
 
 from pydantic import Field
 
 from kiara.interfaces.python_api.models.info import ItemInfo
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.utils.components import create_list_component
 from streamlit.delta_generator import DeltaGenerator
 
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
+
 
 class InfoCompOptions(ComponentOptions):
     class Config:
         arbitrary_types_allowed = True
 
     columns: Union[
         Tuple[int, int], Tuple[DeltaGenerator, DeltaGenerator], None
     ] = Field(description="The column layout to use for the next step.", default=(1, 4))
     height: Union[int, None] = Field(
-        description="The height of the list component.", default=None
+        description="The height of the list component.", default=400
     )
     items: Union[str, List[str], None] = Field(
         description="The item(s) to show info for."
     )
 
 
 ITEM_TYPE = TypeVar("ITEM_TYPE", bound=ItemInfo)
@@ -34,15 +37,15 @@
 
     @classmethod
     @abc.abstractmethod
     def get_info_type(cls) -> Type[ITEM_TYPE]:
         pass
 
     def _render(
-        self, st: DeltaGenerator, options: InfoCompOptions
+        self, st: "KiaraStreamlitAPI", options: InfoCompOptions
     ) -> Union[ITEM_TYPE, None]:
 
         items = options.items
         if items is None:
 
             _items = self.get_all_item_infos()
 
@@ -93,48 +96,54 @@
 
     @abc.abstractmethod
     def get_info_item(self, item_id: str) -> ITEM_TYPE:
         pass
 
     @abc.abstractmethod
     def render_info(
-        self, st: DeltaGenerator, key: str, item: ITEM_TYPE, options: InfoCompOptions
+        self,
+        st: "KiaraStreamlitAPI",
+        key: str,
+        item: ITEM_TYPE,
+        options: InfoCompOptions,
     ):
         pass
 
     def render_all_info(  # type: ignore
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         key: str,
         items: Mapping[str, ITEM_TYPE],
         options: InfoCompOptions,
     ) -> Union[None, ITEM_TYPE]:
 
         if options.columns is None:
             left, right = st.columns((1, 4))
         elif isinstance(options.columns[0], int):
             left, right = st.columns(options.columns)
         else:
             left, right = options.columns
 
         info_type_name = self.__class__.get_info_type().__name__.lower()
 
+        _key = options.create_key(*items.keys(), key, info_type_name, "list")
+
         selected_op = create_list_component(
             st=left,
             title=info_type_name.capitalize(),
             items=list(items.keys()),
-            key=f"{key}_{info_type_name}_list",
+            key=_key,
             height=options.height,
         )
 
         if selected_op:
             item = items[selected_op]
 
             self.render_info(
-                st=right,
+                st=right,  # type: ignore
                 key=f"{key}__{info_type_name}_{selected_op}",
                 item=item,
                 options=options,
             )
             return item
         else:
             return None
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/api.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 # -*- coding: utf-8 -*-
-from typing import ClassVar, Mapping, Type, Union
+from typing import TYPE_CHECKING, ClassVar, Mapping, Type, Union
+
+from pydantic import Field
 
 from kiara.interfaces.python_api import OperationInfo
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.info import InfoCompOptions, KiaraInfoComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 # class KiaraApiHelpCompOptions(ComponentOptions):
 #     class Config:
 #         arbitrary_types_allowed = True
 #
 #     columns: Union[Tuple[int, int], Tuple[DeltaGenerator, DeltaGenerator]] = Field(
 #         description="The column layout to use for the next step.", default=(1, 4)
@@ -18,15 +22,15 @@
 #     )
 #
 #
 # class KiaraApiHelpComponent(KiaraComponent[KiaraApiHelpCompOptions]):
 #
 #     _component_name = "kiara_api_help"
 #
-#     def _render(self, st: DeltaGenerator, options: KiaraApiHelpCompOptions):
+#     def _render(self, st: KiaraStreamlitAPI, options: KiaraApiHelpCompOptions):
 #
 #         doc = self.api.doc
 #         left, right = options.columns
 #         if isinstance(left, int):
 #             left, right = st.columns(options.columns)  # type: ignore
 #
 #         _key = options.create_key("api_command_selection")
@@ -79,15 +83,15 @@
         return self.api.retrieve_operations_info().item_infos
 
     def get_info_item(self, item_id: str) -> OperationInfo:
 
         return self.api.retrieve_operation_info(operation=item_id)
 
     def render_info(  # type: ignore
-        self, st: DeltaGenerator, key: str, item: OperationInfo, options: InfoCompOptions  # type: ignore
+        self, st: "KiaraStreamlitAPI", key: str, item: OperationInfo, options: InfoCompOptions  # type: ignore
     ):
         st.markdown(f"#### Operation: `{item.operation.operation_id}`")
         st.markdown(item.documentation.full_doc)
 
         comp = self.get_component("fields_info")
         st.markdown("##### Inputs")
         # opts = FieldsInfoOptions(
@@ -111,53 +115,63 @@
 #     _component_name = "module_type_info"
 #
 #     @classmethod
 #     def get_info_type(cls) -> str:
 #         return "module_type"
 #
 #     def render_info(  # type: ignore
-#         self, st: DeltaGenerator, key: str, item: ModuleTypeInfo, options: InfoCompOptions  # type: ignore
+#         self, st: KiaraStreamlitAPI, key: str, item: ModuleTypeInfo, options: InfoCompOptions  # type: ignore
 #     ):
 #         st.write(item)
 #
 #
 # class KiaraDataTypeInfoComponent(KiaraInfoComponent):
 #
 #     _component_name = "data_type_info"
 #
 #     @classmethod
 #     def get_info_type(cls) -> str:
 #         return "data_type"
 #
 #     def render_info(  # type: ignore
-#         self, st: DeltaGenerator, key: str, item: DataTypeClassInfo, options: InfoCompOptions  # type: ignore
+#         self, st: KiaraStreamlitAPI, key: str, item: DataTypeClassInfo, options: InfoCompOptions  # type: ignore
 #     ):
 #         st.write(item)
 
 
 class OperationDocsOptions(ComponentOptions):
-    pass
+    height: Union[int, None] = Field(
+        description="The height of the list component.", default=400
+    )
 
 
 class OperationDocs(KiaraComponent):
     """Displays documentation for all available operations."""
 
     _component_name = "operation_documentation"
     _options = OperationDocsOptions
 
-    def _render(self, st: DeltaGenerator, options: OperationDocsOptions):
+    _examples: ClassVar = [
+        {
+            "doc": "Display operations doc.",
+        },
+    ]
+
+    def _render(self, st: "KiaraStreamlitAPI", options: OperationDocsOptions):
 
         left, right = st.columns([1, 3])
 
         tab_names = ["Overview", "Demo"]
         overview, demo = right.tabs(tab_names)
 
         op_info = self.get_component("operation_info")
         selected: Union[OperationInfo, None] = op_info.render_func(st)(
-            key=options.create_key("ops_info"), columns=(left, overview), height=500
+            key=options.create_key("ops_info"),
+            columns=(left, overview),
+            height=options.height,
         )
 
         if not selected:
             demo.markdown("No operation selected.")
         else:
             code = """import streamlit as st
 import kiara_plugin.streamlit as kst
@@ -165,12 +179,12 @@
 
 result = st.kiara.process_operation("{}")
 """.format(
                 selected.operation.operation_id
             )
 
             demo.code(code)
-            comp = self.get_component("process_operation")
+            comp = self.get_component("operation_process_panel")
             comp.render_func(demo)(
                 key=options.create_key("demo"),
                 operation_id=selected.operation.operation_id,
             )
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/info/components.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/info/components.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
-from typing import Any, Dict, List, Mapping, Type
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, Type
 
 from kiara.api import Value, ValueMap
 from kiara.models.documentation import DocumentationMetadataModel
 from kiara_plugin.streamlit.components import ComponentInfo, ComponentsInfo
 from kiara_plugin.streamlit.components.info import InfoCompOptions, KiaraInfoComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class KiaraComponentInfoComponent(KiaraInfoComponent[ComponentInfo]):
     """Display information about a kiara streamlit component.
 
     This is used to create what you see here.
     """
@@ -51,105 +53,170 @@
 
         comp = self.kiara_streamlit.get_component(item_id)
         return ComponentInfo.create_from_instance(
             kiara=self.kiara_streamlit.api.context, instance=comp
         )
 
     def render_info(  # type: ignore
-        self, st: DeltaGenerator, key: str, item: ComponentInfo, options: InfoCompOptions  # type: ignore
+        self, st: "KiaraStreamlitAPI", key: str, item: ComponentInfo, options: InfoCompOptions  # type: ignore
     ):
         st.markdown(f"#### Component: `{item.type_name}`")
-        st.markdown(item.documentation.full_doc)
-
-        st.markdown("##### Component code")
-
-        with st.expander(f"Class: `{item.python_class.python_class_name}`"):
-            st.write(item.python_class.dict())
 
-        comp = self.get_component("fields_info")
-        st.markdown("##### Arguments")
-        arg_table: Dict[str, List[Any]] = {
-            "field": [],
-            "type": [],
-            "required": [],
-            "default": [],
-            "description": [],
-        }
-        for arg_name in item.arguments.keys():
-            arg = item.arguments[arg_name]
-            arg_table["field"].append(arg_name)
-            arg_table["type"].append(arg.python_type)
-            arg_table["required"].append("yes" if arg.required else "no")
-            arg_table["default"].append("" if arg.default is None else str(arg.default))
-            arg_table["description"].append(arg.description)
-
-        st.table(arg_table)
-
-        st.markdown("##### Usage")
-        code = """import streamlit as st
-import kiara_plugin.streamlit as kst
-kst.init()
+        if item.examples:
+            details_tab, examples_tab = st.tabs(["Details", "Examples"])
+        else:
+            tabs = st.tabs(["Details"])  # type: ignore
+            # no idea, bug in streamlit?
+            details_tab = tabs[0]
+
+        with details_tab:
+            details_tab.markdown(item.documentation.full_doc)
+
+            expander = details_tab.expander("Component details", expanded=False)
+
+            pkg_name = item.context.labels.get("package", "-- n/a --")
+            table_md = f"""
+            | attribute | value |
+            | --------- | ----- |
+            | Python class      | `{item.python_class.full_name}` |
+            | Plugin            | `{pkg_name}` |
+            """
+            expander.markdown(table_md)
+            expander.write("---")
+            expander.write("##### Source code")
+            expander.code(item.python_class.get_source_code())
+
+            # comp = self.get_component("fields_info")
+            details_tab.markdown("##### Arguments")
+            arg_table: Dict[str, List[Any]] = {
+                "field": [],
+                "type": [],
+                "required": [],
+                "default": [],
+                "description": [],
+            }
+
+            is_type_specific_select_comp = (
+                item.python_class.full_name
+                == "kiara_plugin.streamlit.components.input.DefaultInputComponent"
+                and item.type_name != "select_value"
+            )
+
+            for arg_name in item.arguments.keys():
+
+                # better hide this argument, otherwise it might be confusing
+                if is_type_specific_select_comp and arg_name in [
+                    "value_schema",
+                    "data_type",
+                ]:
+                    continue
+
+                arg = item.arguments[arg_name]
+                arg_table["field"].append(arg_name)
+                arg_table["type"].append(arg.python_type_string)
+                arg_table["required"].append("yes" if arg.required else "no")
+                arg_table["default"].append(
+                    "" if arg.default is None else str(arg.default)
+                )
+                arg_table["description"].append(arg.description)
+
+            hide_table_row_index = """
+                        <style>
+                        thead tr th:first-child {display:none}
+                        tbody th {display:none}
+                        </style>
+                        """
+            # Inject CSS with Markdown
+            details_tab.markdown(hide_table_row_index, unsafe_allow_html=True)
+            details_tab.table(arg_table)
+
+            details_tab.markdown("##### Usage")
+            code = """from kiara_plugin.streamlit import kiara_streamlit_init
+st = kiara_streamlit_init
 
 result = st.kiara.{}({})
-        """.format(
-            item.type_name, "<options>"
-        )
-        st.code(code)
+            """.format(
+                item.type_name, "<options>"
+            )
+            details_tab.code(code)
 
         if item.examples:
-            st.markdown("##### Examples")
-            comp = self.get_component(item.type_name)
-            for idx, example in enumerate(item.examples, start=1):
-                doc = example.get("doc", None)
-                if doc:
-                    d = DocumentationMetadataModel.create(doc)
-                    title = f"**Example**: *{d.description}*"
-                    txt = d.doc
-                else:
-                    title = f"**Example** *#{idx}*"
-                    txt = None
-
-                with st.expander(title, expanded=idx == 1):
-
-                    if txt:
-                        self._st.markdown(txt)
-
-                    _options = []
-                    example_args = example.get("args", {})
-                    for arg_name in item.arguments.keys():
-                        if arg_name in example_args.keys():
-                            v = example_args[arg_name]
-                            if isinstance(v, str):
-                                v = f'"{v}"'
-                            else:
-                                v = str(v)
-                            _options.append(f"{arg_name}={v}")
-
-                    arg_str = ", ".join(_options)
-
-                    code = """result = st.kiara.{}({})
-        """.format(
-                        item.type_name, arg_str
-                    )
-                    self._st.code(code)
-
-                    with self._st.expander("***Rendered component***", expanded=True):
-
-                        try:
-                            result = comp.render_func(self._st)(
-                                **example.get("args", {})
-                            )
-                        except Exception as e:
-                            st.error(e)
-                            result = None
-                        if result:
-                            if isinstance(result, Value):
-                                with self._st.expander("*result*"):
-                                    self.kiara_streamlit.preview(result)
-                            elif isinstance(result, ValueMap):
-                                with self._st.expander("*result*"):
-                                    self.kiara_streamlit.value_map_preview(
-                                        value_map=dict(result)
-                                    )
-                            else:
-                                with self._st.expander("*result*"):
-                                    self._st.markdown(f"***Result***: {result}")
+            with examples_tab:
+                examples_tab.markdown("##### Examples")
+                comp = self.get_component(item.type_name)
+                for idx, example in enumerate(item.examples, start=1):
+                    doc = example.get("doc", None)
+                    if len(item.examples) > 1:
+                        idx_str = f" #{idx}"
+                    else:
+                        idx_str = ""
+                    if doc:
+                        d = DocumentationMetadataModel.create(doc)
+                        title = f"**Example{idx_str}**: *{d.description}*"
+                        txt = d.doc
+                    else:
+                        title = f"**Example{idx_str}** *#{idx}*"
+                        txt = None
+
+                    with examples_tab.expander(title, expanded=idx == 1):
+
+                        if txt:
+                            self._st.markdown(txt)
+
+                        _options = []
+                        example_args = example.get("args", {})
+                        for arg_name in item.arguments.keys():
+                            if arg_name in example_args.keys():
+                                v = example_args[arg_name]
+                                if isinstance(v, str):
+                                    v = f'"{v}"'
+                                else:
+                                    v = str(v)
+                                _options.append(f"{arg_name}={v}")
+
+                        arg_str = ", ".join(_options)
+
+                        code = """from kiara_plugin.streamlit import kiara_streamlit_init
+st = kiara_streamlit_init
+
+result = st.kiara.{}({})
+            """.format(
+                            item.type_name, arg_str
+                        )
+                        self._st.code(code)
+
+                        with self._st.expander(
+                            "***Rendered component***", expanded=True
+                        ):
+
+                            try:
+                                result = comp.render_func(self._st)(
+                                    **example.get("args", {})
+                                )
+                            except Exception as e:
+                                self._st.error(e)
+                                result = None
+                            if result:
+                                title = "**Component result (not rendered)**"
+                                if isinstance(result, Value):
+                                    with self._st.expander(title):
+                                        self._st.markdown(
+                                            "Result type: [`Value`](https://dharpa.org/kiara/latest/reference/kiara/models/values/value/#kiara.models.values.value.Value)"
+                                        )
+                                        self.kiara_streamlit.preview(
+                                            result, key=f"{key}_example_result_{idx}"
+                                        )
+                                elif isinstance(result, ValueMap):
+                                    with self._st.expander(title):
+                                        self._st.markdown(
+                                            "Result type: [`ValueMap`](https://dharpa.org/kiara/latest/reference/kiara/models/values/value/#kiara.models.values.value.ValueMap)"
+                                        )
+                                        self.kiara_streamlit.value_map_preview(
+                                            value_map=dict(result),
+                                            key=f"{key}_example_result_map_{idx}",
+                                        )
+                                else:
+                                    with self._st.expander(title):
+                                        self._st.markdown(
+                                            f"Result type: Python instace of type ``{type(result)}`'"
+                                        )
+                                        self._st.write(result)
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,285 +1,300 @@
 # -*- coding: utf-8 -*-
-import abc
-import copy
 import uuid
-from typing import TYPE_CHECKING, Any, Callable, Iterable, List, Tuple, TypeVar, Union
+from abc import abstractmethod
+from typing import TYPE_CHECKING, List, Mapping, Union
 
 from pydantic import Field
 
-from kiara.api import Value, ValueSchema
-from kiara.defaults import SpecialValue
-from kiara.registries.data import ValueLink
+from kiara.api import Value, ValueMap
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
-from kiara_plugin.streamlit.defaults import NO_LABEL_MARKER, NO_VALUE_MARKER
-from streamlit.delta_generator import DeltaGenerator
+from kiara_plugin.streamlit.components.models import (
+    create_recursive_table_from_model_object,
+)
+from kiara_plugin.streamlit.utils.components import create_list_component
 
 if TYPE_CHECKING:
-    from kiara_plugin.streamlit.streamlit import KiaraStreamlit
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
-class InputOptions(ComponentOptions):
+class PreviewOptions(ComponentOptions):
 
-    display_style: str = Field(
-        description="The display style to use for this input field.", default="default"
-    )
-    smart_label: bool = Field(
-        description="Whether to try to shorten the label.", default=True
-    )
-    label: str = Field(
-        description="The label to use for the input field.", default=NO_LABEL_MARKER
+    show_properties: bool = Field(
+        description="Whether to show the properties of the value.", default=True
     )
-    help: Union[str, None] = Field(
-        description="The help to display for this input field."
+    height: Union[int, None] = Field(
+        description="The height of the preview.", default=None
     )
-    value_schema: Union[None, ValueSchema] = Field(
-        description="The schema for the value in question."
+    display_style: str = Field(
+        description="The display style to use for this preview.", default="default"
     )
-
-    def get_default(self) -> Any:
-        if self.value_schema is None:
-            return None
-        return copy.deepcopy(self.value_schema.default)
-
-
-INPUT_OPTIONS_TYPE = TypeVar("INPUT_OPTIONS_TYPE", bound=InputOptions)
+    value: Union[str, uuid.UUID, Value] = Field(description="The value to preview.")
 
 
-class InputComponent(KiaraComponent[INPUT_OPTIONS_TYPE]):
+class PreviewComponent(KiaraComponent[PreviewOptions]):
 
-    _options = InputOptions  # type: ignore
+    _options = PreviewOptions  # type: ignore
 
     @classmethod
-    @abc.abstractmethod
+    @abstractmethod
     def get_data_type(cls) -> str:
         pass
 
     @classmethod
-    def get_input_profile(cls) -> str:
+    def get_preview_name(cls) -> str:
         return "default"
 
-    @classmethod
-    def get_default_label(cls) -> str:
-        if cls.get_data_type() == "any":
-            return "Select value"
-        else:
-            return f"Select {cls.get_data_type()} value"
-
-    @abc.abstractmethod
-    def render_input_field(
-        self,
-        st: DeltaGenerator,
-        options: INPUT_OPTIONS_TYPE,
-    ) -> Union[ValueLink, None, str, uuid.UUID]:
+    @abstractmethod
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions):
         pass
 
     def _render(
-        self, st: DeltaGenerator, options: INPUT_OPTIONS_TYPE
-    ) -> Union[Value, None]:
+        self,
+        st: "KiaraStreamlitAPI",
+        options: PreviewOptions,
+    ):
 
-        if options.label == NO_LABEL_MARKER:
-            options.label = self.get_default_label()
+        self.render_preview(st=st, options=options)
 
-        value = self.render_input_field(st, options=options)
-        if not value:
-            return None
-        else:
-            return self.api.get_value(value)  # type: ignore
 
-    def _create_session_store_callback(
-        self, options: ComponentOptions, *key, default=None
-    ) -> Tuple[Callable, str]:
+class PropertiesViewOptions(ComponentOptions):
+    """Options for the properties view component."""
 
-        _widget_key = options.create_key(*key)
+    value: Union[str, uuid.UUID, Value] = Field(description="The value to preview.")
 
-        current = self.get_session_var(options, *key, default=default)
 
-        if current is not None and _widget_key not in self._session_state:
-            self._session_state[_widget_key] = current
+class PropertiesViewComponent(KiaraComponent[PropertiesViewOptions]):
+    """Display the properties of a value."""
 
-        def callback():
-            self._st.session_state[
-                options.get_session_key(*key)
-            ] = self._st.session_state[_widget_key]
+    _component_name = "display_value_properties"
+    _options = PropertiesViewOptions
 
-        return callback, _widget_key
+    def _render(self, st: "KiaraStreamlitAPI", options: PropertiesViewOptions):
 
+        value = self.api.get_value(value=options.value)
 
-class DefaultInputOptions(InputOptions):
+        for prop_name, prop_value in value.property_values.items():
+            _prop_name = prop_name.replace("metadata.", "")
+            st.write(f"Metadata item: **{_prop_name}**")
 
-    value_has_alias: bool = Field(
-        description="Whether the values to present need to have a registered alias.",
-        default=True,
-    )
-    preview: str = Field(
-        description="The preview to use for the value.", default="auto"
-    )
-    display_value_type: Union[bool, None] = Field(
-        description="Whether to display the data type in the list.", default=None
-    )
-    data_type: Union[str, List[str], None] = Field(
-        description="The data type(s) to display as selection.", default=None
-    )
+            table_data = create_recursive_table_from_model_object(prop_value.data)
+            name_col, val_col = st.columns([1, 3])
 
+            for key, value in table_data.items():
 
-class DefaultInputComponent(InputComponent):
-    """Render a selectbox with all available values (for a specific type, if applicable)."""
+                with name_col:
+                    name_col.write(key)
 
-    _component_name = "value_input"
-    _options = DefaultInputOptions  # type: ignore
+                with val_col:
+                    if isinstance(value, (Mapping, List)):
+                        val_col.json(value, expanded=False)
+                    else:
+                        val_col.write(value)
 
-    def __init__(
-        self,
-        kiara_streamlit: "KiaraStreamlit",
-        component_name: str,
-        data_types: Union[str, Iterable[str], None] = None,
-        doc: Any = None,
-    ):
 
-        if data_types:
-            if isinstance(data_types, str):
-                data_types = [data_types]
-
-        self._data_types: Union[None, Iterable[str]] = data_types
-        super().__init__(
-            kiara_streamlit=kiara_streamlit, component_name=component_name, doc=doc
-        )
+class DefaultPreviewComponent(PreviewComponent):
+    """The default preview component, will render a preview component dependent on the data type of the provided value."""
+
+    _component_name = "preview"
+    _examples = [
+        {"doc": "Preview a table value.", "args": {"value": "nodes_table"}},
+    ]
 
     @classmethod
     def get_data_type(cls) -> str:
         return "any"
 
-    def render_input_field(
+    def render_preview(
         self,
-        st: DeltaGenerator,
-        options: DefaultInputOptions,
-    ) -> Union[ValueLink, None, str, uuid.UUID]:
-
-        if options.smart_label:
-            options.label = options.label.split("__")[-1]
-
-        if options.data_type is None:
-            data_types: List[str] = []
-        elif isinstance(options.data_type, str):
-            data_types = [options.data_type]
-        else:
-            data_types = options.data_type
+        st: "KiaraStreamlitAPI",
+        options: PreviewOptions,
+    ):
 
-        if self._data_types and data_types:
-            raise Exception("'data_types' argument not allowed for this component.")
+        preview_name = options.display_style
+        height = options.height
+        if not height:
+            height = 400
+
+        _value = self.api.get_value(options.value)
+        if not _value.is_set:
+            st.write("Value not set.")
+            return
 
-        if not data_types:
-            if self._data_types is None:
-                data_types = []
+        component = self._kiara_streamlit.get_preview_component(
+            data_type=_value.data_type_name, preview_name=preview_name
+        )
+        if component is not None:
+            component.render_func(st)(value=_value, key=options.create_key("preview"))
+        else:
+            if isinstance(options.value, Value):
+                name = str(_value.value_id)
             else:
-                data_types = list(self._data_types)
+                name = str(options.value)
+
+            renderable = self.api.render_value(
+                value=_value, target_format="string", use_pretty_print=True
+            )
+            st.text_area(
+                f"Value: {name}",
+                value=renderable,
+                disabled=True,
+                height=height,
+                key=options.create_key("preview", "default"),
+            )
+
+
+class PreviewListOptions(ComponentOptions):
+
+    data_types: Union[str, List[str], None] = Field(
+        description="The data types to display.", default=None
+    )
+
+
+class ValueList(KiaraComponent[PreviewListOptions]):
 
-        if not data_types:
-            data_types.append(self.get_data_type())
+    _component_name = "value_list"
+    _options = PreviewListOptions
 
-        _key = options.create_key(*sorted(data_types))
+    def _render(
+        self, st: "KiaraStreamlitAPI", options: PreviewListOptions
+    ) -> Union[str, None]:
+
+        data_types = []
+        if options.data_types:
+            if isinstance(options.data_types, str):
+                data_types.append(options.data_types)
+            else:
+                data_types.extend(options.data_types)
 
-        if len(data_types) == 1:
-            dt = data_types[0]
-            inp_comp = self.kiara_streamlit.get_input_component(dt)
-            if inp_comp and inp_comp.__class__ != self.__class__:
-                copy_options = options.copy()
-                _key_selectbox = f"{_key}_value_select_{_key}"
-                copy_options.key = _key_selectbox
-                return inp_comp.render_input_field(st, options=copy_options)
-
-        has_alias = options.value_has_alias
-        available_values = self.api.list_aliases(
-            data_types=list(data_types), has_alias=has_alias
+        values = self.api.list_aliases(data_types=data_types)
+
+        _key = options.create_key("value_list")
+        selected_alias = create_list_component(
+            st=st, key=_key, title="Values", items=list(values.keys())
         )
 
-        optional = False
-        default = None
-        if options.value_schema:
-            if options.value_schema.default not in [
-                SpecialValue.NO_VALUE,
-                SpecialValue.NOT_SET,
-                None,
-            ]:
-                default = options.value_schema.default
-            optional = options.value_schema.optional
-
-        display_type = options.display_value_type
-        if display_type is None and data_types != 1:
-            display_type = True
-        elif display_type is None:
-            display_type = False
-
-        format_func: Callable = str
-        if display_type:
-
-            def format_func(v: Any) -> str:
-                if v == NO_VALUE_MARKER:
-                    return v
-                return f"{v} ({available_values[v].data_type_name})"
-
-        if optional:
-            _item_options = [NO_VALUE_MARKER, *available_values.keys()]
-            if not default:
-                default = NO_VALUE_MARKER
-        else:
-            _item_options = list(available_values.keys())
+        return selected_alias
 
-        with_preview = options.preview
 
-        if with_preview == "auto":
-            with_preview = "checkbox"
+class ValueListPreview(KiaraComponent[PreviewListOptions]):
 
-        callback, _select_key = self._create_session_store_callback(
-            options, "input", "value", "select", default=default
+    _component_name = "value_list_preview"
+    _options = PreviewListOptions
+
+    def _render(
+        self,
+        st: "KiaraStreamlitAPI",
+        options: PreviewListOptions,
+    ) -> Union[str, None]:
+        ratio_preview: int = 3
+        data_list_column, preview_column = st.columns([1, ratio_preview])
+
+        _key = options.create_key("data_list")
+
+        comp = self.get_component("value_list")
+        selected_alias = comp.render_func(data_list_column)(
+            key=_key, data_types=options.data_types
         )
 
-        if not with_preview or with_preview.lower() in ["false", "no"]:
-            result = st.selectbox(
-                label=options.label,
-                options=_item_options,
-                key=_select_key,
-                format_func=format_func,
-                on_change=callback,
-                help=options.help,
-            )
+        if selected_alias:
+            value = self.api.get_value(selected_alias)
+            component = self.kiara_streamlit.get_preview_component(value.data_type_name)
+
+            if component is None:
+                component = self.kiara_streamlit.get_preview_component("any")
+
+            pr_opts = PreviewOptions(key=options.create_key("preview"), value=value)
+            component.render_preview(preview_column, options=pr_opts)  # type: ignore
+
+        return selected_alias
+
+
+class ValueMapPreviewOptions(ComponentOptions):
+
+    add_value_types: bool = Field(
+        description="Whether to add the type of the value to the tab titles.",
+        default=True,
+    )
+    add_save_option: bool = Field(
+        description="Whether to add a save option for every value.", default=False
+    )
+    value_map: Mapping[str, Union[str, uuid.UUID, Value]] = Field(
+        description="The values to display."
+    )
+
+
+class ValueMapPreview(KiaraComponent[ValueMapPreviewOptions]):
+
+    _component_name = "value_map_preview"
+    _options = ValueMapPreviewOptions
+
+    def _render(
+        self,
+        st: "KiaraStreamlitAPI",
+        options: ValueMapPreviewOptions,
+    ) -> Union[ValueMap, None]:
+
+        if not options.value_map:
+            st.write("-- no values --")
+            return None
+
+        _values = self.api.assemble_value_map(options.value_map)
+
+        field_names = sorted(_values.keys())
+        if not options.add_value_types:
+            tab_names = field_names
         else:
-            result = st.selectbox(
-                label=options.label,
-                options=_item_options,
-                key=_select_key,
-                format_func=format_func,
-                on_change=callback,
-                help=options.help,
+            tab_names = sorted(
+                (f"{x} ({_values[x].data_type_name})" for x in _values.keys())
             )
-            if result == NO_VALUE_MARKER:
-                result = None
-            if with_preview == "checkbox":
-                if result:
-                    _key = options.create_key("preview", result)
-                else:
-                    _key = options.create_key("preview", "no_value")
-                if result is None:
-                    disabled = True
-                else:
-                    disabled = False
-                show_preview = st.checkbox(
-                    "Preview", key=f"preview_{_select_key}", disabled=disabled
+
+        tabs = st.tabs(tab_names)
+        for idx, field in enumerate(field_names):
+
+            value = _values[field]
+            if not value.is_set:
+                tabs[idx].markdown("-- value not set --")
+            else:
+                component = self.kiara_streamlit.get_preview_component(
+                    value.data_type_name
                 )
-                if show_preview:
-                    comp = self.get_component("preview")
-                    if hasattr(st, "__enter__"):
-                        with st:
-                            comp.render_func(st)(key=_key, value=result)
-                    else:
-                        comp.render_func(st)(key=_key, value=result)
-            elif with_preview:
-                if result is not None:
-                    _key = options.create_key("preview", result)
-                    comp = self.get_component("preview")
-                    if hasattr(st, "__enter__"):
-                        with st:
-                            comp.render_func(st)(key=_key, value=result)
-                    else:
-                        comp.render_func(st)(key=_key, value=result)
+                if component is None:
+                    component = self.kiara_streamlit.get_preview_component("any")
+
+                if options.add_save_option:
+                    center, right = tabs[idx].columns([4, 1])
+                else:
+                    center = tabs[idx]
+                    right = None
+
+                _key = options.create_key("preview", f"{idx}_{field}")
+                preview_opts = PreviewOptions(key=_key, value=value)
+                component.render_preview(st=center, options=preview_opts)  # type: ignore
+
+                if options.add_save_option:
+                    assert right is not None
+                    right.write("Save value")
+                    with right.form(
+                        key=options.create_key("save_form", f"{idx}_{field}")
+                    ):
+                        _key = options.create_key("alias", f"{idx}_{field}")
+                        alias = self._st.text_input(
+                            "alias",
+                            value="",
+                            key=_key,
+                            placeholder="alias",
+                            label_visibility="hidden",
+                        )
+                        # _key = options.create_key("save", f"{idx}_{field}")
+                        save = self._st.form_submit_button("Save")
+
+                    if save and alias:
+                        store_result = self.api.store_value(
+                            value=value, alias=alias, allow_overwrite=False
+                        )
+                        if store_result.error:
+                            right.error(store_result.error)
+                        else:
+                            right.success("Value saved")
+                            st.experimental_rerun()
 
-        return result
+        return _values
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/assemblies.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/assemblies.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 # -*- coding: utf-8 -*-
 import abc
 import uuid
-from typing import Dict, Mapping, TypeVar, Union
+from typing import TYPE_CHECKING, Any, Dict, List, Mapping, TypeVar, Union
 
 from pydantic import Field
 
 from kiara.api import ValueMap, ValueSchema
 from kiara.registries.data import ValueLink
 from kiara.utils.values import construct_valuemap
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.input import DefaultInputOptions, InputComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class AssemblyOptions(ComponentOptions):
 
     max_columns: int = Field(
         description="The maximum number of columns to use for the assembly.", default=3
     )
     profile: str = Field(
         description="The name of the profile that renders the assembly. Available: 'default' and 'all'",
         default="default",
     )
     smart_label: bool = Field(
         description="Whether to try to shorten the label.", default=True
     )
+    constants: Dict[str, Any] = Field(
+        description="Constants, no input fields will be rendered for them, and they will be included in the result.",
+        default_factory=dict,
+    )
 
 
 ASSEMBLY_OPTIONS_TYPE = TypeVar("ASSEMBLY_OPTIONS_TYPE", bound=AssemblyOptions)
 
 
 class InputAssemblyComponent(KiaraComponent[ASSEMBLY_OPTIONS_TYPE]):
 
@@ -36,32 +42,48 @@
 
     @abc.abstractmethod
     def get_input_fields(
         self, options: ASSEMBLY_OPTIONS_TYPE
     ) -> Mapping[str, ValueSchema]:
         pass
 
-    def _render(self, st: DeltaGenerator, options: ASSEMBLY_OPTIONS_TYPE) -> ValueMap:
+    def _render(
+        self, st: "KiaraStreamlitAPI", options: ASSEMBLY_OPTIONS_TYPE
+    ) -> ValueMap:
 
         profile = options.profile
 
         method_name = f"render_{profile}"
         if not hasattr(self, method_name):
             raise Exception(f"No input fields render profile '{profile}' available.'")
 
-        fields = self.get_input_fields(options=options)
+        fields: Mapping[str, Any] = self.get_input_fields(options=options)
+
+        if options.constants:
+            _fields_input = {}
+            for k, v in fields.items():
+                if k in options.constants.keys():
+                    continue
+                _fields_input[k] = v
+            fields_input: Mapping[str, Any] = _fields_input
+        else:
+            fields_input = fields
+
         func = getattr(self, method_name)
-        result = func(st, fields, options=options)
+        result = func(st, fields_input, options=options)
+
+        if options.constants:
+            result.update(options.constants)
 
         value_map = self.api.assemble_value_map(result, values_schema=fields)
         return value_map
 
     def render_all(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         fields: Mapping[str, ValueSchema],
         options: ASSEMBLY_OPTIONS_TYPE,
     ) -> Mapping[str, Union[str, uuid.UUID, ValueLink, None]]:
 
         max_columns = options.max_columns
 
         if not fields:
@@ -91,23 +113,23 @@
             input_opts = DefaultInputOptions(
                 key=_key,
                 label=field_name,
                 value_schema=schema,
                 help=help,
                 smart_label=options.smart_label,
             )
-            r = comp.render_input_field(columns[column_idx], input_opts)
+            r = comp.render_input_field(columns[column_idx], input_opts)  # type: ignore
 
             values[field_name] = r
 
         return values
 
     def render_default(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         fields: Mapping[str, ValueSchema],
         options: AssemblyOptions,
     ) -> Mapping[str, Union[str, None, uuid.UUID, ValueLink]]:
 
         required: Dict[str, ValueSchema] = {}
         optional: Dict[str, ValueSchema] = {}
         max_columns = options.max_columns
@@ -145,15 +167,15 @@
                     key=_key,
                     label=field_name,
                     value_schema=schema,
                     help=help,
                     smart_label=options.smart_label,
                 )
 
-                r = comp.render_input_field(columns[column_idx], input_opts)
+                r = comp.render_input_field(columns[column_idx], input_opts)  # type: ignore
 
                 values[field_name] = r
 
         if optional:
             opt_expander = st.expander("Optional inputs", expanded=optional_expanded)
 
             if not max_columns:
@@ -183,21 +205,28 @@
                     key=_key,
                     label=field_name,
                     value_schema=schema,
                     help=help,
                     smart_label=options.smart_label,
                 )
 
-                r = comp.render_input_field(opt_columns[column_idx], input_opts)
+                r = comp.render_input_field(opt_columns[column_idx], input_opts)  # type: ignore
                 values[field_name] = r
 
         return values
 
 
 class OperationInputsOptions(AssemblyOptions):
+
+    module_config: Union[Dict[str, Any], None] = Field(
+        description="Optional module config.", default=None
+    )
+    ignore_inputs: List[str] = Field(
+        description="Don't render input widgets for those fields.", default_factory=list
+    )
     operation_id: str = Field(
         description="The id of the operation to render the inputs for."
     )
 
 
 class OperationInputs(InputAssemblyComponent):
     """Render all inputs for a specifc operation."""
@@ -212,16 +241,28 @@
     ]
 
     def get_input_fields(
         self, options: OperationInputsOptions
     ) -> Mapping[str, ValueSchema]:
 
         # TODO: check argument
-        op = self.api.get_operation(options.operation_id)
-        return op.inputs_schema
+        data = {
+            "module_type": options.operation_id,
+            "module_config": options.module_config,
+        }
+        op = self.api.get_operation(data)
+
+        if not options.ignore_inputs:
+            return op.inputs_schema
+        else:
+            return {
+                k: v
+                for k, v in op.inputs_schema.items()
+                if k not in options.ignore_inputs
+            }
 
 
 class InputFieldsOptions(AssemblyOptions):
     fields: Mapping[str, ValueSchema] = Field(description="The fields to render.")
 
 
 class InputFields(InputAssemblyComponent):
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/container_types.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/container_types.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 # -*- coding: utf-8 -*-
+from typing import TYPE_CHECKING
+
 from streamlit_tags import st_tags
 
 from kiara_plugin.streamlit.components.input import InputComponent, InputOptions
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class ListInput(InputComponent):
     """Render a widget for input a list.
 
     Currently, only lists of strings are supported.
     """
@@ -22,15 +26,15 @@
 
     @classmethod
     def get_default_label(cls) -> str:
         return "Provide items"
 
     def render_input_field(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
         if options.smart_label:
             options.label = options.label.split("__")[-1]
 
         with st.container():
             items = st_tags(
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/input/scalars.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/input/scalars.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
 import abc
-from typing import Any
+from typing import TYPE_CHECKING, Any
 
 from kiara.defaults import SpecialValue
+from kiara.exceptions import KiaraException
 from kiara_plugin.streamlit.components.input import InputComponent, InputOptions
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class ScalarInput(InputComponent):
     @classmethod
     def get_default_label(cls) -> str:
         return "Provide value"
 
     def render_input_field(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
         if options.smart_label:
             options.label = options.label.split("__")[-1]
 
         scalar = self.render_scalar_input(st, options=options)
         if scalar is None:
@@ -27,15 +30,15 @@
             scalar, data_type=self.get_data_type(), reuse_existing=True
         )
         return value
 
     @abc.abstractmethod
     def render_scalar_input(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ) -> Any:
         pass
 
 
 class BooleanInput(ScalarInput):
     """Render a checkbox for a boolean input."""
@@ -51,30 +54,75 @@
 
     @classmethod
     def get_default_label(cls) -> str:
         return "Check enabled"
 
     def render_scalar_input(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
         default = options.get_default()
-        if default in [None, SpecialValue.NO_VALUE, SpecialValue.NOT_SET]:
-            default = False
-        else:
-            default = bool(default)
 
-        callback, _key = self._create_session_store_callback(
-            options, "input", "scalar", self.__class__.get_data_type(), default=default
-        )
+        if options.value_schema and options.value_schema.optional:
+            if default in [None, SpecialValue.NO_VALUE, SpecialValue.NOT_SET]:
+                default = None
+            else:
+                default = bool(default)
+
+            callback, _key = self._create_session_store_callback(
+                options,
+                "input",
+                "scalar",
+                "radio",
+                self.__class__.get_data_type(),
+                default=default,
+            )
 
-        inp = st.checkbox(
-            label=options.label, key=_key, help=options.help, on_change=callback
-        )
+            choices = ["auto", "true", "false"]
+            if default is None:
+                idx = 0
+            elif default:
+                idx = 1
+            else:
+                idx = 2
+
+            result = st.radio(
+                label=options.label,
+                options=choices,
+                index=idx,
+                key=_key,
+                help=options.help,
+                on_change=callback,
+                horizontal=True,
+            )
+            if result == "auto":
+                inp = None
+            elif result == "true":
+                inp = True
+            else:
+                inp = False
+        else:
+            if default in [None, SpecialValue.NO_VALUE, SpecialValue.NOT_SET]:
+                default = False
+            else:
+                default = bool(default)
+
+            callback, _key = self._create_session_store_callback(
+                options,
+                "input",
+                "scalar",
+                "checkbox",
+                self.__class__.get_data_type(),
+                default=default,
+            )
+
+            inp = st.checkbox(
+                label=options.label, key=_key, help=options.help, on_change=callback
+            )
         return inp
 
 
 class StringInput(ScalarInput):
     """Render a text input widget."""
 
     _component_name = "input_string"
@@ -88,15 +136,15 @@
 
     @classmethod
     def get_default_label(cls) -> str:
         return "Enter text"
 
     def render_scalar_input(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
 
         default = options.get_default()
         if default in [None, SpecialValue.NOT_SET, SpecialValue.NO_VALUE]:
             default = ""
 
@@ -133,15 +181,15 @@
 
     @classmethod
     def get_default_label(cls) -> str:
         return "Enter integer"
 
     def render_scalar_input(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
 
         default = options.get_default()
         if default in [None, SpecialValue.NOT_SET, SpecialValue.NO_VALUE]:
             default = int(0)
         else:
@@ -170,18 +218,20 @@
         elif style == "text_input":
             number_str = st.text_input(
                 label=options.label,
                 key=f"{_key}__text_input",
                 on_change=callback,
                 help=options.help,
             )
+            if not number_str:
+                return None
             try:
                 number = int(number_str)
             except Exception:
-                number = None
+                raise KiaraException(f"Can't parse input as integer: {number_str}.")
         else:
             raise Exception(f"Invalid style argument: {style}.")
 
         return number
 
 
 class FloatInput(ScalarInput):
@@ -207,15 +257,15 @@
 
     @classmethod
     def get_default_label(cls) -> str:
         return "Enter float"
 
     def render_scalar_input(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: InputOptions,
     ):
 
         default = options.get_default()
         if default in [None, SpecialValue.NOT_SET, SpecialValue.NO_VALUE]:
             default = 0.0
         else:
@@ -231,27 +281,29 @@
         callback, _key = self._create_session_store_callback(
             options, "input", "scalar", self.__class__.get_data_type(), default=default
         )
 
         if style == "default":
             number = st.number_input(
                 label=options.label,
-                key=_key,
+                key=f"{_key}_number_input",
                 on_change=callback,
                 help=options.help,
                 step=1.0,
             )
         elif style == "text_input":
             number_str = st.text_input(
                 label=options.label,
-                key=_key,
+                key=f"{_key}_text_field",
                 on_change=callback,
                 help=options.help,
             )
+            if not number_str:
+                return None
             try:
                 number = float(number_str)
             except Exception:
-                number = None
+                raise KiaraException(f"Can't parse input as float: {number_str}")
         else:
             raise Exception(f"Invalid style argument: {style}.")
 
         return number
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/pipelines/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/pipelines/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 # -*- coding: utf-8 -*-
-from typing import List, Literal, Union
+from typing import TYPE_CHECKING, List, Literal, Union
 
 import networkx as nx
 from pydantic import Field
 
 from kiara.interfaces.python_api import OperationInfo
 from kiara.models.module.operation import Operation
 from kiara.models.module.pipeline import PipelineConfig
 from kiara.models.module.pipeline.pipeline import Pipeline
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class PipelineSelectOptions(ComponentOptions):
     filters: List[str] = Field(
         description="Filter tokens that must be present in the pipeline/operation name.",
         default_factory=list,
     )
@@ -21,15 +23,15 @@
 
 class PipelineSelect(KiaraComponent[PipelineSelectOptions]):
 
     _component_name = "select_pipeline"
     _options = PipelineSelectOptions
 
     def _render(
-        self, st: DeltaGenerator, options: PipelineSelectOptions
+        self, st: "KiaraStreamlitAPI", options: PipelineSelectOptions
     ) -> Union[None, OperationInfo]:
 
         pipeline_infos = self.api.retrieve_operations_info(
             *options.filters, operation_types=["pipeline"]
         )
 
         op_ids = list(pipeline_infos.item_infos.keys())
@@ -63,15 +65,15 @@
             "args": {
                 "pipeline": "logic.xor",
                 "graph_type": "execution",
             },
         }
     ]
 
-    def _render(self, st: DeltaGenerator, options: PipelineGraphOptions) -> None:
+    def _render(self, st: "KiaraStreamlitAPI", options: PipelineGraphOptions) -> None:
 
         if isinstance(options.pipeline, str):
             op: Operation = self.api.get_operation(options.pipeline)
             structure = op.pipeline_config.structure
         elif isinstance(options.pipeline, OperationInfo):
             structure = options.pipeline.operation.pipeline_config.structure
         elif isinstance(options.pipeline, Operation):
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/assemblies.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/assemblies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 # -*- coding: utf-8 -*-
-from typing import Mapping
+from typing import TYPE_CHECKING, Mapping
 
 from pydantic import Field
 
 from kiara.api import ValueSchema
 from kiara.utils.output import create_dict_from_field_schemas
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class FieldsInfoOptions(ComponentOptions):
 
     fields: Mapping[str, ValueSchema] = Field(
         description="The fields and their schema."
     )
@@ -36,15 +38,15 @@
                     },
                     "number_field": {"type": "integer", "doc": "A number."},
                 }
             },
         }
     ]
 
-    def _render(self, st: DeltaGenerator, options: FieldsInfoOptions):
+    def _render(self, st: "KiaraStreamlitAPI", options: FieldsInfoOptions):
 
         import pandas as pd
 
         fields = options.fields
         fields_data = create_dict_from_field_schemas(fields)
         dataframe = pd.DataFrame(fields_data, columns=list(fields_data.keys()))
         dataframe.set_index("field_name", inplace=True)  # noqa
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/core_types.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/preview/core_types.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,33 @@
 # -*- coding: utf-8 -*-
-from typing import Any, Dict
+from typing import TYPE_CHECKING, Any, Dict
+
+import humanfriendly
+import streamlit_scrollable_textbox as stx
 
 from kiara.models.data_types import KiaraDict
 from kiara.models.filesystem import KiaraFile, KiaraFileBundle
 from kiara.utils.json import orjson_dumps
 from kiara_plugin.core_types.models import KiaraList
 from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class DictPreview(PreviewComponent):
     """Preview a value of type 'dict'."""
 
     _component_name = "preview_dict"
 
     @classmethod
     def get_data_type(cls) -> str:
         return "dict"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         dict_data: KiaraDict = _value.data
 
         data, schema = st.tabs(["Data", "Schema"])
 
         try:
@@ -43,15 +48,15 @@
 
     _component_name = "preview_list"
 
     @classmethod
     def get_data_type(cls) -> str:
         return "list"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         list_data: KiaraList = _value.data
 
         data, schema = st.tabs(["Data", "Schema"])
 
         try:
@@ -72,66 +77,93 @@
 
     _component_name = "preview_file_bundle"
 
     @classmethod
     def get_data_type(cls) -> str:
         return "file_bundle"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         bundle: KiaraFileBundle = _value.data
 
         table: Dict[str, Any] = {}
         for file_path, file_info in bundle.included_files.items():
             table.setdefault("path", []).append(file_path)
             table.setdefault("size", []).append(file_info.size)
             table.setdefault("mime-type", []).append(file_info.mime_type)
 
-        st.dataframe(table, use_container_width=True)
+        st.dataframe(table, use_container_width=True, hide_index=True)
 
 
 class FilePreview(PreviewComponent):
     """Preview a value of type 'file'."""
 
     _component_name = "preview_file"
+    _examples = [{"doc": "A file preview.", "args": {"value": "nodes_file"}}]
 
     @classmethod
     def get_data_type(cls) -> str:
         return "file"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         file_model: KiaraFile = _value.data
 
-        table: Dict[str, Any] = {"key": [], "value": []}
-        table["key"].append("path")
-        table["value"].append(file_model.path)
-        table["key"].append("size")
-        table["value"].append(file_model.size)
-        table["key"].append("mime-type")
-        table["value"].append(file_model.mime_type)
-        table["key"].append("content")
-        table["value"].append(file_model.read_text())
-        st.table(table)
+        _key = options.create_key("file", "preview", file_model.path)
 
+        if options.display_style == "default":
+            # TODO: check if binary file?
+            max_lines = 100
+            with open(file_model.path, "rt") as f:
+                if max_lines <= 0:
+                    content = f.read()
+                else:
+                    lines = []
+                    idx = 0
+                    while idx < max_lines:
+                        lines.append(f.readline())
+                        idx += 1
+
+                    if idx >= max_lines:
+                        lines.append("...\n")
+                        lines.append("...")
+                    content = "".join(lines)
+            stx.scrollableTextbox(content, height=150, fontFamily="monospace", key=_key)
+
+        elif options.display_style == "metadata":
+
+            table: Dict[str, Any] = {"key": [], "value": []}
+            table["key"].append("path")
+            table["value"].append(file_model.path)
+            table["key"].append("size")
+            table["value"].append(humanfriendly.format_size(file_model.size))
+            table["key"].append("mime-type")
+            table["value"].append(file_model.mime_type)
+            table["key"].append("content")
+            table["value"].append(file_model.read_text())
+            st.dataframe(table, hide_index=True)
+        else:
+            raise Exception(
+                f"Unknown display style for file preview: {options.display_style}"
+            )
         # st.table(table, use_container_width=True)
 
 
 class BooleanPreview(PreviewComponent):
     """Preview a value of type 'boolean'."""
 
     _component_name = "preview_boolean"
 
     @classmethod
     def get_data_type(self) -> str:
         return "boolean"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         if _value.data is True:
             st.write("true")
         else:
             st.write("false")
 
@@ -141,15 +173,15 @@
 
     _component_name = "preview_string"
 
     @classmethod
     def get_data_type(self) -> str:
         return "string"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         text = _value.data
         st.text_area(
             label="The string content",
             value=text,
             disabled=True,
@@ -162,15 +194,15 @@
 
     _component_name = "preview_integer"
 
     @classmethod
     def get_data_type(self) -> str:
         return "integer"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         text = _value.data
         st.text_input(label="The integer value", value=str(text), disabled=True)
 
 
 class FloatPreview(PreviewComponent):
@@ -178,15 +210,15 @@
 
     _component_name = "preview_float"
 
     @classmethod
     def get_data_type(self) -> str:
         return "float"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         _value = self.api.get_value(options.value)
         text = _value.data
         st.text_input(label="The float value", value=str(text), disabled=True)
 
 
 class NonePreview(PreviewComponent):
@@ -194,10 +226,10 @@
 
     _component_name = "preview_none"
 
     @classmethod
     def get_data_type(self) -> str:
         return "none"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions) -> None:
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions) -> None:
 
         st.write("-- value not set --")
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/preview/tabular.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/explore/tabular.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,63 +1,91 @@
 # -*- coding: utf-8 -*-
+from typing import TYPE_CHECKING
+
+import pygwalker as pyg
+
+import streamlit.components.v1 as components
 from kiara_plugin.streamlit.components.preview import PreviewComponent, PreviewOptions
-from kiara_plugin.tabular.models.array import KiaraArray
 from kiara_plugin.tabular.models.db import KiaraDatabase
-from kiara_plugin.tabular.models.table import KiaraTable
-from streamlit.delta_generator import DeltaGenerator
+from kiara_plugin.tabular.models.tables import KiaraTable, KiaraTables
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
-class ArrayPreview(PreviewComponent):
-    """Preview a value of type 'array'."""
+class TableExplorer(PreviewComponent):
+    """Explore a 'table' value visually."""
 
-    _component_name = "preview_array"
+    _component_name = "explore_table"
+
+    _examples = [
+        {"doc": "A table explorer component.", "args": {"value": "nodes_table"}},
+    ]
 
     @classmethod
     def get_data_type(cls) -> str:
-        return "array"
-
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions):
+        return "table"
 
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions):
         _value = self.api.get_value(options.value)
-        table: KiaraArray = _value.data
+        table: KiaraTable = _value.data
 
-        st.dataframe(table.to_pandas(), use_container_width=True)
+        df = table.to_polars_dataframe()  # noqa
+        pyg_html = pyg.walk(df, return_html=True)
+        components.html(pyg_html, height=1000, scrolling=True)
 
 
-class TablePreview(PreviewComponent):
-    """Preview a value of type 'table'."""
+class DatabasePreview(PreviewComponent):
+    """Preview a value of type 'database'."""
 
-    _component_name = "preview_table"
+    _component_name = "explore_database"
+    _examples = [
+        {"doc": "A database preview.", "args": {"value": "journals_database"}},
+    ]
 
     @classmethod
     def get_data_type(cls) -> str:
-        return "table"
+        return "database"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions):
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions):
 
         _value = self.api.get_value(options.value)
-        table: KiaraTable = _value.data
+        db: KiaraDatabase = _value.data
 
-        st.dataframe(table.to_pandas_dataframe(), use_container_width=True)
+        table_names = list(db.table_names)
 
+        selected_table = st.selectbox("Select table", table_names)
+        if not selected_table:
+            return
+
+        table = db.get_table_as_pandas_df(selected_table)
+
+        pyg_html = pyg.walk(table, return_html=True)
+        components.html(pyg_html, height=1000, scrolling=True)
 
-class DatabasePreview(PreviewComponent):
-    """Preview a value of type 'database'."""
 
-    _component_name = "preview_database"
+class TablesPreview(PreviewComponent):
+    """Preview a value of type 'tables'."""
+
+    _component_name = "explore_tables"
+    _examples = [
+        {"doc": "A tables preview.", "args": {"value": "journals_tables"}},
+    ]
 
     @classmethod
     def get_data_type(cls) -> str:
         return "database"
 
-    def render_preview(self, st: DeltaGenerator, options: PreviewOptions):
+    def render_preview(self, st: "KiaraStreamlitAPI", options: PreviewOptions):
 
         _value = self.api.get_value(options.value)
-        db: KiaraDatabase = _value.data
-        tabs = st.tabs(list(db.table_names))
+        tables: KiaraTables = _value.data
+
+        selected_table = st.selectbox("Select table", tables.table_names)
+
+        if not selected_table:
+            return
+
+        table = tables.get_table(selected_table).to_polars_dataframe()
 
-        for idx, table_name in enumerate(db.table_names):
-            # TODO: this is probably not ideal, as it always loads all tables because
-            # of how tabs are implemented in streamlit
-            # maybe there is an easy way to do this better, otherwise, maybe not use tabs
-            table = db.get_table_as_pandas_df(table_name)
-            tabs[idx].dataframe(table, use_container_width=True)
+        pyg_html = pyg.walk(table, return_html=True)
+        components.html(pyg_html, height=1000, scrolling=True)
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # -*- coding: utf-8 -*-
+from typing import TYPE_CHECKING
+
 from pydantic import BaseModel, Field
 
 from kiara.interfaces.python_api import Workflow
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
-from streamlit.delta_generator import DeltaGenerator
 
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 KIARA_METADATA = {
     "description": "Kiara streamlit compoents to work with workflows",
     "tags": ["workflows"],
     "labels": {"package": "kiara_plugin.core_types"},
 }
 
 
@@ -25,15 +28,15 @@
 
 
 class WorkflowComponent(KiaraComponent):
 
     _options = WorkflowOptions
     _component_type = "workflow"
 
-    def _render(self, st: DeltaGenerator, options: WorkflowOptions):
+    def _render(self, st: "KiaraStreamlitAPI", options: WorkflowOptions):
 
         from kiara_plugin.streamlit.components.workflow.dynamic import (
             WorkflowSessionDynamic,
         )
         from kiara_plugin.streamlit.components.workflow.static import (
             WorkflowSessionStatic,
         )
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 # -*- coding: utf-8 -*-
-from typing import Dict, List, Union
+from typing import TYPE_CHECKING, Dict, List, Union
 
 from pydantic import Field
 
 from kiara.api import Value
 from kiara.interfaces.python_api import OperationInfo, Workflow
 from kiara_plugin.streamlit.components.workflow import WorkflowSession
 
+if TYPE_CHECKING:
+    pass
+
 LEFT_COLUMN = 1
 RIGHT_COLUMN = 4
 
 
 class WorkflowSessionDynamic(WorkflowSession):
 
     initial_value: Union[None, Value] = Field(
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/components.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 # -*- coding: utf-8 -*-
-from typing import Dict, Mapping, Tuple, TypeVar, Union
+from typing import TYPE_CHECKING, Dict, Mapping, Tuple, TypeVar, Union
 
 from pydantic import Field
 
 from kiara.api import Value
 from kiara.models.module.operation import Operation
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.preview import PreviewOptions
 from kiara_plugin.streamlit.components.workflow.dynamic import WorkflowSessionDynamic
 from streamlit.delta_generator import DeltaGenerator
 
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
+
 
 class DynamicWorkflowOptions(ComponentOptions):
 
     session: WorkflowSessionDynamic = Field(description="The current workflow session.")
 
 
 DYN_WORKFLOW_OPTIONS_TYPE = TypeVar(
@@ -33,15 +36,15 @@
 
 
 class WriteStepComponent(DynamicWorkflowComponent):
 
     _component_name = "write_step_details"
     _options = StepDetailsOptions  # type: ignore
 
-    def _render(self, st: DeltaGenerator, options: StepDetailsOptions):
+    def _render(self, st: "KiaraStreamlitAPI", options: StepDetailsOptions):
 
         idx = options.session.pipeline_steps.index(options.step_id)
 
         with st.expander("Operation", expanded=False):
             operation_id = options.session.operations[idx].operation.operation_id
             comp = self._kiara_streamlit.get_component("operation_info")
             comp.render_func(st)(
@@ -81,15 +84,15 @@
 
 class NextStepComponent(DynamicWorkflowComponent):
 
     _component_name = "ask_next_step"
     _options = NextStepOptions
 
     def _render(
-        self, st: DeltaGenerator, options: NextStepOptions
+        self, st: "KiaraStreamlitAPI", options: NextStepOptions
     ) -> Tuple[Union[Operation, None], Union[str, None]]:
 
         value = options.value
 
         if isinstance(options.columns[0], int):
             left, right = st.columns(options.columns)
         else:
@@ -184,15 +187,15 @@
     class Config:
         arbitrary_types_allowed = True
 
     _component_name = "step_input_fields"
     _options = StepDetailsOptions
 
     def _render(
-        self, st: DeltaGenerator, options: StepDetailsOptions
+        self, st: "KiaraStreamlitAPI", options: StepDetailsOptions
     ) -> Dict[str, Value]:
 
         step_id = options.step_id
         idx = options.session.pipeline_steps.index(step_id)
         workflow = options.session.workflow
 
         fixed_input = options.session.input_values[idx]
@@ -237,15 +240,15 @@
 class CurrentValuesPreview(KiaraComponent[CurrentValuesPreviewOptions]):
 
     _component_name = "current_values_preview"
     _options = CurrentValuesPreviewOptions
 
     def _render(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         options: CurrentValuesPreviewOptions,
     ) -> Union[Value, None]:
 
         if not options.values:
             st.write("-- no values --")
             return None
 
@@ -270,15 +273,15 @@
                 component = self.kiara_streamlit.get_preview_component("any")
             left, center, right = tabs[idx].columns([1, 4, 1])
 
             _key = options.create_key("select", f"{idx}_{field}")
             select = left.button("Select for next step", key=_key)
             _key = options.create_key("preview", f"{idx}_{field}")
             preview_opts = PreviewOptions(key=_key, value=value)
-            component.render_preview(st=center, options=preview_opts)
+            component.render_preview(st=center, options=preview_opts)  # type: ignore
 
             right.write("Save value")
             with right.form(key=options.create_key("save_form", f"{idx}_{field}")):
                 _key = options.create_key("alias", f"{idx}_{field}")
                 alias = self._st.text_input(
                     "alias",
                     value="",
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: utf-8 -*-
-from typing import List, Union
+from typing import TYPE_CHECKING, List, Union
 
 from kiara.api import Value
 from kiara.interfaces.python_api import OperationInfo
 from kiara.models.documentation import DocumentationMetadataModel
 from kiara.models.module.pipeline import PipelineStep, generate_pipeline_endpoint_name
 from kiara_plugin.streamlit.components import KiaraComponent
 from kiara_plugin.streamlit.components.workflow.dynamic import (
@@ -12,14 +12,17 @@
     WorkflowSessionDynamic,
 )
 from kiara_plugin.streamlit.components.workflow.dynamic.components import (
     DynamicWorkflowOptions,
 )
 from streamlit.delta_generator import DeltaGenerator
 
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
+
 
 class DynamicWorkflow(KiaraComponent):
 
     _component_name = "workflow_dynamic"
     _options = DynamicWorkflowOptions
 
     def remove_last_step(self, workflow_session: WorkflowSessionDynamic) -> None:
@@ -41,15 +44,15 @@
             except Exception:
                 pass
             workflow_session.workflow.clear_steps(last_step)
 
         workflow_session.last_step_processed = False
 
     def write_workflow_details(
-        self, st: DeltaGenerator, workflow_session: WorkflowSessionDynamic
+        self, st: "KiaraStreamlitAPI", workflow_session: WorkflowSessionDynamic
     ):
 
         st.write(workflow_session.input_values)
         st.write(workflow_session.pipeline_steps)
 
     def add_step(
         self,
@@ -64,15 +67,15 @@
         workflow_session.pipeline_steps.append(pipeline_step.step_id)
 
         workflow_session.last_step_processed = False
         workflow_session.current_outputs = None
         workflow_session.last_operation = operation
 
     def write_step_desc(
-        self, st: DeltaGenerator, key: str, pipeline_step: PipelineStep
+        self, st: "KiaraStreamlitAPI", key: str, pipeline_step: PipelineStep
     ) -> None:
 
         left, right = st.columns((1, 10))
         left.write("Step description")
         doc = None
         if not pipeline_step.doc.is_set:
             op_id = self.api.find_operation_id(
@@ -83,15 +86,15 @@
                 doc = op.doc
         if not doc:
             doc = DocumentationMetadataModel()
         right.markdown(doc.full_doc)
 
     def display_current_outputs(
         self,
-        st: DeltaGenerator,
+        st: "KiaraStreamlitAPI",
         key: str,
         workflow_session: WorkflowSessionDynamic,
         step_id: str,
     ) -> Union[None, Value]:
 
         if workflow_session.current_outputs is None:
 
@@ -111,24 +114,24 @@
         comp = self._kiara_streamlit.get_component("current_values_preview")
         selected_value = comp.render_func(st)(
             key=f"{key}_preview_result_{step_id}",
             values=workflow_session.current_outputs,
         )
         return selected_value
 
-    def write_columns(self, st: DeltaGenerator) -> List[DeltaGenerator]:
+    def write_columns(self, st: "KiaraStreamlitAPI") -> List[DeltaGenerator]:
 
         columns = st.columns((LEFT_COLUMN, RIGHT_COLUMN))
         return columns
 
-    def write_separator(self, st: DeltaGenerator) -> None:
+    def write_separator(self, st: "KiaraStreamlitAPI") -> None:
 
         st.markdown("---")
 
-    def _render(self, st: DeltaGenerator, options: DynamicWorkflowOptions):
+    def _render(self, st: "KiaraStreamlitAPI", options: DynamicWorkflowOptions):
 
         session: WorkflowSessionDynamic = options.session
         if session.workflow is None:
             session.workflow = self.api.create_workflow()
 
         current_value: Union[None, Value] = session.current_value
 
@@ -137,15 +140,15 @@
         if not current_value or (
             len(session.pipeline_steps) == 1 and not session.last_step_processed
         ):
             # if we are at the beginning, without anything processed yet, we want to give
             # Users the option to change the initial value
 
             with left:
-                init_value: Value = self.kiara_streamlit.value_input(
+                init_value: Value = self.kiara_streamlit.select_value(
                     label="**Select initial value**", preview=False
                 )
 
             right.write("")
             right.write("")
             with right.expander("Value preview", expanded=False):
                 if init_value:
@@ -309,15 +312,15 @@
 
             selected_value = self.display_current_outputs(
                 right, key=_key, workflow_session=session, step_id=pipeline_step
             )
         elif session.last_step_processed:
             _key = options.create_key("display_current_outputs")
             selected_value = self.display_current_outputs(
-                right, key=_key, workflow_session=session, step_id=pipeline_step
+                right, key=_key, workflow_session=session, step_id=pipeline_step  # type: ignore
             )
         else:
             selected_value = None
 
         if selected_value:
             session.current_value = selected_value
             session.last_operation = None
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # -*- coding: utf-8 -*-
-from typing import Union
+from typing import TYPE_CHECKING, Union
 
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.modules import DummyModuleConfig
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class StepRequirementsOptions(ComponentOptions):
     pass
 
 
 class StepRequirement(KiaraComponent[StepRequirementsOptions]):
@@ -15,15 +17,15 @@
 
     _component_name = "step_requirements"
     _options = StepRequirementsOptions
 
     _examples = [{"doc": "A simple example", "args": {}}]
 
     def _render(
-        self, st: DeltaGenerator, options: StepRequirementsOptions
+        self, st: "KiaraStreamlitAPI", options: StepRequirementsOptions
     ) -> Union[None, DummyModuleConfig]:
 
         st.write("INSIDE COMPONENT")
 
         _key = options.create_key("step_title")
         title = st.text_input("Step title", key=_key)
         _key = options.create_key("step_desc")
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/components.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/components.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 # -*- coding: utf-8 -*-
 import uuid
-from typing import Dict, List, TypeVar, Union
+from typing import TYPE_CHECKING, Dict, List, TypeVar, Union
 
 from pydantic import Field
 
 from kiara.api import ValueMap
 from kiara_plugin.streamlit.components import ComponentOptions, KiaraComponent
 from kiara_plugin.streamlit.components.workflow.static import WorkflowSessionStatic
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class StaticWorkflowOptions(ComponentOptions):
 
     session: WorkflowSessionStatic = Field(description="The current workflow session.")
 
 
@@ -34,15 +36,15 @@
 
 class PreviousOutputsPreview(StaticWorkflowComponent):
 
     _component_name = "stage_outputs_preview"
     _options = StageOutputsPreviewOptions
 
     def _render(
-        self, st: DeltaGenerator, options: StageOutputsPreviewOptions
+        self, st: "KiaraStreamlitAPI", options: StageOutputsPreviewOptions
     ) -> Union[ValueMap, None]:
 
         session = options.session
         workflow = session.workflow
         pipeline_structure = workflow.pipeline.structure
 
         current_step_outputs: Dict[str, Dict[str, uuid.UUID]] = {}
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/components/workflow/static/workflow_page.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 # -*- coding: utf-8 -*-
-from typing import Dict
+from typing import TYPE_CHECKING, Dict
 
 from kiara.api import ValueSchema
 from kiara.exceptions import KiaraException
 from kiara.models.module.pipeline import StepStatus
 from kiara.models.module.pipeline.structure import PipelineStructure
 from kiara_plugin.streamlit.components import KiaraComponent
 from kiara_plugin.streamlit.components.workflow.static.components import (
     StaticWorkflowOptions,
 )
-from streamlit.delta_generator import DeltaGenerator
+
+if TYPE_CHECKING:
+    from kiara_plugin.streamlit.api import KiaraStreamlitAPI
 
 
 class WorkflowStatic(KiaraComponent[StaticWorkflowOptions]):
 
     _component_name = "workflow_static"
     _options = StaticWorkflowOptions
 
-    def _render(self, st: DeltaGenerator, options: StaticWorkflowOptions):
+    def _render(self, st: "KiaraStreamlitAPI", options: StaticWorkflowOptions):
 
         session = options.session
         workflow = session.workflow
         pipeline_structure: PipelineStructure = workflow.pipeline.structure
         stages = pipeline_structure.processing_stages
 
         no_input_stages = []
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/interfaces/cli/streamlit.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/models.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/modules/__init__.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/streamlit.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/streamlit.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,18 +5,24 @@
 import uuid
 from pathlib import Path
 from typing import Dict, Mapping, Union
 
 import streamlit as st
 from kiara.api import KiaraAPI
 from kiara.context import KiaraConfig, KiaraContextConfig, KiaraRuntimeConfig
+from kiara.interfaces.python_api import JobDesc
+from kiara.models.values.value import ValueMapReadOnly
 from kiara_plugin.streamlit.components import KiaraComponent
+from kiara_plugin.streamlit.components.data_import import DataImportComponent
 from kiara_plugin.streamlit.components.input import InputComponent
 from kiara_plugin.streamlit.components.preview import PreviewComponent
-from kiara_plugin.streamlit.defaults import kiara_stremalit_app_dirs
+from kiara_plugin.streamlit.defaults import (
+    WANTS_MODAL_MARKER_KEY,
+    kiara_stremalit_app_dirs,
+)
 from kiara_plugin.streamlit.utils.class_loading import (
     find_all_kiara_streamlit_components,
 )
 from streamlit.runtime.scriptrunner import get_script_run_ctx
 
 
 class ComponentMgmt(object):
@@ -30,14 +36,15 @@
         self._exapmle_base_dir: Union[str, None, Path] = example_base_dir
 
         self._components: Union[Dict[str, KiaraComponent], None] = None
         self._preview_components: Union[
             Dict[str, Dict[str, PreviewComponent]], None
         ] = None
         self._input_components: Union[Dict[str, InputComponent], None] = None
+        self._import_components: Union[Dict[str, DataImportComponent], None] = None
 
     def add_component(self, name: str, component: KiaraComponent):
 
         if name in self.components:
             raise ValueError(f"Component with name '{name}' already exists.")
 
         self.components[name] = component  # type: ignore
@@ -74,58 +81,76 @@
 
     def get_input_component(self, data_type: str) -> InputComponent:
         result = self.input_components.get(data_type, None)
         if result is None:
             raise Exception(f"No input component found for data type: '{data_type}'")
         return result
 
+    def get_import_component(self, data_type: str) -> Union[DataImportComponent, None]:
+        result = self.import_components.get(data_type, None)
+        return result
+
     @property
     def components(self) -> Mapping[str, KiaraComponent]:
 
         if self._components is not None:
             return self._components
 
         components = {}
         preview_components: Dict[str, Dict[str, PreviewComponent]] = {}
         input_components: Dict[str, InputComponent] = {}  # type: ignore
+        import_components: Dict[str, DataImportComponent] = {}  # type: ignore
 
         base_input_cls = None
         for name, cls in find_all_kiara_streamlit_components().items():
             instance = cls(kiara_streamlit=self._kiara_streamlit, component_name=name)
 
-            if name == "value_input":
+            if name == "select_value":
                 base_input_cls = cls
 
             components[name] = instance
             if issubclass(cls, PreviewComponent):
-                data_type = cls.get_data_type()
+                data_type: Union[None, str] = cls.get_data_type()
                 preview_name = cls.get_preview_name()
                 if (
                     preview_components.get("data_type", {}).get("preview_name", None)
                     is not None
                 ):
                     raise ValueError(
                         f"Can't register component for data type '{data_type}' and preview name '{preview_name}': more than one component registered."
                     )
                 preview_components.setdefault(data_type, {})[preview_name] = instance  # type: ignore
 
-            if issubclass(cls, InputComponent):
+            elif issubclass(cls, InputComponent):
                 data_type = cls.get_data_type()
-                if data_type in input_components.keys():
-                    raise Exception(
-                        f"Multiple input components for data type: {data_type}"
-                    )
-                input_components[data_type] = instance  # type: ignore
+                if data_type:
+                    if data_type in input_components.keys():
+                        raise Exception(
+                            f"Multiple input components for data type: {data_type}"
+                        )
+                    input_components[data_type] = instance  # type: ignore
+
+            elif issubclass(cls, DataImportComponent):
+                data_type = cls.get_data_type()
+                if data_type:
+                    if data_type in import_components.keys():
+                        raise Exception(
+                            f"Multiple data import components for data type: {data_type}"
+                        )
+                    import_components[data_type] = instance  # type: ignore
 
         for data_type in self._kiara_streamlit.api.list_data_type_names():
 
             if self._kiara_streamlit.api.is_internal_data_type(data_type):
                 continue
 
-            if data_type not in input_components.keys():
+            if (
+                data_type in ["file", "file_bundle"]
+                or data_type not in input_components.keys()
+            ):
 
                 _doc = f"Render an input widget that prompts the user for a value of type '{data_type}'."
                 _name = f"select_{data_type}"
 
                 _example = {
                     "doc": f"Render an input widget for a value of type '{data_type}'.",
                     "args": {},
@@ -135,28 +160,35 @@
                 _comp._instance_examples = [_example]  # type: ignore
                 components[_name] = _comp
                 input_components[data_type] = _comp  # type: ignore
 
         self._components = components
         self._preview_components = preview_components
         self._input_components = input_components
+        self._import_components = import_components
         return self._components
 
     @property
     def preview_components(self) -> Mapping[str, Mapping[str, PreviewComponent]]:
         if self._preview_components is None:
             self.components
         return self._preview_components  # type: ignore
 
     @property
     def input_components(self) -> Mapping[str, InputComponent]:
         if self._input_components is None:
             self.components
         return self._input_components  # type: ignore
 
+    @property
+    def import_components(self) -> Mapping[str, DataImportComponent]:
+        if self._import_components is None:
+            self.components
+        return self._import_components  # type: ignore
+
 
 class KiaraStreamlit(object):
     def __init__(
         self,
         context_config: Union[None, KiaraContextConfig] = None,
         runtime_config: Union[None, KiaraRuntimeConfig] = None,
     ):
@@ -168,40 +200,46 @@
 
         ctx = get_script_run_ctx()
         if ctx is None:
             # means, this is not running as streamlit script
             if self._api_outside_streamlit is None:
                 kc = KiaraConfig()
                 self._api_outside_streamlit = KiaraAPI(kc)
-            self.api = self._api_outside_streamlit
+            self._api = self._api_outside_streamlit
         else:
             if "__kiara_api__" not in st.session_state.keys():
                 kc = KiaraConfig()
                 kiara_api = KiaraAPI(kc)
                 st.session_state["__kiara_api__"] = kiara_api
-            self.api = st.session_state.__kiara_api__
+            self._api = st.session_state.__kiara_api__
 
         self._component_mgmt = ComponentMgmt(
             kiara_streamlit=self, example_base_dir=None
         )
 
         self._temp_dir = os.path.join(
             kiara_stremalit_app_dirs.user_cache_dir, str(uuid.uuid4())
         )
 
+        self._job_cache: Dict[str, ValueMapReadOnly] = {}
+
         def del_temp_dir():
             shutil.rmtree(self._temp_dir, ignore_errors=True)
 
         atexit.register(del_temp_dir)
 
-        self.api
+        # self._api
 
         # self.add_component("test", TestComponent(kiara_streamlit=self))
         # self.add_component("help", HelpComponent(kiara_streamlit=self))
 
+    @property
+    def api(self) -> KiaraAPI:
+        return self._api
+
     def __getattr__(self, item):
 
         # if item in ["api", "components", "get_component"]:
         #     return getattr(self, item)
         if item == "api":
             import traceback
 
@@ -211,59 +249,71 @@
         if not comp:
             raise AttributeError(
                 f"Kiara context object does not have component '{item}'."
             )
 
         return comp.render_func()
 
-    # def add_component(self, name: str, component: KiaraComponent):
-    #
-    #     if name in self._avail_kiara_methods:
-    #         raise ValueError(f"Can't add component with name '{name}', name is already used by Kiara context object.")
-    #
-    #     self._component_mgmt.add_component(name, component)
-
-    # @property
-    # def api(self) -> KiaraAPI:
-    #
-    #     ctx = get_script_run_ctx()
-    #     if ctx is None:
-    #         # means, this is not running as streamlit script
-    #         if self._api_outside_streamlit is None:
-    #             kc = KiaraConfig()
-    #             self._api_outside_streamlit = KiaraAPI(kc)
-    #         return self._api_outside_streamlit
-    #     else:
-    #         if "__kiara_api__" not in st.session_state.keys():
-    #             kc = KiaraConfig()
-    #             kiara_api = KiaraAPI(kc)
-    #             st.session_state["__kiara_api__"] = kiara_api
-    #         return st.session_state.__kiara_api__
-
     @property
     def components(self) -> Mapping[str, KiaraComponent]:
         return self._component_mgmt.components
 
     def get_preview_component(
         self, data_type: str, preview_name: Union[str, None] = None
     ) -> PreviewComponent:
         return self._component_mgmt.get_preview_component(
             data_type=data_type, preview_name=preview_name
         )
 
     def get_input_component(self, data_type: str) -> InputComponent:
-        return self._component_mgmt.get_input_component(data_type=data_type)
+        result = self._component_mgmt.get_input_component(data_type=data_type)
+        return result
 
-    # def wants_onboarding(self) -> bool:
-    #     onboarding = st.session_state.get(ONBOARD_MAKER_KEY, None)
-    #     if onboarding and onboarding.get("enabled", False) is True:
-    #         return True
-    #     else:
-    #         st.session_state.pop(ONBOARD_MAKER_KEY, None)
-    #         return False
+    def get_import_component(self, data_type: str) -> Union[DataImportComponent, None]:
+        result = self._component_mgmt.get_import_component(data_type=data_type)
+        return result
+
+    def wants_modal(self) -> bool:
+        wants_modal = st.session_state.get(WANTS_MODAL_MARKER_KEY, None)
+        if wants_modal and wants_modal.get("enabled", False) is True:
+            return True
+        else:
+            st.session_state.pop(WANTS_MODAL_MARKER_KEY, None)
+            return False
 
     def get_component(self, component_name: str) -> KiaraComponent:
 
         component = self._component_mgmt.get_component(component_name)
         if not component:
             raise Exception(f"No component availble for name: {component_name}")
         return component
+
+    def run_job(self, job: JobDesc, reuse_previous: bool = False) -> ValueMapReadOnly:
+        """Run a job and return the result.
+
+        Arguments:
+            job: the job to run
+            reuse_previous: if True, the result of the job will be cached and returned if the same job is run again.
+        """
+
+        job_cache_key = job.instance_id
+        if reuse_previous:
+            if job_cache_key in self._job_cache.keys():
+                return self._job_cache[job_cache_key]
+
+        result = self._api.run_job(operation=job)
+        if reuse_previous:
+            self._job_cache[job_cache_key] = result
+        return result
+
+    def has_job_result(self, job: JobDesc) -> bool:
+        """Check if a job has already been run and has a result available.
+
+        Arguments:
+            job: the job to check
+        """
+
+        return job.instance_id in self._job_cache.keys()
+
+    def get_previous_job_result(self, job: JobDesc) -> Union[None, ValueMapReadOnly]:
+
+        return self._job_cache.get(job.instance_id, None)
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/class_loading.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/class_loading.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/components.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/components.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin/streamlit/utils/monkey_patches.py` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin/streamlit/utils/monkey_patches.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/PKG-INFO` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.streamlit
-Version: 0.4.4
+Version: 0.4.6
 Summary: Streamlit UI and widgets for kiara
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.streamlit
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.streamlit
 Keywords: kiara,streamlit
-Classifier: Framework :: Django
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
@@ -23,14 +22,15 @@
 Description-Content-Type: text/markdown
 Provides-Extra: workflow_app
 Provides-Extra: all_plugins
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
 Provides-Extra: dev_all
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.streamlit.svg)](https://pypi.python.org/pypi/kiara_plugin.streamlit/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.streamlit/goto?ref=develop)
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/SOURCES.txt` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 setup.cfg
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/suggest-a-module.md
 .github/workflows/build-darwin.yaml
 .github/workflows/build-linux.yaml
 .github/workflows/build-windows.yaml
 apps/components.py
+apps/dev_helper.py
 apps/operations.py
 apps/pipelines.py
 apps/jobs/download_journals.yaml
 apps/pipelines/example_file_onboarding.yaml
 ci/conda/conda-pkg-patch.yaml
 docs/SUMMARY.md
 docs/development.md
@@ -33,55 +34,58 @@
 docs/stylesheets/extra.css
 examples/data/Readme.md
 examples/data/journals/JournalEdges1902.csv
 examples/data/journals/JournalNodes1902.csv
 examples/data/journals/Readme.md
 examples/jobs/Readme.md
 examples/pipelines/Readme.md
-examples/streamlit/example.py
-examples/streamlit/help.py
-examples/streamlit/pipeline.py
-examples/streamlit/step_inputs.py
+examples/streamlit/analyze_network_data.py
 examples/streamlit/workflow_dynamic.py
 examples/streamlit/workflow_static.py
-examples/streamlit/workflows.py
 examples/streamlit/workshop.py
 examples/streamlit/pipelines/example.yaml
 examples/streamlit/pipelines/topic_modeling.yaml
 scripts/documentation/gen_api_doc_pages.py
 scripts/documentation/gen_info_pages.py
 scripts/documentation/gen_module_doc.py
 src/kiara_plugin.streamlit.egg-info/PKG-INFO
 src/kiara_plugin.streamlit.egg-info/SOURCES.txt
 src/kiara_plugin.streamlit.egg-info/dependency_links.txt
 src/kiara_plugin.streamlit.egg-info/entry_points.txt
 src/kiara_plugin.streamlit.egg-info/not-zip-safe
 src/kiara_plugin.streamlit.egg-info/requires.txt
 src/kiara_plugin.streamlit.egg-info/top_level.txt
 src/kiara_plugin/streamlit/__init__.py
+src/kiara_plugin/streamlit/api.py
 src/kiara_plugin/streamlit/data_types.py
 src/kiara_plugin/streamlit/defaults.py
 src/kiara_plugin/streamlit/models.py
 src/kiara_plugin/streamlit/py.typed
 src/kiara_plugin/streamlit/streamlit.py
 src/kiara_plugin/streamlit/components/__init__.py
+src/kiara_plugin/streamlit/components/models.py
 src/kiara_plugin/streamlit/components/context/__init__.py
+src/kiara_plugin/streamlit/components/data_import/__init__.py
+src/kiara_plugin/streamlit/components/data_import/tabular.py
+src/kiara_plugin/streamlit/components/explore/__init__.py
+src/kiara_plugin/streamlit/components/explore/tabular.py
 src/kiara_plugin/streamlit/components/info/__init__.py
 src/kiara_plugin/streamlit/components/info/api.py
 src/kiara_plugin/streamlit/components/info/components.py
 src/kiara_plugin/streamlit/components/input/__init__.py
 src/kiara_plugin/streamlit/components/input/assemblies.py
 src/kiara_plugin/streamlit/components/input/container_types.py
+src/kiara_plugin/streamlit/components/input/files.py
 src/kiara_plugin/streamlit/components/input/scalars.py
+src/kiara_plugin/streamlit/components/modals/__init__.py
 src/kiara_plugin/streamlit/components/operations/__init__.py
 src/kiara_plugin/streamlit/components/pipelines/__init__.py
 src/kiara_plugin/streamlit/components/preview/__init__.py
 src/kiara_plugin/streamlit/components/preview/assemblies.py
 src/kiara_plugin/streamlit/components/preview/core_types.py
-src/kiara_plugin/streamlit/components/preview/network_data.py
 src/kiara_plugin/streamlit/components/preview/tabular.py
 src/kiara_plugin/streamlit/components/workflow/__init__.py
 src/kiara_plugin/streamlit/components/workflow/dynamic/__init__.py
 src/kiara_plugin/streamlit/components/workflow/dynamic/components.py
 src/kiara_plugin/streamlit/components/workflow/dynamic/workflow_page.py
 src/kiara_plugin/streamlit/components/workflow/requirements/__init__.py
 src/kiara_plugin/streamlit/components/workflow/static/__init__.py
@@ -91,14 +95,15 @@
 src/kiara_plugin/streamlit/interfaces/cli/__init__.py
 src/kiara_plugin/streamlit/interfaces/cli/streamlit.py
 src/kiara_plugin/streamlit/modules/__init__.py
 src/kiara_plugin/streamlit/pipelines/.gitkeep
 src/kiara_plugin/streamlit/pipelines/__init__.py
 src/kiara_plugin/streamlit/renderers/__init__.py
 src/kiara_plugin/streamlit/resources/.gitkeep
+src/kiara_plugin/streamlit/resources/templates/code_gen/kiara_streamlit_api.py.j2
 src/kiara_plugin/streamlit/resources/templates/pipeline/streamlit_app.py.j2
 src/kiara_plugin/streamlit/utils/__init__.py
 src/kiara_plugin/streamlit/utils/class_loading.py
 src/kiara_plugin/streamlit/utils/components.py
 src/kiara_plugin/streamlit/utils/monkey_patches.py
 tests/conftest.py
 tests/test_job_descs.py
```

### Comparing `kiara_plugin.streamlit-0.4.4/src/kiara_plugin.streamlit.egg-info/entry_points.txt` & `kiara_plugin.streamlit-0.4.6/src/kiara_plugin.streamlit.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/tests/conftest.py` & `kiara_plugin.streamlit-0.4.6/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.streamlit-0.4.4/tests/test_job_descs.py` & `kiara_plugin.streamlit-0.4.6/tests/test_job_descs.py`

 * *Files identical despite different names*

