# Comparing `tmp/core_validator-0.0.2.tar.gz` & `tmp/core_validator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "core_validator-0.0.2.tar", last modified: Thu Jul 20 14:22:50 2023, max compression
+gzip compressed data, was "core_validator-0.1.0.tar", last modified: Thu Jul 20 18:15:12 2023, max compression
```

## Comparing `core_validator-0.0.2.tar` & `core_validator-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,20 @@
--rw-r--r--   0        0        0     1074 2023-07-20 14:22:42.746569 core_validator-0.0.2/LICENSE
--rw-r--r--   0        0        0     1666 2023-07-20 14:22:42.746569 core_validator-0.0.2/README.md
--rw-r--r--   0        0        0      289 2023-07-20 14:22:42.746569 core_validator-0.0.2/core_validator/__init__.py
--rw-r--r--   0        0        0     1256 2023-07-20 14:22:42.746569 core_validator-0.0.2/core_validator/types.py
--rw-r--r--   0        0        0      274 2023-07-20 14:22:42.746569 core_validator-0.0.2/core_validator/utils.py
--rw-r--r--   0        0        0     3543 2023-07-20 14:22:42.746569 core_validator-0.0.2/core_validator/validator.py
--rw-r--r--   0        0        0        0 2023-07-20 14:22:42.768568 core_validator-0.0.2/examples/__init__.py
--rw-r--r--   0        0        0     2294 2023-07-20 14:22:42.746569 core_validator-0.0.2/examples/multiple_error.py
--rw-r--r--   0        0        0     1843 2023-07-20 14:22:42.746569 core_validator-0.0.2/examples/single_error.py
--rw-r--r--   0        0        0      385 2023-07-20 14:22:42.746569 core_validator-0.0.2/examples/types.py
--rw-r--r--   0        0        0      829 2023-07-20 14:22:50.236464 core_validator-0.0.2/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-20 14:22:42.768568 core_validator-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0      294 2023-07-20 14:22:42.747569 core_validator-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0      239 2023-07-20 14:22:42.747569 core_validator-0.0.2/tests/factories.py
--rw-r--r--   0        0        0      300 2023-07-20 14:22:42.747569 core_validator-0.0.2/tests/test_multiple_error.py
--rw-r--r--   0        0        0      881 2023-07-20 14:22:42.747569 core_validator-0.0.2/tests/test_single_error.py
--rw-r--r--   0        0        0     1943 1970-01-01 00:00:00.000000 core_validator-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-07-20 18:15:04.804776 core_validator-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1735 2023-07-20 18:15:04.804776 core_validator-0.1.0/README.md
+-rw-r--r--   0        0        0      289 2023-07-20 18:15:04.805776 core_validator-0.1.0/core_validator/__init__.py
+-rw-r--r--   0        0        0      679 2023-07-20 18:15:04.805776 core_validator-0.1.0/core_validator/deprecated.py
+-rw-r--r--   0        0        0     1354 2023-07-20 18:15:04.805776 core_validator-0.1.0/core_validator/types.py
+-rw-r--r--   0        0        0      274 2023-07-20 18:15:04.805776 core_validator-0.1.0/core_validator/utils.py
+-rw-r--r--   0        0        0     4072 2023-07-20 18:15:04.805776 core_validator-0.1.0/core_validator/validator.py
+-rw-r--r--   0        0        0        0 2023-07-20 18:15:04.829775 core_validator-0.1.0/examples/__init__.py
+-rw-r--r--   0        0        0     2295 2023-07-20 18:15:04.805776 core_validator-0.1.0/examples/deprecated/multiple_error.py
+-rw-r--r--   0        0        0     1876 2023-07-20 18:15:04.805776 core_validator-0.1.0/examples/deprecated/single_error.py
+-rw-r--r--   0        0        0     2294 2023-07-20 18:15:04.805776 core_validator-0.1.0/examples/multiple_error.py
+-rw-r--r--   0        0        0     1861 2023-07-20 18:15:04.805776 core_validator-0.1.0/examples/single_error.py
+-rw-r--r--   0        0        0      385 2023-07-20 18:15:04.805776 core_validator-0.1.0/examples/types.py
+-rw-r--r--   0        0        0      829 2023-07-20 18:15:12.584705 core_validator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-07-20 18:15:04.830775 core_validator-0.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      294 2023-07-20 18:15:04.806776 core_validator-0.1.0/tests/conftest.py
+-rw-r--r--   0        0        0      239 2023-07-20 18:15:04.806776 core_validator-0.1.0/tests/factories.py
+-rw-r--r--   0        0        0      300 2023-07-20 18:15:04.806776 core_validator-0.1.0/tests/test_multiple_error.py
+-rw-r--r--   0        0        0      881 2023-07-20 18:15:04.806776 core_validator-0.1.0/tests/test_single_error.py
+-rw-r--r--   0        0        0     2012 1970-01-01 00:00:00.000000 core_validator-0.1.0/PKG-INFO
```

### Comparing `core_validator-0.0.2/LICENSE` & `core_validator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `core_validator-0.0.2/README.md` & `core_validator-0.1.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -19,52 +19,50 @@
 class Source(BaseModel):
     local: str
 ```
 
 ### DTO Validator
 ```python
 @dataclasses.dataclass()
-class CommentValidator(Validator[ErrorSchema[Source]]):
-    dto: CommentDto
-
+class CommentValidator(Validator[CommentDto, ErrorSchema[Source]]):
     @validate
     async def test1(self):
         post_ids = list(range(1, 10))
-
-        if self.dto.post_id not in post_ids:
+        if self.data.post_id not in post_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
                     message="Id doen't not exists",
-                    detail=f"Post with id={self.dto.post_id} not found",
+                    detail=f"Post with id={self.data.post_id} not found",
                     source=Source(
                         local="data/post_id",
                     ),
                 )
             )
 
     @validate
+    @pre_state(lambda self: self.data.owner_id > 0, negative_id_error)
     async def test2(self):
         owner_ids = list(range(1, 10))
 
-        if self.dto.owner_id not in owner_ids:
+        if self.data.owner_id not in owner_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
                     message="Id doen't not exists",
-                    detail=f"User with id={self.dto.post_id} not found",
+                    detail=f"User with id={self.data.post_id} not found",
                     source=Source(
                         local="data/owner_id",
                     ),
                 )
             )
 ```
 
 ### Use
 ```python
 async def function():
-    validator = CommentValidator(...)
-    errors = await validator.errors()
+    validator = CommentValidator()
+    errors = await validator.errors(comment)
     # or
     await validator.validate() # raise ValidationError
 
 ```
