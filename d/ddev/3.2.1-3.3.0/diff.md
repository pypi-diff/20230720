# Comparing `tmp/ddev-3.2.1.tar.gz` & `tmp/ddev-3.3.0.tar.gz`

## Comparing `ddev-3.2.1.tar` & `ddev-3.3.0.tar`

### file list

```diff
@@ -1,117 +1,117 @@
--rw-r--r--   0        0        0     5550 2020-02-02 00:00:00.000000 ddev-3.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 ddev-3.2.1/pyoxidizer.bzl
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/__init__.py
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/__main__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/_version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/py.typed
--rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/__init__.py
--rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/application.py
--rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/terminal.py
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/ci/__init__.py
--rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/clean/__init__.py
--rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/config/__init__.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/docs/__init__.py
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/env/__init__.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/__init__.py
--rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/meta/scripts/upgrade_python.py
--rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/__init__.py
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/agent/__init__.py
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/list_versions/__init__.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/show/__init__.py
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/release/stats/__init__.py
--rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/status/__init__.py
--rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/__init__.py
--rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/ci.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/licenses.py
--rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/manifest.py
--rw-r--r--   0        0        0     2918 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/cli/validate/openmetrics.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/constants.py
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/file.py
--rw-r--r--   0        0        0    23643 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/model.py
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/config/utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/__init__.py
--rw-r--r--   0        0        0     3850 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/core.py
--rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/integration/manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/__init__.py
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/api.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/specs.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/__init__.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/hatch/__init__.py
--rw-r--r--   0        0        0     6031 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/hatch/environment_collector.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/__init__.py
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/__main__.py
--rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/plugin/external/starship/prompt.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/__init__.py
--rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/config.py
--rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/constants.py
--rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/repo/core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/__init__.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/ci.py
--rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/fs.py
--rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/git.py
--rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/github.py
--rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/json.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/network.py
--rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/platform.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/structures.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/toml.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/scripts/__init__.py
--rw-r--r--   0        0        0     9620 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/utils/scripts/ci_matrix.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/validation/__init__.py
--rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.2.1/src/ddev/validation/tracker.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/__init__.py
--rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/conftest.py
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/test__utils.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/clean/__init__.py
--rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/clean/test_clean.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/__init__.py
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_edit.py
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_explore.py
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_find.py
--rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_restore.py
--rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_set.py
--rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/config/test_show.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/__init__.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/scripts/__init__.py
--rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/meta/scripts/test_upgrade_python.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/release/__init__.py
--rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/release/test_list_versions.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/status/__init__.py
--rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/status/test_status.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/__init__.py
--rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_licenses.py
--rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_manifest.py
--rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/cli/validate/test_openmetrics.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/config/__init__.py
--rw-r--r--   0        0        0    40884 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/config/test_model.py
--rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/github/get_pr_found.yaml
--rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/github/get_pr_no_match.yaml
--rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
--rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/list_versions/success_disk.yaml
--rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/manifest/missing_app_uuid.yaml
--rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/fixtures/network/manifest/success.yaml
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/helpers/__init__.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/helpers/api.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/__init__.py
--rw-r--r--   0        0        0     7091 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/test_core.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/integration/test_manifest.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/__init__.py
--rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/test_config.py
--rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/repo/test_core.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_fs.py
--rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_git.py
--rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_github.py
--rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_json.py
--rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_platform.py
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/utils/test_structures.py
--rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/validation/__init__.py
--rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.2.1/tests/validation/test_tracker.py
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.2.1/.gitignore
--rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.2.1/README.md
--rw-r--r--   0        0        0      449 2020-02-02 00:00:00.000000 ddev-3.2.1/hatch.toml
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 ddev-3.2.1/pyproject.toml
--rw-r--r--   0        0        0     2014 2020-02-02 00:00:00.000000 ddev-3.2.1/PKG-INFO
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 ddev-3.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     2848 2020-02-02 00:00:00.000000 ddev-3.3.0/pyoxidizer.bzl
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/__init__.py
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/__main__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/_version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/py.typed
+-rw-r--r--   0        0        0     5435 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/__init__.py
+-rw-r--r--   0        0        0     3757 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/application.py
+-rw-r--r--   0        0        0    10141 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/terminal.py
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/ci/__init__.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/clean/__init__.py
+-rw-r--r--   0        0        0     4731 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/config/__init__.py
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/docs/__init__.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/env/__init__.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/meta/__init__.py
+-rw-r--r--   0        0        0      737 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     2575 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/meta/scripts/upgrade_python.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/release/__init__.py
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/release/agent/__init__.py
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/release/list_versions/__init__.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/release/show/__init__.py
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/release/stats/__init__.py
+-rw-r--r--   0        0        0      897 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/status/__init__.py
+-rw-r--r--   0        0        0     2889 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/validate/__init__.py
+-rw-r--r--   0        0        0     3996 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/validate/ci.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/validate/licenses.py
+-rw-r--r--   0        0        0     1872 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/validate/manifest.py
+-rw-r--r--   0        0        0     2618 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/cli/validate/openmetrics.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/config/__init__.py
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/config/constants.py
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/config/file.py
+-rw-r--r--   0        0        0    23643 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/config/model.py
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/config/utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/integration/__init__.py
+-rw-r--r--   0        0        0     4083 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/integration/core.py
+-rw-r--r--   0        0        0      249 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/integration/manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/__init__.py
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/api.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/specs.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/__init__.py
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/hatch/__init__.py
+-rw-r--r--   0        0        0     6030 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/hatch/environment_collector.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/starship/__init__.py
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/starship/__main__.py
+-rw-r--r--   0        0        0      297 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/plugin/external/starship/prompt.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/repo/__init__.py
+-rw-r--r--   0        0        0      501 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/repo/config.py
+-rw-r--r--   0        0        0      441 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/repo/constants.py
+-rw-r--r--   0        0        0     5336 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/repo/core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/__init__.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/ci.py
+-rw-r--r--   0        0        0     3465 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/fs.py
+-rw-r--r--   0        0        0     3765 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/git.py
+-rw-r--r--   0        0        0     3547 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/github.py
+-rw-r--r--   0        0        0     1490 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/json.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/network.py
+-rw-r--r--   0        0        0     6335 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/platform.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/structures.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/toml.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/scripts/__init__.py
+-rw-r--r--   0        0        0     9654 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/utils/scripts/ci_matrix.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/validation/__init__.py
+-rw-r--r--   0        0        0     3965 2020-02-02 00:00:00.000000 ddev-3.3.0/src/ddev/validation/tracker.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/__init__.py
+-rw-r--r--   0        0        0     6225 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/conftest.py
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/test__utils.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/clean/__init__.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/clean/test_clean.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/__init__.py
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_edit.py
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_explore.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_find.py
+-rw-r--r--   0        0        0      780 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_restore.py
+-rw-r--r--   0        0        0     3518 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_set.py
+-rw-r--r--   0        0        0     3062 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/config/test_show.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/meta/__init__.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/meta/scripts/__init__.py
+-rw-r--r--   0        0        0     1472 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/meta/scripts/test_upgrade_python.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/release/__init__.py
+-rw-r--r--   0        0        0     3885 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/release/test_list_versions.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/status/__init__.py
+-rw-r--r--   0        0        0     2597 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/status/test_status.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/validate/__init__.py
+-rw-r--r--   0        0        0     2026 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/validate/test_licenses.py
+-rw-r--r--   0        0        0     2847 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/validate/test_manifest.py
+-rw-r--r--   0        0        0     2473 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/cli/validate/test_openmetrics.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/config/__init__.py
+-rw-r--r--   0        0        0    40884 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/config/test_model.py
+-rw-r--r--   0        0        0     5430 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/github/get_pr_found.yaml
+-rw-r--r--   0        0        0     2200 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/github/get_pr_no_match.yaml
+-rw-r--r--   0        0        0    23688 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml
+-rw-r--r--   0        0        0     4867 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/list_versions/success_disk.yaml
+-rw-r--r--   0        0        0     5954 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/manifest/missing_app_uuid.yaml
+-rw-r--r--   0        0        0     5278 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/fixtures/network/manifest/success.yaml
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/helpers/__init__.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/helpers/api.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     7857 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/integration/test_core.py
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/integration/test_manifest.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/repo/__init__.py
+-rw-r--r--   0        0        0      295 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/repo/test_config.py
+-rw-r--r--   0        0        0     5816 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/repo/test_core.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     3577 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_fs.py
+-rw-r--r--   0        0        0     2870 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_git.py
+-rw-r--r--   0        0        0     1533 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_github.py
+-rw-r--r--   0        0        0     1332 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_json.py
+-rw-r--r--   0        0        0     2217 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_platform.py
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/utils/test_structures.py
+-rw-r--r--   0        0        0      115 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/validation/__init__.py
+-rw-r--r--   0        0        0     4981 2020-02-02 00:00:00.000000 ddev-3.3.0/tests/validation/test_tracker.py
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 ddev-3.3.0/.gitignore
+-rw-r--r--   0        0        0     1060 2020-02-02 00:00:00.000000 ddev-3.3.0/README.md
+-rw-r--r--   0        0        0      335 2020-02-02 00:00:00.000000 ddev-3.3.0/hatch.toml
+-rw-r--r--   0        0        0     2508 2020-02-02 00:00:00.000000 ddev-3.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2042 2020-02-02 00:00:00.000000 ddev-3.3.0/PKG-INFO
```

