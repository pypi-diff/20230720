# Comparing `tmp/extendable_pydantic-0.0.5.tar.gz` & `tmp/extendable_pydantic-1.0.0.tar.gz`

## Comparing `extendable_pydantic-0.0.5.tar` & `extendable_pydantic-1.0.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/extendable_pydantic_patcher.pth
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/src/extendable_pydantic/__init__.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/src/extendable_pydantic/_patch.py
--rw-r--r--   0        0        0     4538 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/src/extendable_pydantic/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/src/extendable_pydantic/py.typed
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/LICENSE
--rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/README.md
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3442 2020-02-02 00:00:00.000000 extendable_pydantic-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/extendable_pydantic_patcher.pth
+-rw-r--r--   0        0        0      163 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/__init__.py
+-rw-r--r--   0        0        0     2661 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/_patch.py
+-rw-r--r--   0        0        0     6136 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/py.typed
+-rw-r--r--   0        0        0     4718 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/utils.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/src/extendable_pydantic/version.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/README.md
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3763 2020-02-02 00:00:00.000000 extendable_pydantic-1.0.0/PKG-INFO
```

### Comparing `extendable_pydantic-0.0.5/.gitignore` & `extendable_pydantic-1.0.0/.gitignore`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.5/LICENSE` & `extendable_pydantic-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `extendable_pydantic-0.0.5/README.md` & `extendable_pydantic-1.0.0/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 [![CI](https://github.com/lmignon/pydantic-ext/actions/workflows/ci.yml/badge.svg)](https://github.com/lmignon/pydantic-ext/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/lmignon/pydantic-ext/branch/master/graph/badge.svg?token=Z9FWM57T14)](https://codecov.io/gh/lmignon/pydantic-ext)
 
-# pydantic-ext
+# Extendable Pydantic
 
 This addons provides a new type used to declare [Pydantic](https://pypi.org/project/pydantic/)
 model as [Extendable](https://pypi.org/project/extendable/) class.
 
+From release 1.0.0 it only supports Pydantic >= 2.0.0.
+
+
 ```python
 from pydantic import BaseModel
 from extendable_pydantic import ExtendableModelMeta
 from extendable import context, registry
 
 class Location(BaseModel, metaclass=ExtendableModelMeta):
     lat = 0.1
@@ -20,25 +23,28 @@
 
 _registry = registry.ExtendableClassesRegistry()
 context.extendable_registry.set(_registry)
 _registry.init_registry()
 
 loc = Location(**{"lat": 12.3, "lng": 13.2, "name": "My Loc"})
 
-loc.dict() == {"lat": 12.3, "lng": 13.2, "name": "My Loc"}
+loc.model_dump() == {"lat": 12.3, "lng": 13.2, "name": "My Loc"}
 #> True
 
-loc.schema()
+loc.model_json_schema()
 #> {'title': 'Location', 'type': 'object', 'properties': {'lat': {'title': 'Lat', 'default': 0.1, 'type': 'number'}, 'lng': {'title': 'Lng', 'default': 10.1, 'type': 'number'}, 'name': {'title': 'Name', 'type': 'string'}}, 'required': ['name']}
 ```
 
 ## Development
 
 `pip install -e .`
 
 Then, copy `extendable_pydantic_patcher.pth` to `$VIRTUAL_ENV/lib/python3.10/site-packages`.
 
 ## Release
 
-* Tag the sources: `git tag x.y.z`
-* Build the package: `hatch build`
-* Publish to pypi: `twine upload dist/*`
+
+* run ``bumpversion patch|minor|major --list
+* Check the new_version value returned by the previous command
+* run towncrier build.
+* Inspect and commit the updated HISTORY.rst.
+* git tag {new_version} ; git push --tags.
```

### Comparing `extendable_pydantic-0.0.5/pyproject.toml` & `extendable_pydantic-1.0.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,43 +1,48 @@
 [build-system]
-requires = ["hatchling", "hatch-vcs"]
+requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "extendable_pydantic"
 authors = [{name = "Laurent Mignon", email = "laurent.mignon@acsone.eu"}]
 readme = "README.md"
 license = {file = "LICENSE"}
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
 ]
 dynamic = ["version", "description"]
 dependencies = [
-    "extendable>=0.0.3",
-    "pydantic",
+    "extendable>=1.0.0",
+    "pydantic>=2.0.2",
     "wrapt",
 ]
-requires-python = ">=3.6"
+requires-python = ">=3.7"
 
 [project.optional-dependencies]
 test = [
     "pytest",
     "coverage[toml]",
 ]
 mypy = [
-    "mypy",
+    "mypy>=1.4.1",
+]
+release = [
+    "towncrier",
+    "bumpversion",
 ]
 
 [project.urls]
 Source = "https://github.com/lmignon/extendable-pydantic"
 
 [tool.hatch.version]
-source = "vcs"
+path="src/extendable_pydantic/version.py"
+
 
 [tool.hatch.build]
 include = ["src/extendable_pydantic", "extendable_pydantic_patcher.pth"]
 # TODO add typodoo_activate.pth to editable wheel?
 directory = "dist"
 
 [tool.hatch.build.targets.wheel]
@@ -72,7 +77,24 @@
 ignore = [
     "E501",  # line too long, handled by black
  ]
 
 [tool.ruff.per-file-ignores]
 "__init__.py" = ["F401"]
 "tests/test_forward_refs.py" = ["F821"]
+
+[[tool.mypy.overrides]]
+module = "pydantic.main"
+implicit_reexport = true
+
+[[tool.mypy.overrides]]
+module="pydantic._internal._generate_schema"
+implicit_reexport = true
+
+[tool.towncrier]
+name = "Extendable Pydantic"
+package = "extendable_pydantic"
+package_dir = "src"
+filename = "HISTORY.rst"
+directory = "news"
+issue_format = "`#{issue} <https://github.com/lmignon/extendable-pydantic/issues/{issue}>`_"
+title_format = "{version} ({project_date})"
```

### Comparing `extendable_pydantic-0.0.5/PKG-INFO` & `extendable_pydantic-1.0.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: extendable_pydantic
-Version: 0.0.5
+Version: 1.0.0
 Project-URL: Source, https://github.com/lmignon/extendable-pydantic
 Author-email: Laurent Mignon <laurent.mignon@acsone.eu>
 License: MIT License
         
         Copyright (c) 2021 Laurent Mignon (ACSONE)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -24,33 +24,39 @@
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 License-File: LICENSE
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Requires-Dist: extendable>=0.0.3
-Requires-Dist: pydantic
+Requires-Python: >=3.7
+Requires-Dist: extendable>=1.0.0
+Requires-Dist: pydantic>=2.0.2
 Requires-Dist: wrapt
 Provides-Extra: mypy
-Requires-Dist: mypy; extra == 'mypy'
+Requires-Dist: mypy>=1.4.1; extra == 'mypy'
+Provides-Extra: release
+Requires-Dist: bumpversion; extra == 'release'
+Requires-Dist: towncrier; extra == 'release'
 Provides-Extra: test
 Requires-Dist: coverage[toml]; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 [![CI](https://github.com/lmignon/pydantic-ext/actions/workflows/ci.yml/badge.svg)](https://github.com/lmignon/pydantic-ext/actions/workflows/ci.yml)
 [![codecov](https://codecov.io/gh/lmignon/pydantic-ext/branch/master/graph/badge.svg?token=Z9FWM57T14)](https://codecov.io/gh/lmignon/pydantic-ext)
 
-# pydantic-ext
+# Extendable Pydantic
 
 This addons provides a new type used to declare [Pydantic](https://pypi.org/project/pydantic/)
 model as [Extendable](https://pypi.org/project/extendable/) class.
 
+From release 1.0.0 it only supports Pydantic >= 2.0.0.
+
+
 ```python
 from pydantic import BaseModel
 from extendable_pydantic import ExtendableModelMeta
 from extendable import context, registry
 
 class Location(BaseModel, metaclass=ExtendableModelMeta):
     lat = 0.1
@@ -61,25 +67,28 @@
 
 _registry = registry.ExtendableClassesRegistry()
 context.extendable_registry.set(_registry)
 _registry.init_registry()
 
 loc = Location(**{"lat": 12.3, "lng": 13.2, "name": "My Loc"})
 
-loc.dict() == {"lat": 12.3, "lng": 13.2, "name": "My Loc"}
+loc.model_dump() == {"lat": 12.3, "lng": 13.2, "name": "My Loc"}
 #> True
 
-loc.schema()
+loc.model_json_schema()
 #> {'title': 'Location', 'type': 'object', 'properties': {'lat': {'title': 'Lat', 'default': 0.1, 'type': 'number'}, 'lng': {'title': 'Lng', 'default': 10.1, 'type': 'number'}, 'name': {'title': 'Name', 'type': 'string'}}, 'required': ['name']}
 ```
 
 ## Development
 
 `pip install -e .`
 
 Then, copy `extendable_pydantic_patcher.pth` to `$VIRTUAL_ENV/lib/python3.10/site-packages`.
 
 ## Release
 
-* Tag the sources: `git tag x.y.z`
-* Build the package: `hatch build`
-* Publish to pypi: `twine upload dist/*`
+
+* run ``bumpversion patch|minor|major --list
+* Check the new_version value returned by the previous command
+* run towncrier build.
+* Inspect and commit the updated HISTORY.rst.
+* git tag {new_version} ; git push --tags.
```

