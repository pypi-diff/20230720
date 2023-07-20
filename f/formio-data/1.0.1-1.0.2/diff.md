# Comparing `tmp/formio-data-1.0.1.tar.gz` & `tmp/formio-data-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "formio-data-1.0.1.tar", max compression
+gzip compressed data, was "formio-data-1.0.2.tar", max compression
```

## Comparing `formio-data-1.0.1.tar` & `formio-data-1.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-1.0.1/LICENSE
--rw-r--r--   0        0        0     6700 2023-07-18 09:56:07.631728 formio-data-1.0.1/README.md
--rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-1.0.1/formiodata/__init__.py
--rw-r--r--   0        0        0     3568 2023-07-18 09:56:07.636728 formio-data-1.0.1/formiodata/builder.py
--rw-r--r--   0        0        0    37451 2023-07-17 11:36:05.958057 formio-data-1.0.1/formiodata/components.py
--rw-r--r--   0        0        0     4204 2023-01-13 07:53:22.436294 formio-data-1.0.1/formiodata/form.py
--rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-1.0.1/formiodata/utils.py
--rw-r--r--   0        0        0      541 2023-07-18 09:56:07.636728 formio-data-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     7834 2023-07-18 09:56:25.275981 formio-data-1.0.1/setup.py
--rw-r--r--   0        0        0     7476 2023-07-18 09:56:25.277065 formio-data-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2022-06-23 06:15:09.395447 formio-data-1.0.2/LICENSE
+-rw-r--r--   0        0        0     7078 2023-07-20 13:19:40.411820 formio-data-1.0.2/README.md
+-rw-r--r--   0        0        0      171 2022-06-23 06:15:09.396448 formio-data-1.0.2/formiodata/__init__.py
+-rw-r--r--   0        0        0     3671 2023-07-20 12:53:08.545895 formio-data-1.0.2/formiodata/builder.py
+-rw-r--r--   0        0        0    37186 2023-07-20 13:04:30.500966 formio-data-1.0.2/formiodata/components.py
+-rw-r--r--   0        0        0     4204 2023-01-13 07:53:22.436294 formio-data-1.0.2/formiodata/form.py
+-rw-r--r--   0        0        0      979 2022-06-23 06:15:09.396448 formio-data-1.0.2/formiodata/utils.py
+-rw-r--r--   0        0        0      541 2023-07-20 13:05:13.439608 formio-data-1.0.2/pyproject.toml
+-rw-r--r--   0        0        0     8230 2023-07-20 15:39:41.701985 formio-data-1.0.2/setup.py
+-rw-r--r--   0        0        0     7854 2023-07-20 15:39:41.703042 formio-data-1.0.2/PKG-INFO
```

### Comparing `formio-data-1.0.1/LICENSE` & `formio-data-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.1/README.md` & `formio-data-1.0.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,7 +1,28 @@
+Metadata-Version: 2.1
+Name: formio-data
+Version: 1.0.2
+Summary: formio.js JSON-data API
+Home-page: https://github.com/novacode-nl/python-formio-data
+License: MIT
+Author: Bob Leers
+Author-email: bob@novacode.nl
+Requires-Python: >=3.6,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Provides-Extra: json_logic
+Requires-Dist: json_logic_qubit (>=0.9.1,<0.10.0); extra == "json_logic"
+Requires-Dist: python-dateutil (>=2.8.2,<3.0.0); python_version <= "3.6"
+Requires-Dist: requests
+Description-Content-Type: text/markdown
+
 # formio-data (Python)
 
 formio.js (JSON Form Builder) data API for Python.
 
 For information about the formio.js project, see https://github.com/formio/formio.js
 
 ## Introduction
@@ -143,43 +164,57 @@
 # alternative example, by getattr
 >> print(form.data.firstname.label)
 'First Name'
 
 >> print(form.data.firstname.value)
 'Bob'
 
-#################
-# components path
-#################
+#############################
+# component path (properties)
+#############################
 
 # datagrid input
 >> datagridMeasurements = builder.components['datagridMeasurements']
 
-# Component builder_path_key property
+# builder_path
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path)
+>>     for row in datagridMeasurements.rows
+>> ]
+[<panelComponent>, <columnsComponent>, <datagridComponent>, <datetimeComponent>]
+
+# builder_path_key
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_path_key)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['pageMeasurements', 'columnsExternal', 'datagridMeasurements', 'measurementDatetime']
 
