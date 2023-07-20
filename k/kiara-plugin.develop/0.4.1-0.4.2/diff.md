# Comparing `tmp/kiara_plugin.develop-0.4.1.tar.gz` & `tmp/kiara_plugin.develop-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kiara_plugin.develop-0.4.1.tar", last modified: Thu Jun 29 08:58:28 2023, max compression
+gzip compressed data, was "kiara_plugin.develop-0.4.2.tar", last modified: Thu Jul 20 09:25:19 2023, max compression
```

## Comparing `kiara_plugin.develop-0.4.1.tar` & `kiara_plugin.develop-0.4.2.tar`

### file list

```diff
@@ -1,197 +1,197 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.cruft.json
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     7464 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      387 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/commitlint.config.js
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/SUMMARY.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/development/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/development/core/
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/development/core/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/development/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/packaging.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/stylesheets/extra.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/docs/usage/index.md
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/jobs/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/examples/pipelines/example_pipeline_develop.yaml
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_models.fbs
--rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_models.ts
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.204245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      834 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     8044 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
--rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4039 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.196245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/mkdocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/output.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/scripts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.208245 kiara_plugin.develop-0.4.1/scripts/development/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/development/install_dev_env.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/scripts/documentation/
--rw-r--r--   0 runner    (1001) docker     (123)      865 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_api_doc_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_info_pages.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/scripts/documentation/gen_module_doc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-06-29 08:58:28.216245 kiara_plugin.develop-0.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.200245 kiara_plugin.develop-0.4.1/src/kiara_plugin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/
--rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/
--rw-r--r--   0 runner    (1001) docker     (123)    19782 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     8692 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/states.py
--rw-r--r--   0 runner    (1001) docker     (123)     2930 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/data_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/defaults.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/debug.py
--rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)      534 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/pipelines/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/pipelines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/.gitkeep
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (123)     7807 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/flatbuffers/
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
--rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/
--rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/flatbuffers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/javascript.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-29 08:57:37.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-29 08:58:28.000000 kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-29 08:58:28.212245 kiara_plugin.develop-0.4.1/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/resources/.gitkeep
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/test_job_descs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-06-29 08:57:25.000000 kiara_plugin.develop-0.4.1/tests/test_kiara_modules_default.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.cruft.json
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.188229 kiara_plugin.develop-0.4.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.196229 kiara_plugin.develop-0.4.2/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.196229 kiara_plugin.develop-0.4.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     7468 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4533 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.188229 kiara_plugin.develop-0.4.2/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.196229 kiara_plugin.develop-0.4.2/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/commitlint.config.js
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/SUMMARY.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/docs/development/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/docs/development/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/development/core/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/development/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/packaging.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/stylesheets/extra.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/docs/usage/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2667 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33121 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/jobs/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.200229 kiara_plugin.develop-0.4.2/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/examples/pipelines/example_pipeline_develop.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_models.fbs
+-rw-r--r--   0 runner    (1001) docker     (123)     2482 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_models.ts
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.envrc.disabled
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      834 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     8048 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    16725 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2307 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     5185 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/ci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/ci/conda/conda-pkg-patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/commitlint.config.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/SUMMARY.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2826 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/stylesheets/extra.css
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/usage.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    33398 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/Readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/jobs/example_job_{{ cookiecutter.project_slug }}.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/Readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1665 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.204229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)     2458 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      298 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_kiara_modules_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/output.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/scripts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/scripts/development/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1521 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/scripts/development/install_dev_env.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/scripts/documentation/
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/scripts/documentation/gen_api_doc_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/scripts/documentation/gen_info_pages.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/scripts/documentation/gen_module_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1717 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1393 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.192229 kiara_plugin.develop-0.4.2/src/kiara_plugin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    19799 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5798 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8815 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/states.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/data_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1244 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/defaults.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/debug.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6461 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)      534 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     3350 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/modules/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/modules/pipelines/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/pipelines/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7807 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/flatbuffers/
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/flatbuffers/schema_def.fbs.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/meta.yaml.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     1301 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/
+-rw-r--r--   0 runner    (1001) docker     (123)     5633 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3314 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/flatbuffers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2353 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/javascript.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.208229 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5771 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6781 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 09:24:29.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 09:25:19.000000 kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 09:25:19.212229 kiara_plugin.develop-0.4.2/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/tests/resources/.gitkeep
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/tests/test_job_descs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      227 2023-07-20 09:24:18.000000 kiara_plugin.develop-0.4.2/tests/test_kiara_modules_default.py
```

### Comparing `kiara_plugin.develop-0.4.1/.cruft.json` & `kiara_plugin.develop-0.4.2/.cruft.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'commit'": "'eeaf4b311c49e023edd827ee634dc9c482136c9b'"}*

