# Comparing `tmp/impunity-0.2.1.tar.gz` & `tmp/impunity-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "impunity-0.2.1.tar", max compression
+gzip compressed data, was "impunity-1.0.tar", max compression
```

## Comparing `impunity-0.2.1.tar` & `impunity-1.0.tar`

### file list

```diff
@@ -1,8 +1,9 @@
--rw-r--r--   0        0        0      911 2023-02-23 08:42:31.215564 impunity-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       54 2022-12-15 08:10:37.693666 impunity-0.2.1/src/impunity/__init__.py
--rw-r--r--   0        0        0      488 2022-12-19 10:37:17.250874 impunity-0.2.1/src/impunity/exception.py
--rw-r--r--   0        0        0      587 2023-02-21 14:08:28.599926 impunity-0.2.1/src/impunity/quantityNode.py
--rw-r--r--   0        0        0    31323 2023-02-22 15:16:03.388724 impunity-0.2.1/src/impunity/visitor.py
--rw-r--r--   0        0        0     5446 2023-02-23 08:44:32.046331 impunity-0.2.1/src/impunity/wrapper.py
--rw-r--r--   0        0        0      851 1970-01-01 00:00:00.000000 impunity-0.2.1/setup.py
--rw-r--r--   0        0        0      598 1970-01-01 00:00:00.000000 impunity-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1086 2023-03-17 15:25:08.762240 impunity-1.0/license.txt
+-rw-r--r--   0        0        0     1361 2023-07-20 08:46:19.598546 impunity-1.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2022-12-15 08:10:37.693666 impunity-1.0/src/impunity/__init__.py
+-rw-r--r--   0        0        0      520 2023-04-26 09:32:15.372322 impunity-1.0/src/impunity/exception.py
+-rw-r--r--   0        0        0        0 2023-03-17 15:25:08.762240 impunity-1.0/src/impunity/py.typed
+-rw-r--r--   0        0        0      859 2023-06-20 08:36:00.376797 impunity-1.0/src/impunity/quantityNode.py
+-rw-r--r--   0        0        0    38089 2023-07-12 12:44:39.459946 impunity-1.0/src/impunity/visitor.py
+-rw-r--r--   0        0        0     9530 2023-07-12 08:34:02.847488 impunity-1.0/src/impunity/wrapper.py
+-rw-r--r--   0        0        0      660 1970-01-01 00:00:00.000000 impunity-1.0/PKG-INFO
```

### Comparing `impunity-0.2.1/pyproject.toml` & `impunity-1.0/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,73 @@
 [tool.poetry]
 name = "impunity"
-version = "0.2.1"
+version = "1.0"
 description = "Static checking for consistency of physical units"
-authors = ["Antoine Chevrot <antoine.chevrot@gmail.com>"]
+authors = [
+  "Antoine Chevrot <antoine.chevrot@gmail.com>",
+  "Xavier Olive <git@xoolive.org>"
+]
+license = "MIT"
+include = [
+  "license.txt"
+]
+
 
 [tool.poetry.dependencies]
 python = "^3.8"
 Pint = ">=0.19.2"
 astor = "^0.8.1"
 typing-extensions = { version=">=4.2.0,<5.0.0", python="<3.10" }
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
+poetry = "^1.5.1"
 black = ">=21.6"
 mypy = ">=0.981"
-isort = "^5.11.2"
-flake8 = ">=5.0"
+ruff = "^0.0.253"
 numpy = "^1.23.5"
 coverage = "^7.0.0"
 codecov = "^2.1.12"
+pre-commit = "^3.3.2"
+Sphinx = ">=5.1"
+sphinx-design = "^0.4.1"
+sphinx-rtd-theme = ">=0.5.2"
+jupyter_sphinx = ">=0.3.2"
+sphinx-autodoc-typehints = ">=1.17,!=1.21.4"
+ipykernel = "^6.23.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
-line-length = 120
+line-length = 79
 target_version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 exclude = '''
 /(
     __pycache__
   | \.git
   | \.mypy_cache
   | \.ipynb_checkpoints
   | build
   | dist
 )/
 '''
 
-[tool.isort]
-line_length = 120
-profile = "black"
-known_first_party = ["numpy", "pandas"]
+[tool.ruff]
+select = [
+  "E", "W",  # pycodestyle
+  "F",  # pyflakes
+  "I",  # isort
+  "NPY",  # numpy
+  # "PD",  # pandas
+  "DTZ", # flake8-datetimez
+  "RUF"
+]
+line-length = 79
+target-version = "py38"
+
+[tool.ruff.isort]
+known-first-party = ["numpy", "pandas"]
 
 [tool.coverage.run]
 source = ["src"]
```

### Comparing `impunity-0.2.1/src/impunity/visitor.py` & `impunity-1.0/src/impunity/visitor.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,261 +1,393 @@
 from __future__ import annotations
 
 import ast
-import collections
 import inspect
 import logging
 import sys
 import types
-from numbers import Number
+import typing
+from math import isclose
 from typing import Any, Dict, Optional, Union, cast
 
 if sys.version_info >= (3, 9):
-    from _collections_abc import Sequence
+    from _collections_abc import Callable, Sequence
 else:
+    from collections import Callable
     from typing import Sequence
 
 import pint
 from pint import UnitRegistry
 
 if sys.version_info >= (3, 10):
     # TBH Annotated from 3.9, TypeGuard from 3.10
     from typing import Annotated, TypeGuard
 else:
     from typing_extensions import Annotated, TypeGuard
 
-from .exception import raise_dim_error
 from .quantityNode import QuantityNode, Unit
 
 annotation_node = Union[ast.Subscript, ast.Name, ast.Constant]
 
 
 # class annot_type(Annotated[int, "spam"]):
 #     """Class to access __metadata__ from Annotated variables"""
 
 #     def __init__(self, *args, **kw):
 #         super(annot_type, self).__init__(*args, **kw)
 #         self.__metadata__ = getattr(super(), "__metadata__")
 
 annot_type = type(Annotated[int, "spam"])
 
-_log = logging.getLogger(__name__)
 
 logging.basicConfig(
     level=logging.WARNING,
     format="%(asctime)s [%(levelname)s] %(message)s",
     handlers=[
-        logging.FileHandler("debug.log"),
+        # Creates a file "todays_date.py" with warnings
         logging.StreamHandler(sys.stdout),
     ],
 )
 
+_log = logging.getLogger(__name__)
+
 
 class VarDict(dict):
     def __missing__(self, key):
