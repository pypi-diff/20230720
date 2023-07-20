# Comparing `tmp/cantaloupe-0.1.2.tar.gz` & `tmp/cantaloupe-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cantaloupe-0.1.2.tar", max compression
+gzip compressed data, was "cantaloupe-0.1.4.tar", max compression
```

## Comparing `cantaloupe-0.1.2.tar` & `cantaloupe-0.1.4.tar`

### file list

```diff
@@ -1,18 +1,16 @@
--rw-r--r--   0        0        0     1266 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/README.md
--rw-r--r--   0        0        0      812 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/pyproject.toml
--rw-r--r--   0        0        0       86 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/__init__.py
--rw-r--r--   0        0        0       73 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/__main__.py
--rw-r--r--   0        0        0     1022 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/enums.py
--rw-r--r--   0        0        0      551 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/errors.py
--rw-r--r--   0        0        0     1451 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/hookspecs.py
--rw-r--r--   0        0        0     3382 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/host.py
--rw-r--r--   0        0        0     1658 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/loaders.py
--rw-r--r--   0        0        0      694 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/logger.py
--rw-r--r--   0        0        0     2715 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/models.py
--rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/__init__.py
--rw-r--r--   0        0        0     1140 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_cli.py
--rw-r--r--   0        0        0      695 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_error_handling.py
--rw-r--r--   0        0        0     3557 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/plugins/core_framework.py
--rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/types.py
--rw-r--r--   0        0        0        0 2023-07-11 04:32:38.210359 cantaloupe-0.1.2/src/cantaloupe/utils.py
--rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 cantaloupe-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1266 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/README.md
+-rw-r--r--   0        0        0      794 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/__init__.py
+-rw-r--r--   0        0        0       73 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/__main__.py
+-rw-r--r--   0        0        0     1022 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/enums.py
+-rw-r--r--   0        0        0      551 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/errors.py
+-rw-r--r--   0        0        0     1359 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/hookspecs.py
+-rw-r--r--   0        0        0     3496 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/host.py
+-rw-r--r--   0        0        0     1658 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/loaders.py
+-rw-r--r--   0        0        0      694 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/logger.py
+-rw-r--r--   0        0        0     2887 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/models.py
+-rw-r--r--   0        0        0        0 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/plugins/__init__.py
+-rw-r--r--   0        0        0     1275 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/plugins/core_cli.py
+-rw-r--r--   0        0        0      695 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/plugins/core_error_handling.py
+-rw-r--r--   0        0        0     3552 2023-07-20 17:22:02.073763 cantaloupe-0.1.4/src/cantaloupe/plugins/core_framework.py
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 cantaloupe-0.1.4/PKG-INFO
```

### Comparing `cantaloupe-0.1.2/README.md` & `cantaloupe-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/pyproject.toml` & `cantaloupe-0.1.4/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 [tool.poetry]
 name = "cantaloupe"