```diff
@@ -1,10 +1,10 @@
 {
     "checkout": null,
-    "commit": "f30a92644095dd13556ab071b97d20008badaed3",
+    "commit": "eeaf4b311c49e023edd827ee634dc9c482136c9b",
     "context": {
         "cookiecutter": {
             "_template": "https://github.com/DHARPA-Project/kiara_plugin.develop.git",
             "anaconda_user": "dharpa",
             "email": "markus@frkl.io",
             "full_name": "Markus Binsteiner",
             "github_user": "DHARPA-Project",
```

### Comparing `kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.develop-0.4.2/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.develop-0.4.2/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/.github/workflows/build-darwin.yaml` & `kiara_plugin.develop-0.4.2/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/.github/workflows/build-linux.yaml` & `kiara_plugin.develop-0.4.2/.github/workflows/build-linux.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -148,15 +148,15 @@
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

### Comparing `kiara_plugin.develop-0.4.1/.github/workflows/build-windows.yaml` & `kiara_plugin.develop-0.4.2/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/.gitignore` & `kiara_plugin.develop-0.4.2/.gitignore`

 * *Files 1% similar despite different names*

```diff
@@ -59,8 +59,9 @@
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.develop/
+.pixi
 dev.py
```

### Comparing `kiara_plugin.develop-0.4.1/.pre-commit-config.yaml` & `kiara_plugin.develop-0.4.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/LICENSE` & `kiara_plugin.develop-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/Makefile` & `kiara_plugin.develop-0.4.2/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/PKG-INFO` & `kiara_plugin.develop-0.4.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara_plugin.develop
-Version: 0.4.1
+Version: 0.4.2
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
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
 Provides-Extra: all
 Provides-Extra: all_dev
 Provides-Extra: dev_all
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.develop/goto?ref=develop)
```

### Comparing `kiara_plugin.develop-0.4.1/README.md` & `kiara_plugin.develop-0.4.2/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/docs/development/core/index.md` & `kiara_plugin.develop-0.4.2/docs/development/core/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/docs/development/index.md` & `kiara_plugin.develop-0.4.2/docs/development/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/docs/index.md` & `kiara_plugin.develop-0.4.2/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/docs/packaging.md` & `kiara_plugin.develop-0.4.2/docs/packaging.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/docs/usage/index.md` & `kiara_plugin.develop-0.4.2/docs/usage/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.develop-0.4.2/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.develop-0.4.2/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/examples/pipelines/example_pipeline_develop.yaml` & `kiara_plugin.develop-0.4.2/examples/pipelines/example_pipeline_develop.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_models.ts` & `kiara_plugin.develop-0.4.2/kiara_models.ts`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/ISSUE_TEMPLATE/suggest-a-module.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-darwin.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-linux.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -148,15 +148,15 @@
         run: python -m build
       - name: upload source package
         run: {% raw %}curl -F package=@$(ls dist/kiara*.tar.gz) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/{% endraw %}
       - name: upload wheel
         run: {% raw %}curl -F package=@$(ls dist/kiara*.whl) https://${GEMFURY_PUSH_TOKEN}@dharpa.fury.land:443/pypi/{% endraw %}
       - name: publish to PyPI
         if: startsWith(github.ref, 'refs/tags')
-        uses: pypa/gh-action-pypi-publish@master
+        uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: __token__
           password: {% raw %}"${{ secrets.PYPI_API_TOKEN }}"{% endraw %}
 
   conda_package_build:
     name: conda package build (and upload if release)
     runs-on: ubuntu-latest
```

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.github/workflows/build-windows.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.gitignore`

 * *Files 14% similar despite different names*

```diff
@@ -59,7 +59,9 @@
 .frkl
 .envrc
 build.sh
 onefile.spec
 *_complete.zsh.zwc
 ci/conda/**/build
 ci/conda/kiara_plugin.{{ cookiecutter.project_slug }}/meta.yaml
