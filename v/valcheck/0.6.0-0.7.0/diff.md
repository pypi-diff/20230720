# Comparing `tmp/valcheck-0.6.0.tar.gz` & `tmp/valcheck-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "valcheck-0.6.0.tar", last modified: Sun Jul 16 13:23:53 2023, max compression
+gzip compressed data, was "valcheck-0.7.0.tar", last modified: Thu Jul 20 15:41:40 2023, max compression
```

## Comparing `valcheck-0.6.0.tar` & `valcheck-0.7.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.418991 valcheck-0.6.0/
--rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.6.0/LICENSE
--rw-rw-rw-   0        0        0      760 2023-07-16 13:23:53.417992 valcheck-0.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     2674 2023-07-16 13:12:11.000000 valcheck-0.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-07-16 13:23:53.419998 valcheck-0.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1568 2023-07-16 13:12:11.000000 valcheck-0.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.396372 valcheck-0.6.0/valcheck/
--rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.6.0/valcheck/__init__.py
--rw-rw-rw-   0        0        0     1270 2023-07-02 09:39:38.000000 valcheck-0.6.0/valcheck/exceptions.py
--rw-rw-rw-   0        0        0    21775 2023-07-16 07:09:18.000000 valcheck-0.6.0/valcheck/fields.py
--rw-rw-rw-   0        0        0     2694 2023-07-15 05:51:54.000000 valcheck-0.6.0/valcheck/models.py
--rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-0.6.0/valcheck/utils.py
--rw-rw-rw-   0        0        0     6039 2023-07-16 13:10:09.000000 valcheck-0.6.0/valcheck/validator.py
-drwxrwxrwx   0        0        0        0 2023-07-16 13:23:53.415998 valcheck-0.6.0/valcheck.egg-info/
--rw-rw-rw-   0        0        0      760 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-07-16 13:23:53.000000 valcheck-0.6.0/valcheck.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-07-20 15:41:40.740943 valcheck-0.7.0/
+-rw-rw-rw-   0        0        0     1087 2023-07-02 09:39:38.000000 valcheck-0.7.0/LICENSE
+-rw-rw-rw-   0        0        0      760 2023-07-20 15:41:40.737950 valcheck-0.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1230 2023-07-20 15:41:20.000000 valcheck-0.7.0/README.md
+-rw-rw-rw-   0        0        0       42 2023-07-20 15:41:40.740943 valcheck-0.7.0/setup.cfg
+-rw-rw-rw-   0        0        0     1568 2023-07-20 15:41:20.000000 valcheck-0.7.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-07-20 15:41:40.715492 valcheck-0.7.0/valcheck/
+-rw-rw-rw-   0        0        0        0 2023-07-02 09:39:38.000000 valcheck-0.7.0/valcheck/__init__.py
+-rw-rw-rw-   0        0        0     1570 2023-07-20 15:41:20.000000 valcheck-0.7.0/valcheck/exceptions.py
+-rw-rw-rw-   0        0        0    21939 2023-07-20 15:41:20.000000 valcheck-0.7.0/valcheck/fields.py
+-rw-rw-rw-   0        0        0     2685 2023-07-20 15:41:20.000000 valcheck-0.7.0/valcheck/models.py
+-rw-rw-rw-   0        0        0     3156 2023-07-16 07:09:18.000000 valcheck-0.7.0/valcheck/utils.py
+-rw-rw-rw-   0        0        0     7209 2023-07-20 15:41:20.000000 valcheck-0.7.0/valcheck/validator.py
+drwxrwxrwx   0        0        0        0 2023-07-20 15:41:40.736951 valcheck-0.7.0/valcheck.egg-info/
+-rw-rw-rw-   0        0        0      760 2023-07-20 15:41:40.000000 valcheck-0.7.0/valcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-07-20 15:41:40.000000 valcheck-0.7.0/valcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-07-20 15:41:40.000000 valcheck-0.7.0/valcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-07-20 15:41:40.000000 valcheck-0.7.0/valcheck.egg-info/top_level.txt
```

### Comparing `valcheck-0.6.0/LICENSE` & `valcheck-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `valcheck-0.6.0/PKG-INFO` & `valcheck-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `valcheck-0.6.0/setup.py` & `valcheck-0.7.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import find_packages, setup
 
 # Constants
 PACKAGE_NAME = "valcheck"
