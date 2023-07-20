# Comparing `tmp/ansys_templates-1.1.1.tar.gz` & `tmp/ansys_templates-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_templates-1.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_templates-1.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_templates-1.1.1.tar` & `ansys_templates-1.2.0.tar`

### file list

```diff
@@ -1,278 +1,278 @@
--rw-r--r--   0        0        0     1091 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     9947 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/README.rst
--rw-r--r--   0        0        0     3122 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     2266 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/__init__.py
--rw-r--r--   0        0        0     1284 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/__main__.py
--rw-r--r--   0        0        0     3803 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/cli.py
--rw-r--r--   0        0        0     1106 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/licenses/LICENSE_MIT
--rw-r--r--   0        0        0      199 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/licenses/__init__.py
--rw-r--r--   0        0        0     3894 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/paths.py
--rw-r--r--   0        0        0      398 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/cookiecutter.json
--rw-r--r--   0        0        0       86 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
--rw-r--r--   0        0        0      356 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
--rw-r--r--   0        0        0      265 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0       59 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
--rw-r--r--   0        0        0      418 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0      119 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
--rw-r--r--   0        0        0      594 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
--rw-r--r--   0        0        0     3713 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     2779 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
--rw-r--r--   0        0        0     2987 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      764 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      379 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0     2689 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0      105 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
--rw-r--r--   0        0        0      282 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1052 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
--rw-r--r--   0        0        0      657 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rwxr-xr-x   0        0        0     1026 2023-07-19 14:05:11.437718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      969 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       63 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0       50 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rwxr-xr-x   0        0        0     4076 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0      928 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0     3414 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0      196 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
--rw-r--r--   0        0        0       27 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0       81 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
--rw-r--r--   0        0        0       32 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0     1104 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      140 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     2377 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1087 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/cookiecutter.json
--rw-r--r--   0        0        0     2046 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3238 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
--rw-r--r--   0        0        0     1187 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1134 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
--rw-r--r--   0        0        0      825 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1434 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/cookiecutter.json
--rw-r--r--   0        0        0     7450 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2147 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2944 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      655 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0   221672 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
--rw-r--r--   0        0        0      199 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
--rw-r--r--   0        0        0     3898 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      421 2023-07-19 14:05:11.441718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       50 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0     3919 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
--rw-r--r--   0        0        0       47 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      959 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
--rw-r--r--   0        0        0      725 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      248 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
--rw-r--r--   0        0        0    13429 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
--rw-r--r--   0        0        0      922 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       41 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0     9913 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0     2579 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
--rw-r--r--   0        0        0     3687 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
--rw-r--r--   0        0        0     3177 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
--rw-r--r--   0        0        0     5284 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
--rw-r--r--   0        0        0     1837 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
--rw-r--r--   0        0        0     2482 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
--rw-r--r--   0        0        0     5649 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
--rw-r--r--   0        0        0     1753 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
--rw-r--r--   0        0        0     4962 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
--rw-r--r--   0        0        0     7522 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0     9107 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
--rw-r--r--   0        0        0     3165 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
--rw-r--r--   0        0        0     3676 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
--rw-r--r--   0        0        0      960 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
--rw-r--r--   0        0        0     3626 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
--rw-r--r--   0        0        0      618 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
--rw-r--r--   0        0        0      983 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
--rw-r--r--   0        0        0     1372 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
--rw-r--r--   0        0        0      296 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
--rw-r--r--   0        0        0      714 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
--rw-r--r--   0        0        0      660 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
--rw-r--r--   0        0        0      793 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
--rw-r--r--   0        0        0      574 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
--rw-r--r--   0        0        0       20 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     1560 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
--rw-r--r--   0        0        0     2941 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
--rw-r--r--   0        0        0      800 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1132 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       49 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      111 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       21 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0     1461 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      997 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      186 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      687 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1558 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/cookiecutter.json
--rw-r--r--   0        0        0     3108 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
--rw-r--r--   0        0        0      763 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1133 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0       58 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      104 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      345 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0       25 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
--rw-r--r--   0        0        0      621 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
--rw-r--r--   0        0        0      525 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
--rw-r--r--   0        0        0       21 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
--rw-r--r--   0        0        0       28 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1475 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0     1877 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0      955 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0     1062 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1557 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json
--rw-r--r--   0        0        0     3093 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
--rw-r--r--   0        0        0      951 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1145 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0       10 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0      630 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
--rw-r--r--   0        0        0       44 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
--rw-r--r--   0        0        0      116 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
--rw-r--r--   0        0        0      265 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0      230 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
--rw-r--r--   0        0        0      850 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
--rw-r--r--   0        0        0     1409 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
--rw-r--r--   0        0        0      851 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
--rw-r--r--   0        0        0       23 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
--rw-r--r--   0        0        0      902 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
--rw-r--r--   0        0        0      408 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      641 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      111 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
--rw-r--r--   0        0        0      961 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
--rw-r--r--   0        0        0     1556 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json
--rw-r--r--   0        0        0     2869 2023-07-19 14:05:11.445718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
--rw-r--r--   0        0        0      860 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
--rw-r--r--   0        0        0     1129 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
--rw-r--r--   0        0        0      445 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
--rw-r--r--   0        0        0     1299 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
--rw-r--r--   0        0        0      622 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
--rw-r--r--   0        0        0      184 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
--rw-r--r--   0        0        0      186 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0     1458 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys/cookiecutter.json
--rw-r--r--   0        0        0     1148 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3398 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1540 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
--rw-r--r--   0        0        0     2657 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
--rw-r--r--   0        0        0     6537 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      260 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1879 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
--rw-r--r--   0        0        0     1048 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
--rw-r--r--   0        0        0      241 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
--rw-r--r--   0        0        0     1599 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
--rw-r--r--   0        0        0     1857 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
--rw-r--r--   0        0        0     1726 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
--rw-r--r--   0        0        0     4317 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
--rw-r--r--   0        0        0      975 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pybasic/cookiecutter.json
--rw-r--r--   0        0        0     1073 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
--rw-r--r--   0        0        0     3170 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0      896 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
--rw-r--r--   0        0        0      253 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
--rw-r--r--   0        0        0     1063 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/cookiecutter.json
--rw-r--r--   0        0        0     3338 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/hooks/post_gen_project.py
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
--rw-r--r--   0        0        0      175 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
--rw-r--r--   0        0        0      283 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
--rw-r--r--   0        0        0     2365 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
--rw-r--r--   0        0        0     1710 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
--rw-r--r--   0        0        0      599 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
--rw-r--r--   0        0        0      453 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
--rw-r--r--   0        0        0      213 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
--rw-r--r--   0        0        0     2689 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0       16 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
--rw-r--r--   0        0        0     2566 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
--rw-r--r--   0        0        0     2739 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
--rw-r--r--   0        0        0     1567 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
--rw-r--r--   0        0        0      655 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
--rw-r--r--   0        0        0      753 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
--rw-r--r--   0        0        0      928 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
--rw-r--r--   0        0        0       66 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
--rw-r--r--   0        0        0    17194 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
--rw-r--r--   0        0        0       50 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
--rw-r--r--   0        0        0      439 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
--rw-r--r--   0        0        0     3349 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
--rw-r--r--   0        0        0      180 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
--rw-r--r--   0        0        0       30 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
--rw-r--r--   0        0        0       18 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
--rw-r--r--   0        0        0        0 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
--rw-r--r--   0        0        0       11 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
--rw-r--r--   0        0        0   203654 2023-07-19 14:05:11.449718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
--rw-r--r--   0        0        0     3557 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
--rw-r--r--   0        0        0    38166 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
--rw-r--r--   0        0        0      105 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
--rw-r--r--   0        0        0      583 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
--rw-r--r--   0        0        0       52 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
--rw-r--r--   0        0        0       51 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
--rw-r--r--   0        0        0       52 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
--rw-r--r--   0        0        0      803 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
--rw-r--r--   0        0        0      570 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
--rw-r--r--   0        0        0      274 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
--rw-r--r--   0        0        0      263 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
--rw-r--r--   0        0        0      922 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
--rw-r--r--   0        0        0      755 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
--rw-r--r--   0        0        0       18 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
--rw-r--r--   0        0        0   749872 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
--rw-r--r--   0        0        0     9913 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
--rw-r--r--   0        0        0       37 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
--rw-r--r--   0        0        0       18 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
--rw-r--r--   0        0        0     3490 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
--rw-r--r--   0        0        0     4700 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
--rw-r--r--   0        0        0     5244 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
--rw-r--r--   0        0        0      593 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
--rw-r--r--   0        0        0       20 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
--rw-r--r--   0        0        0      664 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
--rw-r--r--   0        0        0      193 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
--rw-r--r--   0        0        0      193 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
--rw-r--r--   0        0        0     1498 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
--rw-r--r--   0        0        0     4035 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/testing.py
--rw-r--r--   0        0        0     6698 2023-07-19 14:05:11.453718 ansys_templates-1.1.1/src/ansys/templates/utils.py
--rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1091 2023-07-20 14:14:35.536466 ansys_templates-1.2.0/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     9947 2023-07-20 14:14:35.536466 ansys_templates-1.2.0/README.rst
+-rw-r--r--   0        0        0     3122 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2266 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/__init__.py
+-rw-r--r--   0        0        0     1284 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/__main__.py
+-rw-r--r--   0        0        0     3803 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/cli.py
+-rw-r--r--   0        0        0     1106 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/licenses/LICENSE_MIT
+-rw-r--r--   0        0        0      199 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/licenses/__init__.py
+-rw-r--r--   0        0        0     3894 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/paths.py
+-rw-r--r--   0        0        0      398 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/cookiecutter.json
+-rw-r--r--   0        0        0       86 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.coveragerc
+-rw-r--r--   0        0        0      356 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.dockerignore
+-rw-r--r--   0        0        0      265 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0       59 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitattributes
+-rw-r--r--   0        0        0      418 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0      119 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labeler.yml
+-rw-r--r--   0        0        0      594 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml
+-rw-r--r--   0        0        0     3713 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     2779 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml
+-rw-r--r--   0        0        0     2987 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      764 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      379 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/AUTHORS
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0     2689 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0      105 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      282 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1052 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml
+-rw-r--r--   0        0        0      657 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rwxr-xr-x   0        0        0     1026 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      969 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       63 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0       50 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rwxr-xr-x   0        0        0     4076 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0      928 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0     3414 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0      196 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pytest.ini
+-rw-r--r--   0        0        0       27 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0       81 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_doc.txt
+-rw-r--r--   0        0        0       32 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0     1104 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      140 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     2377 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1087 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/cookiecutter.json
+-rw-r--r--   0        0        0     2046 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3238 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml
+-rw-r--r--   0        0        0     1187 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1134 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/ignore_words.txt
+-rw-r--r--   0        0        0      825 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1434 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/cookiecutter.json
+-rw-r--r--   0        0        0     7450 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2147 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-07-20 14:14:35.540467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2944 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      655 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   222334 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0      199 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.toml
+-rw-r--r--   0        0        0     3897 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      421 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       50 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0     3919 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py
+-rw-r--r--   0        0        0       47 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      959 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py
+-rw-r--r--   0        0        0      725 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      248 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/monitoring_step.py
+-rw-r--r--   0        0        0    14653 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py
+-rw-r--r--   0        0        0      922 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       41 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0     9913 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0     2579 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py
+-rw-r--r--   0        0        0     3687 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py
+-rw-r--r--   0        0        0     3177 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py
+-rw-r--r--   0        0        0     5284 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py
+-rw-r--r--   0        0        0     1837 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py
+-rw-r--r--   0        0        0     2482 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py
+-rw-r--r--   0        0        0     5649 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py
+-rw-r--r--   0        0        0     1753 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py
+-rw-r--r--   0        0        0     4962 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py
+-rw-r--r--   0        0        0     7522 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0    15892 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/problem_setup_page.py
+-rw-r--r--   0        0        0     3165 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py
+-rw-r--r--   0        0        0     3676 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py
+-rw-r--r--   0        0        0      960 2023-07-20 14:14:35.544467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py
+-rw-r--r--   0        0        0     3626 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py
+-rw-r--r--   0        0        0      618 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py
+-rw-r--r--   0        0        0      983 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py
+-rw-r--r--   0        0        0     1372 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py
+-rw-r--r--   0        0        0      296 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/result_files_page.py
+-rw-r--r--   0        0        0      714 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py
+-rw-r--r--   0        0        0      660 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py
+-rw-r--r--   0        0        0      793 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py
+-rw-r--r--   0        0        0      574 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py
+-rw-r--r--   0        0        0       20 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     1560 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json
+-rw-r--r--   0        0        0     2941 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      800 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1132 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       49 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      111 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       21 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0     1461 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      997 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      186 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      687 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1558 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/cookiecutter.json
+-rw-r--r--   0        0        0     3108 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      763 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1133 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0       58 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      104 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      345 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0       25 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/__init__.py
+-rw-r--r--   0        0        0      621 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py
+-rw-r--r--   0        0        0      525 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py
+-rw-r--r--   0        0        0       21 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/models/__init__.py
+-rw-r--r--   0        0        0       28 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1475 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0     1877 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0      955 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0     1062 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1557 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json
+-rw-r--r--   0        0        0     3093 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      951 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1145 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0       10 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0      630 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto
+-rw-r--r--   0        0        0       44 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_build.txt
+-rw-r--r--   0        0        0      116 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/requirements_tests.txt
+-rw-r--r--   0        0        0      265 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0      230 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/_version.py
+-rw-r--r--   0        0        0      850 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/__init__.py
+-rw-r--r--   0        0        0     1409 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py
+-rw-r--r--   0        0        0      851 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py
+-rw-r--r--   0        0        0       23 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/__init__.py
+-rw-r--r--   0        0        0      902 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py
+-rw-r--r--   0        0        0      408 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/stubs/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      641 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      111 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_metadata.py
+-rw-r--r--   0        0        0      961 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py
+-rw-r--r--   0        0        0     1556 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json
+-rw-r--r--   0        0        0     2869 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      860 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile
+-rw-r--r--   0        0        0     1129 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml
+-rw-r--r--   0        0        0      445 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/__init__.py
+-rw-r--r--   0        0        0     1299 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py
+-rw-r--r--   0        0        0      622 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py
+-rw-r--r--   0        0        0      184 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/__init__.py
+-rw-r--r--   0        0        0      186 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0     1458 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys/cookiecutter.json
+-rw-r--r--   0        0        0     1148 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3398 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1540 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json
+-rw-r--r--   0        0        0     2657 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     6537 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      260 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/src/ansys/{{cookiecutter.__product_name_slug}}/{{cookiecutter.__library_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1879 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json
+-rw-r--r--   0        0        0     1048 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py
+-rw-r--r--   0        0        0      241 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/dependabot.yml
+-rw-r--r--   0        0        0     1599 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml
+-rw-r--r--   0        0        0     1857 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml
+-rw-r--r--   0        0        0     1726 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml
+-rw-r--r--   0        0        0     4317 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/yaml/{{ cookiecutter.yaml_file_name }}
+-rw-r--r--   0        0        0      975 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pybasic/cookiecutter.json
+-rw-r--r--   0        0        0     1073 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py
+-rw-r--r--   0        0        0     3170 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0      896 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py
+-rw-r--r--   0        0        0      253 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/src/{{cookiecutter.__project_name_slug}}/__init__.py
+-rw-r--r--   0        0        0     1063 2023-07-20 14:14:35.548467 ansys_templates-1.2.0/src/ansys/templates/python/solution/cookiecutter.json
+-rw-r--r--   0        0        0     3338 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/hooks/post_gen_project.py
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.exclude
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.codespell.ignore
+-rw-r--r--   0        0        0      175 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.env
+-rw-r--r--   0        0        0      283 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.flake8
+-rw-r--r--   0        0        0     2365 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     1710 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore
+-rw-r--r--   0        0        0      599 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      453 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.vscode/launch.json
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CHANGELOG.md
+-rw-r--r--   0        0        0      213 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODEOWNERS
+-rw-r--r--   0        0        0     2689 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0       16 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CONTRIBUTING.md
+-rw-r--r--   0        0        0     2566 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst
+-rw-r--r--   0        0        0     2739 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst
+-rw-r--r--   0        0        0     1567 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml
+-rw-r--r--   0        0        0      655 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini
+-rw-r--r--   0        0        0      753 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile
+-rw-r--r--   0        0        0      928 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat
+-rw-r--r--   0        0        0       66 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/README.md
+-rw-r--r--   0        0        0    17194 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png
+-rw-r--r--   0        0        0       50 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/README.md
+-rw-r--r--   0        0        0      439 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_templates/sidebar-nav-bs.html
+-rw-r--r--   0        0        0     3349 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py
+-rw-r--r--   0        0        0      180 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/index.rst
+-rw-r--r--   0        0        0       30 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/.gitignore
+-rw-r--r--   0        0        0       18 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/accept.txt
+-rw-r--r--   0        0        0        0 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/styles/Vocab/ANSYS/reject.txt
+-rw-r--r--   0        0        0       11 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/examples/README.md
+-rw-r--r--   0        0        0   203654 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock
+-rw-r--r--   0        0        0     3557 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml
+-rw-r--r--   0        0        0    38166 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py
+-rw-r--r--   0        0        0      105 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/__init__.py
+-rw-r--r--   0        0        0      583 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py
+-rw-r--r--   0        0        0       52 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/README.md
+-rw-r--r--   0        0        0       51 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/assets/README.md
+-rw-r--r--   0        0        0       52 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/scripts/README.md
+-rw-r--r--   0        0        0      803 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py
+-rw-r--r--   0        0        0      570 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py
+-rw-r--r--   0        0        0      274 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/intro_step.py
+-rw-r--r--   0        0        0      263 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/second_step.py
+-rw-r--r--   0        0        0      922 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py
+-rw-r--r--   0        0        0      755 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css
+-rw-r--r--   0        0        0       18 2023-07-20 14:14:35.552467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/README.md
+-rw-r--r--   0        0        0   749872 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png
+-rw-r--r--   0        0        0     9913 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png
+-rw-r--r--   0        0        0       37 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/scripts/README.md
+-rw-r--r--   0        0        0       18 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/README.md
+-rw-r--r--   0        0        0     3490 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py
+-rw-r--r--   0        0        0     4700 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py
+-rw-r--r--   0        0        0     5244 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py
+-rw-r--r--   0        0        0      593 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py
+-rw-r--r--   0        0        0       20 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/common_test_files/README.md
+-rw-r--r--   0        0        0      664 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py
+-rw-r--r--   0        0        0      193 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/integration/test_integration_dummy.py
+-rw-r--r--   0        0        0      193 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/unit/test_unit_dummy.py
+-rw-r--r--   0        0        0     1498 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini
+-rw-r--r--   0        0        0     4035 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/testing.py
+-rw-r--r--   0        0        0     6698 2023-07-20 14:14:35.556467 ansys_templates-1.2.0/src/ansys/templates/utils.py
+-rw-r--r--   0        0        0    11425 1970-01-01 00:00:00.000000 ansys_templates-1.2.0/PKG-INFO
```