+.pixi
+dev.py
```

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/LICENSE`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/Makefile`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/README.md` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/README.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/development.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/docs/index.md`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalEdges1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/data/journals/JournalNodes1902.csv`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/examples/pipelines/example_pipeline_{{ cookiecutter.project_slug }}.yaml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,29 +13,28 @@
     {name = "{{ cookiecutter.full_name }}", email = "{{ cookiecutter.email }}"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["kiara"]
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
-    "kiara>=0.4.39",
-    "kiara_plugin.core_types>=0.4.17",
+    "kiara>=0.4.48",
+    "kiara_plugin.core_types>=0.4.20",
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]"
 ]
@@ -44,14 +43,17 @@
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
 {{ cookiecutter.project_slug }} = "kiara_plugin.{{ cookiecutter.project_slug }}"
 
 [project.entry-points."kiara.data_types"]
 {{ cookiecutter.project_slug }} = "kiara_plugin.{{ cookiecutter.project_slug }}:find_data_types"
```

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/src/kiara_plugin/{{ cookiecutter.project_slug }}/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/job_tests/example_job_{{ cookiecutter.project_slug }}/outputs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py` & `kiara_plugin.develop-0.4.2/kiara_plugin.{{ cookiecutter.project_slug }}/tests/test_job_descs.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/mkdocs.yml` & `kiara_plugin.develop-0.4.2/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/output.txt` & `kiara_plugin.develop-0.4.2/output.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/pyproject.toml` & `kiara_plugin.develop-0.4.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -13,34 +13,33 @@
     {name = "Markus Binsteiner", email = "markus@frkl.io"}
 ]
 readme = "README.md"
 requires-python = ">=3.8"
 keywords = ["kiara"]
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
-    "kiara>=0.4.44",
+    "kiara>=0.4.48",
     "kiara_plugin.core_types>=0.4.20",
     "kiara_plugin.tabular>=0.4.28",
     "kiara_plugin.onboarding>=0.4.5",
     "diskcache>=5.4.0",
     "httpx>=0.23.0",
-    "pydantic-to-typescript>=1.0.9"
+    "pydantic-to-typescript>=1.0.10"
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 dev_documentation = [
     "kiara[dev_documentation]",
 ]
@@ -49,14 +48,17 @@
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
 develop = "kiara_plugin.develop"
 
 [project.entry-points."kiara.cli_subcommands"]
 debug = "kiara_plugin.develop.interfaces.cli.debug:debug"
 dev = "kiara_plugin.develop.interfaces.cli.dev:dev_group"
```