```

### Comparing `core_validator-0.0.2/core_validator/types.py` & `core_validator-0.1.0/core_validator/types.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import dataclasses
 from enum import Enum
 from collections.abc import Callable, Coroutine, Sequence
 from typing import Any, Generic, TypeAlias, TypeVar
 
 
-_T = TypeVar("_T")
+TError = TypeVar("TError")
 _S = TypeVar("_S")
 
+TValidationData = TypeVar("TValidationData")
+
 SelfValidator: TypeAlias = Any  # heh
 
 ValidatorFunc: TypeAlias = Callable[[Any], Coroutine[Any, Any, None] | None]
 
 
 class ErrorCodeEnum(str, Enum):
     unique_constraint = "UNIQUE CONSTRAINT"
@@ -22,29 +24,29 @@
 class ErrorSchema(Generic[_S]):
     code: str
     message: str
     detail: str | None = None
     source: _S | None = None
 
 
-class ValidationError(Generic[_T], Exception):
-    messages: list[_T]
+class ValidationError(Generic[TError], Exception):
+    messages: list[TError]
 
-    def __init__(self, messages: list[_T], *args: object) -> None:
+    def __init__(self, messages: list[TError], *args: object) -> None:
         super().__init__(*args)
         self.messages = messages
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
-class ValidationContext(Generic[_T]):
-    _errors: list[_T] = dataclasses.field(default_factory=list)
+class ValidationContext(Generic[TError]):
+    _errors: list[TError] = dataclasses.field(default_factory=list, init=False)
 