-        if isinstance(key, Number):
-            _log.warning(f"The value {key} is not annotated. Defaulted to dimensionless")
-        else:
-            _log.warning(f"The variable {key} is not annotated. Defaulted to dimensionless")
-        return "dimensionless"
+        _log.warning(
+            f"The variable {key} is not annotated. "
+            + "Defaulted to dimensionless"
+        )
+        return None
 
 
-def get_annotation_unit(annotation: annotation_node | ast.expr) -> str:
+def get_annotation_unit(
+    node: annotation_node | ast.expr,
+) -> Optional[str]:
+    """
+    Return a UoM from an AST Node. Return None if the node is not compatible.
+
+    :param node: Node with an annotation
+    :type node: ast.expr with annotation
+    :return: Optional str of the UoM
+    :rtype: Optional[str]
+    """
+
     unit = None
-    if isinstance(annotation, ast.Constant):
-        unit = annotation.value
-    elif isinstance(annotation, ast.Subscript):
-        if isinstance(annotation.slice, ast.Index):
-            if isinstance(annotation.slice.value, ast.Tuple):
-                unit_node = annotation.slice.value.elts[1]
-        elif isinstance(annotation.slice, ast.Tuple):
-            unit_node = annotation.slice.elts[1]
+    if isinstance(node, ast.Constant):
+        unit = node.value
+    elif isinstance(node, ast.Subscript):
+        if isinstance(node.slice, ast.Index):
+            if isinstance(node.slice.value, ast.Tuple):  # type: ignore
+                unit_node = node.slice.value.elts[1]  # type: ignore
+        elif isinstance(node.slice, ast.Tuple):
+            unit_node = node.slice.elts[1]
         if isinstance(unit_node, ast.Constant):
             unit = unit_node.value
 
-    if unit is not None:
-        return unit
-    else:
-        raise TypeError(f"{annotation} is not an annotation type expected by impunity")
+    return unit
 
 
-def is_annotated(hint: Any, annot_type=annot_type) -> TypeGuard[annot_type]:  # type: ignore
+def is_annotated(
+    hint: Any, annot_type=annot_type
+) -> TypeGuard[annot_type]:  # type: ignore
+    """Determines whether the annotation is of type Annotated"""
     return (type(hint) is annot_type) and hasattr(hint, "__metadata__")
 
 
 class Visitor(ast.NodeTransformer):
-    couscous_func: dict[str, collections.Callable] = {}
+
+    """Impunity AST visitor class checking for Annotations
+    to transform the code if necessary
+
+    Attributes:
+        impunity_func : dict[str, Callable]
+            Dictionnary of Callables to keep track of functions
+            tracked by impunity
+        ureg : pint.UnitRegistry
+            Unit Registry from Pint to manage UoMs.
+    """
+
+    impunity_func: dict[str, Callable] = {}
     ureg = UnitRegistry()
 
-    def visit(self, root: ast.AST) -> Any:
+    def __init__(self, fun) -> None:
+        """
+        Constructs all the necessary attributes for the visitor using the
+        attributes of the fun Callable.
+
+        Parameters
+        ----------
+            fun : Callable[..., Any]
+                Callable checked by impunity
+        """
+
+        self.nested_flag = False
+        x: Dict[str, str] = {}
+        self.vars = VarDict(x)
+
+        # For class decorators
+        if isinstance(fun, type):
+            method_list = [
+                getattr(fun, func)
+                for func in dir(fun)
+                if callable(getattr(fun, func)) and not func.startswith("__")
+            ]
+            self.add_func(fun.__init__)  # type: ignore
+            for function in method_list:
+                self.add_func(function)
+            self.class_attr: Dict[str, Unit] = {}
+        else:
+            self.add_func(fun)
+
+    def visit(self, root: ast.AST) -> ast.AST:
+        """
+        Initiate the visit of the root AST. Returns a checked ast.AST
+        eventually modified to keep UoM coherence.
+
+        Args:
+            root : ast.AST
+                root of the AST to visit
+        """
+
         # Adding the "parent" attribute to every nodes of the AST
         for node in ast.walk(root):
             for child in ast.iter_child_nodes(node):
                 child.parent = node  # type: ignore
-        return super().visit(root)
+        method = "visit_" + root.__class__.__name__
+        visitor = getattr(self, method, self.generic_visit)
+        new_node = visitor(root)
+        return new_node
 
     @classmethod
     def add_func(cls, fun):
+        """Add function to the impunity function dictionnary"""
         if isinstance(fun, ast.FunctionDef):
-            cls.couscous_func[fun.name] = fun
+            cls.impunity_func[fun.name] = fun
         else:
-            cls.couscous_func[fun.__name__] = fun
+            cls.impunity_func[fun.__name__] = fun
 
-    @classmethod
-    def insert_node_above(cls, original_node, new_node) -> None:
-        parent_function: ast.AST = original_node.parent
-        line_node: ast.AST = original_node
-        while not isinstance(parent_function, ast.FunctionDef):
-            line_node = parent_function
-            # TODO Inherit AST NODE to get parents. Ignored as for now
-            parent_function = parent_function.parent  # type: ignore
-
-        new_body = parent_function.body.copy()
-        for i, node in enumerate(parent_function.body):
-            if line_node == node:
-                new_body.insert(i, new_node)
-        parent_function.body = new_body
+    def node_convert(self, expected_unit, received_unit, received_node):
+        """check if the expected and the received units are coherents with
+        each other by using the Pint library. Modify the received node
+        accordingly and returns it.
+
+        Parameters:
+            - expected_unit : str
+                expected Unit of Measure string
+            - received_unit : str
+                received Unit of Measure string
+            - received_node : QuantityNode
+                received Quantity Node
+
+        Returns:
+            - QuantityNode: Input Quantity Node, eventually modified for unit
+            coherence.
+
+        """
+        if (
+            received_unit != expected_unit
+            and "dimensionless"
+            not in (
+                received_unit,
+                expected_unit,
+            )
+            and received_unit is not None
+        ):
+            if pint.Unit(received_unit).is_compatible_with(
+                pint.Unit(expected_unit)
+            ):
+                Q_ = self.ureg.Quantity
+                r0 = Q_(0, received_unit)
+                r1 = Q_(1, received_unit)
+                r10 = Q_(10, received_unit)
+
+                e0 = r0.to(expected_unit)
+                e1 = r1.to(expected_unit)
+                e10 = r10.to(expected_unit)
+
+                if r0.m == e0.m:
+                    conv_value = (
+                        pint.Unit(expected_unit)
+                        .from_(pint.Unit(received_unit))
+                        .m
+                    )
+
+                    if conv_value == 1:
+                        new_node = received_node
+                    else:
+                        new_node = ast.BinOp(
+                            received_node,
+                            ast.Mult(),
+                            ast.Constant(conv_value),
+                        )
+
+                elif (e1.m - e0.m) == 1:
+                    conv_value = (
+                        pint.Unit(expected_unit)
+                        .from_(pint.Unit(received_unit))
+                        .m
+                    ) - 1
+
+                    # if conv_value == 0:
+                    #     new_node = received_node
+                    # else:
+                    new_node = ast.BinOp(
+                        received_node,
+                        ast.Add(),
+                        ast.Constant(conv_value),
+                    )
+
+                elif isclose(10 * (e1.m - e0.m) + e0.m, e10.m):
+                    new_node = ast.BinOp(
+                        ast.BinOp(
+                            received_node,
+                            ast.Mult(),
+                            ast.Constant((e1.m - e0.m)),
+                        ),
+                        ast.Add(),
+                        ast.Constant(e0.m),
+                    )
+                else:
+                    new_node = received_node  # log
+
+            else:
+                _log.warning(
+                    f"In function {self.fun.__module__}/"
+                    + f"{self.fun.__name__}: "
+                    + f"Expected unit {expected_unit} "
+                    + f"but received incompatible unit {received_unit}."
+                )
+                new_node = received_node
+        else:
+            new_node = received_node
+        return new_node
 
     @classmethod
     def func_flush(cls):
         return
 
     @classmethod
     def get_annotations(cls, name) -> Optional[Dict[str, Any]]:
