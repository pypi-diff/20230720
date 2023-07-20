# Comparing `tmp/idf_build_apps-1.0.3.tar.gz` & `tmp/idf_build_apps-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idf_build_apps-1.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "idf_build_apps-1.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `idf_build_apps-1.0.3.tar` & `idf_build_apps-1.0.4.tar`

### file list

```diff
@@ -1,52 +1,52 @@
--rw-r--r--   0        0        0      351 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.editorconfig
--rw-r--r--   0        0        0      123 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.git-blame-ignore-revs
--rw-r--r--   0        0        0       25 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.gitattributes
--rw-r--r--   0        0        0      513 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/dependabot.yml
--rw-r--r--   0        0        0      253 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/check-pre-commit.yml
--rw-r--r--   0        0        0      675 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/issue_comment.yml
--rw-r--r--   0        0        0      620 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/new_issues.yml
--rw-r--r--   0        0        0      796 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/new_prs.yml
--rw-r--r--   0        0        0      438 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/publish-pypi.yml
--rw-r--r--   0        0        0      521 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/test-build-docs.yml
--rw-r--r--   0        0        0     3870 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.github/workflows/test-build-idf-apps.yml
--rw-r--r--   0        0        0     3076 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.gitignore
--rw-r--r--   0        0        0     1077 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      383 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/.readthedocs.yml
--rw-r--r--   0        0        0     5583 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/CHANGELOG.md
--rw-r--r--   0        0        0     1882 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/CONTRIBUTING.md
--rw-r--r--   0        0        0    11358 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/LICENSE
--rw-r--r--   0        0        0     3843 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/README.md
--rw-r--r--   0        0        0       33 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/CHANGELOG.md
--rw-r--r--   0        0        0       36 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/CONTRIBUTING.md
--rw-r--r--   0        0        0      634 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/Makefile
--rw-r--r--   0        0        0     6947 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_static/espressif-logo.svg
--rw-r--r--   0        0        0      942 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_static/theme_overrides.css
--rw-r--r--   0        0        0      119 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/_templates/layout.html
--rw-r--r--   0        0        0      490 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/api.rst
--rw-r--r--   0        0        0     1449 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/conf.py
--rw-r--r--   0        0        0     2652 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/config_file.md
--rw-r--r--   0        0        0    10473 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/find_build.md
--rw-r--r--   0        0        0      474 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/index.rst
--rw-r--r--   0        0        0     5894 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/docs/manifest.md
--rw-r--r--   0        0        0      481 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/__init__.py
--rw-r--r--   0        0        0      182 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/__main__.py
--rw-r--r--   0        0        0    27235 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/app.py
--rw-r--r--   0        0        0     2794 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/config.py
--rw-r--r--   0        0        0     2182 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/constants.py
--rw-r--r--   0        0        0     6328 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/finder.py
--rw-r--r--   0        0        0     2220 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/log.py
--rw-r--r--   0        0        0    30514 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/main.py
--rw-r--r--   0        0        0      133 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/__init__.py
--rw-r--r--   0        0        0     6368 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/if_parser.py
--rw-r--r--   0        0        0     5956 2023-07-19 02:39:01.631996 idf_build_apps-1.0.3/idf_build_apps/manifest/manifest.py
--rw-r--r--   0        0        0     3423 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/idf_build_apps/manifest/soc_header.py
--rw-r--r--   0        0        0     7081 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/idf_build_apps/utils.py
--rw-r--r--   0        0        0      101 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/license_header.txt
--rw-r--r--   0        0        0     2060 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/pyproject.toml
--rw-r--r--   0        0        0     1221 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/conftest.py
--rw-r--r--   0        0        0     3347 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_build.py
--rw-r--r--   0        0        0    17534 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_finder.py
--rw-r--r--   0        0        0     1568 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_manifest.py
--rw-r--r--   0        0        0     3710 2023-07-19 02:39:01.635996 idf_build_apps-1.0.3/tests/test_utils.py
--rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.3/setup.py
--rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.3/PKG-INFO
+-rw-r--r--   0        0        0      351 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.editorconfig
+-rw-r--r--   0        0        0      123 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.git-blame-ignore-revs
+-rw-r--r--   0        0        0       25 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.gitattributes
+-rw-r--r--   0        0        0      513 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/dependabot.yml
+-rw-r--r--   0        0        0      253 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/check-pre-commit.yml
+-rw-r--r--   0        0        0      675 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/issue_comment.yml
+-rw-r--r--   0        0        0      620 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/new_issues.yml
+-rw-r--r--   0        0        0      796 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/new_prs.yml
+-rw-r--r--   0        0        0      438 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/publish-pypi.yml
+-rw-r--r--   0        0        0      521 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/test-build-docs.yml
+-rw-r--r--   0        0        0     3870 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.github/workflows/test-build-idf-apps.yml
+-rw-r--r--   0        0        0     3076 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.gitignore
+-rw-r--r--   0        0        0     1077 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      383 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/.readthedocs.yml
+-rw-r--r--   0        0        0     5702 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/CHANGELOG.md
+-rw-r--r--   0        0        0     1882 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/CONTRIBUTING.md
+-rw-r--r--   0        0        0    11358 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/LICENSE
+-rw-r--r--   0        0        0     3843 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/README.md
+-rw-r--r--   0        0        0       33 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/CHANGELOG.md
+-rw-r--r--   0        0        0       36 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/CONTRIBUTING.md
+-rw-r--r--   0        0        0      634 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/Makefile
+-rw-r--r--   0        0        0     6947 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_static/espressif-logo.svg
+-rw-r--r--   0        0        0      942 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_static/theme_overrides.css
+-rw-r--r--   0        0        0      119 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/_templates/layout.html
+-rw-r--r--   0        0        0      490 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/api.rst
+-rw-r--r--   0        0        0     1449 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/conf.py
+-rw-r--r--   0        0        0     2652 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/config_file.md
+-rw-r--r--   0        0        0    10473 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/find_build.md
+-rw-r--r--   0        0        0      474 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/index.rst
+-rw-r--r--   0        0        0     5894 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/docs/manifest.md
+-rw-r--r--   0        0        0      481 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/__init__.py
+-rw-r--r--   0        0        0      182 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/__main__.py
+-rw-r--r--   0        0        0    27235 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/app.py
+-rw-r--r--   0        0        0     2794 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/config.py
+-rw-r--r--   0        0        0     2182 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/constants.py
+-rw-r--r--   0        0        0     6328 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/finder.py
+-rw-r--r--   0        0        0     2220 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/log.py
+-rw-r--r--   0        0        0    30514 2023-07-20 09:25:13.138605 idf_build_apps-1.0.4/idf_build_apps/main.py
+-rw-r--r--   0        0        0      133 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/__init__.py
+-rw-r--r--   0        0        0     6368 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/if_parser.py
+-rw-r--r--   0        0        0     6535 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/manifest.py
+-rw-r--r--   0        0        0     3423 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/manifest/soc_header.py
+-rw-r--r--   0        0        0     7081 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/idf_build_apps/utils.py
+-rw-r--r--   0        0        0      101 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/license_header.txt
+-rw-r--r--   0        0        0     2060 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1221 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/conftest.py
+-rw-r--r--   0        0        0     3347 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_build.py
+-rw-r--r--   0        0        0    18222 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_finder.py
+-rw-r--r--   0        0        0     1568 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_manifest.py
+-rw-r--r--   0        0        0     3710 2023-07-20 09:25:13.142605 idf_build_apps-1.0.4/tests/test_utils.py
+-rw-r--r--   0        0        0     1115 1970-01-01 00:00:00.000000 idf_build_apps-1.0.4/setup.py
+-rw-r--r--   0        0        0     5540 1970-01-01 00:00:00.000000 idf_build_apps-1.0.4/PKG-INFO
```