-PACKAGE_VERSION = "0.6.0"
+PACKAGE_VERSION = "0.7.0"
 AUTHOR_NAME = "Nishant Rao"
 AUTHOR_EMAIL_ID = "nishant.rao173@gmail.com"
 FILEPATH_TO_README = os.path.join(os.path.abspath(os.path.dirname(__file__)), "README.md")
 FILEPATH_TO_REQUIREMENTS = os.path.join(os.path.abspath(os.path.dirname(__file__)), "requirements.txt")
 REPOSITORY_URL = "https://github.com/Nishant173/valcheck"
 
 # Requirements
```

### Comparing `valcheck-0.6.0/valcheck/exceptions.py` & `valcheck-0.7.0/valcheck/exceptions.py`

 * *Files 23% similar despite different names*

```diff
@@ -6,14 +6,24 @@
 
 def _validate_list_of_errors(obj: Any, /) -> None:
     """Ensures that the given object is a list of errors (each of type `valcheck.models.Error`)"""
     if not is_list_of_instances_of_type(obj, type_=Error, allow_empty=True):
         raise ValueError("Must be list of errors (each of type `valcheck.models.Error`)")
 
 
+class DuplicateSourcesException(Exception):
+    """Exception to be raised when a validator finds duplicate sources for it's fields"""
+    pass
+
+
+class DuplicateTargetsException(Exception):
+    """Exception to be raised when a validator finds duplicate targets for it's fields"""
+    pass
+
+
 class MissingFieldException(Exception):
     """Exception to be raised when a field is missing"""
     pass
 
 
 class ValidationException(Exception):
     """Exception to be raised when data validation fails"""
```

### Comparing `valcheck-0.6.0/valcheck/fields.py` & `valcheck-0.7.0/valcheck/fields.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from __future__ import annotations
 
-from copy import deepcopy
+import copy
 from typing import Any, Callable, Iterable, List, Optional, Type, Union
 
 from valcheck.models import Error
 from valcheck import utils
 
 
 class ValidatedField:
     """Class that represents a validated field"""
 
     def __init__(
             self,
             *,
-            field_identifier: str,
-            field_name: str,
-            field_value: Union[Any, utils.Empty],
+            field: Field,
             errors: List[Error],
         ) -> None:
-        assert isinstance(field_identifier, str), "Param `field_identifier` must be of type 'str'"
-        assert isinstance(field_name, str), "Param `field_name` must be of type 'str'"
+        assert isinstance(field, Field), "Param `field` must be of type `valcheck.fields.Field`"
         assert utils.is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "Param `errors` must be a list where each item is of type `valcheck.models.Error`"
         )
-
-        self.field_identifier = field_identifier
-        self.field_name = field_name
-        self._field_value = field_value
+        self._field = field
         self._errors = errors
 
     def __str__(self) -> str:
-        return f"{self.__class__.__name__}(field_identifier='{self.field_identifier}', field_name='{self.field_name}')"
+        kwargs_list = [
+            f"is_valid={not bool(self.errors)}",
+            f"field_identifier={utils.wrap_in_quotes_if_string(self.field.field_identifier)}",
+            f"field_value={utils.wrap_in_quotes_if_string(self.field.field_value)}",
+            f"source={utils.wrap_in_quotes_if_string(self.field.source)}",
+            f"target={utils.wrap_in_quotes_if_string(self.field.target)}",
+            f"required={self.field.required}",
+            f"nullable={self.field.nullable}",
+        ]
+        kwargs_string = "(" + ", ".join(kwargs_list) + ")"
+        return f"{self.__class__.__name__}{kwargs_string}"
 
     @property
-    def field_value(self) -> Union[Any, utils.Empty]:
-        return self._field_value
+    def field(self) -> Field:
+        return self._field
 
-    @field_value.setter
-    def field_value(self, value: Union[Any, utils.Empty]) -> None:
-        self._field_value = value
+    @field.setter
+    def field(self, value: Field) -> None:
+        assert isinstance(value, Field), "Param `field` must be of type `valcheck.fields.Field`"
+        self._field = value
 
     @property
     def errors(self) -> List[Error]:
         return self._errors
 
     @errors.setter
     def errors(self, value: List[Error]) -> None:
@@ -54,37 +59,42 @@
 
 class Field:
     """Class that represents a field (that needs to be validated)"""
 
     def __init__(
             self,
             *,
-            alias: Optional[str] = None,
+            source: Optional[str] = None,
+            target: Optional[str] = None,
             required: Optional[bool] = True,
             nullable: Optional[bool] = False,
             default_factory: Optional[Callable] = None,
             converter_factory: Optional[Callable] = None,
             validators: Optional[List[Callable]] = None,
             error: Optional[Error] = None,
         ) -> None:
         """
         Parameters:
-            - alias (str): Alias for the field's name (optional)
+            - source (str): Field name used in the input data (optional)
+            - target (str): Field name used in the validated data (optional)
             - required (bool): True if the field is required, else False. Default: True
             - nullable (bool): True if the field is nullable, else False. Default: False
             - default_factory (callable): Callable that returns the default value to set for the field
             if `required=False` and the field is missing.
             - converter_factory (callable): Callable that takes in the validated value (of the field), and returns
             the converted value (for the field).
             - validators (list of callables): List of callables that each return a boolean (takes the field value as a param).
             The callable returns True if validation is successful, else False.
             - error (Error instance): Instance of type `valcheck.models.Error`.
         """
-        assert alias is None or utils.is_valid_object_of_type(alias, type_=str, allow_empty=False), (
-            "Param `alias` must be of type 'str' and must be non-empty"
+        assert source is None or utils.is_valid_object_of_type(source, type_=str, allow_empty=False), (
+            "Param `source` must be of type 'str' and must be non-empty"
+        )
+        assert target is None or utils.is_valid_object_of_type(target, type_=str, allow_empty=False), (
+            "Param `target` must be of type 'str' and must be non-empty"
         )
         assert isinstance(required, bool), "Param `required` must be of type 'bool'"
         assert isinstance(nullable, bool), "Param `nullable` must be of type 'bool'"
         assert default_factory is None or callable(default_factory), (
             "Param `default_factory` must be a callable that returns the default value if the field is missing when `required=False`"
         )
         assert converter_factory is None or callable(converter_factory), (
@@ -94,34 +104,34 @@
         assert validators is None or isinstance(validators, list), "Param `validators` must be of type 'list'"
         if isinstance(validators, list):
             for validator in validators:
                 assert callable(validator), "Param `validators` must be a list of callables"
         assert error is None or isinstance(error, Error), "Param `error` must be of type `valcheck.models.Error`"
 
         self._field_identifier = utils.set_as_empty()
-        self._field_name = utils.set_as_empty()
         self._field_value = utils.set_as_empty()
-        self.alias = alias
+        self.source = source
+        self.target = target
         self.required = required
         self.nullable = nullable
         self.default_factory = default_factory
         self.converter_factory = converter_factory
         self.validators = validators or []
         self.error = error or Error()
 
     def copy(self) -> Field:
         """Returns deep-copy of current `Field` object"""
-        return deepcopy(self)
+        return copy.deepcopy(self)
 
     def __str__(self) -> str:
         kwargs_list = [
             f"field_identifier={utils.wrap_in_quotes_if_string(self.field_identifier)}",
-            f"field_name={utils.wrap_in_quotes_if_string(self.field_name)}",
             f"field_value={utils.wrap_in_quotes_if_string(self.field_value)}",
-            f"alias={utils.wrap_in_quotes_if_string(self.alias)}",
+            f"source={utils.wrap_in_quotes_if_string(self.source)}",
+            f"target={utils.wrap_in_quotes_if_string(self.target)}",
             f"required={self.required}",
             f"nullable={self.nullable}",
         ]
         kwargs_string = "(" + ", ".join(kwargs_list) + ")"
         return f"{self.__class__.__name__}{kwargs_string}"
 
     @property
@@ -130,28 +140,19 @@
 
     @field_identifier.setter
     def field_identifier(self, value: str) -> None:
         assert isinstance(value, str), "Param `field_identifier` must be of type 'str'"
         self._field_identifier = value
 
     @property
-    def field_name(self) -> str:
-        return self._field_name
-
-    @field_name.setter
-    def field_name(self, value: str) -> None:
-        assert isinstance(value, str), "Param `field_name` must be of type 'str'"
-        self._field_name = value
-
-    @property
-    def field_value(self) -> Any:
+    def field_value(self) -> Union[Any, utils.Empty]:
         return self._field_value
 
     @field_value.setter
-    def field_value(self, value: Any) -> None:
+    def field_value(self, value: Union[Any, utils.Empty]) -> None:
         self._field_value = value
 
     def _can_be_set_to_null(self) -> bool:
         return self.nullable and self.field_value is None
 
     def _has_valid_custom_validators(self) -> bool:
         if not self.validators:
@@ -170,24 +171,19 @@
     def validate(self) -> List[Error]:
         """Returns list of errors (each of type `valcheck.models.Error`)"""
         raise NotImplementedError()
 
     def run_validations(self) -> ValidatedField:
         if utils.is_empty(self.field_value) and not self.required and self.default_factory:
             self.field_value = self.default_factory()
-        validated_field = ValidatedField(
-            field_identifier=self.field_identifier,
-            field_name=self.field_name,
-            field_value=self.field_value,
-            errors=[],
-        )
+        validated_field = ValidatedField(field=self, errors=[])
         if utils.is_empty(self.field_value) and not self.required and not self.default_factory:
             return validated_field
         if self._can_be_set_to_null():
-            validated_field.field_value = self._convert_field_value_if_needed()
+            validated_field.field.field_value = self._convert_field_value_if_needed()
             return validated_field
         if utils.is_empty(self.field_value) and self.required:
             validated_field.errors += [
                 self.create_error_instance(validator_message=self.missing_field_error_message()),
             ]
             return validated_field
         errors = self.validate()
@@ -195,36 +191,36 @@
             validated_field.errors += errors
             return validated_field
         if not self._has_valid_custom_validators():
             validated_field.errors += [
                 self.create_error_instance(validator_message=self.invalid_field_error_message()),
             ]
             return validated_field
-        validated_field.field_value = self._convert_field_value_if_needed()
+        validated_field.field.field_value = self._convert_field_value_if_needed()
         return validated_field
 
     def invalid_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
         return (
             f"{prefix if prefix else ''}"
-            f"Invalid {self.__class__.__name__} '{self.field_name}'"
+            f"Invalid {self.__class__.__name__} '{self.source}'"
             f"{suffix if suffix else ''}"
         )
 
     def missing_field_error_message(self, *, prefix: Optional[str] = None, suffix: Optional[str] = None) -> str:
         return (
             f"{prefix if prefix else ''}"
-            f"Missing {self.__class__.__name__} '{self.field_name}'"
+            f"Missing {self.__class__.__name__} '{self.source}'"
             f"{suffix if suffix else ''}"
         )
 
     def create_error_instance(self, *, validator_message: str) -> Error:
         """Creates and returns a new `valcheck.models.Error` instance for the field"""
         error_copy = self.error.copy()
         error_copy.validator_message = validator_message
-        error_copy.append_to_field_path(self.field_name)
+        error_copy.append_to_field_path(self.source)
         return error_copy
 
 
 class AnyField(Field):
     def __init__(self, **kwargs: Any) -> None:
         super(AnyField, self).__init__(**kwargs)
 
@@ -446,15 +442,15 @@
                 validator_message=self.invalid_field_error_message(suffix=" - Field is not a dictionary"),
             )
             return [error]
         validator = self.validator_model(data=self.field_value)
         error_objs = validator.run_validations()
         for error_obj in error_objs:
             error_obj.validator_message = self.invalid_field_error_message(suffix=f" - {error_obj.validator_message}")
-            error_obj.append_to_field_path(self.field_name)
+            error_obj.append_to_field_path(self.source)
         if not error_objs:
             self.field_value = validator.validated_data
         return error_objs
 
 
 class ModelListField(Field):
     def __init__(self, *, validator_model: Type, allow_empty: Optional[bool] = True, **kwargs: Any) -> None:
@@ -498,13 +494,13 @@
             validator = self.validator_model(data=item)
             error_objs = validator.run_validations()
             validated_field_value.append(validator.validated_data)
             for error_obj in error_objs:
                 error_obj.validator_message = self.invalid_field_error_message(
                     suffix=f" - {error_obj.validator_message} {row_number_string}",
                 )
-                error_obj.append_to_field_path(self.field_name)
+                error_obj.append_to_field_path(self.source)
             errors.extend(error_objs)
         if not errors:
             self.field_value = validated_field_value
         return errors
```

### Comparing `valcheck-0.6.0/valcheck/models.py` & `valcheck-0.7.0/valcheck/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from __future__ import annotations
 
-from copy import deepcopy
+import copy
 from typing import Any, Dict, Optional
 
 
 class Error:
     """Class that represents an error"""
 
     def __init__(
@@ -21,15 +21,15 @@
         self.code = code or ""
         self.details = details or {}
         self._validator_message = ""
         self._field_path = ""
 
     def copy(self) -> Error:
         """Returns deep-copy of current `Error` object"""
-        return deepcopy(self)
+        return copy.deepcopy(self)
 
     @property
     def validator_message(self) -> str:
         return self._validator_message
 
     @validator_message.setter
     def validator_message(self, value: str) -> None:
```

### Comparing `valcheck-0.6.0/valcheck/utils.py` & `valcheck-0.7.0/valcheck/utils.py`

 * *Files identical despite different names*

### Comparing `valcheck-0.6.0/valcheck/validator.py` & `valcheck-0.7.0/valcheck/validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import Any, Dict, List, Optional, Union
 
-from valcheck.exceptions import MissingFieldException, ValidationException
+from valcheck.exceptions import (
+    DuplicateSourcesException,
+    DuplicateTargetsException,
+    MissingFieldException,
+    ValidationException,
+)
 from valcheck.fields import Field
 from valcheck.models import Error
 from valcheck.utils import Empty, is_empty, is_list_of_instances_of_type, set_as_empty
 
 
 class Validator:
     """
@@ -37,37 +42,56 @@
         return self._context
 
     def list_field_validators(self) -> List[Dict[str, Any]]:
         return [
             {
                 "field_type": field.__class__.__name__,
                 "field_identifier": field_identifier,
-                "field_name": field.field_name,
-                "alias": field.alias,
+                "source": field.source,
+                "target": field.target,
                 "required": field.required,
                 "nullable": field.nullable,
             } for field_identifier, field in self._field_info.items()
         ]
 
+    def _validate_uniqueness_of_sources_and_targets(self, field_info: Dict[str, Field], /) -> None:
+        """
+        If duplicate sources/targets are found, raises `valcheck.exceptions.DuplicateSourcesException`
+        or `valcheck.exceptions.DuplicateTargetsException`
+        """
+        sources, targets = [], []
+        for _, field in field_info.items():
+            if field.source:
+                sources.append(field.source)
+            if field.target:
+                targets.append(field.target)
+        if len(sources) != len(set(sources)):
+            raise DuplicateSourcesException(f"Received duplicate values for `source`: {sorted(sources)}")
+        if len(targets) != len(set(targets)):
+            raise DuplicateTargetsException(f"Received duplicate values for `target`: {sorted(targets)}")
+
     def _initialise_fields(self) -> Dict[str, Field]:
         """Returns dictionary having keys = field identifiers, and values = initialised field instances"""
         field_info = {}
         vars_dict = vars(self.__class__)
         for field_identifier in vars_dict:
-            field: Field = vars_dict[field_identifier]
+            temp_field: Field = vars_dict[field_identifier]
             if (
                 not field_identifier.startswith("__")
                 and isinstance(field_identifier, str)
-                and field.__class__ is not Field
-                and issubclass(field.__class__, Field)
+                and temp_field.__class__ is not Field
+                and issubclass(temp_field.__class__, Field)
             ):
+                field = temp_field.copy()
                 field.field_identifier = field_identifier
-                field.field_name = field.alias if field.alias else field_identifier
-                field.field_value = self.data.get(field.field_name, set_as_empty())
+                field.source = field.source if field.source else field_identifier
+                field.target = field.target if field.target else field_identifier
+                field.field_value = self.data.get(field.source, set_as_empty())
                 field_info[field_identifier] = field
+        self._validate_uniqueness_of_sources_and_targets(field_info)
         return field_info
 
     def _clear_errors(self) -> None:
         """Clears out the list of errors"""
         self._errors.clear()
 
     def _register_errors(self, *, errors: List[Error]) -> None:
@@ -97,16 +121,19 @@
 
     def _perform_field_validation_checks(self, *, field: Field) -> None:
         """Performs validation checks for the given field, and registers errors (if any) and validated-data"""
         validated_field = field.run_validations()
         if validated_field.errors:
             self._register_errors(errors=validated_field.errors)
             return
-        if not is_empty(validated_field.field_value):
-            self._register_validated_data(key=validated_field.field_identifier, value=validated_field.field_value)
+        if not is_empty(validated_field.field.field_value):
+            self._register_validated_data(
+                key=validated_field.field.target,
+                value=validated_field.field.field_value,
+            )
 
     def _perform_model_validation_checks(self) -> None:
         """Performs model validation checks, and registers errors (if any)"""
         errors = self.model_validator()
         assert is_list_of_instances_of_type(errors, type_=Error, allow_empty=True), (
             "The output of the model validator method must be a list of errors (each of type `valcheck.models.Error`)."
             " Must be an empty list if there are no errors."
```

### Comparing `valcheck-0.6.0/valcheck.egg-info/PKG-INFO` & `valcheck-0.7.0/valcheck.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: valcheck
-Version: 0.6.0
+Version: 0.7.0
 Summary: Package for quick data validation (in Python)
 Home-page: https://github.com/Nishant173/valcheck
 Author: Nishant Rao
 Author-email: nishant.rao173@gmail.com
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