-        # if sys.version_info >= (3, 10):
-        #     from inspect import get_annotations as get_ann
+        """Get annotations of a function found in the impunity_func class dict.
+        Returns None if the function is not annotated.
 
-        #     if callable(name):
-        #         return get_ann(name, eval_str=True)
-        #     else:
-        #         return cls.couscous_func.get(name)
-        if isinstance(fun := cls.couscous_func.get(name), ast.FunctionDef):
-            params = {}
-            for arg in fun.args.args:
-                ann = arg.annotation
-                annotation = inspect.Parameter.empty
-                if isinstance(ann, ast.Constant):
-                    annotation = ann.value
-                elif isinstance(ann, ast.Name):
-                    annotation = ann.id
-                elif isinstance(ann, ast.Subscript):
-                    data_type = eval(ann.slice.elts[0].id)
-                    annotation = ann.slice.elts[1].value
-                    annotation = Annotated[data_type, annotation]
-                params.append(
-                    inspect.Parameter(
-                        arg.arg,
-                        inspect.Parameter.POSITIONAL_OR_KEYWORD,
-                        annotation=annotation,
-                    )
-                )
-            return inspect.Signature(
-                params,
-                return_annotation=fun.returns.value if not getattr(fun, "returns", False) else inspect._empty,
-            )
-        elif fun is not None:
+        Parameters:
+            - name : str
+                name of the function for which annotations are required
+
+        Returns:
+            - Optional dict of annotations
+        """
 
+        if (fun := cls.impunity_func.get(name)) is not None:
             annotations = getattr(fun, "__annotations__", None)
             if annotations:
-                globals = list(cls.couscous_func.values())[-1].__globals__
+                globals = list(cls.impunity_func.values())[-1].__globals__
                 locals = fun.__globals__
                 annotations = {
-                    k: v if not isinstance(v, str) else eval(v, globals, locals) for k, v in annotations.items()
+                    k: v
+                    if not isinstance(v, str)
+                    else eval(v, globals, locals)
+                    for k, v in annotations.items()
                 }
                 return cast(Dict, annotations)
         elif callable(name):
             annotations = getattr(name, "__annotations__", None)
             if annotations:
-                globals = list(cls.couscous_func.values())[-1].__globals__
-                locals = name.__globals__
+                globals = list(cls.impunity_func.values())[-1].__globals__
+                locals = fun.__globals__  # type: ignore
                 annotations = {
-                    k: v if not isinstance(v, str) else eval(v, globals, locals) for k, v in annotations.items()
+                    k: v
+                    if not isinstance(v, str)
+                    else eval(v, globals, locals)
+                    for k, v in annotations.items()
                 }
-            return cast(Dict, annotations)
+                return cast(Dict, annotations)
 
         return None
 
     @classmethod
     def get_func(cls, name):
-        return cls.couscous_func.get(name)
-
-    def __init__(self, fun) -> None:
+        """getter function for the class dict"""
+        return cls.impunity_func.get(name)
 
-        self.nested_flag = False
+    def visit_FunctionDef(self, node: ast.FunctionDef) -> ast.FunctionDef:
+        """Method called by the visitor if the visited node is
+        function defintion. Is usually the root node in impunity
 
-        # For class decorators
-        if isinstance(fun, type):
-            method_list = [
-                getattr(fun, func) for func in dir(fun) if callable(getattr(fun, func)) and not func.startswith("__")
-            ]
-            self.add_func(fun.__init__)  # type: ignore
-            for function in method_list:
-                self.add_func(function)
-            self.class_attr: Dict[str, Unit] = {}
-        else:
-            self.add_func(fun)
-
-    def visit_FunctionDef(self, node: ast.FunctionDef) -> Any:
+        Args:
+            node (ast.FunctionDef): Visited Function Definition
 
+        """
         if not self.nested_flag:
             self.func_flush()
-        # check for couscous decorator:
+        # check for impunity decorator:
         if node.decorator_list:
             for decorator in node.decorator_list:
-                if isinstance(decorator, ast.Call) and isinstance(decorator.func, ast.Name):
-                    if decorator.func.id == "couscous":
+                if isinstance(decorator, ast.Call) and isinstance(
+                    decorator.func, ast.Name
+                ):
+                    if decorator.func.id == "impunity":
                         for kw in decorator.keywords:
                             if hasattr(kw, "value"):
-                                if kw.arg == "ignore" and kw.value.value:  # type: ignore
-                                    self.couscous_func.pop(node.name, False)
+                                if (
+                                    kw.arg == "ignore"
+                                    and kw.value.value  # type: ignore
+                                ):
+                                    self.impunity_func.pop(node.name, False)
                                     return node
 
         if (fun := self.get_func(node.name)) is not None:
             self.nested_flag = True
             self.fun = fun
             self.fun_globals = fun.__globals__
-            x: Dict[str, str] = {}
-            self.vars = VarDict(x)
             if getattr(self, "class_attr", False):
                 self.vars.update(self.class_attr)
         elif self.nested_flag:
             self.add_func(node)
         else:
             return node
 
         # Adding all annotations from own module
-        annotations = getattr(sys.modules[self.fun.__module__], "__annotations__", None)
+        annotations = getattr(
+            sys.modules[self.fun.__module__], "__annotations__", None
+        )
         if annotations is not None:
             for name, anno in annotations.items():
                 if is_annotated(anno):
                     self.vars[name] = anno.__metadata__[0]  # type: ignore
                 if isinstance(anno, str):
                     self.vars[name] = anno
 
         # Adding all annotations from imported modules
         for _, val in self.fun_globals.items():
             if isinstance(val, types.ModuleType):
                 annotations = getattr(val, "__annotations__", None)
                 if annotations is not None:
                     for name, anno in annotations.items():
                         if is_annotated(anno):
