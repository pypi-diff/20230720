# Comparing `tmp/flex-config-2.2.0rc0.tar.gz` & `tmp/flex_config-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flex-config-2.2.0rc0.tar", max compression
+gzip compressed data, was "flex_config-2.2.1.tar", max compression
```

## Comparing `flex-config-2.2.0rc0.tar` & `flex_config-2.2.1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0     1075 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/LICENSE
--rw-r--r--   0        0        0     2657 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/docs/README.md
--rw-r--r--   0        0        0     3446 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/__init__.py
--rw-r--r--   0        0        0     2486 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/aws_source.py
--rw-r--r--   0        0        0      372 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/config_source.py
--rw-r--r--   0        0        0     1896 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/env_source.py
--rw-r--r--   0        0        0      144 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/file_sources/__init__.py
--rw-r--r--   0        0        0     1614 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/file_sources/file_source.py
--rw-r--r--   0        0        0     1033 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/file_sources/json_source.py
--rw-r--r--   0        0        0     1312 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/file_sources/toml_source.py
--rw-r--r--   0        0        0     1305 2023-01-12 16:25:12.105836 flex-config-2.2.0rc0/flex_config/file_sources/yaml_source.py
--rw-r--r--   0        0        0       26 2023-01-12 16:25:12.109836 flex-config-2.2.0rc0/flex_config/py.typed
--rw-r--r--   0        0        0      384 2023-01-12 16:25:12.109836 flex-config-2.2.0rc0/flex_config/utils.py
--rw-r--r--   0        0        0     4813 2023-01-12 16:25:12.109836 flex-config-2.2.0rc0/pyproject.toml
--rw-r--r--   0        0        0     3733 2023-01-12 16:26:22.368254 flex-config-2.2.0rc0/setup.py
--rw-r--r--   0        0        0     3857 2023-01-12 16:26:22.368719 flex-config-2.2.0rc0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-07-20 15:44:02.392885 flex_config-2.2.1/LICENSE
+-rw-r--r--   0        0        0     2505 2023-07-20 15:44:02.392885 flex_config-2.2.1/docs/README.md
+-rw-r--r--   0        0        0     3446 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/__init__.py
+-rw-r--r--   0        0        0     2486 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/aws_source.py
+-rw-r--r--   0        0        0      372 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/config_source.py
+-rw-r--r--   0        0        0     1896 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/env_source.py
+-rw-r--r--   0        0        0      144 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/file_sources/__init__.py
+-rw-r--r--   0        0        0     1614 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/file_sources/file_source.py
+-rw-r--r--   0        0        0     1033 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/file_sources/json_source.py
+-rw-r--r--   0        0        0     1312 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/file_sources/toml_source.py
+-rw-r--r--   0        0        0     1305 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/file_sources/yaml_source.py
+-rw-r--r--   0        0        0       26 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/py.typed
+-rw-r--r--   0        0        0      384 2023-07-20 15:44:02.392885 flex_config-2.2.1/flex_config/utils.py
+-rw-r--r--   0        0        0     4808 2023-07-20 15:44:02.392885 flex_config-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3807 1970-01-01 00:00:00.000000 flex_config-2.2.1/PKG-INFO
```

### Comparing `flex-config-2.2.0rc0/LICENSE` & `flex_config-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/docs/README.md` & `flex_config-2.2.1/docs/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # Flex Config
-[![triaxtec](https://circleci.com/gh/triaxtec/flex-config.svg?style=svg)](https://app.circleci.com/pipelines/github/triaxtec/flex-config?branch=master)
 [![codecov](https://codecov.io/gh/triaxtec/flex-config/branch/master/graph/badge.svg?token=3utvPfZSLB)](https://codecov.io/gh/triaxtec/flex-config)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Generic badge](https://img.shields.io/badge/type_checked-mypy-informational.svg)](https://mypy.readthedocs.io/en/stable/introduction.html)
 [![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
 
 
 Configure your applications as easily as possible.
```

### Comparing `flex-config-2.2.0rc0/flex_config/__init__.py` & `flex_config-2.2.1/flex_config/__init__.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/aws_source.py` & `flex_config-2.2.1/flex_config/aws_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/env_source.py` & `flex_config-2.2.1/flex_config/env_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/file_sources/file_source.py` & `flex_config-2.2.1/flex_config/file_sources/file_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/file_sources/json_source.py` & `flex_config-2.2.1/flex_config/file_sources/json_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/file_sources/toml_source.py` & `flex_config-2.2.1/flex_config/file_sources/toml_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/flex_config/file_sources/yaml_source.py` & `flex_config-2.2.1/flex_config/file_sources/yaml_source.py`

 * *Files identical despite different names*

### Comparing `flex-config-2.2.0rc0/pyproject.toml` & `flex_config-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flex-config"
-version = "2.2.0-rc.0"
+version = "2.2.1"
 description="Easily configure Python apps via environment variables, YAML, and AWS SSM Param Store."
 repository="https://github.com/triaxtec/flex-config"
 documentation="https://triaxtec.github.io/flex-config"
 keywords=["config", "AWS", "SSM", "serverless", "environment"]
 readme = "docs/README.md"
 packages = [
     {include = "flex_config"}
@@ -21,15 +21,15 @@
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 boto3 = {version = "^1.13.1", optional = true}
-pyyaml = {version = "^5.3.1", optional = true}
+pyyaml = {version = "^6.0.1", optional = true}
 pydantic = "^1.7.2"
 toml = {version = "^0.10.2", optional = true}
 
 [tool.poetry.extras]
 aws = ["boto3"]
 yaml = ["pyyaml"]
 toml = ["toml"]
```

### Comparing `flex-config-2.2.0rc0/setup.py` & `flex_config-2.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,93 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: flex-config
+Version: 2.2.1
+Summary: Easily configure Python apps via environment variables, YAML, and AWS SSM Param Store.
+Home-page: https://github.com/triaxtec/flex-config
+License: MIT
+Keywords: config,AWS,SSM,serverless,environment
+Author: Dylan Anthony
+Author-email: danthony@triaxtec.com
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Utilities
+Provides-Extra: all
+Provides-Extra: aws
+Provides-Extra: toml
+Provides-Extra: yaml
+Requires-Dist: boto3 (>=1.13.1,<2.0.0) ; extra == "aws" or extra == "all"
+Requires-Dist: pydantic (>=1.7.2,<2.0.0)
+Requires-Dist: pyyaml (>=6.0.1,<7.0.0) ; extra == "yaml" or extra == "all"
+Requires-Dist: toml (>=0.10.2,<0.11.0) ; extra == "toml" or extra == "all"
+Project-URL: Documentation, https://triaxtec.github.io/flex-config
+Project-URL: Repository, https://github.com/triaxtec/flex-config
+Description-Content-Type: text/markdown
+
+# Flex Config
+[![codecov](https://codecov.io/gh/triaxtec/flex-config/branch/master/graph/badge.svg?token=3utvPfZSLB)](https://codecov.io/gh/triaxtec/flex-config)
+[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Generic badge](https://img.shields.io/badge/type_checked-mypy-informational.svg)](https://mypy.readthedocs.io/en/stable/introduction.html)
+[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)
+
+
+Configure your applications as easily as possible.
+
+## Main Features
+### Load config from wherever
+- Comes with built in support for loading from dicts, environment variables, JSON/YAML/TOML files, and AWS SSM Parameter Store.
+- Super easy to set up a custom source and load from anywhere.
+
+### Type conversion, validation, and hints via [Pydantic]
+```python
+# "ConfigSchema" is pydantic's BaseModel renamed and re-exported for easier use 
+from flex_config import ConfigSchema, construct_config
+
+class Config(ConfigSchema):
+    a_string: str
+    an_int: int
+
+# Raises ValidationError
+my_bad_config = construct_config(Config, {"a_string": ["not", "a", "string"], "an_int": "seven"})
+
+my_good_config = construct_config(Config, {"a_string": "my_string", "an_int": "7"})
+assert isinstance(my_good_config.an_int, int)
+```
+
+### Dynamic loading of config values
+```python
+from pathlib import Path
+from typing import Dict, Any
+
+# "ConfigSchema" is pydantic's BaseModel renamed and re-exported for easier use 
+from flex_config import ConfigSchema, construct_config, AWSSource, YAMLSource, EnvSource, ConfigSource
+
+class Config(ConfigSchema):
+    env: str
+    my_thing: str
+
+def get_ssm_params(config_so_far: Dict[str, Any]) -> ConfigSource:
+    # env is set to live or dev via environment variables in the deployment environment
+    env = config_so_far.get("env")
+    if env == "local":  # Not a live deployment, my_thing is in a local yaml file
+        return {}
+    return AWSSource(f"my_app/{config_so_far['env']}")
+
+
+my_config = construct_config(Config, [EnvSource("MY_APP_"), YAMLSource(Path("my_file.yaml")), get_ssm_params])
+```
+
+## Installation
+Basic install: `poetry install flex_config`
+With all optional dependencies (support for AWS SSM, YAML, and TOML): `poetry install flex_config -E all`
 
-packages = \
-['flex_config', 'flex_config.file_sources']
+For a full tutorial and API docs, check out the [hosted documentation]
 
-package_data = \
-{'': ['*']}
+[Pydantic]: https://github.com/samuelcolvin/pydantic/
+[hosted documentation]: https://triaxtec.github.io/flex-config
 
-install_requires = \
-['pydantic>=1.7.2,<2.0.0']
-
-extras_require = \
-{'all': ['boto3>=1.13.1,<2.0.0',
-         'pyyaml>=5.3.1,<6.0.0',
-         'toml>=0.10.2,<0.11.0'],
- 'aws': ['boto3>=1.13.1,<2.0.0'],
- 'toml': ['toml>=0.10.2,<0.11.0'],
- 'yaml': ['pyyaml>=5.3.1,<6.0.0']}
-
-setup_kwargs = {
-    'name': 'flex-config',
-    'version': '2.2.0rc0',
-    'description': 'Easily configure Python apps via environment variables, YAML, and AWS SSM Param Store.',
-    'long_description': '# Flex Config\n[![triaxtec](https://circleci.com/gh/triaxtec/flex-config.svg?style=svg)](https://app.circleci.com/pipelines/github/triaxtec/flex-config?branch=master)\n[![codecov](https://codecov.io/gh/triaxtec/flex-config/branch/master/graph/badge.svg?token=3utvPfZSLB)](https://codecov.io/gh/triaxtec/flex-config)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)\n[![Generic badge](https://img.shields.io/badge/type_checked-mypy-informational.svg)](https://mypy.readthedocs.io/en/stable/introduction.html)\n[![MIT license](https://img.shields.io/badge/License-MIT-blue.svg)](https://lbesson.mit-license.org/)\n\n\nConfigure your applications as easily as possible.\n\n## Main Features\n### Load config from wherever\n- Comes with built in support for loading from dicts, environment variables, JSON/YAML/TOML files, and AWS SSM Parameter Store.\n- Super easy to set up a custom source and load from anywhere.\n\n### Type conversion, validation, and hints via [Pydantic]\n```python\n# "ConfigSchema" is pydantic\'s BaseModel renamed and re-exported for easier use \nfrom flex_config import ConfigSchema, construct_config\n\nclass Config(ConfigSchema):\n    a_string: str\n    an_int: int\n\n# Raises ValidationError\nmy_bad_config = construct_config(Config, {"a_string": ["not", "a", "string"], "an_int": "seven"})\n\nmy_good_config = construct_config(Config, {"a_string": "my_string", "an_int": "7"})\nassert isinstance(my_good_config.an_int, int)\n```\n\n### Dynamic loading of config values\n```python\nfrom pathlib import Path\nfrom typing import Dict, Any\n\n# "ConfigSchema" is pydantic\'s BaseModel renamed and re-exported for easier use \nfrom flex_config import ConfigSchema, construct_config, AWSSource, YAMLSource, EnvSource, ConfigSource\n\nclass Config(ConfigSchema):\n    env: str\n    my_thing: str\n\ndef get_ssm_params(config_so_far: Dict[str, Any]) -> ConfigSource:\n    # env is set to live or dev via environment variables in the deployment environment\n    env = config_so_far.get("env")\n    if env == "local":  # Not a live deployment, my_thing is in a local yaml file\n        return {}\n    return AWSSource(f"my_app/{config_so_far[\'env\']}")\n\n\nmy_config = construct_config(Config, [EnvSource("MY_APP_"), YAMLSource(Path("my_file.yaml")), get_ssm_params])\n```\n\n## Installation\nBasic install: `poetry install flex_config`\nWith all optional dependencies (support for AWS SSM, YAML, and TOML): `poetry install flex_config -E all`\n\nFor a full tutorial and API docs, check out the [hosted documentation]\n\n[Pydantic]: https://github.com/samuelcolvin/pydantic/\n[hosted documentation]: https://triaxtec.github.io/flex-config\n',
-    'author': 'Dylan Anthony',
-    'author_email': 'danthony@triaxtec.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://github.com/triaxtec/flex-config',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'extras_require': extras_require,
-    'python_requires': '>=3.8,<4.0',
-}
-
-
-setup(**setup_kwargs)
```