### Comparing `idf_build_apps-1.0.3/.github/dependabot.yml` & `idf_build_apps-1.0.4/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.github/workflows/issue_comment.yml` & `idf_build_apps-1.0.4/.github/workflows/issue_comment.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.github/workflows/new_issues.yml` & `idf_build_apps-1.0.4/.github/workflows/new_issues.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.github/workflows/new_prs.yml` & `idf_build_apps-1.0.4/.github/workflows/new_prs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.github/workflows/test-build-docs.yml` & `idf_build_apps-1.0.4/.github/workflows/test-build-docs.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.github/workflows/test-build-idf-apps.yml` & `idf_build_apps-1.0.4/.github/workflows/test-build-idf-apps.yml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.gitignore` & `idf_build_apps-1.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/.pre-commit-config.yaml` & `idf_build_apps-1.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/CHANGELOG.md` & `idf_build_apps-1.0.4/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
+## v1.0.4 (2023-07-20)
+
+### Fix
+
+- stop overriding supported targets with sdkconfig file defined one for disabled app
+
 ## v1.0.3 (2023-07-19)
 
 ### Fix
 
 - correct final reports with skipped apps and failed built apps
 - skip while collecting only when both depend components and files unmatched
```

### Comparing `idf_build_apps-1.0.3/CONTRIBUTING.md` & `idf_build_apps-1.0.4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/LICENSE` & `idf_build_apps-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/README.md` & `idf_build_apps-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/Makefile` & `idf_build_apps-1.0.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/_static/espressif-logo.svg` & `idf_build_apps-1.0.4/docs/_static/espressif-logo.svg`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/_static/theme_overrides.css` & `idf_build_apps-1.0.4/docs/_static/theme_overrides.css`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/conf.py` & `idf_build_apps-1.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/config_file.md` & `idf_build_apps-1.0.4/docs/config_file.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/find_build.md` & `idf_build_apps-1.0.4/docs/find_build.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/docs/manifest.md` & `idf_build_apps-1.0.4/docs/manifest.md`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/app.py` & `idf_build_apps-1.0.4/idf_build_apps/app.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/config.py` & `idf_build_apps-1.0.4/idf_build_apps/config.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/constants.py` & `idf_build_apps-1.0.4/idf_build_apps/constants.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/finder.py` & `idf_build_apps-1.0.4/idf_build_apps/finder.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/log.py` & `idf_build_apps-1.0.4/idf_build_apps/log.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/main.py` & `idf_build_apps-1.0.4/idf_build_apps/main.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/manifest/if_parser.py` & `idf_build_apps-1.0.4/idf_build_apps/manifest/if_parser.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/manifest/manifest.py` & `idf_build_apps-1.0.4/idf_build_apps/manifest/manifest.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,17 @@
 import os.path
 from pathlib import (
     Path,
 )
 
 import yaml
 
+from .. import (
+    LOGGER,
+)
 from ..constants import (
     ALL_TARGETS,
     SUPPORTED_TARGETS,
 )
 from .if_parser import (
     BOOL_EXPR,
     BoolExpr,
@@ -101,16 +104,29 @@
         self, default_sdkconfig_target=None, config_name=None
     ):  # type: (str | None, str | None) -> list[str]
         res = []
         for target in ALL_TARGETS:
             if self._enable_build(target, config_name):
                 res.append(target)
 
-        if default_sdkconfig_target and res != [default_sdkconfig_target]:
-            res = [default_sdkconfig_target]
+        if default_sdkconfig_target:
+            if default_sdkconfig_target not in res:
+                LOGGER.warning(
+                    'sdkconfig defined `CONFIG_IDF_TARGET=%s` is not enabled for folder %s. Skip building this App...',
+                    default_sdkconfig_target,
+                    self.folder,
+                )
+                return []
+            else:
+                LOGGER.debug(
+                    'sdkconfig defined `CONFIG_IDF_TARGET=%s` overrides the supported targets for folder %s',
+                    default_sdkconfig_target,
+                    self.folder,
+                )
+                res = [default_sdkconfig_target]
 
         return sorted(res)
 
     def enable_test_targets(
         self, default_sdkconfig_target=None, config_name=None
     ):  # type: (str | None, str | None) -> list[str]
         res = []
```