-                            self.vars[name] = anno.__metadata__[0]  # type: ignore
+                            x = anno.__metadata__[0]  # type: ignore
+                            self.vars[name] = x
                         if isinstance(anno, str):
                             self.vars[name] = anno
 
         # from function signature
         for arg in node.args.args:
             if arg.annotation is not None:
                 anno_unit = get_annotation_unit(arg.annotation)
-                if anno_unit in self.ureg:
+                if anno_unit is not None and anno_unit in self.ureg:
                     self.vars[arg.arg] = anno_unit
                 else:
+                    self.vars[arg.arg] = None
                     _log.warning(
-                        f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                        "Signature of couscoussed functions must be of type string or typing.Annotated"
+                        f"In function {self.fun.__module__}/"
+                        + f"{self.fun.__name__}: "
+                        + "Signature of annotated functions must be "
+                        + "of type string or typing.Annotated"
                     )
 
         # Check units in the return node
         node = self.generic_visit(node)  # type: ignore
         return node
 
     def get_node_unit(self, node: Optional[ast.expr]) -> QuantityNode:
@@ -268,299 +400,429 @@
         Returns:
             QuantityNode: QuantityNode(node, induced_unit)
         """
 
         new_node: Union[ast.BinOp, ast.IfExp, ast.Call]
 
         if isinstance(node, ast.Constant):
-            return QuantityNode(node, self.vars[node.value])
+            return QuantityNode(node, None)  # self.vars[node.value])
+        if isinstance(node, ast.Attribute):
+            return QuantityNode(node, self.vars[node.attr])
         if isinstance(node, ast.Subscript):
             return QuantityNode(node, self.get_node_unit(node.value).unit)
         elif isinstance(node, ast.Tuple):
             elems = list(map(self.get_node_unit, node.elts))
-            return QuantityNode(
-                ast.Tuple([elem.node for elem in elems], ctx=node.ctx),
-                cast(Sequence[Unit], [elem.unit for elem in elems]),
-            )
-        elif isinstance(node, ast.List):
-            if not node.elts:
-                return QuantityNode(node, None)
+            if len(elems) == 1:
+                return QuantityNode(elems[0].node, elems[0].unit)
             else:
-                elems = list(map(self.get_node_unit, node.elts))
                 return QuantityNode(
-                    ast.List([elem.node for elem in elems], ctx=node.ctx),
+                    ast.Tuple([elem.node for elem in elems], ctx=node.ctx),
                     cast(Sequence[Unit], [elem.unit for elem in elems]),
                 )
+        elif isinstance(node, ast.List):
+            _log.warning(
+                f"In function {self.fun.__module__}"
+                + f"/{self.fun.__name__}"
+                + ": List not supported by impunity. "
+                + "Please use numpy arrays."
+            )
+            return QuantityNode(node, "dimensionless")
+
         elif isinstance(node, ast.Set):
             elems = list(map(self.get_node_unit, node.elts))
             return QuantityNode(
                 ast.Set([elem.node for elem in elems]),
                 cast(Sequence[Unit], [elem.unit for elem in elems]),
             )
+
         elif isinstance(node, ast.Dict):
             if not node.keys:
                 return QuantityNode(node, None)
             else:
                 elems = list(map(self.get_node_unit, node.values))
                 return QuantityNode(
                     ast.Dict(zip(node.keys, [elem.node for elem in elems])),
                     cast(Sequence[Unit], [elem.unit for elem in elems]),
                 )
         elif isinstance(node, ast.Name):
             return QuantityNode(node, self.vars[node.id])
 
-        elif isinstance(node, ast.BinOp) and isinstance(node.op, (ast.Add, ast.Sub)):
+        elif isinstance(node, ast.BinOp) and isinstance(
+            node.op, (ast.Add, ast.Sub)
+        ):
             left = self.get_node_unit(node.left)
             right = self.get_node_unit(node.right)
 
             if left.unit is None or right.unit is None:
                 new_node = ast.BinOp(left.node, node.op, right.node)
-                return QuantityNode(ast.copy_location(new_node, node), None)
+                return QuantityNode(
+                    ast.copy_location(new_node, node),
+                    left.unit if left.unit is not None else right.unit,
+                )
 
-            if pint.Unit(left.unit).is_compatible_with(pint.Unit(right.unit)):
-                if "dimensionless" in (left.unit, right.unit):
-                    conv_value = 1
-                else:
-                    conv_value = pint.Unit(left.unit).from_(pint.Unit(right.unit)).m
+            if pint.Unit(left.unit).is_compatible_with(  # type: ignore
+                pint.Unit(right.unit)  # type: ignore
+            ):
+                conv_value = (
+                    pint.Unit(left.unit)  # type: ignore
+                    .from_(pint.Unit(right.unit))  # type: ignore
+                    .m
+                )
                 new_node = ast.BinOp(
                     left.node,
                     node.op,
-                    ast.BinOp(right.node, ast.Mult(), ast.Constant(conv_value)),
+                    ast.BinOp(
+                        right.node, ast.Mult(), ast.Constant(conv_value)
+                    ),
+                )
+                return QuantityNode(
+                    ast.copy_location(new_node, node), left.unit
                 )
-                return QuantityNode(ast.copy_location(new_node, node), left.unit)
 
             else:
                 _log.warning(
                     f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                    f"Type {left.unit} and {right.unit} are not compatible. Defaulted to dimensionless"
+                    + f"Type {left.unit} and {right.unit} "
+                    + "are not compatible. Defaulted to dimensionless"
                 )
                 return QuantityNode(node, "dimensionless")
 
-        elif isinstance(node, ast.BinOp) and isinstance(node.op, (ast.Mult, ast.Div)):
+        elif isinstance(node, ast.BinOp) and isinstance(
+            node.op, (ast.Mult, ast.Div)
+        ):
             left = self.get_node_unit(node.left)
             right = self.get_node_unit(node.right)
 
             if left.unit is None or right.unit is None:
                 new_node = ast.BinOp(left.node, node.op, right.node)
-                return QuantityNode(ast.copy_location(new_node, node), None)
+                return QuantityNode(
+                    ast.copy_location(new_node, node),
+                    left.unit if left.unit is not None else right.unit,
+                )
 
-            if pint.Unit(left.unit).is_compatible_with(pint.Unit(right.unit)):
-                if "dimensionless" in (left.unit, right.unit):
-                    conv_value = 1
-                else:
-                    conv_value = pint.Unit(left.unit).from_(pint.Unit(right.unit)).m
+            if is_annotated(left.unit):
+                left.unit = left.unit.__metadata__[0]  # type: ignore
+
+            if is_annotated(right.unit):
+                right.unit = right.unit.__metadata__[0]  # type: ignore
+
+            if pint.Unit(left.unit).is_compatible_with(  # type: ignore
+                pint.Unit(right.unit)  # type: ignore
+            ):
+                conv_value = (
+                    pint.Unit(left.unit)  # type: ignore
+                    .from_(pint.Unit(right.unit))  # type: ignore
+                    .m
+                )
                 new_node = ast.BinOp(
                     left.node,
                     node.op,
-                    ast.BinOp(right.node, ast.Mult(), ast.Constant(conv_value)),
+                    ast.BinOp(
+                        right.node, ast.Mult(), ast.Constant(conv_value)
+                    ),
+                )
+                unit = (
+                    f"{left.unit}*{left.unit}"
+                    if isinstance(node.op, ast.Mult)
+                    else "dimensionless"
                 )
-                unit = f"{left.unit}*{left.unit}" if isinstance(node.op, ast.Mult) else "dimensionless"
                 return QuantityNode(ast.copy_location(new_node, node), unit)
 
             else:
                 new_node = ast.BinOp(left.node, node.op, right.node)
-                unit = f"{left.unit}*{right.unit}" if isinstance(node.op, ast.Mult) else f"{left.unit}/{right.unit}"
+                unit = (
+                    f"{left.unit}*{right.unit}"
+                    if isinstance(node.op, ast.Mult)
+                    else f"{left.unit}/{right.unit}"
+                )
                 return QuantityNode(ast.copy_location(new_node, node), unit)
 
-        elif isinstance(node, ast.BinOp):
+        elif isinstance(node, ast.BinOp) and isinstance(node.op, ast.Pow):
             left = self.get_node_unit(node.left)
             right = self.get_node_unit(node.right)
 
-            new_node = ast.BinOp(left.node, node.op, right.node)
-            return QuantityNode(
-                ast.copy_location(new_node, node),
-                self.get_node_unit(node.left).unit,
+            if left.unit is None:
+                new_node = ast.BinOp(left.node, node.op, right.node)
+                return QuantityNode(
+                    ast.copy_location(new_node, node),
+                    left.unit if left.unit is not None else None,
+                )
+
+            if is_annotated(left.unit):
+                left.unit = left.unit.__metadata__[0]  # type: ignore
+
+            if is_annotated(right.unit):
+                right.unit = right.unit.__metadata__[0]  # type: ignore
+
+            if left.unit == "dimensionless":
+                new_node = ast.BinOp(left.node, node.op, right.node)
+                return QuantityNode(new_node, "dimensionless")
+
+            if right.unit is not None:
+                _log.warning(
+                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    + "The exponent cannot be evaluated statically or is "
+                    + "not dimensionless."
+                )
+
+                return QuantityNode(node, None)
+
+            elif isinstance(right.node, ast.Constant):
+                unit = f"({left.unit})^({right.node.value})"
+                new_node = ast.BinOp(left.node, node.op, right.node)
+                return QuantityNode(new_node, unit)
+
+            elif isinstance(right.node, ast.BinOp):
+                pow_right = right.node.right
+                pow_left = right.node.left
+                if isinstance(pow_left, ast.Constant) and isinstance(
+                    pow_right, ast.Constant
+                ):
+                    if isinstance(right.node.op, ast.Mult):
+                        unit = (
+                            f"({left.unit})^({pow_left.value}"
+                            + f"*{pow_right.value})"
+                        )
+                    elif isinstance(right.node.op, ast.Div):
+                        unit = (
+                            f"({left.unit})^({pow_left.value}"
+                            + f"/{pow_right.value})"
+                        )
+                    elif isinstance(right.node.op, ast.Add):
+                        unit = (
+                            f"({left.unit})^({pow_left.value}"
+                            + f"+{pow_right.value})"
+                        )
+                    elif isinstance(right.node.op, ast.Sub):
+                        unit = (
+                            f"({left.unit})^({pow_left.value}"
+                            + f"-{pow_right.value})"
+                        )
+                    else:
+                        _log.warning(
+                            f"In function {self.fun.__module__}"
+                            + f"/{self.fun.__name__}: "
+                            + "The exponent cannot be "
+                            + "evaluated statically or is "
+                            + "not dimensionless."
+                        )
+                        new_node = ast.BinOp(left.node, node.op, right.node)
+                        return QuantityNode(new_node, None)
+                new_node = ast.BinOp(left.node, node.op, right.node)
+                return QuantityNode(new_node, unit)
+
+            else:
+                _log.warning(
+                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    + "The exponent cannot be evaluated statically or is "
+                    + "not dimensionless."
+                )
+                new_node = ast.BinOp(left.node, node.op, right.node)
+                return QuantityNode(new_node, None)
+
+        elif isinstance(node, ast.BinOp):
+            _log.warning(
+                f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                + "Binary Operation not supported yet."
             )
+            return QuantityNode(node, None)
 
         elif isinstance(node, ast.IfExp):
             body = self.get_node_unit(node.body)
             orelse = self.get_node_unit(node.orelse)
 
-            new_node = ast.IfExp(test=node.test, body=body.node, orelse=orelse.node)
+            new_node = ast.IfExp(
+                test=node.test, body=body.node, orelse=orelse.node
+            )
 
             if body.unit != orelse.unit:
                 _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: Ternary operator with mixed units"
+                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    + "Ternary operator with mixed units."
                 )
                 return QuantityNode(ast.copy_location(new_node, node), None)
             else:
-                return QuantityNode(ast.copy_location(new_node, node), body.unit)
+                return QuantityNode(
+                    ast.copy_location(new_node, node), body.unit
+                )
 
         elif isinstance(node, ast.Call):
-
+            node = self.generic_visit(node)  # type: ignore
             if isinstance(node.func, ast.Name):
                 id = node.func.id
             elif isinstance(node.func, ast.Attribute):
                 id = node.func.attr
 
             signature = self.get_annotations(id)
 
             new_args = []
             offset = 0
 
             # if not a known impunity function or no return signature
-            if signature is None or not signature or list(signature.items())[-1][0] != "return":
+            if (
+                signature is None
+                or not signature
+                or list(signature.items())[-1][0] != "return"
+            ):
                 return QuantityNode(node, None)
             else:
                 fun_signature = list(signature.items())[:-1]
                 return_signature = list(signature.items())[-1]
 
                 for i, arg in enumerate(node.args):
                     expected = fun_signature[i + offset][1]
                     if fun_signature[i][0] == "self":
                         offset = 1
                     if is_annotated(expected):
                         expected = expected.__metadata__[0]  # type: ignore
 
                     msg = (
-                        f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                        f"Function {id} expected unit {expected} but received unitless quantity"
+                        f"In function {self.fun.__module__}"
+                        + f"/{self.fun.__name__}: "
+                        + f"Function {id} expected unit "
+                        + f"{expected} but received unitless quantity"
                     )
 
-                    if (received := self.get_node_unit(arg).unit) is None:
+                    if (received := self.get_node_unit(arg)).unit is None:
                         if expected is not inspect._empty:
                             _log.warning(msg)
-                        new_args.append(node.args[i])
+                        new_args.append(arg)
                         continue
-                    if is_annotated(received):
-                        received = received.__metadata__[0]  # type: ignore
-                    if received != expected:
-                        if pint.Unit(received).is_compatible_with(pint.Unit(expected)):
-                            if "dimensionless" in (received, expected):
-                                conv_value = 1
-                            else:
-                                conv_value = pint.Unit(expected).from_(pint.Unit(received)).m
-                            new_arg = ast.BinOp(
-                                node.args[i],
-                                ast.Mult(),
-                                ast.Constant(conv_value),
-                            )
-                            new_args.append(new_arg)
-                        else:
-                            _log.warning(
-                                f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                                f"Function {id} expected unit {expected} but received incompatible unit {received}."
-                            )
-                    else:
-                        new_args.append(node.args[i])
+
+                    received.unit = (
+                        received.unit.__metadata__[0]  # type: ignore
+                        if is_annotated(received.unit)
+                        else received.unit
+                    )
+
+                    new_arg = self.node_convert(
+                        expected, received.unit, received.node
+                    )
+                    new_args.append(new_arg)
 
             new_node = (
                 node
                 if not new_args
                 else ast.Call(
                     func=node.func,
                     args=new_args,
                     keywords=node.keywords,
                 )
             )
 
-            return QuantityNode(ast.copy_location(new_node, node), return_signature[1])
+            return QuantityNode(
+                ast.copy_location(new_node, node), return_signature[1]
+            )
 
         elif isinstance(node, ast.Attribute):
             if isinstance(node.value, ast.Name):
                 if node.value.id == "self":
                     return QuantityNode(node, self.class_attr[node.attr])
             return QuantityNode(node, None)
 
         else:
             return QuantityNode(node, None)
 
-    def visit_Call(self, node: ast.Call) -> Any:
+    def visit_Call(self, node: ast.Call) -> ast.Call:
+        """Method called by the visitor if the visited node is a Call node.
+        Checks the units in the node and returns it eventually modified.
 