-    def add_error(self, error: _T) -> None:
+    def add_error(self, error: TError) -> None:
         if error not in self._errors:
             self._errors.append(error)
 
-    def extend_error(self, errors: Sequence[_T]) -> None:
+    def extend_error(self, errors: Sequence[TError]) -> None:
         self._errors.extend(errors)
 
     @property
-    def errors(self) -> list[_T]:
+    def errors(self) -> list[TError]:
         return self._errors
```

### Comparing `core_validator-0.0.2/core_validator/validator.py` & `core_validator-0.1.0/core_validator/validator.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,98 +3,84 @@
 import functools
 from collections.abc import Callable, Sequence
 from typing import Any, Coroutine, Generic, Literal
 from core_validator.types import (
     ValidationContext,
     ValidationError,
     ValidatorFunc,
-    _T,
+    TError,
     SelfValidator,
+    TValidationData,
 )
 from core_validator.utils import await_maybe
 
 
 def callable_true(x: SelfValidator) -> bool:
     return True
 
 
 @dataclasses.dataclass(frozen=True, slots=True)
-class ValidatingFunction(Generic[_T]):
+class ValidatingFunction(Generic[TError]):
     validator_function: ValidatorFunc
 
     __is_validator__: Literal[True] = True
     __pre_condition__: Callable[
         [SelfValidator],
         Coroutine[Any, Any, bool] | bool,
     ] = callable_true
-    __pre_state_error__: _T | None = None
+    __pre_state_error__: TError | None = None
 
-    async def __call__(self, validator: Validator[_T]) -> None:
+    async def __call__(self, validator: ValidatorBase[TError]) -> None:
         await await_maybe(self.validator_function(validator))
 
 
 def validate(
-    f: ValidatorFunc | ValidatingFunction[_T],
-) -> ValidatingFunction[_T]:
+    f: ValidatorFunc | ValidatingFunction[TError],
+) -> ValidatingFunction[TError]:
     if isinstance(f, ValidatingFunction):
         return ValidatingFunction(
             f.validator_function,
             __pre_condition__=f.__pre_condition__,
             __pre_state_error__=f.__pre_state_error__,
         )
     return ValidatingFunction(f)
 
 
 def pre_state(
     function: Callable[
         [SelfValidator],
         Coroutine[Any, Any, bool] | bool,
     ],
-    error: _T | None = None,
+    error: TError | None = None,
 ) -> Callable[[ValidatorFunc], ValidatorFunc]:
-    def decorator(f: ValidatorFunc | ValidatingFunction[_T]) -> ValidatingFunction[_T]:
+    def decorator(
+        f: ValidatorFunc | ValidatingFunction[TError],
+    ) -> ValidatingFunction[TError]:
         if isinstance(f, ValidatingFunction):
             raise NotImplementedError
         return ValidatingFunction(
             validator_function=f,
             __pre_condition__=function,
             __pre_state_error__=error,
         )
 
     return decorator
 
 
-class Validator(Generic[_T]):
+class ValidatorBase(Generic[TError]):
     async def setup(self) -> None:
         ...
 
     async def dispose(self) -> None:
         ...
 
-    async def validate(self) -> None:
-        await self.setup()
-        try:
-            await self._run_validate_process()
-        finally:
-            await self.dispose()
-
-        if self.context.errors:
-            raise ValidationError(self.context.errors)
-
     @functools.cached_property
-    def context(self) -> ValidationContext[_T]:
+    def context(self) -> ValidationContext[TError]:
         return ValidationContext()
 