### Comparing `ddev-3.2.1/CHANGELOG.md` & `ddev-3.3.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,22 @@
 # CHANGELOG - ddev
 
+## 3.3.0 / 2023-07-20
+
+***Added***:
+
+* Upgrade datadog-checks-dev to 22.1. See [#15325](https://github.com/DataDog/integrations-core/pull/15325).
+* Upgrade click to 8.1.6. See [#15272](https://github.com/DataDog/integrations-core/pull/15272).
+* Update generated config models. See [#15212](https://github.com/DataDog/integrations-core/pull/15212).
+
+***Fixed***:
+
+* Add logic for integration package files. See [#14544](https://github.com/DataDog/integrations-core/pull/14544).
+* Add `snmp/data/default_profiles` to matrix TESTABLE_FILE_PATTERN. See [#15267](https://github.com/DataDog/integrations-core/pull/15267).
+
 ## 3.2.1 / 2023-07-10
 
 ***Fixed***:
 
 * Exclude click 8.1.4 to solve mypy issues. See [#15201](https://github.com/DataDog/integrations-core/pull/15201).
 
 ## 3.2.0 / 2023-07-05
@@ -21,139 +34,124 @@
 
 * Update version of datadog-checks-dev. See [#14865](https://github.com/DataDog/integrations-core/pull/14865).
 * Add Git utilities. See [#14838](https://github.com/DataDog/integrations-core/pull/14838).
 * Add pluggy to ddev dependencies. See [#14821](https://github.com/DataDog/integrations-core/pull/14821).
 
 ## 3.0.0 / 2023-06-20
 
-***Changed***: 
+***Changed***:
 
 * Remove `pyperclip` dependency and clipboard functionality. See [#14782](https://github.com/DataDog/integrations-core/pull/14782).
 
-***Added***: 
+***Added***:
 
 * Bump the minimum version of datadog-checks-dev. See [#14785](https://github.com/DataDog/integrations-core/pull/14785).
 * Upgrade Pydantic model code generator. See [#14779](https://github.com/DataDog/integrations-core/pull/14779).
 * Use Git for versioning. See [#14778](https://github.com/DataDog/integrations-core/pull/14778).
 * Add validations for removed dependencies. See [#14556](https://github.com/DataDog/integrations-core/pull/14556).
 * Migrate `clean` command. See [#14726](https://github.com/DataDog/integrations-core/pull/14726).
 * Add `release list` command to list integration version releases. See [#14687](https://github.com/DataDog/integrations-core/pull/14687).
 * Migrate command to upgrade Python. See [#14700](https://github.com/DataDog/integrations-core/pull/14700).
 
-***Fixed***: 
+***Fixed***:
 
 * Bump Python version from py3.8 to py3.9. See [#14701](https://github.com/DataDog/integrations-core/pull/14701).
 
-
 ## 2.1.0 / 2023-05-26
 
-***Added***: 
+***Added***:
 
 * Add validation for metric limit. See [#14528](https://github.com/DataDog/integrations-core/pull/14528).
 
-***Fixed***: 
+***Fixed***:
 
 * Consider changes to `metadata.csv` as testable. See [#14429](https://github.com/DataDog/integrations-core/pull/14429).
 * Account for dependency upgrades in CI matrix logic. See [#14366](https://github.com/DataDog/integrations-core/pull/14366).
 * Fix edge case in CI matrix construction. See [#14355](https://github.com/DataDog/integrations-core/pull/14355).
 
-
 ## 2.0.0 / 2023-04-11
 
-***Changed***: 
+***Changed***:
 
 * Replace flake8 and isort with Ruff. See [#14212](https://github.com/DataDog/integrations-core/pull/14212).
 
-
 ## 1.6.0 / 2023-03-31
 
-***Added***: 
+***Added***:
 
 * Add GitHub Actions workflows. See [#14187](https://github.com/DataDog/integrations-core/pull/14187).
 
-
 ## 1.5.0 / 2023-03-23
 
-***Added***: 
+***Added***:
 
 * Bump datadog-checks-dev to 18.x. See [#14225](https://github.com/DataDog/integrations-core/pull/14225).
 
-
 ## 1.4.3 / 2023-03-01
 
-***Fixed***: 
+***Fixed***:
 
 * Bump datadog_checks_dev dependency version. See [#14064](https://github.com/DataDog/integrations-core/pull/14064).
 
-
 ## 1.4.2 / 2023-02-27
 
-***Fixed***: 
+***Fixed***:
 
 * Bump datadog_checks_dev dependency version. See [#14040](https://github.com/DataDog/integrations-core/pull/14040).
 
-
 ## 1.4.1 / 2023-01-25
 
-***Fixed***: 
+***Fixed***:
 
 * Pin and bump the datadog_checks_dev version. See [#13557](https://github.com/DataDog/integrations-core/pull/13557).
 
-
 ## 1.4.0 / 2023-01-20
 
-***Added***: 
+***Added***:
 
 * Update manifest validation. See [#13637](https://github.com/DataDog/integrations-core/pull/13637).
 * Standardize integration selection. See [#13570](https://github.com/DataDog/integrations-core/pull/13570).
 
-***Fixed***: 
+***Fixed***:
 
 * And fallbacks to some org config options. See [#13629](https://github.com/DataDog/integrations-core/pull/13629).
 
-
 ## 1.3.0 / 2022-12-09
 
-***Added***: 
+***Added***:
 
 * Add `validate license-header` subcommand. See [#13417](https://github.com/DataDog/integrations-core/pull/13417).
 * Add JSON Pointer utilities. See [#13464](https://github.com/DataDog/integrations-core/pull/13464).
 * Add utility for displaying warnings and errors. See [#13427](https://github.com/DataDog/integrations-core/pull/13427).
 * Add `config` commands. See [#13412](https://github.com/DataDog/integrations-core/pull/13412).
 
-***Fixed***: 
+***Fixed***:
 
 * Bump datadog_checks_dev dependency to 17.5.0. See [#13490](https://github.com/DataDog/integrations-core/pull/13490).
 * Output non-critical information to stderr. See [#13459](https://github.com/DataDog/integrations-core/pull/13459).
 
-
 ## 1.2.0 / 2022-11-23
 
-***Added***: 
+***Added***:
 
 * Upgrade dependencies. See [#13375](https://github.com/DataDog/integrations-core/pull/13375).
 
-
 ## 1.1.0 / 2022-10-28
 
-***Added***: 
+***Added***:
 
 * Add `status` command. See [#13197](https://github.com/DataDog/integrations-core/pull/13197).
 * Add Git utilities. See [#13185](https://github.com/DataDog/integrations-core/pull/13185).
 * Add utilities for filtering integrations. See [#13156](https://github.com/DataDog/integrations-core/pull/13156).
 * Add more utilities. See [#13136](https://github.com/DataDog/integrations-core/pull/13136).
 
-
 ## 1.0.1 / 2022-09-16
 
-***Fixed***: 
+***Fixed***:
 
 * Fix legacy tooling initialization when using the --here flag. See [#12823](https://github.com/DataDog/integrations-core/pull/12823).
 
-
 ## 1.0.0 / 2022-08-05
 
-***Added***: 
+***Added***:
 
 * Make ddev a standalone package. See [#12565](https://github.com/DataDog/integrations-core/pull/12565).
-
-
```

### Comparing `ddev-3.2.1/pyoxidizer.bzl` & `ddev-3.3.0/pyoxidizer.bzl`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/__init__.py` & `ddev-3.3.0/src/ddev/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/application.py` & `ddev-3.3.0/src/ddev/cli/application.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/terminal.py` & `ddev-3.3.0/src/ddev/cli/terminal.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/clean/__init__.py` & `ddev-3.3.0/src/ddev/cli/clean/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/config/__init__.py` & `ddev-3.3.0/src/ddev/cli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/env/__init__.py` & `ddev-3.3.0/src/ddev/cli/env/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/meta/__init__.py` & `ddev-3.3.0/src/ddev/cli/meta/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/meta/scripts/__init__.py` & `ddev-3.3.0/src/ddev/cli/meta/scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/meta/scripts/upgrade_python.py` & `ddev-3.3.0/src/ddev/cli/meta/scripts/upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/release/__init__.py` & `ddev-3.3.0/src/ddev/cli/release/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/release/agent/__init__.py` & `ddev-3.3.0/src/ddev/cli/release/agent/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/release/list_versions/__init__.py` & `ddev-3.3.0/src/ddev/cli/release/list_versions/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/release/show/__init__.py` & `ddev-3.3.0/src/ddev/cli/release/show/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/status/__init__.py` & `ddev-3.3.0/src/ddev/cli/status/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/validate/__init__.py` & `ddev-3.3.0/src/ddev/cli/validate/__init__.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/validate/ci.py` & `ddev-3.3.0/src/ddev/cli/validate/ci.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/validate/licenses.py` & `ddev-3.3.0/src/ddev/cli/validate/licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/cli/validate/manifest.py` & `ddev-3.3.0/src/ddev/cli/validate/manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/config/file.py` & `ddev-3.3.0/src/ddev/config/file.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/config/model.py` & `ddev-3.3.0/src/ddev/config/model.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/config/utils.py` & `ddev-3.3.0/src/ddev/config/utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/integration/core.py` & `ddev-3.3.0/src/ddev/integration/core.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
 from __future__ import annotations
 
+import os
 from functools import cached_property
-from typing import TYPE_CHECKING
+from typing import TYPE_CHECKING, Iterator
 
 from ddev.repo.constants import NOT_SHIPPABLE
+from ddev.utils.fs import Path
 
 if TYPE_CHECKING:
     from ddev.integration.manifest import Manifest
     from ddev.repo.config import RepositoryConfig
-    from ddev.utils.fs import Path
 
 
 class Integration:
     def __init__(self, path: Path, repo_path: Path, repo_config: RepositoryConfig):
         # Do nothing but simple assignment here as we initialize often without
         # use just to access the `is_*` properties
         self.__path = path
@@ -55,14 +56,20 @@
             elif self.name == 'datadog_checks_downloader':
                 directory = 'downloader'
             else:
                 directory = self.package_directory_name
 
             return self.path / 'datadog_checks' / directory
 
+    def package_files(self) -> Iterator[Path]:
+        for root, _, files in os.walk(self.package_directory):
+            for f in files:
+                if f.endswith('.py'):
+                    yield Path(root, f)
+
     @property
     def release_tag_pattern(self) -> str:
         version_part = r'\d+\.\d+\.\d+'
         if self.name == 'ddev':
             version_part = f'v{version_part}'
 
         return f'{self.name}-{version_part}'
```

### Comparing `ddev-3.2.1/src/ddev/plugin/external/hatch/environment_collector.py` & `ddev-3.3.0/src/ddev/plugin/external/hatch/environment_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
                 'all': ['style'],
             },
             # We pin deps in order to make CI more stable/reliable.
             'dependencies': [
                 'black==22.12.0',
                 'ruff==0.0.257',
                 # Keep in sync with: /datadog_checks_base/pyproject.toml
-                'pydantic==1.10.8',
+                'pydantic==2.0.2',
             ],
         }
         config = {'lint': lint_env}
 
         if self.check_types:
             lint_env['scripts']['typing'] = [
                 f'mypy --config-file=../pyproject.toml {" ".join(self.mypy_args)}'.rstrip()
```

### Comparing `ddev-3.2.1/src/ddev/repo/core.py` & `ddev-3.3.0/src/ddev/repo/core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/fs.py` & `ddev-3.3.0/src/ddev/utils/fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/git.py` & `ddev-3.3.0/src/ddev/utils/git.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/github.py` & `ddev-3.3.0/src/ddev/utils/github.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/json.py` & `ddev-3.3.0/src/ddev/utils/json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/platform.py` & `ddev-3.3.0/src/ddev/utils/platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/structures.py` & `ddev-3.3.0/src/ddev/utils/structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/src/ddev/utils/scripts/ci_matrix.py` & `ddev-3.3.0/src/ddev/utils/scripts/ci_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     r"""
     assets/configuration/.+
   | tests/.+
   | [^/]+\.py
   | hatch\.toml
   | metadata\.csv
   | pyproject\.toml
+  | snmp/data/default_profiles/.+
     """,
     re.VERBOSE,
 )
 AGENT_REQUIREMENTS_FILE = 'datadog_checks_base/datadog_checks/base/data/agent_requirements.in'
 NON_TESTABLE_FILES = {'auto_conf.yaml'}
 DISPLAY_ORDER_OVERRIDE = {
     _d: _i
```

### Comparing `ddev-3.2.1/src/ddev/validation/tracker.py` & `ddev-3.3.0/src/ddev/validation/tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/conftest.py` & `ddev-3.3.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/test__utils.py` & `ddev-3.3.0/tests/test__utils.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/clean/test_clean.py` & `ddev-3.3.0/tests/cli/clean/test_clean.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/config/test_restore.py` & `ddev-3.3.0/tests/cli/config/test_restore.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/config/test_set.py` & `ddev-3.3.0/tests/cli/config/test_set.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/config/test_show.py` & `ddev-3.3.0/tests/cli/config/test_show.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/meta/scripts/test_upgrade_python.py` & `ddev-3.3.0/tests/cli/meta/scripts/test_upgrade_python.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/release/test_list_versions.py` & `ddev-3.3.0/tests/cli/release/test_list_versions.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/status/test_status.py` & `ddev-3.3.0/tests/cli/status/test_status.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/validate/test_licenses.py` & `ddev-3.3.0/tests/cli/validate/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/validate/test_manifest.py` & `ddev-3.3.0/tests/cli/validate/test_manifest.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/cli/validate/test_openmetrics.py` & `ddev-3.3.0/tests/cli/validate/test_openmetrics.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 import pytest
 
 
+@pytest.mark.usefixtures('repository')
 @pytest.mark.parametrize(
-    "check_name",
+    "check_name, classes",
     [
-        pytest.param("aerospike", id="Aerospike check.py OpenMetricsV2"),
-        pytest.param("amazon_msk", id="Amazon MSK amazon_msk.py OpenMetricsV1 and V2"),
+        pytest.param("aerospike", 1, id="Aerospike check.py OpenMetricsV2"),
+        pytest.param("amazon_msk", 2, id="Amazon MSK amazon_msk.py OpenMetricsV1 and V2"),
     ],
 )
-def test_openmetrics_pass_single_parameter(ddev, repository, check_name, helpers, network_replay):
+def test_openmetrics_pass_single_parameter(ddev, helpers, check_name, classes):
     result = ddev("validate", "openmetrics", check_name)
 
     assert result.exit_code == 0, result.output
 
     assert helpers.remove_trailing_spaces(result.output) == helpers.dedent(
-        """
+        f"""
         Validating default metric limit for OpenMetrics integrations ...
-        OpenMetrics Metric limit
+        OpenMetrics metric limit
 
-        Passed: 1
+        Passed: {classes}
         """
     )
 
 
-def test_openmetrics_fail_single_parameter(ddev, helpers, repository, network_replay):
+def test_openmetrics_fail_single_parameter(ddev, helpers, repository):
     missing_metric_limit = '''
             class ArangodbCheck(OpenMetricsBaseCheckV2, ConfigMixin):
             __NAMESPACE__ = 'arangodb'
             def __init__(self, name, init_config, instances):
                 super(ArangodbCheck, self).__init__(name, init_config, instances)
         '''
 
@@ -40,34 +41,36 @@
     result = ddev("validate", "openmetrics", "arangodb")
 
     assert result.exit_code == 1, result.output
 
     assert "Errors: 1" in helpers.remove_trailing_spaces(result.output)
 
 
-def test_openmetrics_skip_openmetrics(ddev, helpers, repository, network_replay):
+@pytest.mark.usefixtures('repository')
+def test_openmetrics_skip_openmetrics(ddev, helpers):
     result = ddev("validate", "openmetrics", "openmetrics")
 
     assert result.exit_code == 0, result.output
 
     assert "Passed" not in helpers.remove_trailing_spaces(result.output)
     assert "Errors" not in helpers.remove_trailing_spaces(result.output)
 
 
+@pytest.mark.usefixtures('repository')
 @pytest.mark.parametrize(
     "repo, expected_message",
     [
         pytest.param("core", "Passed:", id="Core integrations"),
         pytest.param(
             "marketplace",
             "OpenMetrics validations is only enabled for core or extras integrations, skipping for repo marketplace",
             id="Marketplace integrations",
         ),
     ],
 )
-def test_openmetrics_validate_repo(repo, repository, expected_message, ddev, helpers, config_file):
+def test_openmetrics_validate_repo(repo, expected_message, ddev, helpers, config_file):
     config_file.model.repo = repo
     config_file.save()
 
     result = ddev("validate", "openmetrics", "all")
 
     assert expected_message in helpers.remove_trailing_spaces(result.output)
```

### Comparing `ddev-3.2.1/tests/config/test_model.py` & `ddev-3.3.0/tests/config/test_model.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/github/get_pr_found.yaml` & `ddev-3.3.0/tests/fixtures/network/github/get_pr_found.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/github/get_pr_no_match.yaml` & `ddev-3.3.0/tests/fixtures/network/github/get_pr_no_match.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml` & `ddev-3.3.0/tests/fixtures/network/list_versions/success_datadog_checks_base.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/list_versions/success_disk.yaml` & `ddev-3.3.0/tests/fixtures/network/list_versions/success_disk.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/manifest/missing_app_uuid.yaml` & `ddev-3.3.0/tests/fixtures/network/manifest/missing_app_uuid.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/fixtures/network/manifest/success.yaml` & `ddev-3.3.0/tests/fixtures/network/manifest/success.yaml`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/helpers/api.py` & `ddev-3.3.0/tests/helpers/api.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/integration/test_core.py` & `ddev-3.3.0/tests/integration/test_core.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,14 @@
 # (C) Datadog, Inc. 2022-present
 # All rights reserved
 # Licensed under a 3-clause BSD style license (see LICENSE)
+import os
+
 from ddev.repo.core import Repository
+from ddev.utils.fs import Path
 
 
 def test_attributes(local_repo, valid_integration):
     repo = Repository(local_repo.name, str(local_repo))
     integration = repo.integrations.get(valid_integration)
 
     expected_path = repo.path / valid_integration
@@ -185,14 +188,34 @@
     def test_normalization(self, local_repo):
         repo = Repository(local_repo.name, str(local_repo))
         integration = repo.integrations.get('go-metro')
 
         assert integration.package_directory == local_repo / integration.name / 'datadog_checks' / 'go_metro'
 
 
+class TestPackageFiles:
+    def test_base_package_file(self, local_repo):
+        repo = Repository(local_repo.name, str(local_repo))
+        integration = repo.integrations.get('datadog_checks_base')
+
+        expected_files = []
+        for root, _, files in os.walk(integration.package_directory):
+            for f in files:
+                if f.endswith(".py"):
+                    expected_files.append(Path(root, f))
+
+        assert list(integration.package_files()) == expected_files
+
+    def test_tile_only_package_file(self, local_repo):
+        repo = Repository(local_repo.name, str(local_repo))
+        integration = repo.integrations.get('agent_metrics')
+
+        assert not list(integration.package_files())
+
+
 class TestReleaseTagPattern:
     def test_shipped(self, local_repo):
         repo = Repository(local_repo.name, str(local_repo))
         integration = repo.integrations.get('datadog_checks_base')
 
         assert integration.release_tag_pattern == r'datadog_checks_base-\d+\.\d+\.\d+'
```

### Comparing `ddev-3.2.1/tests/repo/test_core.py` & `ddev-3.3.0/tests/repo/test_core.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_fs.py` & `ddev-3.3.0/tests/utils/test_fs.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_git.py` & `ddev-3.3.0/tests/utils/test_git.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_github.py` & `ddev-3.3.0/tests/utils/test_github.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_json.py` & `ddev-3.3.0/tests/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_platform.py` & `ddev-3.3.0/tests/utils/test_platform.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/utils/test_structures.py` & `ddev-3.3.0/tests/utils/test_structures.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/tests/validation/test_tracker.py` & `ddev-3.3.0/tests/validation/test_tracker.py`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/.gitignore` & `ddev-3.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/README.md` & `ddev-3.3.0/README.md`

 * *Files identical despite different names*

### Comparing `ddev-3.2.1/pyproject.toml` & `ddev-3.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,16 @@
     "Intended Audience :: System Administrators",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.9",
 ]
 dependencies = [
-    "datadog-checks-dev[cli]~=22.0",
+    "click~=8.1.6",
+    "datadog-checks-dev[cli]~=22.1",
     "hatch>=1.6.3",
     "httpx",
     "jsonpointer",
     "pluggy",
     "rich>=12.5.1",
     "tomli; python_version < '3.11'",
     "tomli-w",
```

### Comparing `ddev-3.2.1/PKG-INFO` & `ddev-3.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: ddev
-Version: 3.2.1
+Version: 3.3.0
 Summary: The Datadog Agent integration developer tool
 Project-URL: Source, https://github.com/DataDog/integrations-core
 Author-email: Datadog <packages@datadoghq.com>
 License-Expression: BSD-3-Clause
 Keywords: agent,datadog,integration
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
-Requires-Dist: datadog-checks-dev[cli]~=22.0
+Requires-Dist: click~=8.1.6
+Requires-Dist: datadog-checks-dev[cli]~=22.1
 Requires-Dist: hatch>=1.6.3
 Requires-Dist: httpx
 Requires-Dist: jsonpointer
 Requires-Dist: pluggy
 Requires-Dist: rich>=12.5.1
 Requires-Dist: tomli-w
 Requires-Dist: tomli; python_version < '3.11'
```