-        if isinstance(node.func, ast.Name):
+        Args:
+            node (ast.Call): input node
 
-            if node.func.id in __builtins__.keys():  # type: ignore
-                return node
+        """
 
-            # parameters = inspect.getfullargspec(self.fun_globals[node.func.id])
-            signature = self.get_annotations(self.fun_globals[node.func.id])
+        if isinstance(node.func, ast.Name):
+            fun_id = node.func.id
+        elif isinstance(node.func, ast.Attribute):
+            attr = node.func
+            fun_id = ""
+            while isinstance(attr, ast.Attribute):
+                fun_id = "." + attr.attr + fun_id  # type: ignore
+                attr = attr.value  # type: ignore
+            if isinstance(attr, ast.Name):
+                fun_id = attr.id + fun_id  # type: ignore
 
-            new_args: list[ast.BinOp | ast.expr] = []
-            new_keywords: list[ast.BinOp | ast.expr] = []
-            if node.args or node.keywords:
-                if signature:
-                    fun_signature = list(signature.items())[:-1]
+        if fun_id in __builtins__.keys():  # type: ignore
+            node = self.generic_visit(node)  # type: ignore
+            return node
+
+        # parameters = inspect.getfullargspec(self.fun_globals[
+        # node.func.id])
+        signature = self.get_annotations(fun_id)  # type: ignore
+
+        new_args: list[ast.BinOp | ast.expr] = []
+        new_keywords: list[ast.BinOp | ast.expr] = []
+        if node.args or node.keywords:
+            if signature:
+                fun_signature = list(signature.items())[:-1]
+            else:
+                return node
+            for i, arg in enumerate(node.args):
+                if (received := self.get_node_unit(arg)).unit != (
+                    expected := fun_signature[i][1]
+                ):
+                    if is_annotated(expected):
+                        expected = expected.__metadata__[0]  # type: ignore
+                    new_arg = self.node_convert(
+                        expected, received.unit, received.node
+                    )
+                    new_args.append(new_arg)
                 else:
-                    return None
-                for i, arg in enumerate(node.args):
-                    if (received := self.get_node_unit(arg).unit) != (expected := fun_signature[i][1]):
+                    new_args.append(arg)
+
+            for keyword in node.keywords:
+                if keyword.arg:
+                    if (received := self.get_node_unit(keyword.value)) != (
+                        expected := signature[keyword.arg]
+                    ):
                         if is_annotated(expected):
-                            expected = expected.__metadata__[0]  # type: ignore
-                        if pint.Unit(received).is_compatible_with(pint.Unit(expected)):
-                            if "dimensionless" in (received, expected):
-                                conv_value = 1
-                            else:
-                                conv_value = pint.Unit(expected).from_(pint.Unit(received)).m
-                        else:
-                            _log.warning(
-                                f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                                f"Function {node.func.id} expected unit {expected}"
-                                + f"but received incompatible unit {received}."
-                            )
+                            x = expected.__metadata__[0]  # type: ignore
+                            expected = x
+                        if not (
+                            isinstance(expected, str)
+                            and isinstance(received.unit, str)
+                        ):
+                            # TODO To avoid annoying typing for now
                             return node
 
-                        new_arg = ast.BinOp(
-                            arg,
-                            ast.Mult(),
-                            ast.Constant(conv_value),
+                        new_value = self.node_convert(
+                            expected, received.unit, received.node
                         )
-                        new_args.append(new_arg)
-                    else:
-                        new_args.append(arg)
 
-                for keyword in node.keywords:
-                    if keyword.arg:
-                        if (received := self.get_node_unit(keyword.value).unit) != (expected := signature[keyword.arg]):
-                            if is_annotated(expected):
-                                expected = expected.__metadata__[0]  # type: ignore
-                            if not (isinstance(expected, str) and isinstance(received, str)):
-                                # TODO To avoid annoying typing for now
-                                return node
-
-                            if pint.Unit(received).is_compatible_with(pint.Unit(expected)):
-                                if "dimensionless" in (received, expected):
-                                    conv_value = 1
-                                else:
-                                    conv_value = pint.Unit(expected).from_(pint.Unit(received)).m
-                            else:
-                                _log.warning(
-                                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                                    f"Function {node.func.id} expected unit {expected}"
-                                    + f"but received incompatible unit {received}."
-                                )
-                                return node
-                            new_value = ast.BinOp(
-                                keyword.value,
-                                ast.Mult(),
-                                ast.Constant(conv_value),
-                            )
-                            new_keyword = cast(
-                                ast.expr,
-                                ast.keyword(
-                                    keyword.arg,
-                                    new_value,
-                                ),
-                            )
+                        new_keyword = cast(
+                            ast.expr,
+                            ast.keyword(
+                                keyword.arg,
+                                new_value,
+                            ),
+                        )
 
-                            new_keywords.append(new_keyword)
-                        else:
-                            new_args.append(arg)
+                        new_keywords.append(new_keyword)
 
-            if new_args:
-                new_node = ast.Call(
-                    func=node.func,
-                    args=new_args,
-                    keywords=new_keywords,
-                )
+        if new_args or new_keywords:
+            new_node = ast.Call(
+                func=node.func,
+                args=new_args,
+                keywords=new_keywords,
+            )
 
-                return ast.copy_location(new_node, node)
+            return ast.copy_location(new_node, node)
 
         return node
 
-    def visit_AnnAssign(self, node: ast.AnnAssign) -> Any:
+    def visit_AnnAssign(self, node: ast.AnnAssign) -> ast.AnnAssign:
+        """Method called by the visitor if the visited node is an
+        Annotated Assignement node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.AnnAssign): input node
+
+        """
 
         value = self.get_node_unit(node.value)
 
         if value is None:
             pass
 
         if value.node != node.value:
@@ -570,195 +832,226 @@
                 value=value.node,
                 simple=node.simple,
             )
 
             node = ast.copy_location(new_node, node)
 
         if value.unit is None:
-            # _log.warning(
-            #     f"In function {self.fun.__module__}/{self.fun.__name__}:
-            # The unit of {node.target.id} could not be checked."
-            # )
             new_node = node
 
-        elif (received := value.unit) != (expected := cast(annotation_node, node.annotation)):
-
+        elif (received := value).unit != (
+            expected := cast(annotation_node, node.annotation)
+        ):
             expected_unit = get_annotation_unit(expected)
-            if is_annotated(received):
-                received = received.__metadata__[0]  # type: ignore
-            if received == "dimensionless":
-                new_node = node
-
-            elif pint.Unit(received).is_compatible_with(pint.Unit(expected_unit)):
-                if "dimensionless" in (received, expected_unit):
-                    conv_value = 1
-                else:
-                    conv_value = pint.Unit(expected_unit).from_(pint.Unit(received)).m
-                new_value = ast.BinOp(
-                    node.value,
-                    ast.Mult(),
-                    ast.Constant(conv_value),
-                )
-                new_node = ast.AnnAssign(
-                    target=node.target,
-                    annotation=node.annotation,
-                    value=new_value,
-                    simple=node.simple,
-                )
+            if is_annotated(received.unit):
+                received.unit = received.unit.__metadata__[0]  # type: ignore
 
-            else:
-                _log.warning(
-                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
-                    f"Assignement expected unit {expected} but received incompatible unit {received}."
-                )
-                return node
-        else:
-            new_node = node
+            new_value = self.node_convert(
+                expected_unit, received.unit, received.node
+            )
+            new_node = ast.AnnAssign(
+                target=node.target,
+                annotation=node.annotation,
+                value=new_value,
+                simple=node.simple,
+            )
 
         if isinstance(node.target, ast.Attribute):
             if isinstance(node.target.value, ast.Name):
                 if node.target.value.id == "self":
                     self.class_attr[node.target.attr] = value.unit
         else:
             if isinstance(node.target, ast.Name):
-                annotation = get_annotation_unit(cast(annotation_node, node.annotation))
+                annotation = get_annotation_unit(
+                    cast(annotation_node, node.annotation)
+                )
                 self.vars[node.target.id] = annotation
         # ast.fix_missing_locations(new_node)
         return ast.copy_location(new_node, node)
 
-    def visit_BinOp(self, node: ast.BinOp) -> Any:
+    def visit_BinOp(self, node: ast.BinOp) -> ast.BinOp:
+        """Method called by the visitor if the visited node is an
+        Binary Operation node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.BinOp): input node
+
+        """
+
         return self.get_node_unit(node).node
 
-    def visit_For(self, node: ast.For) -> Any:
+    def visit_For(self, node: ast.For) -> ast.For:
+        """Method called by the visitor if the visited node is a for loop node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.For): input node
+
+        """
         if isinstance(node.target, ast.Name):
             self.vars[node.target.id] = None
         self.generic_visit(node)
         return node
 
-    def visit_ListComp(self, node: ast.ListComp) -> Any:
+    def visit_ListComp(self, node: ast.ListComp) -> ast.ListComp:
+        """Method called by the visitor if the visited node is a List
+        Comprehension node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.ListComp): input node
+
+        """
+
         # Calling the comprehension before the generic
         # visit to get indices into self.vars
         self.visit_comprehension(node.generators[0])
         self.generic_visit(node)
         return node
 
-    def visit_comprehension(self, node: ast.comprehension) -> Any:
+    def visit_comprehension(
+        self, node: ast.comprehension
+    ) -> ast.comprehension:
+        """Method called by the visitor if the visited node is a
+        Comprehension node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.comprehension): input node
+
+        """
+
         if isinstance(node.target, ast.Name):
             self.vars[node.target.id] = None
         return node
 
-    def visit_Assign(self, node: ast.Assign) -> Any:
+    def visit_Assign(self, node: ast.Assign) -> ast.Assign:
+        """Method called by the visitor if the visited node is an
+        Assignement node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.Assign): input node
 