-    async def errors(self) -> Sequence[_T]:
-        try:
-            await self.validate()
-        except ValidationError as e:
-            return e.messages
-        return []
-
     async def _run_validate_process(self):
         queue = list(self._get_validation_methods())
         failed_pre_state_validators = []
         while queue:
             for validator in queue:
                 if await await_maybe(validator.__pre_condition__(self)):
                     await await_maybe(validator(self))
@@ -110,16 +96,44 @@
         for validator in failed_pre_state_validators:
             if validator.__pre_state_error__ is not None:
                 self.context.add_error(validator.__pre_state_error__)
 
     @classmethod
     def _get_validation_methods(
         cls,
-    ) -> Sequence[ValidatingFunction[_T]]:
+    ) -> Sequence[ValidatingFunction[TError]]:
         return [
             function
             for value in dir(cls)
             if isinstance(
                 function := getattr(cls, value),
                 ValidatingFunction,
             )
         ]
+
+
+class Validator(ValidatorBase[TError], Generic[TValidationData, TError]):
+    __validation_data__: TValidationData | None = None
+
+    @property
+    def data(self) -> TValidationData:
+        if self.__validation_data__ is None:
+            raise ValueError
+        return self.__validation_data__
+
+    async def validate(self, validation_data: TValidationData) -> None:
+        self.__validation_data__ = validation_data
+        await self.setup()
+        try:
+            await self._run_validate_process()
+        finally:
+            await self.dispose()
+
+        if self.context.errors:
+            raise ValidationError(self.context.errors)
+
+    async def errors(self, validation_data: TValidationData) -> Sequence[TError]:
+        try:
+            await self.validate(validation_data)
+        except ValidationError as e:
+            return e.messages
+        return []
```

### Comparing `core_validator-0.0.2/examples/multiple_error.py` & `core_validator-0.1.0/examples/multiple_error.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,32 +1,30 @@
 import asyncio
 import dataclasses
 import functools
 from core_validator import (
-    Validator,
     ValidationError,
     ErrorSchema,
     ErrorCodeEnum,
     validate,
 )
+from core_validator import Validator
 from examples.types import CommentDto, CustomValidationContext, SourceMultiple
 
 
 @dataclasses.dataclass()
-class CommentValidator(Validator[ErrorSchema[SourceMultiple]]):
-    dto_list: list[CommentDto]
-
+class CommentValidator(Validator[list[CommentDto], ErrorSchema[SourceMultiple]]):
     @functools.cached_property
     def context(self) -> CustomValidationContext:  # type: ignore[override]
         return CustomValidationContext()
 
     @validate
     async def test1(self):
         post_ids = range(1, 10)
-        for i, dto in enumerate(self.dto_list):
+        for i, dto in enumerate(self.data):
             if dto.post_id not in post_ids:
                 self.context.add_error(
                     ErrorSchema(
                         code=ErrorCodeEnum.not_found.value,
                         message="Id doen't not exists",
                         detail=f"Post with id={dto.post_id} not found",
                         source=SourceMultiple(
@@ -35,15 +33,15 @@
                         ),
                     )
                 )
 
     @validate
     async def test2(self):
         owner_ids = range(1, 10)
