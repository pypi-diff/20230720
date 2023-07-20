# Comparing `tmp/pydantic_avro-0.5.2.tar.gz` & `tmp/pydantic_avro-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_avro-0.5.2.tar", max compression
+gzip compressed data, was "pydantic_avro-0.6.0.tar", max compression
```

## Comparing `pydantic_avro-0.5.2.tar` & `pydantic_avro-0.6.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/LICENSE
--rw-r--r--   0        0        0     1863 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/README.md
--rw-r--r--   0        0        0     1515 2023-07-20 12:49:21.638046 pydantic_avro-0.5.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/__init__.py
--rw-r--r--   0        0        0      685 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/__main__.py
--rw-r--r--   0        0        0     5180 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/avro_to_pydantic.py
--rw-r--r--   0        0        0     7384 2023-07-20 12:49:00.944616 pydantic_avro-0.5.2/src/pydantic_avro/base.py
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.5.2/setup.py
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.5.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1863 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/README.md
+-rw-r--r--   0        0        0     1515 2023-07-20 13:08:40.073604 pydantic_avro-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/src/pydantic_avro/__init__.py
+-rw-r--r--   0        0        0      685 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/src/pydantic_avro/__main__.py
+-rw-r--r--   0        0        0     5180 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/src/pydantic_avro/avro_to_pydantic.py
+-rw-r--r--   0        0        0     7384 2023-07-20 13:08:22.957612 pydantic_avro-0.6.0/src/pydantic_avro/base.py
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.6.0/setup.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.6.0/PKG-INFO
```

### Comparing `pydantic_avro-0.5.2/LICENSE` & `pydantic_avro-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.2/README.md` & `pydantic_avro-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.2/pyproject.toml` & `pydantic_avro-0.6.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-avro"
-version = "0.5.2"
+version = "0.6.0"
 description = "Converting pydantic classes to avro schemas"
 authors = ["Peter van 't Hof' <peter.vanthof@godatadriven.com>"]
 
 keywords = ["pydantic", "avro"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/godatadriven/pydantic-avro"
```

### Comparing `pydantic_avro-0.5.2/src/pydantic_avro/__main__.py` & `pydantic_avro-0.6.0/src/pydantic_avro/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.2/src/pydantic_avro/avro_to_pydantic.py` & `pydantic_avro-0.6.0/src/pydantic_avro/avro_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.2/src/pydantic_avro/base.py` & `pydantic_avro-0.6.0/src/pydantic_avro/base.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.2/setup.py` & `pydantic_avro-0.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['pydantic>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pydantic-avro = pydantic_avro.__main__:root_main']}
 
 setup_kwargs = {
     'name': 'pydantic-avro',
-    'version': '0.5.2',
+    'version': '0.6.0',
     'description': 'Converting pydantic classes to avro schemas',
     'long_description': '[![Python package](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml)\n[![codecov](https://codecov.io/gh/godatadriven/pydantic-avro/branch/main/graph/badge.svg?token=5L08GOERAW)](https://codecov.io/gh/godatadriven/pydantic-avro)\n[![PyPI version](https://badge.fury.io/py/pydantic-avro.svg)](https://badge.fury.io/py/pydantic-avro)\n[![CodeQL](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml)\n\n# pydantic-avro\n\nThis library can convert a pydantic class to a avro schema or generate python code from a avro schema.\n\n### Install\n\n```bash\npip install pydantic-avro\n```\n\n### Pydantic class to avro schema\n\n```python\nimport json\nfrom typing import Optional\n\nfrom pydantic_avro.base import AvroBase\n\nclass TestModel(AvroBase):\n    key1: str\n    key2: int\n    key2: Optional[str]\n\nschema_dict: dict = TestModel.avro_schema()\nprint(json.dumps(schema_dict))\n\n```\n\n### Avro schema to pydantic\n\n```shell\n# Print to stdout\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc\n\n# Save it to a file\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc --output /path/to/output.py\n```\n\n\n### Install for developers\n\n###### Install package\n\n- Requirement: Poetry 1.*\n\n```shell\npoetry install\n```\n\n###### Run unit tests\n```shell\npytest\ncoverage run -m pytest  # with coverage\n# or (depends on your local env) \npoetry run pytest\npoetry run coverage run -m pytest  # with coverage\n```\n\n##### Run linting\n\nThe linting is checked in the github workflow. To fix and review issues run this:\n```shell\nblack .   # Auto fix all issues\nisort .   # Auto fix all issues\npflake .  # Only display issues, fixing is manual\n```\n',
     'author': "Peter van 't Hof'",
     'author_email': 'peter.vanthof@godatadriven.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/godatadriven/pydantic-avro',
```

### Comparing `pydantic_avro-0.5.2/PKG-INFO` & `pydantic_avro-0.6.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-avro
-Version: 0.5.2
+Version: 0.6.0
 Summary: Converting pydantic classes to avro schemas
 Home-page: https://github.com/godatadriven/pydantic-avro
 License: MIT
 Keywords: pydantic,avro
 Author: Peter van 't Hof'
 Author-email: peter.vanthof@godatadriven.com
 Requires-Python: >=3.7,<4.0
```