### Comparing `ansys_templates-1.1.1/LICENSES/MIT.txt` & `ansys_templates-1.2.0/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/README.rst` & `ansys_templates-1.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/pyproject.toml` & `ansys_templates-1.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-templates"
-version = "1.1.1"
+version = "1.2.0"
 description = "Creates Python projects according to PyAnsys guidelines"
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSES/MIT.txt"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
```

### Comparing `ansys_templates-1.1.1/src/ansys/templates/__init__.py` & `ansys_templates-1.2.0/src/ansys/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/__main__.py` & `ansys_templates-1.2.0/src/ansys/templates/__main__.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/cli.py` & `ansys_templates-1.2.0/src/ansys/templates/cli.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/licenses/LICENSE_MIT` & `ansys_templates-1.2.0/src/ansys/templates/licenses/LICENSE_MIT`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/paths.py` & `ansys_templates-1.2.0/src/ansys/templates/paths.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/labels.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.github/workflows/label.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/azure-pipeline.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/docker/Docker.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/common/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.github/workflows/ci_cd.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/doc_project/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/poetry.lock`

 * *Files 1% similar despite different names*

```diff
@@ -216,45 +216,45 @@
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
 name = "ansys-solutions-dash-lib"
-version = "0.4.2"
+version = "0.4.3"
 description = "A collection of functions and classes to design solution's frontend using Dash components."
 optional = false
 python-versions = ">=3.8,<3.11"
 files = [
-    {file = "ansys_solutions_dash_lib-0.4.2-py3-none-any.whl", hash = "sha256:21bd1225591d290ff463602ff83c033bfe35fd7b4418db496654eb1c8e25084c"},
-    {file = "ansys_solutions_dash_lib-0.4.2.tar.gz", hash = "sha256:285ccf20b01e1de03ea288f2fced6bb16d6d1d8dc4a09d647626d57c551681df"},
+    {file = "ansys_solutions_dash_lib-0.4.3-py3-none-any.whl", hash = "sha256:ca801f10ecd6f74915356cb857e7cdc820db4749200ad43dc82e89f066bb2d8d"},
+    {file = "ansys_solutions_dash_lib-0.4.3.tar.gz", hash = "sha256:4ace8f27a85e2e9a8051f9a40a9d33834d1f2c5a7019d56375e3a2bc8ad77ef5"},
 ]
 
 [package.dependencies]
 dash = ">=2.5,<3.0"
 dash_bootstrap_components = ">=1.3,<2.0"
 
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
 name = "ansys-solutions-optislang-frontend-components"
-version = "0.1.dev6"
+version = "0.1.dev7"
 description = ""
 optional = false
 python-versions = ">=3.8,<3.11"
 files = [
-    {file = "ansys_solutions_optislang_frontend_components-0.1.dev6-py3-none-any.whl", hash = "sha256:0ca79c5f8fc799ac68723287e00ac0bd81ac1580908c312cf89698ea60c9cd3b"},
-    {file = "ansys_solutions_optislang_frontend_components-0.1.dev6.tar.gz", hash = "sha256:aa23ea70987986a8a38722bc53d6279db34073f7f4927a4e02c17b31f58ade3b"},
+    {file = "ansys_solutions_optislang_frontend_components-0.1.dev7-py3-none-any.whl", hash = "sha256:f3bf22503b0b337c60bd449b21585e0a71f4192d422030161b97d8932be4c4bf"},
+    {file = "ansys_solutions_optislang_frontend_components-0.1.dev7.tar.gz", hash = "sha256:5c6c629041e7cfb826bb0d9ed6631c8cb6c21eed6b7ab3fd5f8e2d4c5e7ccf64"},
 ]
 
 [package.dependencies]
-ansys-solutions-dash-lib = "0.4.2"
+ansys-solutions-dash-lib = "0.4.3"
 
 [package.source]
 type = "legacy"
 url = "https://pkgs.dev.azure.com/pyansys/_packaging/ansys-solutions/pypi/simple"
 reference = "solutions-private-pypi"
 
 [[package]]
@@ -652,21 +652,21 @@
     {file = "charset_normalizer-3.2.0-cp39-cp39-win32.whl", hash = "sha256:6c409c0deba34f147f77efaa67b8e4bb83d2f11c8806405f76397ae5b8c0d1c9"},
     {file = "charset_normalizer-3.2.0-cp39-cp39-win_amd64.whl", hash = "sha256:7095f6fbfaa55defb6b733cfeb14efaae7a29f0b59d8cf213be4e7ca0b857b80"},
     {file = "charset_normalizer-3.2.0-py3-none-any.whl", hash = "sha256:8e098148dd37b4ce3baca71fb394c81dc5d9c7728c95df695d2dca218edf40e6"},
 ]
 
 [[package]]
 name = "click"
-version = "8.1.4"
+version = "8.1.5"
 description = "Composable command line interface toolkit"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "click-8.1.4-py3-none-any.whl", hash = "sha256:2739815aaa5d2c986a88f1e9230c55e17f0caad3d958a5e13ad0797c166db9e3"},
-    {file = "click-8.1.4.tar.gz", hash = "sha256:b97d0c74955da062a7d4ef92fadb583806a585b2ea81958a81bd72726cbb8e37"},
+    {file = "click-8.1.5-py3-none-any.whl", hash = "sha256:e576aa487d679441d7d30abb87e1b43d24fc53bffb8758443b1a9e1cee504548"},
+    {file = "click-8.1.5.tar.gz", hash = "sha256:4be4b1af8d665c6d942909916d31a213a106800c47d0eeba73d34da3cbc11367"},
 ]
 
 [package.dependencies]
 colorama = {version = "*", markers = "platform_system == \"Windows\""}
 
 [[package]]
 name = "clr-loader"
@@ -756,38 +756,42 @@
 tomli = {version = "*", optional = true, markers = "python_full_version <= \"3.11.0a6\" and extra == \"toml\""}
 
 [package.extras]
 toml = ["tomli"]
 
 [[package]]
 name = "cryptography"
-version = "41.0.1"
+version = "41.0.2"
 description = "cryptography is a package which provides cryptographic recipes and primitives to Python developers."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:f73bff05db2a3e5974a6fd248af2566134d8981fd7ab012e5dd4ddb1d9a70699"},
-    {file = "cryptography-41.0.1-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:1a5472d40c8f8e91ff7a3d8ac6dfa363d8e3138b961529c996f3e2df0c7a411a"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:7fa01527046ca5facdf973eef2535a27fec4cb651e4daec4d043ef63f6ecd4ca"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:b46e37db3cc267b4dea1f56da7346c9727e1209aa98487179ee8ebed09d21e43"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:d198820aba55660b4d74f7b5fd1f17db3aa5eb3e6893b0a41b75e84e4f9e0e4b"},
-    {file = "cryptography-41.0.1-cp37-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:948224d76c4b6457349d47c0c98657557f429b4e93057cf5a2f71d603e2fc3a3"},
-    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:059e348f9a3c1950937e1b5d7ba1f8e968508ab181e75fc32b879452f08356db"},
-    {file = "cryptography-41.0.1-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:b4ceb5324b998ce2003bc17d519080b4ec8d5b7b70794cbd2836101406a9be31"},
-    {file = "cryptography-41.0.1-cp37-abi3-win32.whl", hash = "sha256:8f4ab7021127a9b4323537300a2acfb450124b2def3756f64dc3a3d2160ee4b5"},
-    {file = "cryptography-41.0.1-cp37-abi3-win_amd64.whl", hash = "sha256:1fee5aacc7367487b4e22484d3c7e547992ed726d14864ee33c0176ae43b0d7c"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:9a6c7a3c87d595608a39980ebaa04d5a37f94024c9f24eb7d10262b92f739ddb"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:5d092fdfedaec4cbbffbf98cddc915ba145313a6fdaab83c6e67f4e6c218e6f3"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:1a8e6c2de6fbbcc5e14fd27fb24414507cb3333198ea9ab1258d916f00bc3039"},
-    {file = "cryptography-41.0.1-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:cb33ccf15e89f7ed89b235cff9d49e2e62c6c981a6061c9c8bb47ed7951190bc"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:5f0ff6e18d13a3de56f609dd1fd11470918f770c6bd5d00d632076c727d35485"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7bfc55a5eae8b86a287747053140ba221afc65eb06207bedf6e019b8934b477c"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:eb8163f5e549a22888c18b0d53d6bb62a20510060a22fd5a995ec8a05268df8a"},
-    {file = "cryptography-41.0.1-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:8dde71c4169ec5ccc1087bb7521d54251c016f126f922ab2dfe6649170a3b8c5"},
-    {file = "cryptography-41.0.1.tar.gz", hash = "sha256:d34579085401d3f49762d2f7d6634d6b6c2ae1242202e860f4d26b046e3a1006"},
+    {file = "cryptography-41.0.2-cp37-abi3-macosx_10_12_universal2.whl", hash = "sha256:01f1d9e537f9a15b037d5d9ee442b8c22e3ae11ce65ea1f3316a41c78756b711"},
+    {file = "cryptography-41.0.2-cp37-abi3-macosx_10_12_x86_64.whl", hash = "sha256:079347de771f9282fbfe0e0236c716686950c19dee1b76240ab09ce1624d76d7"},
+    {file = "cryptography-41.0.2-cp37-abi3-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:439c3cc4c0d42fa999b83ded80a9a1fb54d53c58d6e59234cfe97f241e6c781d"},
+    {file = "cryptography-41.0.2-cp37-abi3-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f14ad275364c8b4e525d018f6716537ae7b6d369c094805cae45300847e0894f"},
+    {file = "cryptography-41.0.2-cp37-abi3-manylinux_2_28_aarch64.whl", hash = "sha256:84609ade00a6ec59a89729e87a503c6e36af98ddcd566d5f3be52e29ba993182"},
+    {file = "cryptography-41.0.2-cp37-abi3-manylinux_2_28_x86_64.whl", hash = "sha256:49c3222bb8f8e800aead2e376cbef687bc9e3cb9b58b29a261210456a7783d83"},
+    {file = "cryptography-41.0.2-cp37-abi3-musllinux_1_1_aarch64.whl", hash = "sha256:d73f419a56d74fef257955f51b18d046f3506270a5fd2ac5febbfa259d6c0fa5"},
+    {file = "cryptography-41.0.2-cp37-abi3-musllinux_1_1_x86_64.whl", hash = "sha256:2a034bf7d9ca894720f2ec1d8b7b5832d7e363571828037f9e0c4f18c1b58a58"},
+    {file = "cryptography-41.0.2-cp37-abi3-win32.whl", hash = "sha256:d124682c7a23c9764e54ca9ab5b308b14b18eba02722b8659fb238546de83a76"},
+    {file = "cryptography-41.0.2-cp37-abi3-win_amd64.whl", hash = "sha256:9c3fe6534d59d071ee82081ca3d71eed3210f76ebd0361798c74abc2bcf347d4"},
+    {file = "cryptography-41.0.2-pp310-pypy310_pp73-macosx_10_12_x86_64.whl", hash = "sha256:a719399b99377b218dac6cf547b6ec54e6ef20207b6165126a280b0ce97e0d2a"},
+    {file = "cryptography-41.0.2-pp310-pypy310_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:182be4171f9332b6741ee818ec27daff9fb00349f706629f5cbf417bd50e66fd"},
+    {file = "cryptography-41.0.2-pp310-pypy310_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:7a9a3bced53b7f09da251685224d6a260c3cb291768f54954e28f03ef14e3766"},
+    {file = "cryptography-41.0.2-pp310-pypy310_pp73-win_amd64.whl", hash = "sha256:f0dc40e6f7aa37af01aba07277d3d64d5a03dc66d682097541ec4da03cc140ee"},
+    {file = "cryptography-41.0.2-pp38-pypy38_pp73-macosx_10_12_x86_64.whl", hash = "sha256:674b669d5daa64206c38e507808aae49904c988fa0a71c935e7006a3e1e83831"},
+    {file = "cryptography-41.0.2-pp38-pypy38_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:7af244b012711a26196450d34f483357e42aeddb04128885d95a69bd8b14b69b"},
+    {file = "cryptography-41.0.2-pp38-pypy38_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:9b6d717393dbae53d4e52684ef4f022444fc1cce3c48c38cb74fca29e1f08eaa"},
+    {file = "cryptography-41.0.2-pp38-pypy38_pp73-win_amd64.whl", hash = "sha256:192255f539d7a89f2102d07d7375b1e0a81f7478925b3bc2e0549ebf739dae0e"},
+    {file = "cryptography-41.0.2-pp39-pypy39_pp73-macosx_10_12_x86_64.whl", hash = "sha256:f772610fe364372de33d76edcd313636a25684edb94cee53fd790195f5989d14"},
+    {file = "cryptography-41.0.2-pp39-pypy39_pp73-manylinux_2_28_aarch64.whl", hash = "sha256:b332cba64d99a70c1e0836902720887fb4529ea49ea7f5462cf6640e095e11d2"},
+    {file = "cryptography-41.0.2-pp39-pypy39_pp73-manylinux_2_28_x86_64.whl", hash = "sha256:9a6673c1828db6270b76b22cc696f40cde9043eb90373da5c2f8f2158957f42f"},
+    {file = "cryptography-41.0.2-pp39-pypy39_pp73-win_amd64.whl", hash = "sha256:342f3767e25876751e14f8459ad85e77e660537ca0a066e10e75df9c9e9099f0"},
+    {file = "cryptography-41.0.2.tar.gz", hash = "sha256:7d230bf856164de164ecb615ccc14c7fc6de6906ddd5b491f3af90d3514c925c"},
 ]
 
 [package.dependencies]
 cffi = ">=1.12"
 
 [package.extras]
 docs = ["sphinx (>=5.3.0)", "sphinx-rtd-theme (>=1.1.1)"]
@@ -829,21 +833,21 @@
 compress = ["flask-compress"]
 dev = ["PyYAML (>=5.4.1)", "coloredlogs (>=15.0.1)", "fire (>=0.4.0)"]
 diskcache = ["diskcache (>=5.2.1)", "multiprocess (>=0.70.12)", "psutil (>=5.8.0)"]
 testing = ["beautifulsoup4 (>=4.8.2)", "cryptography (<3.4)", "dash-testing-stub (>=0.0.2)", "lxml (>=4.6.2)", "multiprocess (>=0.70.12)", "percy (>=2.0.2)", "psutil (>=5.8.0)", "pytest (>=6.0.2)", "requests[security] (>=2.21.0)", "selenium (>=3.141.0,<=4.2.0)", "waitress (>=1.4.4)"]
 
 [[package]]
 name = "dash-bootstrap-components"
-version = "1.4.1"
+version = "1.4.2"
 description = "Bootstrap themed components for use in Plotly Dash"
 optional = false
 python-versions = ">=3.7, <4"
 files = [
-    {file = "dash-bootstrap-components-1.4.1.tar.gz", hash = "sha256:05c2e2767a8ab104fc950d15482d09dde59d21f1e9bd5809d30672e61b7f420c"},
-    {file = "dash_bootstrap_components-1.4.1-py3-none-any.whl", hash = "sha256:17c9e6b90ff27abd3fbd6fe54ea85987b155414a247010467ec904406dcd3657"},
+    {file = "dash-bootstrap-components-1.4.2.tar.gz", hash = "sha256:b7514be30e229a1701db5010a47d275882a94d1efff4c803ac42a9d222ed86e0"},
+    {file = "dash_bootstrap_components-1.4.2-py3-none-any.whl", hash = "sha256:4f59352a2f81cb0c41ae75dd3e0814f64049a4520f935397298e9a093ace727c"},
 ]
 
 [package.dependencies]
 dash = ">=2.0.0"
 
 [package.extras]
 pandas = ["numpy", "pandas"]
@@ -984,21 +988,21 @@
 wrapt = ">=1.10,<2"
 
 [package.extras]
 dev = ["PyTest", "PyTest-Cov", "bump2version (<1)", "sphinx (<2)", "tox"]
 
 [[package]]
 name = "distlib"
-version = "0.3.6"
+version = "0.3.7"
 description = "Distribution utilities"
 optional = false
 python-versions = "*"
 files = [
-    {file = "distlib-0.3.6-py2.py3-none-any.whl", hash = "sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e"},
-    {file = "distlib-0.3.6.tar.gz", hash = "sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46"},
+    {file = "distlib-0.3.7-py2.py3-none-any.whl", hash = "sha256:2e24928bc811348f0feb63014e97aaae3037f2cf48712d51ae61df7fd6075057"},
+    {file = "distlib-0.3.7.tar.gz", hash = "sha256:9dafe54b34a028eafd95039d5e5d4851a13734540f1331060d31c9916e7147a8"},
 ]
 
 [[package]]
 name = "docutils"
 version = "0.18.1"
 description = "Docutils -- Python Documentation Utilities"
 optional = false
@@ -2175,21 +2179,21 @@
 ]
 
 [package.extras]
 testing = ["pytest", "pytest-cov"]
 
 [[package]]
 name = "platformdirs"
-version = "3.8.1"
+version = "3.9.1"
 description = "A small Python package for determining appropriate platform-specific dirs, e.g. a \"user data dir\"."
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "platformdirs-3.8.1-py3-none-any.whl", hash = "sha256:cec7b889196b9144d088e4c57d9ceef7374f6c39694ad1577a0aab50d27ea28c"},
-    {file = "platformdirs-3.8.1.tar.gz", hash = "sha256:f87ca4fcff7d2b0f81c6a748a77973d7af0f4d526f98f308477c3c436c74d528"},
+    {file = "platformdirs-3.9.1-py3-none-any.whl", hash = "sha256:ad8291ae0ae5072f66c16945166cb11c63394c7a3ad1b1bc9828ca3162da8c2f"},
+    {file = "platformdirs-3.9.1.tar.gz", hash = "sha256:1b42b450ad933e981d56e59f1b97495428c9bd60698baab9f3eb3d00d5822421"},
 ]
 
 [package.extras]
 docs = ["furo (>=2023.5.20)", "proselint (>=0.13)", "sphinx (>=7.0.1)", "sphinx-autodoc-typehints (>=1.23,!=1.23.4)"]
 test = ["appdirs (==1.4.4)", "covdefaults (>=2.3)", "pytest (>=7.3.1)", "pytest-cov (>=4.1)", "pytest-mock (>=3.10)"]
 
 [[package]]
@@ -3102,21 +3106,21 @@
 [package.extras]
 docs = ["sphinxcontrib-websupport"]
 lint = ["docutils-stubs", "flake8 (>=3.5.0)", "flake8-bugbear", "flake8-comprehensions", "isort", "mypy (>=0.971)", "sphinx-lint", "types-requests", "types-typed-ast"]
 test = ["cython", "html5lib", "pytest (>=4.6)", "typed-ast"]
 
 [[package]]
 name = "sphinx-code-tabs"
-version = "0.5.3"
+version = "0.5.5"
 description = "Sphinx extension for adding alternative code-blocks as selectable tabs"
 optional = false
 python-versions = ">=3.5"
 files = [
-    {file = "sphinx_code_tabs-0.5.3-py3-none-any.whl", hash = "sha256:11d9d1fa7eb5f21c5b24a023e3522bbd36b456392a74a5597ca0adde30dc27e3"},
-    {file = "sphinx_code_tabs-0.5.3.tar.gz", hash = "sha256:a17f387a37e09b9deb64c5335023baa0f1f5b47ff451fee4fc0f02ea46a0bed3"},
+    {file = "sphinx_code_tabs-0.5.5-py3-none-any.whl", hash = "sha256:e2cabdcc02b5897b399f6bca36557ce050d2fb7d095c01292b41ad34f1ce2ef0"},
+    {file = "sphinx_code_tabs-0.5.5.tar.gz", hash = "sha256:150acc5190ce3b3d2378af02dc3fb651d32cbfb924a5ed37681418aa7520acea"},
 ]
 
 [package.dependencies]
 sphinx = ">=3"
 
 [package.extras]
 doc = ["sphinx-rtd-theme"]
@@ -3299,60 +3303,60 @@
 
 [package.extras]
 lint = ["docutils-stubs", "flake8", "mypy"]
 test = ["pytest"]
 
 [[package]]
 name = "sqlalchemy"
-version = "2.0.18"
+version = "2.0.19"
 description = "Database Abstraction Library"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:7ddd6d35c598af872f9a0a5bce7f7c4a1841684a72dab3302e3df7f17d1b5249"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:00aa050faf24ce5f2af643e2b86822fa1d7149649995f11bc1e769bbfbf9010b"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b52c6741073de5a744d27329f9803938dcad5c9fee7e61690c705f72973f4175"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:7db97eabd440327c35b751d5ebf78a107f505586485159bcc87660da8bb1fdca"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:589aba9a35869695b319ed76c6f673d896cd01a7ff78054be1596df7ad9b096f"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:9da4ee8f711e077633730955c8f3cd2485c9abf5ea0f80aac23221a3224b9a8c"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-win32.whl", hash = "sha256:5dd574a37be388512c72fe0d7318cb8e31743a9b2699847a025e0c08c5bf579d"},
-    {file = "SQLAlchemy-2.0.18-cp310-cp310-win_amd64.whl", hash = "sha256:6852cd34d96835e4c9091c1e6087325efb5b607b75fd9f7075616197d1c4688a"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:10e001a84f820fea2640e4500e12322b03afc31d8f4f6b813b44813b2a7c7e0d"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:bffd6cd47c2e68970039c0d3e355c9ed761d3ca727b204e63cd294cad0e3df90"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:8b7b3ebfa9416c8eafaffa65216e229480c495e305a06ba176dcac32710744e6"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:79228a7b90d95957354f37b9d46f2cc8926262ae17b0d3ed8f36c892f2a37e06"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:ba633b51835036ff0f402c21f3ff567c565a22ff0a5732b060a68f4660e2a38f"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:8da677135eff43502b7afab5a1e641edfb2dc734ba7fc146e9b1b86817a728e2"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-win32.whl", hash = "sha256:82edf3a6090554a83942cec79151d6b5eb96e63d143e80e4cf6671e5d772f6be"},
-    {file = "SQLAlchemy-2.0.18-cp311-cp311-win_amd64.whl", hash = "sha256:69ae0e9509c43474e33152abe1385b8954922544616426bf793481e1a37e094f"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:09397a18733fa2a4c7680b746094f980060666ee549deafdb5e102a99ce4619b"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:45b07470571bda5ee7f5ec471271bbde97267cc8403fce05e280c36ea73f4754"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:1aac42a21a7fa6c9665392c840b295962992ddf40aecf0a88073bc5c76728117"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:da46beef0ce882546d92b7b2e8deb9e04dbb8fec72945a8eb28b347ca46bc15a"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:a6f1d8256d06f58e6ece150fbe05c63c7f9510df99ee8ac37423f5476a2cebb4"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-win32.whl", hash = "sha256:67fbb40db3985c0cfb942fe8853ad94a5e9702d2987dec03abadc2f3b6a24afb"},
-    {file = "SQLAlchemy-2.0.18-cp37-cp37m-win_amd64.whl", hash = "sha256:afb322ca05e2603deedbcd2e9910f11a3fd2f42bdeafe63018e5641945c7491c"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:908c850b98cac1e203ababd4ba76868d19ae0d7172cdc75d3f1b7829b16837d2"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:10514adc41fc8f5922728fbac13d401a1aefcf037f009e64ca3b92464e33bf0e"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2b791577c546b6bbd7b43953565fcb0a2fec63643ad605353dd48afbc3c48317"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:420bc6d06d4ae7fb6921524334689eebcbea7bf2005efef070a8562cc9527a37"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:ebdd2418ab4e2e26d572d9a1c03877f8514a9b7436729525aa571862507b3fea"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:556dc18e39b6edb76239acfd1c010e37395a54c7fde8c57481c15819a3ffb13e"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-win32.whl", hash = "sha256:7b8cba5a25e95041e3413d91f9e50616bcfaec95afa038ce7dc02efefe576745"},
-    {file = "SQLAlchemy-2.0.18-cp38-cp38-win_amd64.whl", hash = "sha256:0f7fdcce52cd882b559a57b484efc92e108efeeee89fab6b623aba1ac68aad2e"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:d7a2c1e711ce59ac9d0bba780318bcd102d2958bb423209f24c6354d8c4da930"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:5c95e3e7cc6285bf7ff263eabb0d3bfe3def9a1ff98124083d45e5ece72f4579"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fc44e50f9d5e96af1a561faa36863f9191f27364a4df3eb70bca66e9370480b6"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:bfa1a0f83bdf8061db8d17c2029454722043f1e4dd1b3d3d3120d1b54e75825a"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:194f2d5a7cb3739875c4d25b3fe288ab0b3dc33f7c857ba2845830c8c51170a0"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:4ebc542d2289c0b016d6945fd07a7e2e23f4abc41e731ac8ad18a9e0c2fd0ec2"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-win32.whl", hash = "sha256:774bd401e7993452ba0596e741c0c4d6d22f882dd2a798993859181dbffadc62"},
-    {file = "SQLAlchemy-2.0.18-cp39-cp39-win_amd64.whl", hash = "sha256:2756485f49e7df5c2208bdc64263d19d23eba70666f14ad12d6d8278a2fff65f"},
-    {file = "SQLAlchemy-2.0.18-py3-none-any.whl", hash = "sha256:6c5bae4c288bda92a7550fe8de9e068c0a7cd56b1c5d888aae5b40f0e13b40bd"},
-    {file = "SQLAlchemy-2.0.18.tar.gz", hash = "sha256:1fb792051db66e09c200e7bc3bda3b1eb18a5b8eb153d2cedb2b14b56a68b8cb"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-macosx_10_9_x86_64.whl", hash = "sha256:9deaae357edc2091a9ed5d25e9ee8bba98bcfae454b3911adeaf159c2e9ca9e3"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-macosx_11_0_arm64.whl", hash = "sha256:0bf0fd65b50a330261ec7fe3d091dfc1c577483c96a9fa1e4323e932961aa1b5"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:1d90ccc15ba1baa345796a8fb1965223ca7ded2d235ccbef80a47b85cea2d71a"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:cb4e688f6784427e5f9479d1a13617f573de8f7d4aa713ba82813bcd16e259d1"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-musllinux_1_1_aarch64.whl", hash = "sha256:584f66e5e1979a7a00f4935015840be627e31ca29ad13f49a6e51e97a3fb8cae"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-musllinux_1_1_x86_64.whl", hash = "sha256:2c69ce70047b801d2aba3e5ff3cba32014558966109fecab0c39d16c18510f15"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-win32.whl", hash = "sha256:96f0463573469579d32ad0c91929548d78314ef95c210a8115346271beeeaaa2"},
+    {file = "SQLAlchemy-2.0.19-cp310-cp310-win_amd64.whl", hash = "sha256:22bafb1da60c24514c141a7ff852b52f9f573fb933b1e6b5263f0daa28ce6db9"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-macosx_10_9_x86_64.whl", hash = "sha256:d6894708eeb81f6d8193e996257223b6bb4041cb05a17cd5cf373ed836ef87a2"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-macosx_11_0_arm64.whl", hash = "sha256:d8f2afd1aafded7362b397581772c670f20ea84d0a780b93a1a1529da7c3d369"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:b15afbf5aa76f2241184c1d3b61af1a72ba31ce4161013d7cb5c4c2fca04fd6e"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8fc05b59142445a4efb9c1fd75c334b431d35c304b0e33f4fa0ff1ea4890f92e"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-musllinux_1_1_aarch64.whl", hash = "sha256:5831138f0cc06b43edf5f99541c64adf0ab0d41f9a4471fd63b54ae18399e4de"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-musllinux_1_1_x86_64.whl", hash = "sha256:3afa8a21a9046917b3a12ffe016ba7ebe7a55a6fc0c7d950beb303c735c3c3ad"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-win32.whl", hash = "sha256:c896d4e6ab2eba2afa1d56be3d0b936c56d4666e789bfc59d6ae76e9fcf46145"},
+    {file = "SQLAlchemy-2.0.19-cp311-cp311-win_amd64.whl", hash = "sha256:024d2f67fb3ec697555e48caeb7147cfe2c08065a4f1a52d93c3d44fc8e6ad1c"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-macosx_10_9_x86_64.whl", hash = "sha256:89bc2b374ebee1a02fd2eae6fd0570b5ad897ee514e0f84c5c137c942772aa0c"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:dd4d410a76c3762511ae075d50f379ae09551d92525aa5bb307f8343bf7c2c12"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:f469f15068cd8351826df4080ffe4cc6377c5bf7d29b5a07b0e717dddb4c7ea2"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-musllinux_1_1_aarch64.whl", hash = "sha256:cda283700c984e699e8ef0fcc5c61f00c9d14b6f65a4f2767c97242513fcdd84"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-musllinux_1_1_x86_64.whl", hash = "sha256:43699eb3f80920cc39a380c159ae21c8a8924fe071bccb68fc509e099420b148"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-win32.whl", hash = "sha256:61ada5831db36d897e28eb95f0f81814525e0d7927fb51145526c4e63174920b"},
+    {file = "SQLAlchemy-2.0.19-cp37-cp37m-win_amd64.whl", hash = "sha256:57d100a421d9ab4874f51285c059003292433c648df6abe6c9c904e5bd5b0828"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-macosx_10_9_x86_64.whl", hash = "sha256:16a310f5bc75a5b2ce7cb656d0e76eb13440b8354f927ff15cbaddd2523ee2d1"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-macosx_11_0_arm64.whl", hash = "sha256:cf7b5e3856cbf1876da4e9d9715546fa26b6e0ba1a682d5ed2fc3ca4c7c3ec5b"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:2e7b69d9ced4b53310a87117824b23c509c6fc1f692aa7272d47561347e133b6"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:8f9eb4575bfa5afc4b066528302bf12083da3175f71b64a43a7c0badda2be365"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-musllinux_1_1_aarch64.whl", hash = "sha256:6b54d1ad7a162857bb7c8ef689049c7cd9eae2f38864fc096d62ae10bc100c7d"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-musllinux_1_1_x86_64.whl", hash = "sha256:5d6afc41ca0ecf373366fd8e10aee2797128d3ae45eb8467b19da4899bcd1ee0"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-win32.whl", hash = "sha256:430614f18443b58ceb9dedec323ecddc0abb2b34e79d03503b5a7579cd73a531"},
+    {file = "SQLAlchemy-2.0.19-cp38-cp38-win_amd64.whl", hash = "sha256:eb60699de43ba1a1f77363f563bb2c652f7748127ba3a774f7cf2c7804aa0d3d"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-macosx_10_9_x86_64.whl", hash = "sha256:a752b7a9aceb0ba173955d4f780c64ee15a1a991f1c52d307d6215c6c73b3a4c"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-macosx_11_0_arm64.whl", hash = "sha256:7351c05db355da112e056a7b731253cbeffab9dfdb3be1e895368513c7d70106"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl", hash = "sha256:fa51ce4aea583b0c6b426f4b0563d3535c1c75986c4373a0987d84d22376585b"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl", hash = "sha256:ae7473a67cd82a41decfea58c0eac581209a0aa30f8bc9190926fbf628bb17f7"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-musllinux_1_1_aarch64.whl", hash = "sha256:851a37898a8a39783aab603c7348eb5b20d83c76a14766a43f56e6ad422d1ec8"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-musllinux_1_1_x86_64.whl", hash = "sha256:539010665c90e60c4a1650afe4ab49ca100c74e6aef882466f1de6471d414be7"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-win32.whl", hash = "sha256:f82c310ddf97b04e1392c33cf9a70909e0ae10a7e2ddc1d64495e3abdc5d19fb"},
+    {file = "SQLAlchemy-2.0.19-cp39-cp39-win_amd64.whl", hash = "sha256:8e712cfd2e07b801bc6b60fdf64853bc2bd0af33ca8fa46166a23fe11ce0dbb0"},
+    {file = "SQLAlchemy-2.0.19-py3-none-any.whl", hash = "sha256:314145c1389b021a9ad5aa3a18bac6f5d939f9087d7fc5443be28cba19d2c972"},
+    {file = "SQLAlchemy-2.0.19.tar.gz", hash = "sha256:77a14fa20264af73ddcdb1e2b9c5a829b8cc6b8304d0f093271980e36c200a3f"},
 ]
 
 [package.dependencies]
 greenlet = {version = "!=0.4.17", markers = "platform_machine == \"win32\" or platform_machine == \"WIN32\" or platform_machine == \"AMD64\" or platform_machine == \"amd64\" or platform_machine == \"x86_64\" or platform_machine == \"ppc64le\" or platform_machine == \"aarch64\""}
 typing-extensions = ">=4.2.0"
 
 [package.extras]
@@ -3537,21 +3541,21 @@
 h11 = ">=0.8"
 
 [package.extras]
 standard = ["colorama (>=0.4)", "httptools (>=0.5.0)", "python-dotenv (>=0.13)", "pyyaml (>=5.1)", "uvloop (>=0.14.0,!=0.15.0,!=0.15.1)", "watchfiles (>=0.13)", "websockets (>=10.4)"]
 
 [[package]]
 name = "virtualenv"
-version = "20.23.1"
+version = "20.24.0"
 description = "Virtual Python Environment builder"
 optional = false
 python-versions = ">=3.7"
 files = [
-    {file = "virtualenv-20.23.1-py3-none-any.whl", hash = "sha256:34da10f14fea9be20e0fd7f04aba9732f84e593dac291b757ce42e3368a39419"},
-    {file = "virtualenv-20.23.1.tar.gz", hash = "sha256:8ff19a38c1021c742148edc4f81cb43d7f8c6816d2ede2ab72af5b84c749ade1"},
+    {file = "virtualenv-20.24.0-py3-none-any.whl", hash = "sha256:18d1b37fc75cc2670625702d76849a91ebd383768b4e91382a8d51be3246049e"},
+    {file = "virtualenv-20.24.0.tar.gz", hash = "sha256:e2a7cef9da880d693b933db7654367754f14e20650dc60e8ee7385571f8593a3"},
 ]
 
 [package.dependencies]
 distlib = ">=0.3.6,<1"
 filelock = ">=3.12,<4"
 platformdirs = ">=3.5.1,<4"
 
@@ -3683,24 +3687,24 @@
     {file = "wrapt-1.15.0-cp39-cp39-win_amd64.whl", hash = "sha256:eef4d64c650f33347c1f9266fa5ae001440b232ad9b98f1f43dfe7a79435c0a6"},
     {file = "wrapt-1.15.0-py3-none-any.whl", hash = "sha256:64b1df0f83706b4ef4cfb4fb0e4c2669100fd7ecacfb59e091fad300d4e04640"},
     {file = "wrapt-1.15.0.tar.gz", hash = "sha256:d06730c6aed78cee4126234cf2d071e01b44b915e725a6cb439a879ec9754a3a"},
 ]
 
 [[package]]
 name = "zipp"
-version = "3.16.0"
+version = "3.16.2"
 description = "Backport of pathlib-compatible object wrapper for zip files"
 optional = false
 python-versions = ">=3.8"
 files = [
-    {file = "zipp-3.16.0-py3-none-any.whl", hash = "sha256:5dadc3ad0a1f825fe42ce1bce0f2fc5a13af2e6b2d386af5b0ff295bc0a287d3"},
-    {file = "zipp-3.16.0.tar.gz", hash = "sha256:1876cb065531855bbe83b6c489dcf69ecc28f1068d8e95959fe8bbc77774c941"},
+    {file = "zipp-3.16.2-py3-none-any.whl", hash = "sha256:679e51dd4403591b2d6838a48de3d283f3d188412a9782faadf845f298736ba0"},
+    {file = "zipp-3.16.2.tar.gz", hash = "sha256:ebc15946aa78bd63458992fc81ec3b6f7b1e92d51c35e6de1c3804e73b799147"},
 ]
 
 [package.extras]
 docs = ["furo", "jaraco.packaging (>=9.3)", "jaraco.tidelift (>=1.4)", "rst.linker (>=1.9)", "sphinx (>=3.5)", "sphinx-lint"]
-testing = ["big-O", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=2.2)", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
+testing = ["big-O", "jaraco.functools", "jaraco.itertools", "more-itertools", "pytest (>=6)", "pytest-black (>=0.3.7)", "pytest-checkdocs (>=2.4)", "pytest-cov", "pytest-enabler (>=2.2)", "pytest-ignore-flaky", "pytest-mypy (>=0.9.1)", "pytest-ruff"]
 
 [metadata]
 lock-version = "2.0"
 python-versions = ">=3.8, <3.11"
-content-hash = "cf4de03dd2db8969450768172fe750c8758737defc1329f206ca61c3e4fa49cd"
+content-hash = "1d07f28eb022fb5c4494dd202f423a268b5f5516d3f537cf7267256459bdf60e"
```

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,18 +43,18 @@
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
 ansys-optislang-core = "^0.3.0"
 ansys-saf-glow = {version = "0.3.0", source = "solutions-private-pypi"}