-        for i, dto in enumerate(self.dto_list):
+        for i, dto in enumerate(self.data):
             if dto.owner_id not in owner_ids:
                 self.context.add_error(
                     ErrorSchema(
                         code=ErrorCodeEnum.not_found.value,
                         message="Id doen't not exists",
                         detail=f"User with id={dto.post_id} not found",
                         source=SourceMultiple(
@@ -58,15 +56,15 @@
     dto_list = [
         CommentDto(comment="comment", owner_id=1, post_id=1),
         CommentDto(comment="comment", owner_id=1, post_id=100),
         CommentDto(comment="comment", owner_id=100, post_id=1),
         CommentDto(comment="comment", owner_id=1234, post_id=1234),
     ]
     try:
-        await CommentValidator(dto_list).validate()
+        await CommentValidator().validate(dto_list)
     except ValidationError as e:
         for message in e.messages:
             print(message)
 
 
 if __name__ == "__main__":
     asyncio.run(main())
```

### Comparing `core_validator-0.0.2/examples/single_error.py` & `core_validator-0.1.0/examples/deprecated/single_error.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import asyncio
 import dataclasses
 from core_validator import (
-    Validator,
     ValidationError,
     ErrorSchema,
     ErrorCodeEnum,
     validate,
     pre_state,
 )
+from core_validator.deprecated import Validator
 from examples.types import CommentDto, Source
 
 
 negative_id_error = ErrorSchema(
     code=ErrorCodeEnum.not_found.value,
     message="Id < 0",
     detail="Id must > 0",
```

### Comparing `core_validator-0.0.2/pyproject.toml` & `core_validator-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "core-validator"
-version = "0.0.2"
+version = "0.1.0"
 authors = [
     { name = "maksyutov vlad", email = "maksyutov.vlad@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.11"
 readme = "README.md"
```

### Comparing `core_validator-0.0.2/tests/test_single_error.py` & `core_validator-0.1.0/tests/test_single_error.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,19 +4,19 @@
 
 
 pytestmark = [pytest.mark.anyio]
 
 
 async def test_random_data(random_body: list[CommentDto]) -> None:
     for comment in random_body:
-        validator = CommentValidator(comment)
+        validator = CommentValidator()
         post_in_db = 1 <= comment.post_id < 10
         owner_in_db = 1 <= comment.owner_id < 10
 
-        errors = await validator.errors()
+        errors = await validator.errors(comment)
         if not post_in_db:
             assert any(
                 [
                     error.source is not None and error.source.local == "data/post_id"
                     for error in errors
                 ]
             )
```

### Comparing `core_validator-0.0.2/PKG-INFO` & `core_validator-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: core-validator
-Version: 0.0.2
+Version: 0.1.0
 Author-Email: maksyutov vlad <maksyutov.vlad@gmail.com>
 License: MIT
 Project-URL: Homepage, https://gitlab.com/pachek-opensource/validator/core-validator
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # Core-Validator
@@ -28,52 +28,50 @@
 class Source(BaseModel):
     local: str
 ```
 
 ### DTO Validator
 ```python
 @dataclasses.dataclass()
-class CommentValidator(Validator[ErrorSchema[Source]]):
-    dto: CommentDto
-
+class CommentValidator(Validator[CommentDto, ErrorSchema[Source]]):
     @validate
     async def test1(self):
         post_ids = list(range(1, 10))
-
-        if self.dto.post_id not in post_ids:
+        if self.data.post_id not in post_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
                     message="Id doen't not exists",
-                    detail=f"Post with id={self.dto.post_id} not found",
+                    detail=f"Post with id={self.data.post_id} not found",
                     source=Source(
                         local="data/post_id",
                     ),
                 )
             )
 
     @validate
+    @pre_state(lambda self: self.data.owner_id > 0, negative_id_error)
     async def test2(self):
         owner_ids = list(range(1, 10))
 
-        if self.dto.owner_id not in owner_ids:
+        if self.data.owner_id not in owner_ids:
             self.context.add_error(
                 ErrorSchema(
                     code=ErrorCodeEnum.not_found.value,
                     message="Id doen't not exists",
-                    detail=f"User with id={self.dto.post_id} not found",
+                    detail=f"User with id={self.data.post_id} not found",
                     source=Source(
                         local="data/owner_id",
                     ),
                 )
             )
 ```
 
 ### Use
 ```python
 async def function():
-    validator = CommentValidator(...)
-    errors = await validator.errors()
+    validator = CommentValidator()
+    errors = await validator.errors(comment)
     # or
     await validator.validate() # raise ValidationError
 
 ```
```

