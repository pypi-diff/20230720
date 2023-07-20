# Comparing `tmp/syrupy-4.0.7.tar.gz` & `tmp/syrupy-4.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syrupy-4.0.7.tar", max compression
+gzip compressed data, was "syrupy-4.0.8.tar", max compression
```

## Comparing `syrupy-4.0.7.tar` & `syrupy-4.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    10769 2023-07-20 12:01:49.665236 syrupy-4.0.7/LICENSE
--rw-r--r--   0        0        0    26662 2023-07-20 12:01:49.665236 syrupy-4.0.7/README.md
--rw-r--r--   0        0        0     2461 2023-07-20 12:03:06.138246 syrupy-4.0.7/pyproject.toml
--rw-r--r--   0        0        0     6097 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/__init__.py
--rw-r--r--   0        0        0    11493 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/assertion.py
--rw-r--r--   0        0        0      469 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/constants.py
--rw-r--r--   0        0        0     4213 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/data.py
--rw-r--r--   0        0        0      531 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/exceptions.py
--rw-r--r--   0        0        0       86 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/__init__.py
--rw-r--r--   0        0        0     2688 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/amber/__init__.py
--rw-r--r--   0        0        0    15524 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/amber/serializer.py
--rw-r--r--   0        0        0    14619 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/base.py
--rw-r--r--   0        0        0      521 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/image.py
--rw-r--r--   0        0        0     4511 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/json/__init__.py
--rw-r--r--   0        0        0     4490 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/extensions/single_file.py
--rw-r--r--   0        0        0      840 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/filters.py
--rw-r--r--   0        0        0     4087 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/location.py
--rw-r--r--   0        0        0     2029 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/matchers.py
--rw-r--r--   0        0        0        0 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/py.typed
--rw-r--r--   0        0        0    19775 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/report.py
--rw-r--r--   0        0        0     6729 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/session.py
--rw-r--r--   0        0        0     2355 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/terminal.py
--rw-r--r--   0        0        0      970 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/types.py
--rw-r--r--   0        0        0     3292 2023-07-20 12:01:49.677236 syrupy-4.0.7/src/syrupy/utils.py
--rw-r--r--   0        0        0    28039 1970-01-01 00:00:00.000000 syrupy-4.0.7/setup.py
--rw-r--r--   0        0        0    27917 1970-01-01 00:00:00.000000 syrupy-4.0.7/PKG-INFO
+-rw-r--r--   0        0        0    10769 2023-07-20 21:39:00.129176 syrupy-4.0.8/LICENSE
+-rw-r--r--   0        0        0    26662 2023-07-20 21:39:00.129176 syrupy-4.0.8/README.md
+-rw-r--r--   0        0        0     2461 2023-07-20 21:40:07.737544 syrupy-4.0.8/pyproject.toml
+-rw-r--r--   0        0        0     6097 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/__init__.py
+-rw-r--r--   0        0        0    11493 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/assertion.py
+-rw-r--r--   0        0        0      498 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/constants.py
+-rw-r--r--   0        0        0     4213 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/data.py
+-rw-r--r--   0        0        0      531 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/exceptions.py
+-rw-r--r--   0        0        0       86 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/extensions/__init__.py
+-rw-r--r--   0        0        0     2688 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/extensions/amber/__init__.py
+-rw-r--r--   0        0        0    15524 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/extensions/amber/serializer.py
+-rw-r--r--   0        0        0    14619 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/extensions/base.py
+-rw-r--r--   0        0        0      521 2023-07-20 21:39:00.141176 syrupy-4.0.8/src/syrupy/extensions/image.py
+-rw-r--r--   0        0        0     4511 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/extensions/json/__init__.py
+-rw-r--r--   0        0        0     4490 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/extensions/single_file.py
+-rw-r--r--   0        0        0      840 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/filters.py
+-rw-r--r--   0        0        0     4087 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/location.py
+-rw-r--r--   0        0        0     2029 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/matchers.py
+-rw-r--r--   0        0        0        0 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/py.typed
+-rw-r--r--   0        0        0    19775 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/report.py
+-rw-r--r--   0        0        0     6729 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/session.py
+-rw-r--r--   0        0        0     2355 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/terminal.py
+-rw-r--r--   0        0        0      970 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/types.py
+-rw-r--r--   0        0        0     5320 2023-07-20 21:39:00.145176 syrupy-4.0.8/src/syrupy/utils.py
+-rw-r--r--   0        0        0    28039 1970-01-01 00:00:00.000000 syrupy-4.0.8/setup.py
+-rw-r--r--   0        0        0    27917 1970-01-01 00:00:00.000000 syrupy-4.0.8/PKG-INFO
```

### Comparing `syrupy-4.0.7/LICENSE` & `syrupy-4.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/README.md` & `syrupy-4.0.8/README.md`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/pyproject.toml` & `syrupy-4.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = 'syrupy'
 license = 'Apache-2.0'
-version = "4.0.7"
+version = "4.0.8"
 description = 'Pytest Snapshot Test Utility'
 authors = ['Top Hat Open Source <opensource@tophat.com>']
 readme = 'README.md'
 packages = [{ include = 'syrupy', from = 'src' }]
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'Framework :: Pytest',
```