### Comparing `idf_build_apps-1.0.3/idf_build_apps/manifest/soc_header.py` & `idf_build_apps-1.0.4/idf_build_apps/manifest/soc_header.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/idf_build_apps/utils.py` & `idf_build_apps-1.0.4/idf_build_apps/utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/pyproject.toml` & `idf_build_apps-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -56,15 +56,15 @@
 changelog = "https://github.com/espressif/idf-build-apps/blob/master/CHANGELOG.md"
 
 [project.scripts]
 idf-build-apps = "idf_build_apps:main.main"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.3"
+version = "1.0.4"
 tag_format = "v$version"
 version_files = [
     "idf_build_apps/__init__.py",
 ]
 
 [tool.pytest.ini_options]
 addopts = "-s --log-cli-level DEBUG"
```

### Comparing `idf_build_apps-1.0.3/tests/conftest.py` & `idf_build_apps-1.0.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/tests/test_build.py` & `idf_build_apps-1.0.4/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/tests/test_finder.py` & `idf_build_apps-1.0.4/tests/test_finder.py`

 * *Files 2% similar despite different names*

```diff
@@ -314,14 +314,36 @@
         finally:
             try:
                 os.remove(_default_sdkconfig_path)
                 logging.info('Removed temp %s %s', DEFAULT_SDKCONFIG, _default_sdkconfig_path)
             except:  # noqa
                 pass
 