+        """
         value = self.get_node_unit(node.value)
-        if value.node != node.value:
 
+        if value.unit is None:
+            return node
+        if value.node != node.value:
             new_node = ast.Assign(
                 targets=node.targets,
                 value=value.node,
             )
             node = ast.copy_location(new_node, node)
 
-        if isinstance(node.value, ast.Call):
-            for target in node.targets:
-                if isinstance(target, ast.Tuple):
-                    if isinstance(node.value.func, ast.Name):
-                        func_name = node.value.func.id
-                    elif isinstance(node.value.func, ast.Attribute):
-                        if isinstance(node.value.func.value, ast.Name):
-                            func_name = (
-                                self.vars[node.value.func.value.id]
-                                if node.value.func.value.id in self.vars
-                                else node.value.func.value.id
-                            )
-                        func_name += "." + node.value.func.attr
-                    for i, elem in enumerate(target.elts):
-                        # if return values are tuples
-                        if isinstance(elem, ast.Name):
-                            if (sign := self.get_annotations(func_name)) is not None:
-                                if is_annotated(sign["return"].__args__[i]):
-                                    self.vars[elem.id] = sign["return"].__args__[i].__metadata__[0]
-                                else:
-                                    self.vars[elem.id] = sign["return"].__args__[i].__forward_value__
-                elif isinstance(target, ast.Name):
-                    if isinstance(node.value.func, ast.Name):
-                        func_name = node.value.func.id
-                    elif isinstance(node.value.func, ast.Attribute):
-                        if isinstance(node.value.func.value, ast.Name):
-                            func_name = (
-                                self.vars[node.value.func.value.id]
-                                if node.value.func.value.id in self.vars
-                                else node.value.func.value.id
-                            )
-                        func_name += "." + node.value.func.attr
-                elif isinstance(target, ast.Attribute):
-                    if isinstance(target.value, ast.Name):
-                        if target.value.id == "self":
-                            self.class_attr[target.attr] = value.unit
-            new_node = node
+        new_node = ast.Assign(
+            targets=node.targets,
+            value=value.node,
+            type_comment=f"unit: {value.unit}",
+        )
+
+        for target in node.targets:
+            if isinstance(target, ast.Tuple):
+                received = (
+                    [
+                        arg.__metadata__[0]  # type: ignore
+                        if is_annotated(arg)
+                        else arg
+                        for arg in value.unit.__args__
+                    ]
+                    if hasattr(value.unit, "__args__")
+                    else value.unit
+                )
+                for i, elem in enumerate(target.elts):
+                    if isinstance(elem, ast.Name):
+                        if isinstance(received[i], typing.ForwardRef):
+                            self.vars[elem.id] = received[i].__forward_arg__
+                        else:
+                            self.vars[elem.id] = received[i]
 
-        else:
-            new_node = ast.Assign(
-                targets=node.targets,
-                value=value.node,
-                type_comment=f"unit: {value.unit}",
-            )
-            for target in node.targets:
-                if isinstance(target, ast.Tuple):
-                    for i, elem in enumerate(target.elts):
-                        if isinstance(elem, ast.Name):
-                            self.vars[elem.id] = value.unit[i]
-
-                elif isinstance(target, ast.Name):
-                    self.vars[target.id] = value.unit
-                elif isinstance(target, ast.Attribute):
-                    if isinstance(target.value, ast.Name):
-                        if target.value.id == "self":
-                            self.class_attr[target.attr] = value.unit
+            elif isinstance(target, ast.Name):
+                self.vars[target.id] = value.unit
+            elif isinstance(target, ast.Attribute):
+                if isinstance(target.value, ast.Name):
+                    if target.value.id == "self":
+                        self.class_attr[target.attr] = value.unit
 
         return ast.copy_location(new_node, node)
 
-    def visit_Return(self, node: ast.Return) -> Any:
+    def visit_Return(self, node: ast.Return) -> ast.Return:
+        """Method called by the visitor if the visited node is a
+        Return node.
+        Checks the units in the node and returns it eventually modified.
+
+        Args:
+            node (ast.Return): input node
+
+        """
         for frameinfo in inspect.stack():
             if frameinfo.function == "visit_FunctionDef":
                 fun = frameinfo.frame.f_locals["node"].name
                 break
         return_annotation = self.get_annotations(fun)
-        value = self.get_node_unit(node.value)
+        received = self.get_node_unit(node.value)
 
-        if value.node != node.value:
-            new_node = ast.Return(value=value.node)
+        if received.node != node.value:
+            new_node = ast.Return(value=received.node)
             node = ast.copy_location(new_node, node)
 
-        if return_annotation is inspect._empty:
-            _log.warning(f"In function {self.fun.__module__}/{self.fun.__name__}: Some return annotations are missing")
+        if return_annotation is inspect._empty or return_annotation is None:
+            _log.warning(
+                f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                + "Some return annotations are missing"
+            )
+            new_node = node
+            return ast.copy_location(new_node, node)
 
-        if is_annotated(return_annotation):
-            expected = return_annotation.__metadata__[1]  # type: ignore
-        elif isinstance(return_annotation, str):
-            expected = return_annotation
+        if isinstance(return_annotation, Dict):
+            if is_annotated(return_annotation["return"]):
+                ret = return_annotation["return"]
+                if len(ret.__args__) > 1:  # type: ignore
+                    expected = [
+                        x.__metadata__[0]  # type: ignore
+                        if is_annotated(x)
+                        else x
+                        for x in ret.__args__  # type: ignore
+                    ]
+                else:
+                    expected = ret.__metadata__[0]  # type: ignore
+            else:  # string annotations
+                expected = return_annotation["return"]
         else:
             _log.warning(
                 f"In function {self.fun.__module__}/{self.fun.__name__}: "
                 "Type of the return annotation not supported yet"
             )
-            return node
+            new_node = node
+            return ast.copy_location(new_node, node)
 
-        if (received := value.unit) != expected:
-            if pint.Unit(received).is_compatible_with(pint.Unit(expected)):
-                if "dimensionless" in (received, expected):
-                    conv_value = 1
-                else:
-                    conv_value = pint.Unit(expected).from_(pint.Unit(received)).m
-                new_value = ast.BinOp(
-                    node.value,
-                    ast.Mult(),
-                    ast.Constant(conv_value),
-                )
-                new_node = ast.Return(value=new_value)
+        if is_annotated(received.unit):
+            received.unit = received.unit.__metadata__[0]  # type: ignore
 
+        if isinstance(expected, list):
+            if isinstance(received.unit, list):
+                new_node = node
             else:
-                raise_node = raise_dim_error(pint.errors.DimensionalityError, received, expected)
-                return raise_node
+                _log.warning(
+                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    "Expected more than one return value"
+                )
+                new_node = node
         else:
-            new_node = node
+            if isinstance(received.unit, list):
+                _log.warning(
+                    f"In function {self.fun.__module__}/{self.fun.__name__}: "
+                    "Expected more than one return value"
+                )
+                new_node = node
+            else:
+                new_value = self.node_convert(
+                    expected, received.unit, received.node
+                )
+                new_node = ast.Return(value=new_value)
 
         return ast.copy_location(new_node, node)
```

### Comparing `impunity-0.2.1/PKG-INFO` & `impunity-1.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: impunity
-Version: 0.2.1
+Version: 1.0
 Summary: Static checking for consistency of physical units
+License: MIT
 Author: Antoine Chevrot
 Author-email: antoine.chevrot@gmail.com
 Requires-Python: >=3.8,<4.0
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: Pint (>=0.19.2)
 Requires-Dist: astor (>=0.8.1,<0.9.0)
```