### Comparing `syrupy-4.0.7/src/syrupy/__init__.py` & `syrupy-4.0.8/src/syrupy/__init__.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/assertion.py` & `syrupy-4.0.8/src/syrupy/assertion.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/data.py` & `syrupy-4.0.8/src/syrupy/data.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/exceptions.py` & `syrupy-4.0.8/src/syrupy/exceptions.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/amber/__init__.py` & `syrupy-4.0.8/src/syrupy/extensions/amber/__init__.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/amber/serializer.py` & `syrupy-4.0.8/src/syrupy/extensions/amber/serializer.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/base.py` & `syrupy-4.0.8/src/syrupy/extensions/base.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/image.py` & `syrupy-4.0.8/src/syrupy/extensions/image.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/json/__init__.py` & `syrupy-4.0.8/src/syrupy/extensions/json/__init__.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/extensions/single_file.py` & `syrupy-4.0.8/src/syrupy/extensions/single_file.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/filters.py` & `syrupy-4.0.8/src/syrupy/filters.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/location.py` & `syrupy-4.0.8/src/syrupy/location.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/matchers.py` & `syrupy-4.0.8/src/syrupy/matchers.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/report.py` & `syrupy-4.0.8/src/syrupy/report.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/session.py` & `syrupy-4.0.8/src/syrupy/session.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/terminal.py` & `syrupy-4.0.8/src/syrupy/terminal.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/src/syrupy/types.py` & `syrupy-4.0.8/src/syrupy/types.py`

 * *Files identical despite different names*