+    def test_with_sdkconfig_defaults_idf_target_but_disabled(self, tmp_path):
+        manifest_file = tmp_path / 'manifest.yml'
+        manifest_file.write_text(
+            f'''
+{IDF_PATH}/examples:
+    disable:
+       - if: IDF_TARGET == "esp32s2"
+'''
+        )
+
+        sdkconfig_defaults = tmp_path / 'sdkconfig.defaults'
+        sdkconfig_defaults.write_text('CONFIG_IDF_TARGET="esp32s2"')
+
+        test_dir = str(IDF_PATH / 'examples' / 'get-started' / 'hello_world')
+        assert not find_apps(
+            test_dir,
+            'esp32s2',
+            recursive=True,
+            sdkconfig_defaults=str(sdkconfig_defaults),
+            manifest_files=[manifest_file],
+        )
+
     def test_with_config_rules(self, tmp_path, monkeypatch):
         create_project('test1', tmp_path)
 
         (tmp_path / 'test1' / 'sdkconfig.defaults').touch()
         (tmp_path / 'test1' / 'sdkconfig.defaults_new').touch()
         (tmp_path / 'test1' / 'sdkconfig.ci.foo').touch()
```

### Comparing `idf_build_apps-1.0.3/tests/test_manifest.py` & `idf_build_apps-1.0.4/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/tests/test_utils.py` & `idf_build_apps-1.0.4/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `idf_build_apps-1.0.3/setup.py` & `idf_build_apps-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
          'sphinxcontrib-mermaid'],
  'test': ['pytest', 'pytest-cov']}
 
 entry_points = \
 {'console_scripts': ['idf-build-apps = idf_build_apps:main.main']}
 
 setup(name='idf-build-apps',
-      version='1.0.3',
+      version='1.0.4',
       description='Tools for building ESP-IDF related apps.',
       author=None,
       author_email='Fu Hanxi <fuhanxi@espressif.com>',
       url=None,
       packages=packages,
       package_data=package_data,
       install_requires=install_requires,
```

### Comparing `idf_build_apps-1.0.3/PKG-INFO` & `idf_build_apps-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idf-build-apps
-Version: 1.0.3
+Version: 1.0.4
 Summary: Tools for building ESP-IDF related apps.
 Author-email: Fu Hanxi <fuhanxi@espressif.com>
 Requires-Python: >=2.7, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 2.7
```

