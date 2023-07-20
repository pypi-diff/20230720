# Comparing `tmp/findmyorder-1.6.0.tar.gz` & `tmp/findmyorder-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "findmyorder-1.6.0.tar", max compression
+gzip compressed data, was "findmyorder-1.6.1.tar", max compression
```

## Comparing `findmyorder-1.6.0.tar` & `findmyorder-1.6.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1064 2023-07-11 19:37:13.897006 findmyorder-1.6.0/LICENSE
--rw-r--r--   0        0        0     3049 2023-07-11 19:37:13.897006 findmyorder-1.6.0/README.md
--rw-r--r--   0        0        0      113 2023-07-11 19:37:14.641029 findmyorder-1.6.0/findmyorder/__init__.py
--rw-r--r--   0        0        0      660 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/config.py
--rw-r--r--   0        0        0     2533 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/default_settings.toml
--rw-r--r--   0        0        0     5875 2023-07-11 19:37:13.897006 findmyorder-1.6.0/findmyorder/main.py
--rw-r--r--   0        0        0     2380 2023-07-11 19:37:14.641029 findmyorder-1.6.0/pyproject.toml
--rw-r--r--   0        0        0     3922 1970-01-01 00:00:00.000000 findmyorder-1.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-20 14:52:48.244794 findmyorder-1.6.1/LICENSE
+-rw-r--r--   0        0        0     3022 2023-07-20 14:52:48.244794 findmyorder-1.6.1/README.md
+-rw-r--r--   0        0        0      113 2023-07-20 14:52:57.316883 findmyorder-1.6.1/findmyorder/__init__.py
+-rw-r--r--   0        0        0      660 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/config.py
+-rw-r--r--   0        0        0     3221 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/default_settings.toml
+-rw-r--r--   0        0        0     5903 2023-07-20 14:52:48.244794 findmyorder-1.6.1/findmyorder/main.py
+-rw-r--r--   0        0        0     2959 2023-07-20 14:52:57.308883 findmyorder-1.6.1/pyproject.toml
+-rw-r--r--   0        0        0     3895 1970-01-01 00:00:00.000000 findmyorder-1.6.1/PKG-INFO
```

### Comparing `findmyorder-1.6.0/LICENSE` & `findmyorder-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.0/README.md` & `findmyorder-1.6.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
-      <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
+      <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
    <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/findmyorder/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-findmyorder-main"><img src="https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/findmyorder"><img src="https://codecov.io/gh/mraniki/findmyorder/branch/main/graph/badge.svg?token=4838MSZNCC"/> </a><br>
     </td>
      <td align="left"> 
         Find My order,<br>
        a parsing package to find trading order
```

#### html2text {}

```diff
@@ -10,18 +10,17 @@
 badge&logo=telegram&logoColor=white] [https://
 img.shields.io/discord/1049307055867035648?style=for-the-
 badge&logo=discord&logoColor=white&label=%20%20&color=blue]
 [https://img.shields.io/pypi/v/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/github/actions/workflow/status/
-mraniki/findmyorder/                                        Find My order,
-%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  a parsing package
-the-badge&logo=GitHub&logoColor=white]                      to find trading
+[https://img.shields.io/github/actions/workflow/status/     Find My order,
+mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-     a parsing package
+badge&logo=GitHub&logoColor=white]                          to find trading
 [https://readthedocs.org/projects/findmyorder/badge/        order
 ?version=latest&style=for-the-badge]
 [https://codebeat.co/badges/9b113098-d22d-498d-9c61-
 eb1e96c1311a]
 [https://codecov.io/gh/mraniki/findmyorder/branch/main/
 graph/badge.svg?token=4838MSZNCC]
 ** How to use it **
