# Comparing `tmp/pydantic_avro-0.5.1.tar.gz` & `tmp/pydantic_avro-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_avro-0.5.1.tar", max compression
+gzip compressed data, was "pydantic_avro-0.5.2.tar", max compression
```

## Comparing `pydantic_avro-0.5.1.tar` & `pydantic_avro-0.5.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2021-12-17 10:39:19.013474 pydantic_avro-0.5.1/LICENSE
--rw-r--r--   0        0        0     1863 2021-12-30 18:43:33.078382 pydantic_avro-0.5.1/README.md
--rw-r--r--   0        0        0     1515 2023-04-18 11:57:54.151329 pydantic_avro-0.5.1/pyproject.toml
--rw-r--r--   0        0        0        0 2021-12-17 10:46:42.844382 pydantic_avro-0.5.1/src/pydantic_avro/__init__.py
--rw-r--r--   0        0        0      685 2021-12-17 15:30:57.013907 pydantic_avro-0.5.1/src/pydantic_avro/__main__.py
--rw-r--r--   0        0        0     5180 2023-04-18 11:57:37.546545 pydantic_avro-0.5.1/src/pydantic_avro/avro_to_pydantic.py
--rw-r--r--   0        0        0     6987 2023-04-18 11:57:37.547329 pydantic_avro-0.5.1/src/pydantic_avro/base.py
--rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.5.1/setup.py
--rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/LICENSE
+-rw-r--r--   0        0        0     1863 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/README.md
+-rw-r--r--   0        0        0     1515 2023-07-20 12:49:21.638046 pydantic_avro-0.5.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/__init__.py
+-rw-r--r--   0        0        0      685 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/__main__.py
+-rw-r--r--   0        0        0     5180 2023-07-20 12:49:00.940616 pydantic_avro-0.5.2/src/pydantic_avro/avro_to_pydantic.py
+-rw-r--r--   0        0        0     7384 2023-07-20 12:49:00.944616 pydantic_avro-0.5.2/src/pydantic_avro/base.py
+-rw-r--r--   0        0        0     2822 1970-01-01 00:00:00.000000 pydantic_avro-0.5.2/setup.py
+-rw-r--r--   0        0        0     2671 1970-01-01 00:00:00.000000 pydantic_avro-0.5.2/PKG-INFO
```

### Comparing `pydantic_avro-0.5.1/LICENSE` & `pydantic_avro-0.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.1/README.md` & `pydantic_avro-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.1/pyproject.toml` & `pydantic_avro-0.5.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pydantic-avro"
-version = "0.5.1"
+version = "0.5.2"
 description = "Converting pydantic classes to avro schemas"
 authors = ["Peter van 't Hof' <peter.vanthof@godatadriven.com>"]
 
 keywords = ["pydantic", "avro"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/godatadriven/pydantic-avro"
```

### Comparing `pydantic_avro-0.5.1/src/pydantic_avro/__main__.py` & `pydantic_avro-0.5.2/src/pydantic_avro/__main__.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.1/src/pydantic_avro/avro_to_pydantic.py` & `pydantic_avro-0.5.2/src/pydantic_avro/avro_to_pydantic.py`

 * *Files identical despite different names*

### Comparing `pydantic_avro-0.5.1/src/pydantic_avro/base.py` & `pydantic_avro-0.5.2/src/pydantic_avro/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -88,14 +88,22 @@
                 # If items in array are a logicalType
                 if (
                     isinstance(tn, dict)
                     and isinstance(tn.get("type", {}), dict)
                     and tn.get("type", {}).get("logicalType") is not None
                 ):
                     tn = tn["type"]
+                # If items in array are an array, the structure must be corrected
+                if (
+                    isinstance(tn, dict)
+                    and isinstance(tn.get("type", {}), dict)
+                    and tn.get("type", {}).get("type") == "array"
+                ):
+                    items = tn["type"]["items"]
+                    tn = {"type": "array", "items": items}
                 avro_type_dict["type"] = {"type": "array", "items": tn}
             elif t == "string" and f == "date-time":
                 avro_type_dict["type"] = {
                     "type": "long",
                     "logicalType": "timestamp-micros",
                 }
             elif t == "string" and f == "date":
```

### Comparing `pydantic_avro-0.5.1/setup.py` & `pydantic_avro-0.5.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['pydantic>=1.4.0,<2.0.0']
 
 entry_points = \
 {'console_scripts': ['pydantic-avro = pydantic_avro.__main__:root_main']}
 
 setup_kwargs = {
     'name': 'pydantic-avro',
-    'version': '0.5.1',
+    'version': '0.5.2',
     'description': 'Converting pydantic classes to avro schemas',
     'long_description': '[![Python package](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/python-package.yml)\n[![codecov](https://codecov.io/gh/godatadriven/pydantic-avro/branch/main/graph/badge.svg?token=5L08GOERAW)](https://codecov.io/gh/godatadriven/pydantic-avro)\n[![PyPI version](https://badge.fury.io/py/pydantic-avro.svg)](https://badge.fury.io/py/pydantic-avro)\n[![CodeQL](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/godatadriven/pydantic-avro/actions/workflows/codeql-analysis.yml)\n\n# pydantic-avro\n\nThis library can convert a pydantic class to a avro schema or generate python code from a avro schema.\n\n### Install\n\n```bash\npip install pydantic-avro\n```\n\n### Pydantic class to avro schema\n\n```python\nimport json\nfrom typing import Optional\n\nfrom pydantic_avro.base import AvroBase\n\nclass TestModel(AvroBase):\n    key1: str\n    key2: int\n    key2: Optional[str]\n\nschema_dict: dict = TestModel.avro_schema()\nprint(json.dumps(schema_dict))\n\n```\n\n### Avro schema to pydantic\n\n```shell\n# Print to stdout\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc\n\n# Save it to a file\npydantic-avro avro_to_pydantic --asvc /path/to/schema.asvc --output /path/to/output.py\n```\n\n\n### Install for developers\n\n###### Install package\n\n- Requirement: Poetry 1.*\n\n```shell\npoetry install\n```\n\n###### Run unit tests\n```shell\npytest\ncoverage run -m pytest  # with coverage\n# or (depends on your local env) \npoetry run pytest\npoetry run coverage run -m pytest  # with coverage\n```\n\n##### Run linting\n\nThe linting is checked in the github workflow. To fix and review issues run this:\n```shell\nblack .   # Auto fix all issues\nisort .   # Auto fix all issues\npflake .  # Only display issues, fixing is manual\n```\n',
     'author': "Peter van 't Hof'",
     'author_email': 'peter.vanthof@godatadriven.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/godatadriven/pydantic-avro',
```

### Comparing `pydantic_avro-0.5.1/PKG-INFO` & `pydantic_avro-0.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-avro
-Version: 0.5.1
+Version: 0.5.2
 Summary: Converting pydantic classes to avro schemas
 Home-page: https://github.com/godatadriven/pydantic-avro
 License: MIT
 Keywords: pydantic,avro
 Author: Peter van 't Hof'
 Author-email: peter.vanthof@godatadriven.com
 Requires-Python: >=3.7,<4.0
```