### Comparing `kiara_plugin.develop-0.4.1/scripts/development/install_dev_env.sh` & `kiara_plugin.develop-0.4.2/scripts/development/install_dev_env.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/scripts/documentation/gen_api_doc_pages.py` & `kiara_plugin.develop-0.4.2/scripts/documentation/gen_api_doc_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/scripts/documentation/gen_info_pages.py` & `kiara_plugin.develop-0.4.2/scripts/documentation/gen_info_pages.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/scripts/documentation/gen_module_doc.py` & `kiara_plugin.develop-0.4.2/scripts/documentation/gen_module_doc.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/setup.cfg` & `kiara_plugin.develop-0.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/setup.py` & `kiara_plugin.develop-0.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/__init__.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/__init__.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 class CondaEnvMgmt(object):
     def __init__(self) -> None:
 
         self._states: States = States()
         self._states.add_state(
             MicroMambaAvailable(
-                "micromamba_available", root_path=KIARA_DEV_CACHE_FOLDER
+                "micromamba_available", root_path=KIARA_DEV_CACHE_FOLDER, version="1.4.6"
             )
         )
         channels = ["conda-forge", "dharpa", "anaconda"]
         # deps = [f"python=={DEFAULT_PYTHON_VERSION}", "boa", "mamba", "anaconda"]
         deps = ["python==3.9", "boa", "mamba", "anaconda-client", "conda-verify"]
         conda_build_env = MambaEnvironment(
             "conda-build-env",
```

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/models.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/conda/states.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/conda/states.py`

 * *Files 4% similar despite different names*

```diff
@@ -156,15 +156,20 @@
 
         token = ARCH_MAP.get(this_os, {}).get(this_arch, None)
         if token is None:
             raise Exception(
                 f"No micromamba executable available for: {this_os} / {this_arch}."
             )
 
-        url = f"https://micro.mamba.pm/api/micromamba/{token}/latest"
+        try:
+            version = self.get_config("version")
+        except Exception:
+            version = "latest"
+
+        url = f"https://micro.mamba.pm/api/micromamba/{token}/{version}"
 
         root_path: Path = self.get_config("root_path")
         # bin_path = root_path / "bin" / "micromamba"
         # bin_path.parent.mkdir(parents=True, exist_ok=True)
         terminal_print("Downloading micromamba...")
 
         fh = io.BytesIO()
```

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/data_types.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/data_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from kiara.models.module.pipeline import PipelineConfig
 from kiara.models.values.value import SerializedData, Value
 
 logger = structlog.getLogger()
 
 class KiaraPipelineDataType(AnyType[PipelineConfig, DataTypeConfig]):
 
-    _data_type_name = "pipeline"
+    _data_type_name = "kiara_pipeline"
     @classmethod
     def python_class(cls) -> Type[PipelineConfig]:
         return PipelineConfig
 
     def serialize(self, data: PipelineConfig) -> SerializedData:
 
         _data = {
```

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/defaults.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/defaults.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/conda.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/conda.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/debug.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/debug.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/interfaces/cli/dev.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/interfaces/cli/dev.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/models.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/models.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/modules/__init__.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/scripts/build-conda-packages.sh`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/meta.yaml.j2` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/meta.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/resources/templates/recipe.yaml.j2`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/__init__.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/__init__.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/flatbuffers.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/flatbuffers.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/schema/javascript.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/schema/javascript.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin/develop/utils.py` & `kiara_plugin.develop-0.4.2/src/kiara_plugin/develop/utils.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/PKG-INFO` & `kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: kiara-plugin.develop
-Version: 0.4.1
+Version: 0.4.2
 Summary: Development utilities for kiara.
 Author-email: Markus Binsteiner <markus@frkl.io>
 License: MPL-2.0
 Project-URL: homepage, https://github.com/DHARPA-Project/kiara_plugin.develop
 Project-URL: documentation, https://DHARPA-Project.github.io/kiara_plugin.develop
 Project-URL: repository, https://github.com/DHARPA-Project/kiara_plugin.develop
 Keywords: kiara
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
 Provides-Extra: all
 Provides-Extra: all_dev
 Provides-Extra: dev_all
 Provides-Extra: dev_documentation
 Provides-Extra: dev_testing
 Provides-Extra: dev_utils
+Provides-Extra: streamlit
 License-File: LICENSE
 License-File: AUTHORS.md
 
 [![PyPI status](https://img.shields.io/pypi/status/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![PyPI version](https://img.shields.io/pypi/v/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/kiara_plugin.develop.svg)](https://pypi.python.org/pypi/kiara_plugin.develop/)
 [![Build Status](https://img.shields.io/endpoint.svg?url=https%3A%2F%2Factions-badge.atrox.dev%2FDHARPA-Project%2Fkiara%2Fbadge%3Fref%3Ddevelop&style=flat)](https://actions-badge.atrox.dev/DHARPA-Project/kiara_plugin.develop/goto?ref=develop)
```

### Comparing `kiara_plugin.develop-0.4.1/src/kiara_plugin.develop.egg-info/SOURCES.txt` & `kiara_plugin.develop-0.4.2/src/kiara_plugin.develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/tests/conftest.py` & `kiara_plugin.develop-0.4.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `kiara_plugin.develop-0.4.1/tests/test_job_descs.py` & `kiara_plugin.develop-0.4.2/tests/test_job_descs.py`

 * *Files identical despite different names*