-ansys-saf-portal = {version = "0.3.0", source = "solutions-private-pypi"}
-ansys-solutions-dash-lib = {version = "^0.4.1", source = "solutions-private-pypi"}
+ansys-saf-portal = {version = "0.4.1", source = "solutions-private-pypi"}
+ansys-solutions-dash-lib = {version = "0.4.3", source = "solutions-private-pypi"}
 ansys-solutions-products-ecosystem = {version = "^0.1.dev0", source = "solutions-private-pypi"}
-ansys-solutions-optislang-frontend-components = {version = "^0.1.dev6", source = "solutions-private-pypi"}
+ansys-solutions-optislang-frontend-components = {version = "^0.1.dev7", source = "solutions-private-pypi"}
 optislang-dash-lib = {version = "^0.2.1", source = "solutions-private-pypi"}
 dash = "^2.6"
 dash_bootstrap_components = "^1.2"
 dash-extensions = "^0.1"
 dash-iconify = "^0.1"
 dash-loading-spinners = "^1.0.0"
 dash-uploader = "^0.6"
```

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/osl_project_tree.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/model/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/problem_setup_step.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # ©2023, ANSYS Inc. Unauthorized use, distribution or duplication is prohibited.
 
 """Backend of the problem setup step."""
 
+import os
 import json
 from pathlib import Path
 import platform
 import time
 from typing import List
-import subprocess
-import sys
+import tempfile
+
 
 from ansys.optislang.core import Optislang, logging
-from ansys.saf.glow.solution import FileReference, AssetFileReference, StepModel, StepSpec, long_running, transaction
+from ansys.saf.glow.solution import FileReference, FileGroupReference, StepModel, StepSpec, long_running, transaction
 from ansys.solutions.optislang.frontend_components.project_properties import ProjectProperties, write_properties_file, apply_placeholders_to_properties_file
 from ansys.solutions.products_ecosystem.controller import AnsysProductsEcosystemController
 from ansys.solutions.products_ecosystem.utils import convert_to_long_version
 
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.model.osl_project_tree import dump_project_state, get_project_tree, get_node_list, get_step_list
 from ansys.solutions.{{ cookiecutter.__solution_name_slug }}.ui.utils.monitoring import _get_actor_hids, read_optislang_logs
 
@@ -27,14 +28,15 @@
 
     # Frontend persistence
     ansys_ecosystem_ready: bool = False
     optislang_solve_status: str = "initial"  # initial, processing, finished, stopped, aborted, idle
     ui_placeholders: dict = {}
     app_metadata: dict = {}
     analysis_running: bool = False
+    analysis_locked: bool = True
 
     # Backend data model
     tcp_server_host: str = "127.0.0.1"
     tcp_server_port: int = None
     ansys_ecosystem: dict = {
         "optislang": {
             "authorized_versions": ["2022.2", "2023.1"],
@@ -66,14 +68,17 @@
     # File storage ----------------------------------------------------------------------------------------------------
 
     # Inputs
     project_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_application_archive_stem }}.opf")
     properties_file: FileReference = FileReference("Problem_Setup/{{ cookiecutter.__optiSLang_application_archive_stem }}.json")
     metadata_file: FileReference = FileReference("Problem_Setup/metadata.json")
     project_state_file: FileReference = FileReference("Problem_Setup/project_state.json")
+    input_files: FileGroupReference = FileGroupReference("Problem_Setup/Input_Files/*.*")
+    # If folder doesn't exist, it will be created later
+    upload_directory = os.path.join(tempfile.gettempdir(), "GLOW")
 
     # Outputs
     working_properties_file: FileReference = FileReference("Problem_Setup/working_properties_file.json")
     server_info_file: FileReference = FileReference("Problem_Setup/server_info.ini")
     optislang_log_file: FileReference = FileReference("Problem_Setup/pyoptislang.log")
 
     # Methods ---------------------------------------------------------------------------------------------------------
@@ -128,14 +133,46 @@
 
         original_metadata_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "metadata.json"
         self.metadata_file.write_bytes(original_metadata_file.read_bytes())
 
         original_project_state_file = Path(__file__).parent.absolute().parent / "model" / "assets" / "project_state.json"
         self.project_state_file.write_bytes(original_project_state_file.read_bytes())
 
+
+    @transaction(self=StepSpec(download=["properties_file"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    def get_default_placeholder_values(self):
+        """Get placeholder values and definitions using the ProjectProperties class."""
+        pp = ProjectProperties()
+        pp.read_file(self.properties_file.path)
+        self.placeholders = pp._placeholders
+        self.registered_files = pp._registered_files
+        self.settings = pp._settings
+        self.parameter_manager = pp._parameter_manager
+        self.criteria = pp._criteria
+
+    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["working_properties_file", "placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    def write_updated_properties_file(self) -> None:
+        properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
+        self.placeholders = properties["placeholders"]
+        self.registered_files = properties["registered_files"]
+        self.settings = properties["settings"]
+        self.parameter_manager = properties["parameter_manager"]
+        self.criteria = properties["criteria"]
+        write_properties_file(properties, Path(self.working_properties_file.path))
+
+
+    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
+    def update_osl_placeholders_with_ui_values(self) -> None:
+        properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
+        self.placeholders = properties["placeholders"]
+        self.registered_files = properties["registered_files"]
+        self.settings = properties["settings"]
+        self.parameter_manager = properties["parameter_manager"]
+        self.criteria = properties["criteria"]
+
     @transaction(
         self=StepSpec(
             upload=["ansys_ecosystem", "ansys_ecosystem_ready"],
         )
     )
     def check_ansys_ecosystem(self) -> None:
         """Check if Ansys Products are installed and if the appropriate versions are available."""
@@ -183,30 +220,14 @@
                     alert_message += f" {convert_to_long_version(compatible_version)}"
                 alert_message += ".\n"
                 alert_message += "Selected version is %s." % (self.ansys_ecosystem[product_name]["selected_version"])
                 alert_color = "success"
             self.ansys_ecosystem[product_name]["alert_message"] = alert_message
             self.ansys_ecosystem[product_name]["alert_color"] = alert_color
 
-    @transaction(self=StepSpec(download=["properties_file"], upload=["placeholders", "registered_files", "settings", "parameter_manager", "criteria"]))
-    def get_default_placeholder_values(self):
-        """Get placeholder values and definitions using the ProjectProperties class."""
-
-        pp = ProjectProperties()
-        pp.read_file(self.properties_file.path)
-        self.placeholders = pp._placeholders
-        self.registered_files = pp._registered_files
-        self.settings = pp._settings
-        self.parameter_manager = pp._parameter_manager
-        self.criteria = pp._criteria
-
-    @transaction(self=StepSpec(download=["properties_file", "ui_placeholders"], upload=["working_properties_file"]))
-    def write_updated_properties_file(self) -> None:
-        properties = apply_placeholders_to_properties_file(self.ui_placeholders, self.properties_file.path)
-        write_properties_file(properties, Path(self.working_properties_file.path))
 
     @transaction(
         self=StepSpec(
             download=["metadata_file"],
             upload=["app_metadata"]
         )
     )
@@ -300,7 +321,8 @@
             self.transaction.upload(["optislang_logs"])
             # Check if analysis stopped
             if self.optislang_solve_status in self.tcp_server_stopped_states:
                 break
             time.sleep(3)
 
         osl.dispose()
+
```

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_information_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/actor_statistics_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/design_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/logs_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/project_summary_table.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/summary_view.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/components/system_files.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/monitoring_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/alerts.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/common_functions.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/constants.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/monitoring.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/utils/placeholders.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/design_table_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/project_summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/scenery_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/status_overview_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/summary_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/views/visualization_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/osl_solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_fastapi/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/health.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/blueprints/version.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/src/static/swagger.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_flask/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/protobufs/pingserver.proto`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/client.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/observability/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/src/services/pinger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_grpc/{{cookiecutter.__project_name_slug}}/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/docker/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/logger.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyace_pkg/{{cookiecutter.__project_name_slug}}/src/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_advanced/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/build_and_test_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.github/workflows/generate_library.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/.m2/settings.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml` & `ansys_templates-1.2.0/src/ansys/templates/python/pyansys_openapi_client/{{cookiecutter.__project_name_slug}}/pom.xml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pybasic/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/pybasic/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pybasic/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pybasic/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py` & `ansys_templates-1.2.0/src/ansys/templates/python/pybasic/{{cookiecutter.__project_name_slug}}/setup.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/cookiecutter.json` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/hooks/post_gen_project.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/hooks/post_gen_project.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.gitignore`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/compose.yaml`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/.vale.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/Makefile`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/make.bat`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/_static/ansys-solutions-logo-black-background.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/poetry.lock`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 name = "PyPI"
 priority = "primary"
 
 [tool.poetry.dependencies]
 python = ">=3.8, <3.11"
 ansys-dash-treeview = {version = "0.0.1.dev0", source = "solutions-private-pypi"}
 ansys-saf-glow = {version = "0.3.0", source = "solutions-private-pypi" }
-ansys-saf-portal = {version = "0.3.0", source = "solutions-private-pypi"}
+ansys-saf-portal = {version = "0.4.1", source = "solutions-private-pypi"}
 ansys-solutions-dash-lib = {version = "^0.4", source = "solutions-private-pypi"}
 {% if cookiecutter.with_dash_ui == "yes" %}
 dash = "^2.6"
 dash_bootstrap_components = "^1.2"
 dash-extensions = "^0.1"
 dash-iconify = "^0.1"
 dash-uploader = "^0.6"
```

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/setup_environment.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/main.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/definition.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/solution/first_step.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/app.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/css/style.css`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/images/solution-workflow-sketch.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/assets/logos/ansys-solutions-horizontal-logo.png`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/first_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/intro_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/src/ansys/solutions/{{cookiecutter.__solution_name_slug}}/ui/pages/second_page.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini` & `ansys_templates-1.2.0/src/ansys/templates/python/solution/{{cookiecutter.__project_name_slug}}/tox.ini`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/testing.py` & `ansys_templates-1.2.0/src/ansys/templates/testing.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/src/ansys/templates/utils.py` & `ansys_templates-1.2.0/src/ansys/templates/utils.py`

 * *Files identical despite different names*

### Comparing `ansys_templates-1.1.1/PKG-INFO` & `ansys_templates-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-templates
-Version: 1.1.1
+Version: 1.2.0
 Summary: Creates Python projects according to PyAnsys guidelines
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAnsys developers <pyansys.maintainers@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3
```