-# Component builder_path_labels property
+# builder_path_labels
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_path_labels)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['Page Measurements', 'Columns External', 'Data Grid Measurements', 'Measurement Datetime']
 
-# Component builder_input_path_key property
+# builder_input_path
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path)
+>>     for row in datagridMeasurements.rows
+>> ]
+[<datagridComponent>, <datetimeComponent>]
+
+# builder_input_path_key
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_input_path_key)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['datagridMeasurements', 'measurementDatetime']
 
-# Component builder_input_path_labels property
+# builder_input_path_labels
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_input_path_labels)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['Data Grid Measurements', 'Measurement Datetime']
 
 #################################
@@ -228,7 +263,8 @@
 ```
 
 ### Run specific component unittest
 
 ```
 poetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear
 ```
+
```

### Comparing `formio-data-1.0.1/formiodata/builder.py` & `formio-data-1.0.2/formiodata/builder.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,24 +15,28 @@
 class Builder:
 
     def __init__(self, schema_json, **kwargs):
         """
         @param schema_json
         @param lang
         """
+
         if isinstance(schema_json, dict):
             self.schema = schema_json
         else:
             self.schema = json.loads(schema_json)
 
         self.language = kwargs.get('language', 'en')
         # i18n (translations)
         self.i18n = kwargs.get('i18n', {})
         self.resources = kwargs.get('resources', {})
 
+        # options from kwargs
+        self.load_path_objects = kwargs.get('load_path_objects', True)
+
         # Raw components from the schema
         self._raw_components = []
 
         # Raw components enriched with Component(object) API.
         self.raw_components = []
 
         # Key/value dictionay of all components for instant access.
```

### Comparing `formio-data-1.0.1/formiodata/components.py` & `formio-data-1.0.2/formiodata/components.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,19 @@
         self.builder = builder
 
         self._parent = None
         self._component_owner = None
         # components can also be seen as children
         self.components = OrderedDict()
 
-        # List of complete path components with keys. This includes
-        # layout components.
-        self.builder_path_key = []
-        # List of complete path components with labels. This includes
-        # layout components.
-        self.builder_path_label = []
-        # List of input components in path with keys. This only
+        # List of complete path components. This includes layout
+        # components.
+        self.builder_path = []
         # includes input components, so no layout components.
-        self.builder_input_path_key = []
-        # List of input components in path with labels. This only
-        # includes input components, so no layout components.
-        self.builder_input_path_label = []
+        self.builder_input_path = []
 
         # XXX uuid to ensure (hope this won't break anything)
         self.id = self.raw.get('id', str(uuid.uuid4()))
 
         # submission at this level {key: value, ...}
         # This includes a pseudo 'value' key which always encodes the current
         # component's value.  NOTE: This should be refactored away for conditionals
@@ -68,16 +61,17 @@
 
         self._all_data = all_data
         self.load_data(data)
 
         self.builder.component_ids[self.id] = self
 
         # parh
-        self.set_builder_path()
-        builder_path_key = '.'.join(self.builder_path_key)
+        self.set_builder_paths()
+        builder_path_keys = [p.key for p in self.builder_path]
+        builder_path_key = '.'.join(builder_path_keys)
         self.builder.components_path_key[builder_path_key] = self
 
     def load_data(self, data):
         if self.input and data:
             try:
                 self.value = data[self.key]
                 self.raw_value = data[self.key]
@@ -139,46 +133,54 @@
             self._component_owner.input_components[self.key] = self
 
     @property
     def child_component_owner(self):
         """The owner object for child components, to use in the recursion"""
         return self.component_owner
 
-    def set_builder_path(self):
-        builder_path_key = [self.key]
-        builder_path_label = [self.label]
-        builder_input_path_key = []
-        builder_input_path_label = []
+    @property
+    def builder_path_key(self):
+        return [p.key for p in self.builder_path]
 
-        if self.is_form_component:
-            builder_input_path_key.append(self.key)
-            builder_input_path_label.append(self.label)
+    @property
+    def builder_path_label(self):
+        return [p.label for p in self.builder_path]
 
+    @property
+    def builder_input_path_key(self):
+        return [p.key for p in self.builder_input_path]
+
+    @property
+    def builder_input_path_label(self):
+        return [p.label for p in self.builder_input_path]
+
+    def set_builder_paths(self):
+        builder_path = [self]
+        builder_input_path = []
+        if self.is_form_component:
+            if self.builder.load_path_objects:
+                builder_input_path.append(self)
         parent = self.parent
         while parent:
             if hasattr(parent, 'key'):