-version = "0.1.2"
+version = "0.1.4"
 description = "An extensible framework for building browser automations."
 authors = ["Lemuel Boyce <lemuelboyce@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "cantaloupe", from = "src" }]
 
 [tool.poetry.scripts]
 cantaloupe = "cantaloupe.__main__:entry"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-pydantic = "^2.0.2"
-jinja2 = "^3.1.2"
+pydantic = "^2.0.3"
 pluggy = "^1.2.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pyyaml = "^6.0"
 black = "^22.12.0"
 pytest-playwright = "^0.3.0"
```

### Comparing `cantaloupe-0.1.2/src/cantaloupe/enums.py` & `cantaloupe-0.1.4/src/cantaloupe/enums.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/src/cantaloupe/errors.py` & `cantaloupe-0.1.4/src/cantaloupe/errors.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/src/cantaloupe/hookspecs.py` & `cantaloupe-0.1.4/src/cantaloupe/hookspecs.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 import typing
-from argparse import ArgumentParser
-from typing import Any, Callable, TypeVar, cast
 
 import pluggy
 
 if typing.TYPE_CHECKING:
-    from .models import Step, Workflow, Config, Context
+    from argparse import ArgumentParser
 
-F = TypeVar("F", bound=Callable[..., Any])
+    from .models import Config, Context, Step, Workflow
 
-hookspec = cast(Callable[[F], F], pluggy.HookspecMarker("cantaloupe"))
+
+hookspec = pluggy.HookspecMarker("cantaloupe")
 
 
 @hookspec
-def cantaloupe_addoption(parser: ArgumentParser) -> None:
+def cantaloupe_addoption(parser: "ArgumentParser") -> None:
     """
     Called to add arguments to the argument parser.
 
     :param parser: the parser to add arguments to
     :type parser: argparse.ArgumentParser
     :return:
     :rtype:
@@ -49,15 +48,15 @@
     """
 
 
 @hookspec
 def cantaloupe_resolve_step_variables(
     workflow: "Workflow",
     step: "Step",
-) -> "Step":
+) -> "Step":  # type: ignore
     """
     Called to resolve variables for a given step.
     """
 
 
 @hookspec
 def cantaloupe_validate_step_imports(
```

### Comparing `cantaloupe-0.1.2/src/cantaloupe/host.py` & `cantaloupe-0.1.4/src/cantaloupe/host.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 from .plugins import core_cli, core_error_handling, core_framework
 
 if typing.TYPE_CHECKING:
     from pluggy._hooks import _HookRelay
 
 parser = argparse.ArgumentParser(
     prog="cantaloupe",
-    description="Cantaloupe is a tool for automating web applications.",
+    description="An extensible framework for building browser automations.",
 )
 
 
 def _make_path(workflow_path: PosixPath) -> Path:
     """A little hacky, potentially unstable."""
     cwd = Path(os.getcwd())
     if workflow_path == ".":
@@ -66,28 +66,32 @@
 def main(args: list[Any]) -> None:
     """
     Main entry point for the Cantaloupe CLI.
     """
 
     manager = get_plugin_manager()
 
-    # Add all plugin options to parser
+    # collect all the options from plugins
     manager.hook.cantaloupe_addoption(parser=parser)
 
     opts = parser.parse_args(args)
     config = Config(
         option=opts,
+        dry_run=opts.dry_run,
         workflow_dir=_make_path(opts.workflows),
         pluginmanager=manager,
     )
 
     logger = get_root_logger(level=config.get_log_level())
+    if config.dry_run:
+        logger.info("Running in dry-run mode...")
+
     context = load_context(workflows=config.workflow_dir)
     if context is None:
-        logger.error("No context file found.")
+        logger.error("No context file found...")
         return
 
     cantaloupe = Cantaloupe(manager.hook, logger)
 
     # Add workflows to context
     logger.debug("Loading workflows from %s", config.workflow_dir)
     context.workflows = list(load_workflows(workflows=config.workflow_dir))
```

### Comparing `cantaloupe-0.1.2/src/cantaloupe/loaders.py` & `cantaloupe-0.1.4/src/cantaloupe/loaders.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/src/cantaloupe/logger.py` & `cantaloupe-0.1.4/src/cantaloupe/logger.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/src/cantaloupe/models.py` & `cantaloupe-0.1.4/src/cantaloupe/models.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,36 @@
 from __future__ import annotations
 
 import argparse
 import logging
-from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Iterable
 
 import pluggy
-from pydantic import BaseModel, Field
+from pydantic import BaseModel, ConfigDict, Field
 
 from .enums import Action, Browser, ScreenshotOpts, TraceVideoOpts
 
 
-@dataclass(frozen=True)
-class Config:
+class Config(BaseModel):
     """
-    This class represents a configuration file.
+    This class represents an immutable configuration object.
     """
 
     option: argparse.Namespace
+    dry_run: bool = Field(default=False)
+    workflow_dir: Path
     pluginmanager: pluggy.PluginManager
-    workflow_dir: Path | None = Field(default=None)
 
-    class ConfigDict:
-        use_enum_values = True
-        arbitrary_types_allowed = True
+    # Pydantic Config
+    model_config = ConfigDict(
+        frozen=True,
+        use_enum_values=True,
+        arbitrary_types_allowed=True,
+    )
 
     def get_log_level(self) -> int:
         """
         Returns the log level.
         """
         if self.option.debug:
             return logging.DEBUG
@@ -39,63 +41,63 @@
     """Defines an action to be taken as part of a workflow."""
 
     use: str | None = Field(default=None)
     config: dict[str, Any] = Field(default_factory=dict)
     action: Action
     variables: dict[str, Any] = Field(default_factory=dict)
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class WorkflowVariable(BaseModel):
     name: str
     type: str = Field(default="string")
     default: Any = Field(default=None)
     required: bool = Field(default=False)
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class Workflow(BaseModel):
     name: str
     steps: list[Step]
     file_name: str
     file_path: Path | str
     variables: list[WorkflowVariable] = Field(default_factory=list)
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class ContextAssetOpts(BaseModel):
     trace: TraceVideoOpts = Field(default=TraceVideoOpts.OFF)
     video: TraceVideoOpts = Field(default=TraceVideoOpts.ON)
     screenshot: ScreenshotOpts = Field(default=ScreenshotOpts.ON_FAILURE)
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class ContextTimeoutOpts(BaseModel):
     script_timeout: int = Field(default=120000)  # 2 minutes
     global_timeout: int = Field(default=3600000)  # 1 hour
     action_timeout: int = Field(default=60000)  # 1 minute
     expect_timeout: int = Field(default=15000)  # 15 seconds
     navigation_timeout: int = Field(default=15000)  # 15 seconds
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
 
 
 class Context(BaseModel):
     assets: ContextAssetOpts = Field(default_factory=ContextAssetOpts)
     browser: Browser = Field(default=Browser.CHROMIUM)
     retries: int = Field(default=0)
     timeouts: ContextTimeoutOpts = Field(default_factory=ContextTimeoutOpts)
     headless: bool = Field(default=True)
     base_url: str = Field(default=None)
     workflows: Iterable[Workflow] = Field(default_factory=list)
 
-    class ConfigDict:
-        use_enum_values = True
+    # Pydantic Config
+    model_config = ConfigDict(use_enum_values=True)
```

### Comparing `cantaloupe-0.1.2/src/cantaloupe/plugins/core_cli.py` & `cantaloupe-0.1.4/src/cantaloupe/plugins/core_cli.py`

 * *Files 7% similar despite different names*

```diff
@@ -43,7 +43,13 @@
     parser.add_argument(
         "-ff",
         "--failfast",
         action="store_true",
         help="Stop on first failure.",
         required=False,
     )
+    parser.add_argument(
+        "--dry-run",
+        action="store_true",
+        help="Dry run mode.",
+        required=False,
+    )
```

### Comparing `cantaloupe-0.1.2/src/cantaloupe/plugins/core_error_handling.py` & `cantaloupe-0.1.4/src/cantaloupe/plugins/core_error_handling.py`

 * *Files identical despite different names*

### Comparing `cantaloupe-0.1.2/src/cantaloupe/plugins/core_framework.py` & `cantaloupe-0.1.4/src/cantaloupe/plugins/core_framework.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
                 index=index,
                 step=step,
                 workflow=workflow,
             )
             if not step.use:
                 steps.append(step)
             else:
-                # Load the workflow referenced in "use" and merge its steps them into the current workflow.
+                # Load the workflow referenced in "use" and merge its steps into the current workflow.
                 imported_workflow = load_workflow(
                     os.path.join(config.option.workflows, step.use)
                 )
                 if not imported_workflow.variables:
                     for imported_steps in imported_workflow.steps:
                         steps.append(imported_steps)
                 else:
```

### Comparing `cantaloupe-0.1.2/PKG-INFO` & `cantaloupe-0.1.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 Metadata-Version: 2.1
 Name: cantaloupe
-Version: 0.1.2
+Version: 0.1.4
 Summary: An extensible framework for building browser automations.
 Author: Lemuel Boyce
 Author-email: lemuelboyce@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: jinja2 (>=3.1.2,<4.0.0)
 Requires-Dist: pluggy (>=1.2.0,<2.0.0)
-Requires-Dist: pydantic (>=2.0.2,<3.0.0)
+Requires-Dist: pydantic (>=2.0.3,<3.0.0)
 Description-Content-Type: text/markdown
 
 # Cantaloupe
 
 An extensible framework for building browser automations.
 
 > #### Note: This library is still very much WIP 🧪. This means that breaking changes can be introduced at any point in time.
```