```

### Comparing `findmyorder-1.6.0/findmyorder/config.py` & `findmyorder-1.6.1/findmyorder/config.py`

 * *Files identical despite different names*

### Comparing `findmyorder-1.6.0/findmyorder/default_settings.toml` & `findmyorder-1.6.1/findmyorder/default_settings.toml`

 * *Files 24% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # or load the settings from .env file or vars.
 # As an example, to change the port settings:
 # settings.toml
 # [default]
 # port = 8081
 # or via ENVVARS 
 # export TT_PORT=8081
-
+ 
 
 [default]
 VALUE = "Production - Default"
 findmyorder_enabled = true
 action_identifier = "BUY SELL LONG SHORT"
 stop_loss_identifier = "sl="
 take_profit_identifier = 'tp='
@@ -31,14 +31,38 @@
     { id = "GOLD", alt = "XAUUSD" },
     { id = "SILVER", alt = "XAGUSD" },
     { id = "BTC", alt = "WBTC" },
     { id = "ETH", alt = "WETH" },
 ]
 ignore_instrument = "US500 USTEC DOGE"
 
+########################################
+###     END OF DEFAULT SETTINGS      ###
+########################################
+
+
+
+
+                                        
+# _   _                           _   ___  
+#| | | |                         | | |__ \ 
+#| |_| |__   ___    ___ _ __   __| |    )|
+#| __| '_ \ / _ \  / _ \ '_ \ / _` |   / / 
+#| |_| | | |  __/ |  __/ | | | (_| |  |_|  
+# \__|_| |_|\___|  \___|_| |_|\__,_|  (_)  
+########################################                                                                                      
+
+
+
+
+
+
+########################################
+###         TESTING SETTINGS         ###
+########################################
 
 [testing]
 VALUE = "On Testing"
 findmyorder_enabled = true
 action_identifier = "BUY SELL LONG SHORT"
 actions = [
     { identifier = "BUY", type = "BUY" },
```

### Comparing `findmyorder-1.6.0/findmyorder/main.py` & `findmyorder-1.6.1/findmyorder/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,26 @@
  FindMyOrder Main
 """
 import logging
 from datetime import datetime
 
 import emoji
 from pyparsing import (
-    Combine, Optional, Word, alphas,
-    nums, one_of, pyparsing_common, Suppress)
+    Combine,
+    Optional,
+    Suppress,
+    Word,
+    alphas,
+    nums,
+    one_of,
+    pyparsing_common,
+)
+
 from findmyorder import __version__
+
 from .config import settings
 
 
 class FindMyOrder:
     """find an order class """
 
     def __init__(
```

### Comparing `findmyorder-1.6.0/pyproject.toml` & `findmyorder-1.6.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "findmyorder"
-version = "1.6.0"
+version = "1.6.1"
 description = "A python package to identify and parse order for trade execution."
 authors = ["mraniki <8766259+mraniki@users.noreply.github.com>"]
 license = "MIT License"
 readme = "README.md"
 keywords = ["trading", "order", "trade","buy","sell"]
 packages = [
     {include = "findmyorder"}
@@ -24,16 +24,40 @@
 
 [tool.poetry.dependencies]
 python = "^3.10"
 dynaconf = "^3.1.12"
 pyparsing = "^3.0.9"
 emoji = "^2.5.1"
 
-[tool.poetry.dev-dependencies]
-python-semantic-release = "^7.34.3"
+
+[tool.poetry.group.dev.dependencies]
+python-semantic-release = "^8.0.2"
+ruff = "^0.0.278"
+
+[tool.ruff]
+select = [
+  "E",  # pycodestyle
+  "F",  # pyflakes
+  "I",  # isort
+]
+exclude = [
+  ".github/*",
+  "docs/*",
+]
+ignore = ["E401","F401","F811"]
+format = "github"
+fixable = ["ALL"]
+
+[tool.pylint.exceptions]
+overgeneral-exceptions = [
+    "builtins.BaseException",
+    "builtins.Exception",
+    "builtins.RuntimeError",
+]
+
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.0"
 pytest-cov = "^4.1"
 pytest-asyncio = "^0.21.0"
 pytest-mock = "^3.11.1"
 
@@ -62,18 +86,50 @@
     "tests/*",
     "examples/*",
     "docs/*",
     "*/config.py"
 ]
 
 [tool.semantic_release]
-version_variable = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
-branch = "main"
-upload_to_pypi = true
-upload_to_release = true
+upload_to_vcs_release = true
+version_variables = ["pyproject.toml:version","findmyorder/__init__.py:__version__"]
 build_command = "pip install poetry && poetry build"
-commit_parser = "semantic_release.history.emoji_parser"
-use_textual_changelog_sections = true
-major_emoji = "BREAKING,💥,:boom:"
-minor_emoji = "feat,🥚,:egg:,🚀,:rocket:,💄,:lipstick:,✨,:sparkles:"
-patch_emoji = "fix,bump,Update,🎨,:art:,🐛,:bug:,🚑,:ambulance:,⚡,:zap:,🔥,:fire:,🚨,:rotating_light:,♻️,:recycle:,🔧,:wrench:,⬆️,:arrow_up:,🩹,:adhesive_bandage:,👷,:construction_worker:,📝,:memo:,🔒,:lock:,👽,:alien:,💬,:speech_balloon:,🥅,:goal_net:,✅,:white_check_mark:,🐳,:whale:,🙈,:see_no_evil:,⚗️,:alembic:,🧐,:monocle_face:,🔇,:mute:,🔊:volume:"
+commit_parser = "emoji"
+
+[tool.semantic_release.commit_parser_options]
+major_tags = [
+    "BREAKING",
+    "💥",
+    ":boom:",
+  ]
+minor_tags = ["feat",
+    "🥚",":egg:",
+    "🚀",":rocket:",
+    "💄",":lipstick:",
+    "✨",":sparkles:",
+]
 
+patch_tags = ["fix","bump","Update",
+    "🎨",":art:",
+    "🐛",":bug:",
+    "🚑",":ambulance:",
+    "⚡",":zap:",
+    "🔥",":fire:",
+    "🚨",":rotating_light:",
+    "♻️",":recycle:",
+    "🔧",":wrench:",
+    "⬆️",":arrow_up:",
+    "🩹",":adhesive_bandage:",
+    "👷",":construction_worker:",
+    "📝",":memo:",
+    "🔒",":lock:",
+    "👽",":alien:",
+    "💬",":speech_balloon:",
+    "🥅",":goal_net:",
+    "✅",":white_check_mark:",
+    "🐳",":whale:",
+    "🙈",":see_no_evil:",
+    "⚗️",":alembic:",
+    "🧐",":monocle_face:",
+    "🔇",":mute:",
+    "🔊",":volume:",
+]
```

### Comparing `findmyorder-1.6.0/PKG-INFO` & `findmyorder-1.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: findmyorder
-Version: 1.6.0
+Version: 1.6.1
 Summary: A python package to identify and parse order for trade execution.
 License: MIT
 Keywords: trading,order,trade,buy,sell
 Author: mraniki
 Author-email: 8766259+mraniki@users.noreply.github.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -31,15 +31,15 @@
     </td>
     <td align="center"><img width="200" alt="Logo" src="https://user-images.githubusercontent.com/8766259/233823991-cceaa05a-ff15-4796-a6bb-bcb3ee0d8859.jpg"></td>
   </tr>
   <tr>
     <td>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/v/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
       <a href="https://pypi.org/project/findmyorder/"><img src="https://img.shields.io/pypi/dm/findmyorder?style=for-the-badge&logo=PyPI&logoColor=white"></a><br>
-      <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
+      <a href="https://github.com/mraniki/findmyorder"><img src="https://img.shields.io/github/actions/workflow/status/mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-badge&logo=GitHub&logoColor=white"></a><br>
    <a href="https://talky.readthedocs.io/projects/findmyorder/index.html"><img src="https://readthedocs.org/projects/findmyorder/badge/?version=latest&style=for-the-badge"></a><br>
    <a href="https://codebeat.co/projects/github-com-mraniki-findmyorder-main"><img src="https://codebeat.co/badges/9b113098-d22d-498d-9c61-eb1e96c1311a"/></a><br>
    <a href="https://codecov.io/gh/mraniki/findmyorder"><img src="https://codecov.io/gh/mraniki/findmyorder/branch/main/graph/badge.svg?token=4838MSZNCC"/> </a><br>
     </td>
      <td align="left"> 
         Find My order,<br>
        a parsing package to find trading order
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: findmyorder Version: 1.6.0 Summary: A python
+Metadata-Version: 2.1 Name: findmyorder Version: 1.6.1 Summary: A python
 package to identify and parse order for trade execution. License: MIT Keywords:
 trading,order,trade,buy,sell Author: mraniki Author-email:
 8766259+mraniki@users.noreply.github.com Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: dynaconf
 (>=3.1.12,<4.0.0) Requires-Dist: emoji (>=2.5.1,<3.0.0) Requires-Dist:
@@ -22,18 +22,17 @@
 badge&logo=telegram&logoColor=white] [https://
 img.shields.io/discord/1049307055867035648?style=for-the-
 badge&logo=discord&logoColor=white&label=%20%20&color=blue]
 [https://img.shields.io/pypi/v/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
 [https://img.shields.io/pypi/dm/findmyorder?style=for-the-
 badge&logo=PyPI&logoColor=white]
-[https://img.shields.io/github/actions/workflow/status/
-mraniki/findmyorder/                                        Find My order,
-%F0%9F%91%B7%E2%80%8D%E2%99%82%EF%B8%8FFlow.yml?style=for-  a parsing package
-the-badge&logo=GitHub&logoColor=white]                      to find trading
+[https://img.shields.io/github/actions/workflow/status/     Find My order,
+mraniki/findmyorder/%F0%9F%91%B7Flow.yml?style=for-the-     a parsing package
+badge&logo=GitHub&logoColor=white]                          to find trading
 [https://readthedocs.org/projects/findmyorder/badge/        order
 ?version=latest&style=for-the-badge]
 [https://codebeat.co/badges/9b113098-d22d-498d-9c61-
 eb1e96c1311a]
 [https://codecov.io/gh/mraniki/findmyorder/branch/main/
 graph/badge.svg?token=4838MSZNCC]
 ** How to use it **
```