### Comparing `syrupy-4.0.7/setup.py` & `syrupy-4.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 ['colored>=1.3.92,<2.0.0', 'pytest>=7.0.0,<8.0.0']
 
 entry_points = \
 {'pytest11': ['syrupy = syrupy']}
 
 setup_kwargs = {
     'name': 'syrupy',
-    'version': '4.0.7',
+    'version': '4.0.8',
     'description': 'Pytest Snapshot Test Utility',
     'long_description': '# syrupy\n\n<img align="right" width="100px" height="100px" src="https://user-images.githubusercontent.com/2528959/69500147-85d71400-0ec6-11ea-867a-277881278e57.png" alt="Logo">\n\n[![All Contributors](https://img.shields.io/badge/all_contributors-2-orange.svg?style=flat-square)](#contributors) [![Maturity badge - level 4](https://img.shields.io/badge/Maturity-Level%204%20--%20Critical-brightgreen.svg)](https://github.com/tophat/getting-started/blob/master/scorecard.md) [![Stage](https://img.shields.io/pypi/status/syrupy)](https://pypi.org/project/syrupy/) [![Discord](https://img.shields.io/discord/809577721751142410?label=community%20chat)](https://discord.gg/YhK3GFcZrk)\n\n![Pytest>=5.1.0,<8.0.0](https://img.shields.io/badge/pytest-%3E%3D5.1.0,%20%3C8.0.0-green) [![Pypi](https://img.shields.io/pypi/v/syrupy)](https://pypi.org/project/syrupy/) [![Wheel](https://img.shields.io/pypi/wheel/syrupy)](https://pypi.org/project/syrupy/) ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/syrupy) [![PyPI - Downloads](https://img.shields.io/pypi/dm/syrupy)](https://pypi.org/project/syrupy/) [![PyPI - License](https://img.shields.io/pypi/l/syrupy)](./LICENSE)\n\n![Build Status](https://github.com/tophat/syrupy/workflows/Syrupy%20CICD/badge.svg) [![codecov](https://codecov.io/gh/tophat/syrupy/branch/main/graph/badge.svg)](https://codecov.io/gh/tophat/syrupy)\n\n![Next Status](https://github.com/tophat/syrupy/workflows/Next%20Version/badge.svg)\n\n## Overview\n\nSyrupy is a [pytest](https://docs.pytest.org/en/latest/) snapshot plugin. It enables developers to write tests which assert immutability of computed results.\n\n## Motivation\n\nThe most popular snapshot test plugin compatible with pytest has some core limitations which this package attempts to address by upholding some key values:\n\n- Extensible: If a particular data type is not supported, users should be able to easily and quickly add support.\n- Idiomatic: Snapshot testing should fit naturally among other test cases in pytest, e.g. `assert x == snapshot` vs. `snapshot.assert_match(x)`.\n- Soundness: Snapshot tests should uncover even the most minute issues. Unlike other snapshot libraries, Syrupy will fail a test suite if a snapshot does not exist, not just on snapshot differences.\n\n## Installation\n\n```shell\npython -m pip install syrupy\n```\n\n### Migration from snapshottest\n\nYou cannot use syrupy alongside snapshottest due to argument conflicts. To ease migration, we\'ve made syrupy aware of snapshottest call syntax. Simply uninstall snapshottest and remove old snapshots:\n\n```shell\npip uninstall snapshottest -y;\nfind . -type d ! -path \'*/\\.*\' -name \'snapshots\' | xargs rm -r\n```\n\n### Pytest and Python Compatibility\n\nSyrupy will always be compatible with the latest version of Python and Pytest. If you\'re running an old version of Python or Pytest, you will need to use an older major version of Syrupy:\n\n| Syrupy Version | Python Support | Pytest Support |\n| -------------- | -------------- | -------------- |\n| 4.x.x          | >3.8.1         | >=7            |\n| 3.x.x          | >=3.7, <4      | >=5.1, <8      |\n| 2.x.x          | >=3.6, <4      | >=5.1, <8      |\n\n## Usage\n\n### Basic Usage\n\nIn a pytest test file `test_file.py`:\n\n```python\ndef test_foo(snapshot):\n    actual = "Some computed value!"\n    assert actual == snapshot\n```\n\nwhen you run `pytest`, the above test should fail due to a missing snapshot. Re-run pytest with the update snapshots flag like so:\n\n```shell\npytest --snapshot-update\n```\n\nA snapshot file should be generated under a `__snapshots__` directory in the same directory as `test_file.py`. The `__snapshots__` directory and all its children should be committed along with your test code.\n\n[![Usage Demo](https://tophat.github.io/syrupy/assets/usage_demo.gif)](https://asciinema.org/a/369462)\n\n#### Custom Objects\n\nThe default serializer supports all python built-in types and provides a sensible default for custom objects.\n\n#### Representation\n\nIf you need to customise your object snapshot, it is as easy as overriding the default `__repr__` implementation.\n\n```python\ndef __repr__(self) -> str:\n    return "MyCustomClass(...)"\n```\n\n#### Attributes\n\nIf you want to limit what properties are serialized at a class type level you could either:\n\n**A**. Provide a filter function to the snapshot [exclude](#exclude) configuration option.\n\n```py\ndef limit_foo_attrs(prop, path):\n  allowed_foo_attrs = {"only", "serialize", "these", "attrs"}\n  return isinstance(path[-1][1], Foo) and prop in allowed_foo_attrs\n\ndef test_bar(snapshot):\n    actual = Foo(...)\n    assert actual == snapshot(exclude=limit_foo_attrs)\n```\n\n**B**. Or override the `__dir__` implementation to control the attribute list.\n\n```py\nclass Foo:\n  def __dir__(self):\n    return ["only", "serialize", "these", "attrs"]\n\ndef test_bar(snapshot):\n    actual = Foo(...)\n    assert actual == snapshot\n```\n\nBoth options will generate equivalent snapshots but the latter is only viable when you have control over the class implementation and do not need to share the exclusion logic with other objects.\n\n### CLI Options\n\nThese are the cli options exposed to `pytest` by the plugin.\n\n| Option                         | Description                                                                                                                    | Default                                                                                                      |\n| ------------------------------ | ------------------------------------------------------------------------------------------------------------------------------ | ------------------------------------------------------------------------------------------------------------ |\n| `--snapshot-update`            | Snapshots will be updated to match assertions and unused snapshots will be deleted.                                            | `False`                                                                                                      |\n| `--snapshot-details`           | Includes details of unused snapshots (test name and snapshot location) in the final report.                                    | `False`                                                                                                      |\n| `--snapshot-warn-unused`       | Prints a warning on unused snapshots rather than fail the test suite.                                                          | `False`                                                                                                      |\n| `--snapshot-default-extension` | Use to change the default snapshot extension class.                                                                            | [AmberSnapshotExtension](https://github.com/tophat/syrupy/blob/main/src/syrupy/extensions/amber/__init__.py) |\n| `--snapshot-no-colors`         | Disable test results output highlighting. Equivalent to setting the environment variables `ANSI_COLORS_DISABLED` or `NO_COLOR` | Disabled by default if not in terminal.                                                                      |\n\n### Assertion Options\n\nThese are the options available on the `snapshot` assertion fixture.\nUse of these options are one shot and do not persist across assertions.\nFor more persistent options see [advanced usage](#advanced-usage).\n\n#### `matcher`\n\nThis allows you to match on a property path and value to control how specific object shapes are serialized.\n\nThe matcher is a function that takes two keyword arguments.\nIt should return the replacement value to be serialized or the original unmutated value.\n\n| Argument | Description                                                                                                        |\n| -------- | ------------------------------------------------------------------------------------------------------------------ |\n| `data`   | Current serializable value being matched on                                                                        |\n| `path`   | Ordered path traversed to the current value e.g. `(("a", dict), ("b", dict))` from `{ "a": { "b": { "c": 1 } } }`} |\n\n**NOTE:** Do not mutate the value received as it could cause unintended side effects.\n\n##### Built-In Matchers\n\nSyrupy comes with built-in helpers that can be used to make easy work of using property matchers.\n\n###### `path_type(mapping=None, *, types=(), strict=True, regex=False)`\n\nEasy way to build a matcher that uses the path and value type to replace serialized data.\nWhen strict, this will raise a `ValueError` if the types specified are not matched.\n\n| Argument  | Description                                                                                                                        |\n| --------- | ---------------------------------------------------------------------------------------------------------------------------------- |\n| `mapping` | Dict of path string to tuples of class types, including primitives e.g. (MyClass, UUID, datetime, int, str)                        |\n| `types`   | Tuple of class types used if none of the path strings from the mapping are matched                                                 |\n| `strict`  | If a path is matched but the value at the path does not match one of the class types in the tuple then a `PathTypeError` is raised |\n| `regex`   | If true, the `mapping` key is treated as a regular expression when matching paths                                                  |\n\n```py\nfrom syrupy.matchers import path_type\n\ndef test_bar(snapshot):\n    actual = {\n      "date_created": datetime.now(),\n      "value": "Some computed value!!",\n    }\n    assert actual == snapshot(matcher=path_type({\n      "date_created": (datetime,),\n      "nested.path.id": (int,),\n    }))\n```\n\n```py\n# name: test_bar\n  dict({\n    \'date_created\': datetime,\n    \'value\': \'Some computed value!!\',\n  })\n# ---\n```\n\n#### `exclude`\n\nThis allows you to filter out object properties from the serialized snapshot.\n\nThe exclude parameter takes a filter function that accepts two keyword arguments.\nIt should return `true` or `false` if the property should be excluded or included respectively.\n\n| Argument | Description                                                                                                                                   |\n| -------- | --------------------------------------------------------------------------------------------------------------------------------------------- |\n| `prop`   | Current property on the object, could be any hashable value that can be used to retrieve a value e.g. `1`, `"prop_str"`, `SomeHashableObject` |\n| `path`   | Ordered path traversed to the current value e.g. `(("a", dict), ("b", dict))` from `{ "a": { "b": { "c": 1 } } }`}                            |\n\n##### Built-In Filters\n\nSyrupy comes with built-in helpers that can be used to make easy work of using the filter options.\n\n###### `props(prop_name, *prop_name)`\n\nEasy way to build a filter that excludes based on string based property names.\n\nTakes an argument list of property names, with support for indexed iterables.\n\n```py\nfrom syrupy.filters import props\n\ndef test_bar(snapshot):\n    actual = {\n      "id": uuid.uuid4(),\n      "list": [1,2,3],\n    }\n    assert actual == snapshot(exclude=props("id", "1"))\n```\n\n```py\n# name: test_bar\n  dict({\n    \'list\': list([\n      1,\n      3,\n    ]),\n  })\n# ---\n```\n\n###### `paths(path_string, *path_strings)`\n\nEasy way to build a filter that uses full path strings delimited with `.`.\n\nTakes an argument list of path strings.\n\n```py\nfrom syrupy.filters import paths\n\ndef test_bar(snapshot):\n    actual = {\n      "date": datetime.now(),\n      "list": [1,2,3],\n    }\n    assert actual == snapshot(exclude=paths("date", "list.1"))\n```\n\n```py\n# name: test_bar\n  dict({\n    \'list\': list([\n      1,\n      3,\n    ]),\n  })\n# ---\n```\n\n#### `extension_class`\n\nThis is a way to modify how the snapshot matches and serializes your data in a single assertion.\n\n```py\ndef test_foo(snapshot):\n    actual_svg = "<svg></svg>"\n    assert actual_svg == snapshot(extension_class=SVGImageSnapshotExtension)\n```\n\n#### `diff`\n\nThis is an option to snapshot only the diff between the actual object and a previous snapshot, with the `diff` argument being the previous snapshot `index`/`name`.\n\n```py\ndef test_diff(snapshot):\n    actual0 = [1,2,3,4]\n    actual1 = [0,1,3,4]\n\n    assert actual0 == snapshot\n    assert actual1 == snapshot(diff=0)\n    # This is equivalent to the lines above\n    # Must use the index name to diff when given\n    assert actual0 == snapshot(name=\'snap_name\')\n    assert actual1 == snapshot(diff=\'snap_name\')\n```\n\n##### Built-In Extensions\n\nSyrupy comes with a few built-in preset configurations for you to choose from. You should also feel free to extend the `AbstractSyrupyExtension` if your project has a need not captured by one our built-ins.\n\n- **`AmberSnapshotExtension`**: This is the default extension which generates `.ambr` files. Serialization of most data types are supported.\n  - Line control characters are normalised when snapshots are generated i.e. `\\r` and `\\n` characters are all written as `\\n`. This is to allow interoperability of snapshots between operating systems that use disparate line control characters.\n- **`SingleFileSnapshotExtension`**: Unlike the `AmberSnapshotExtension`, which groups all tests within a single test file into a singular snapshot file, this extension creates one `.raw` file per test case.\n- **`PNGImageSnapshotExtension`**: An extension of single file, this should be used to produce `.png` files from a byte string.\n- **`SVGImageSnapshotExtension`**: Another extension of single file. This produces `.svg` files from an svg string.\n- **`JSONSnapshotExtension`**: Another extension of single file. This produces `.json` files from dictionaries and lists.\n\n#### `name`\n\nBy default, if you make multiple snapshot assertions within a single test case, an auto-increment identifier will be used to index the snapshots. You can override this behaviour by specifying a custom snapshot name to use in place of the auto-increment number.\n\n```py\ndef test_case(snapshot):\n    assert "actual" == snapshot(name="case_a")\n    assert "other" == snapshot(name="case_b")\n```\n\n> _Warning_: If you use a custom name, you must make sure the name is not re-used within a test case.\n\n### Advanced Usage\n\nBy overriding the provided [`AbstractSnapshotExtension`](https://github.com/tophat/syrupy/tree/main/src/syrupy/extensions/base.py) you can implement varied custom behaviours.\n\nSee examples of how syrupy can be used and extended in the [test examples](https://github.com/tophat/syrupy/tree/main/tests/examples).\n\n#### JSONSnapshotExtension\n\nThis extension can be useful when testing API responses, or when you have to deal with long dictionaries that are cumbersome to validate inside a test. For example:\n\n```python\nimport pytest\n\nfrom syrupy.extensions.json import JSONSnapshotExtension\n\n@pytest.fixture\ndef snapshot_json(snapshot):\n    return snapshot.use_extension(JSONSnapshotExtension)\n\n\ndef test_api_call(client, snapshot_json):\n    resp = client.post("/endpoint")\n    assert resp.status_code == 200\n    assert snapshot_json == resp.json()\n```\n\nAPI responses often contain dynamic data, like IDs or dates. You can still validate and store other data of a response by leveraging syrupy matchers. For example:\n\n```py\nfrom datetime import datetime\n\nfrom syrupy.matchers import path_type\n\ndef test_api_call(client, snapshot_json):\n    resp = client.post("/user", json={"name": "Jane"})\n    assert resp.status_code == 201\n\n    matcher = path_type({\n      "id": (int,),\n      "registeredAt": (datetime,)\n    })\n    assert snapshot_json(matcher=matcher) == resp.json()\n```\n\nThe generated snapshot:\n\n```json\n{\n  "id": "<class \'int\'>",\n  "registeredAt": "<class \'datetime\'>",\n  "name": "Jane"\n}\n```\n\n### Extending Syrupy\n\n- [Custom snapshot directory 1](https://github.com/tophat/syrupy/tree/main/tests/examples/test_custom_snapshot_directory.py)\n- [Custom snapshot directory 2](https://github.com/tophat/syrupy/tree/main/tests/examples/test_custom_snapshot_directory_2.py)\n- [Custom snapshot name](https://github.com/tophat/syrupy/tree/main/tests/examples/test_custom_snapshot_name.py)\n- [Custom object snapshots](https://github.com/tophat/syrupy/tree/main/tests/examples/test_custom_object_repr.py)\n- [Custom comparator](https://github.com/tophat/syrupy/tree/main/tests/integration/test_custom_comparator.py)\n- [JPEG image extension](https://github.com/tophat/syrupy/tree/main/tests/examples/test_custom_image_extension.py)\n- [Built-in image extensions](https://github.com/tophat/syrupy/blob/main/tests/syrupy/extensions/image/test_image_svg.py)\n\n## Uninstalling\n\n```python\npip uninstall syrupy\n```\n\nIf you have decided not to use Syrupy for your project after giving us a try, we\'d love to get your feedback. Please create a GitHub issue if applicable, or drop a comment in our [Discord server](https://discord.gg/YhK3GFcZrk).\n\n## Benchmarks\n\nBenchmarks are automatically published to <https://tophat.github.io/syrupy/dev/bench/>.\n\n## Known Limitations\n\n- `pytest-xdist` support only partially exists. There is no issue when it comes to reads however when you attempt to run `pytest --snapshot-update`, if running with more than 1 process, the ability to detect unused snapshots is disabled. See [#535](https://github.com/tophat/syrupy/issues/535) for more information.\n\n_We welcome contributions to patch these known limitations._\n\n## Contributing\n\nFeel free to open a PR or GitHub issue. Contributions welcome!\n\nTo develop locally, clone this repository and run `. script/bootstrap` to install test dependencies. You can then use `invoke --list` to see available commands.\n\n### See contributing [guide](https://github.com/tophat/syrupy/tree/main/CONTRIBUTING.md)\n\n## Contributors\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore-start -->\n<!-- markdownlint-disable -->\n<table>\n  <tbody>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://noahnu.com"><img src="https://avatars0.githubusercontent.com/u/1297096?v=4?s=100" width="100px;" alt="Noah"/><br /><sub><b>Noah</b></sub></a><br /><a href="#infra-noahnu" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="#ideas-noahnu" title="Ideas, Planning, & Feedback">🤔</a> <a href="https://github.com/tophat/syrupy/commits?author=noahnu" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/commits?author=noahnu" title="Documentation">📖</a> <a href="https://github.com/tophat/syrupy/commits?author=noahnu" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://emmanuel.ogbizi.com"><img src="https://avatars0.githubusercontent.com/u/2528959?v=4?s=100" width="100px;" alt="Emmanuel Ogbizi"/><br /><sub><b>Emmanuel Ogbizi</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=iamogbz" title="Code">💻</a> <a href="#design-iamogbz" title="Design">🎨</a> <a href="#infra-iamogbz" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/tophat/syrupy/commits?author=iamogbz" title="Documentation">📖</a> <a href="https://github.com/tophat/syrupy/commits?author=iamogbz" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/adamlazz"><img src="https://avatars3.githubusercontent.com/u/453811?v=4?s=100" width="100px;" alt="Adam Lazzarato"/><br /><sub><b>Adam Lazzarato</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=adamlazz" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://mcataford.github.io"><img src="https://avatars2.githubusercontent.com/u/6210361?v=4?s=100" width="100px;" alt="Marc Cataford"/><br /><sub><b>Marc Cataford</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=mcataford" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/commits?author=mcataford" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://msrose.github.io"><img src="https://avatars3.githubusercontent.com/u/3495264?v=4?s=100" width="100px;" alt="Michael Rose"/><br /><sub><b>Michael Rose</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=msrose" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/commits?author=msrose" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://fashionablenonsense.com/"><img src="https://avatars0.githubusercontent.com/u/3112159?v=4?s=100" width="100px;" alt="Jimmy Jia"/><br /><sub><b>Jimmy Jia</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=taion" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/commits?author=taion" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://stevenloria.com"><img src="https://avatars2.githubusercontent.com/u/2379650?v=4?s=100" width="100px;" alt="Steven Loria"/><br /><sub><b>Steven Loria</b></sub></a><br /><a href="#infra-sloria" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/arturbalabanov"><img src="https://avatars1.githubusercontent.com/u/3062003?v=4?s=100" width="100px;" alt="Artur Balabanov"/><br /><sub><b>Artur Balabanov</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=arturbalabanov" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="http://huonw.github.io/"><img src="https://avatars1.githubusercontent.com/u/1203825?v=4?s=100" width="100px;" alt="Huon Wilson"/><br /><sub><b>Huon Wilson</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=huonw" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/issues?q=author%3Ahuonw" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/eaculb"><img src="https://avatars.githubusercontent.com/u/31480498?v=4?s=100" width="100px;" alt="Elizabeth Culbertson"/><br /><sub><b>Elizabeth Culbertson</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=eaculb" title="Code">💻</a> <a href="https://github.com/tophat/syrupy/commits?author=eaculb" title="Tests">⚠️</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/joakimnordling"><img src="https://avatars.githubusercontent.com/u/6637576?v=4?s=100" width="100px;" alt="Joakim Nordling"/><br /><sub><b>Joakim Nordling</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Ajoakimnordling" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/bendidi"><img src="https://avatars.githubusercontent.com/u/22003440?v=4?s=100" width="100px;" alt="Ouail"/><br /><sub><b>Ouail</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=bendidi" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/fbjorn"><img src="https://avatars.githubusercontent.com/u/9670990?v=4?s=100" width="100px;" alt="Denis"/><br /><sub><b>Denis</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=fbjorn" title="Code">💻</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/N0124"><img src="https://avatars.githubusercontent.com/u/29734397?v=4?s=100" width="100px;" alt="N0124"/><br /><sub><b>N0124</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=N0124" title="Code">💻</a></td>\n    </tr>\n    <tr>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/dtczest"><img src="https://avatars.githubusercontent.com/u/97055299?v=4?s=100" width="100px;" alt="dtczest"/><br /><sub><b>dtczest</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Adtczest" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/spagh-eddie"><img src="https://avatars.githubusercontent.com/u/58013020?v=4?s=100" width="100px;" alt="Eddie Darling"/><br /><sub><b>Eddie Darling</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=spagh-eddie" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/darrenburns"><img src="https://avatars.githubusercontent.com/u/5740731?v=4?s=100" width="100px;" alt="darrenburns"/><br /><sub><b>darrenburns</b></sub></a><br /><a href="https://github.com/tophat/syrupy/commits?author=darrenburns" title="Documentation">📖</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/mhwaage"><img src="https://avatars.githubusercontent.com/u/57612883?v=4?s=100" width="100px;" alt="Magnus Heskestad Waage"/><br /><sub><b>Magnus Heskestad Waage</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Amhwaage" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/herb"><img src="https://avatars.githubusercontent.com/u/139780?v=4?s=100" width="100px;" alt="Herbert Ho"/><br /><sub><b>Herbert Ho</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Aherb" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://github.com/tolgaeren"><img src="https://avatars.githubusercontent.com/u/794719?v=4?s=100" width="100px;" alt="Tolga Eren"/><br /><sub><b>Tolga Eren</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Atolgaeren" title="Bug reports">🐛</a></td>\n      <td align="center" valign="top" width="14.28%"><a href="https://johnkurkowski.com"><img src="https://avatars.githubusercontent.com/u/299487?v=4?s=100" width="100px;" alt="John Kurkowski"/><br /><sub><b>John Kurkowski</b></sub></a><br /><a href="https://github.com/tophat/syrupy/issues?q=author%3Ajohn-kurkowski" title="Bug reports">🐛</a></td>\n    </tr>\n  </tbody>\n</table>\n\n<!-- markdownlint-restore -->\n<!-- prettier-ignore-end -->\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis section is automatically generated via tagging the all-contributors bot in a PR:\n\n```text\n@all-contributors please add <username> for <contribution type>\n```\n\n## License\n\nSyrupy is licensed under [Apache License Version 2.0](https://github.com/tophat/syrupy/tree/main/LICENSE).\n',
     'author': 'Top Hat Open Source',
     'author_email': 'opensource@tophat.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/tophat/syrupy',
```

### Comparing `syrupy-4.0.7/PKG-INFO` & `syrupy-4.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syrupy
-Version: 4.0.7
+Version: 4.0.8
 Summary: Pytest Snapshot Test Utility
 Home-page: https://github.com/tophat/syrupy
 License: Apache-2.0
 Author: Top Hat Open Source
 Author-email: opensource@tophat.com
 Requires-Python: >=3.8.1,<4
 Classifier: Development Status :: 5 - Production/Stable
```