-                builder_path_key.append(parent.key)
-                builder_path_label.append(parent.label)
+                if self.builder.load_path_objects:
+                    builder_path.append(parent)
                 if parent.is_form_component:
-                    builder_input_path_key.append(parent.key)
-                    builder_input_path_label.append(parent.label)
+                    if self.builder.load_path_objects:
+                        builder_input_path.append(parent)
                 parent = parent.parent
             elif parent.__class__.__name__ == 'gridRow':
                 parent = parent.grid
             else:
                 parent = parent.component_owner
-        builder_path_key.reverse()
-        builder_path_label.reverse()
-        self.builder_path_key = builder_path_key
-        self.builder_path_label = builder_path_label
+        builder_path.reverse()
+        self.builder_path = builder_path
         # input path
-        builder_input_path_key.reverse()
-        builder_input_path_label.reverse()
-        self.builder_input_path_key = builder_input_path_key
-        self.builder_input_path_label = builder_input_path_label
+        builder_input_path.reverse()
+        self.builder_input_path = builder_input_path
 
     @property
     def validate(self):
         return self.raw.get('validate')
 
     @property
     def required(self):
@@ -968,15 +970,15 @@
         partial interface with input_components and components.
         TODO: Consider if there should be a shared base component for
         this (ComponentOwner?)
         """
         def __init__(self, grid, data):
             self.grid = grid
             self.builder = grid.builder
-            self.builder_path_key = None
+            self.builder_path = None
             self.input_components = {}
             self.components = OrderedDict()
             self.form = grid.form
             self.row = data
             self.html_component = ''
             grid.create_component_objects(self, data)
```

### Comparing `formio-data-1.0.1/formiodata/form.py` & `formio-data-1.0.2/formiodata/form.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.1/formiodata/utils.py` & `formio-data-1.0.2/formiodata/utils.py`

 * *Files identical despite different names*

### Comparing `formio-data-1.0.1/pyproject.toml` & `formio-data-1.0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "formio-data"
-version = "1.0.1"
+version = "1.0.2"
 homepage = "https://github.com/novacode-nl/python-formio-data"
 description = "formio.js JSON-data API"
 readme = "README.md"
 authors = ["Bob Leers <bob@novacode.nl>"]
 license = "MIT"
 packages = [ { include = "formiodata/**/*.py" } ]
 exclude = ["tests/*"]
```

### Comparing `formio-data-1.0.1/setup.py` & `formio-data-1.0.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,17 +12,17 @@
 
 extras_require = \
 {':python_version <= "3.6"': ['python-dateutil>=2.8.2,<3.0.0'],
  'json_logic': ['json_logic_qubit>=0.9.1,<0.10.0']}
 
 setup_kwargs = {
     'name': 'formio-data',
-    'version': '1.0.1',
+    'version': '1.0.2',
     'description': 'formio.js JSON-data API',
-    'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#################\n# components path\n#################\n\n# datagrid input\n>> datagridMeasurements = builder.components[\'datagridMeasurements\']\n\n# Component builder_path_key property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'pageMeasurements\', \'columnsExternal\', \'datagridMeasurements\', \'measurementDatetime\']\n\n# Component builder_path_labels property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Page Measurements\', \'Columns External\', \'Data Grid Measurements\', \'Measurement Datetime\']\n\n# Component builder_input_path_key property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'datagridMeasurements\', \'measurementDatetime\']\n\n# Component builder_input_path_labels property\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Data Grid Measurements\', \'Measurement Datetime\']\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
+    'long_description': '# formio-data (Python)\n\nformio.js (JSON Form Builder) data API for Python.\n\nFor information about the formio.js project, see https://github.com/formio/formio.js\n\n## Introduction\n\n**python-formio-data** is a Python package, which loads and transforms\nformio.js **Builder JSON** and **Form JSON** into **usable Python objects**.  It\'s main\naim is to provide easy access to a Form its components/fields, also\ncaptured as **Python objects**, which makes this API very versatile and usable.\n\n**Notes about terms:**\n  - **Builder:** The Form Builder which is the design/blueprint of a Form.\n  - **Form:** A filled-in Form, aka Form submission.\n  - **Component:** Input (field) or layout component in the Form Builder and Form.\n\n## Features\n\n  - Compatible with Python 3.6 and later\n  - Constructor of the **Builder** and **Form** class, only requires\n    the JSON and an optional language code for translations.\n  - Get a Form object its Components as a usable object e.g. datetime, boolean, dict (for select component) etc.\n  - Open source (MIT License)\n\n## Installation\n\nThe source code is currently hosted on GitHub at:\nhttps://github.com/novacode-nl/python-formio-data\n\n### PyPI - Python Package Index\n\nBinary installers for the latest released version are available at the [Python\nPackage Index](https://pypi.python.org/pypi/formio-data)\n\n```sh\npip(3) install formio-data\n```\n\n#### Optional dependencies\n\nTo support conditional visibility using JSON logic, you can install\nthe `json-logic-qubit` package (the `json-logic` package it is forked\noff of is currently unmaintained).  It\'s also possible to install it\nvia the pip feature `json_logic` like so:\n\n```sh\npip(3) install -U formio-data[json_logic]\n```\n\n### Source Install with Poetry (recommended)\n\nConvenient for developers. Also useful for running the (unit)tests.\n\n```sh\ngit clone git@github.com:novacode-nl/python-formio-data.git\npoetry install\n```\n\n#### Optional dependencies\n\nWhen working in the project itself, use\n\n```sh\npoetry install -E json_logic\n```\n\n### Source Install with pip\n\nOptional dependencies need to be installed separately.\n\n```sh\npip(3) install -U -e python-formio-data\n```\n\n## Using direnv\n\nYou can use [nixpkgs](https://nixos.org/) to run a self-contained\nPython environment without any additional setup.  Once you\'ve\ninstalled nixpkgs, switch into the directory and type "nix-shell" to\nget a shell from which the correct Python with packages is available.\n\nIf you\'re using [direnv](https://direnv.net/), use `direnv allow`\nafter changing into the project directory and you\'re good to go.  Also\nconsider [nix-direnv](https://github.com/nix-community/nix-direnv) to\nspeed up the experience (it can re-use a cached local installation).\n\n## License\n[MIT](LICENSE)\n\n## Contributing\nAll contributions, bug reports, bug fixes, documentation improvements, enhancements and ideas are welcome.\n\n## Usage examples\n\nFor more examples of usage, see the unit-tests.\n\n``` python\n>> from formiodata import Builder, Form\n>>\n# builder_json is a formio.js Builder JSON document (text/string)\n# form_json is a formio.js Form JSON document (text/string)\n>>\n>> builder = Builder(builder_json)\n>> form = Form(builder, form_json)\n\n##################\n# input components\n##################\n\n# textfield label\n>> print(form.input_components[\'firstname\'].label)\n\'First Name\'\n\n# textfield value\n>> print(form.input_components[\'firstname\'].value)\n\'Bob\'\n\n# datetime label\n>> print(form.input_components[\'birthday\'].label)\n\'Birthday\'\n\n# datetime value\n>> print(form.input_components[\'birthday\'].value)\ndatetime.date(2009 10 16)\n\n# datagrid (rows property)\n>> print(form.input_components[\'datagridMeasurements\'].rows)\n[\n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}, \n  {\'measurementDatetime\': <datetimeComponent>, \'measurementFahrenheit\': <numberComponent>}\n]\n\n>> for row in form.input_components[\'datagridMeasurements\'].rows:\n>>    dtime = row[\'measurementDatetime\']\n>>    fahrenheit = row[\'measurementFahrenheit\']\n>>    print(%s: %s, %s: %s\' % (dt.label, dt.value, fahrenheit.label, fahrenheit.value))\n\nDatetime: datetime.datetime(2021, 5, 8, 11, 39, 0, 296487), Fahrenheit: 122\nDatetime: datetime.datetime(2021, 5, 8, 11, 41, 5, 919943), Fahrenheit: 131\n\n# alternative example, by getattr\n>> print(form.data.firstname.label)\n\'First Name\'\n\n>> print(form.data.firstname.value)\n\'Bob\'\n\n#############################\n# component path (properties)\n#############################\n\n# datagrid input\n>> datagridMeasurements = builder.components[\'datagridMeasurements\']\n\n# builder_path\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path)\n>>     for row in datagridMeasurements.rows\n>> ]\n[<panelComponent>, <columnsComponent>, <datagridComponent>, <datetimeComponent>]\n\n# builder_path_key\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'pageMeasurements\', \'columnsExternal\', \'datagridMeasurements\', \'measurementDatetime\']\n\n# builder_path_labels\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Page Measurements\', \'Columns External\', \'Data Grid Measurements\', \'Measurement Datetime\']\n\n# builder_input_path\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path)\n>>     for row in datagridMeasurements.rows\n>> ]\n[<datagridComponent>, <datetimeComponent>]\n\n# builder_input_path_key\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_key)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'datagridMeasurements\', \'measurementDatetime\']\n\n# builder_input_path_labels\n>> [\n>>     print(row.input_components[\'measurementDatetime\'].builder_input_path_labels)\n>>     for row in datagridMeasurements.rows\n>> ]\n[\'Data Grid Measurements\', \'Measurement Datetime\']\n\n#################################\n# components (layout, input etc.)\n#################################\n\n# columns\n>> print(form.components[\'addressColumns\'])\n<columnsComponent>\n\n>> print(form.components[\'addressColumns\'].rows)\n[ \n  {\'firstName\': <textfieldComponent>, \'lastName: <textfieldComponent>}, \n  {\'email\': <emailComponent>, \'companyName: <textfieldComponent>}\n]\n```\n\n## Unit tests\n\n**Note:**\n\nInternet access is recommended for running the `filecStorageUrlComponentTestCase`, because this also tests the URL Storage (type).\\\nIf no internet access, this test won\'t fail and a WARNING shall be logged regarding a ConnectionError.\n\n### Run all unittests\n\nFrom toplevel directory:\n\n```\npoetry install -E json_logic  # if you haven\'t already\npoetry run python -m unittest\n```\n\n### Run component unittests\n\nAll Components, from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_component_*.py\n```\n\nNested components (complexity), from toplevel directory:\n\n```\npoetry run python -m unittest tests/test_nested_components.py\n```\n\n### Run specific component unittest\n\n```\npoetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear\n```\n',
     'author': 'Bob Leers',
     'author_email': 'bob@novacode.nl',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/novacode-nl/python-formio-data',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `formio-data-1.0.1/PKG-INFO` & `formio-data-1.0.2/README.md`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,7 @@
-Metadata-Version: 2.1
-Name: formio-data
-Version: 1.0.1
-Summary: formio.js JSON-data API
-Home-page: https://github.com/novacode-nl/python-formio-data
-License: MIT
-Author: Bob Leers
-Author-email: bob@novacode.nl
-Requires-Python: >=3.6,<4.0
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Provides-Extra: json_logic
-Requires-Dist: json_logic_qubit (>=0.9.1,<0.10.0); extra == "json_logic"
-Requires-Dist: python-dateutil (>=2.8.2,<3.0.0); python_version <= "3.6"
-Requires-Dist: requests
-Description-Content-Type: text/markdown
-
 # formio-data (Python)
 
 formio.js (JSON Form Builder) data API for Python.
 
 For information about the formio.js project, see https://github.com/formio/formio.js
 
 ## Introduction
@@ -164,43 +143,57 @@
 # alternative example, by getattr
 >> print(form.data.firstname.label)
 'First Name'
 
 >> print(form.data.firstname.value)
 'Bob'
 
-#################
-# components path
-#################
+#############################
+# component path (properties)
+#############################
 
 # datagrid input
 >> datagridMeasurements = builder.components['datagridMeasurements']
 
-# Component builder_path_key property
+# builder_path
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_path)
+>>     for row in datagridMeasurements.rows
+>> ]
+[<panelComponent>, <columnsComponent>, <datagridComponent>, <datetimeComponent>]
+
+# builder_path_key
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_path_key)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['pageMeasurements', 'columnsExternal', 'datagridMeasurements', 'measurementDatetime']
 
-# Component builder_path_labels property
+# builder_path_labels
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_path_labels)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['Page Measurements', 'Columns External', 'Data Grid Measurements', 'Measurement Datetime']
 
-# Component builder_input_path_key property
+# builder_input_path
+>> [
+>>     print(row.input_components['measurementDatetime'].builder_input_path)
+>>     for row in datagridMeasurements.rows
+>> ]
+[<datagridComponent>, <datetimeComponent>]
+
+# builder_input_path_key
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_input_path_key)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['datagridMeasurements', 'measurementDatetime']
 
-# Component builder_input_path_labels property
+# builder_input_path_labels
 >> [
 >>     print(row.input_components['measurementDatetime'].builder_input_path_labels)
 >>     for row in datagridMeasurements.rows
 >> ]
 ['Data Grid Measurements', 'Measurement Datetime']
 
 #################################
@@ -249,8 +242,7 @@
 ```
 
 ### Run specific component unittest
 
 ```
 poetry run python -m unittest tests.test_component_day.dayComponentTestCase.test_get_form_dayMonthYear
 ```
-
```

