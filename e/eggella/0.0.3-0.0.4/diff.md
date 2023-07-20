# Comparing `tmp/eggella-0.0.3.tar.gz` & `tmp/eggella-0.0.4.tar.gz`

## Comparing `eggella-0.0.3.tar` & `eggella-0.0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/__init__.py
--rw-r--r--   0        0        0     5999 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/app.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/exceptions.py
--rw-r--r--   0        0        0     8043 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/manager.py
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/__init__.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/abc.py
--rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/arg_caster.py
--rw-r--r--   0        0        0     1465 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/completer.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/handler.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/objects.py
--rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/command/parser.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/__init__.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/abc.py
--rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/events/events.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/fsm/__init__.py
--rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/fsm/fsm.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/__init__.py
--rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/cmd_shortcuts.py
--rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/shortcuts/help_pager.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/tools/__init__.py
--rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.3/eggella/tools/type_caster.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.3/.gitignore
--rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 eggella-0.0.3/README.md
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 eggella-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/__init__.py
+-rw-r--r--   0        0        0     6312 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/app.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/exceptions.py
+-rw-r--r--   0        0        0     8901 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/manager.py
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/__init__.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/abc.py
+-rw-r--r--   0        0        0     2402 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/arg_caster.py
+-rw-r--r--   0        0        0     4322 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/completer.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/handler.py
+-rw-r--r--   0        0        0     2100 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/objects.py
+-rw-r--r--   0        0        0      351 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/command/parser.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/__init__.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/abc.py
+-rw-r--r--   0        0        0     2401 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/events/events.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/fsm/__init__.py
+-rw-r--r--   0        0        0     5451 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/fsm/fsm.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/__init__.py
+-rw-r--r--   0        0        0      530 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/cmd_shortcuts.py
+-rw-r--r--   0        0        0     3722 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/shortcuts/help_pager.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/tools/__init__.py
+-rw-r--r--   0        0        0     2113 2020-02-02 00:00:00.000000 eggella-0.0.4/eggella/tools/type_caster.py
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 eggella-0.0.4/.gitignore
+-rw-r--r--   0        0        0     2639 2020-02-02 00:00:00.000000 eggella-0.0.4/README.md
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 eggella-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 eggella-0.0.4/PKG-INFO
```

### Comparing `eggella-0.0.3/eggella/app.py` & `eggella-0.0.4/eggella/app.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
     Type,
     Union,
     overload,
 )
 
 from prompt_toolkit import HTML, PromptSession
 from prompt_toolkit.completion.fuzzy_completer import FuzzyCompleter
+from prompt_toolkit.completion.nested import NestedDict
 from prompt_toolkit.formatted_text import FormattedText
 
 from eggella.command.abc import ABCCommandHandler
 from eggella.exceptions import CommandNotFoundError, CommandParseError
 from eggella.fsm.fsm import FsmController, IntStateGroup
 from eggella.manager import CommandManager, EventManager
 from eggella.shortcuts.cmd_shortcuts import CmdShortCuts
@@ -85,20 +86,24 @@
     def on_command(
         self,
         key: Optional[str] = None,
         short_description: Optional[str] = None,
         *,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
+        nested_completions: Optional[NestedDict] = None,
+        nested_meta: Optional[Dict[str, Any]] = None,
     ):
         return self._command_manager.command(
             key,
             short_description=short_description,
             usage=usage,
             cmd_handler=cmd_handler,
+            nested_completions=nested_completions,
+            nested_meta=nested_meta,
         )
 
     def on_state(self, state: IntStateGroup):
         return self.fsm.state(state)
 
     def register_states(self, states: Type[IntStateGroup]):
         self.fsm.attach(states)
@@ -152,14 +157,15 @@
         if self.has_command(key):
             self._command_manager.commands.pop(key)
         else:
             raise KeyError
 
     def loop(self):
         self.cmd.print_ft(self.intro)
+        self._command_manager.register_buildin_commands()
         self._handle_startup_events()
         self._handle_commands()
         self._handle_close_events()
 
     def _handle_startup_events(self):
         for event in self._event_manager.startup_events:
             event()
```

### Comparing `eggella-0.0.3/eggella/manager.py` & `eggella-0.0.4/eggella/manager.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,16 @@
     List,
     Literal,
     Optional,
     Tuple,
     Type,
 )
 
+from prompt_toolkit.completion.nested import NestedDict
+
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.completer import CommandCompleter
 from eggella.command.handler import CommandHandler
 from eggella.command.objects import Command
 from eggella.events.events import (
     OnCommandCompleteSuccess,
     OnCommandError,
@@ -36,15 +38,14 @@
 
 class CommandManager:
     def __init__(self, app: "Eggella"):
         self._app = app
         self.commands: Dict[str, Command] = {}
         self.error_events: Dict[str, Callable[[str, BaseException, str, str], Any]] = {}
         self.handled_exceptions: _ErrorEventsMapping = {}
-        self._register_buildin_commands()
 
     @staticmethod
     def _simple_parse_arguments(raw_command: str) -> Tuple[Tuple[str, ...], Dict[str, str]]:
         tokens = shlex.split(raw_command)
         args: List[str] = []
         kwargs: Dict[str, str] = {}
         for token in tokens:
@@ -107,22 +108,26 @@
     def command(
         self,
         key: Optional[str] = None,
         *,
         short_description: Optional[str] = None,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
+        nested_completions: Optional[NestedDict] = None,
+        nested_meta: Optional[Dict[str, Any]] = None,
     ):
         def decorator(func: Callable):
             self.register_command(
                 func,
                 key=key,
                 short_description=short_description,
                 usage=usage,
                 cmd_handler=cmd_handler,
+                nested_completions=nested_completions,
+                nested_meta=nested_meta,
             )
 
             @wraps(func)
             def wrapper(*args, **kwargs):
                 return func(*args, **kwargs)
 
             return wrapper
@@ -133,35 +138,41 @@
         self,
         func: Callable,
         key: Optional[str] = None,
         *,
         short_description: Optional[str] = None,
         usage: Optional[str] = None,
         cmd_handler: Optional[ABCCommandHandler] = None,
+        nested_completions: Optional[NestedDict] = None,
+        nested_meta: Optional[Dict[str, Any]] = None,
     ):
         if not key:
             key = func.__name__
         if self.commands.get(key):
             raise TypeError(f"Command '{key}' already register")
 
         if not cmd_handler:
             self.commands[key] = Command(
                 fn=func,
                 key=key,
                 handler=CommandHandler(),
                 short_description=short_description,
                 usage=usage,
+                nested_completions={key: nested_completions},
+                nested_meta=nested_meta or {},
             )
         elif cmd_handler:
             self.commands[key] = Command(
                 fn=func,
                 key=key,
                 handler=cmd_handler,
                 short_description=short_description,
                 usage=usage,
+                nested_completions={key: nested_completions},
+                nested_meta=nested_meta or {},
             )
 
     def _help_command(self, key: Optional[str] = None):
         """show help or show pager documentation for all commands if not argument passed"""
         if not key:
             commands = self.commands.values()
             gen_help_pager(self._app, commands)
@@ -172,17 +183,26 @@
             raise CommandNotFoundError
 
     @staticmethod
     def _exit_command():
         """exit from this application"""
         raise KeyboardInterrupt
 
-    def _register_buildin_commands(self):
-        self.register_command(self._help_command, "help", usage="help; help exit")
+    def register_buildin_commands(self):
         self.register_command(self._exit_command, "exit")
+        _nested_commands = {k: None for k in self.commands.keys()}
+        _nested_meta = {}
+        _nested_meta.update({k: v.short_desc for k, v in self.commands.items()})
+        self.register_command(
+            self._help_command,
+            "help",
+            usage="help; help exit",
+            nested_completions=_nested_commands,
+            nested_meta=_nested_meta,
+        )
 
 
 class EventManager:
     def __init__(self, app: "Eggella"):
         self.app = app
         self.startup_events: List[Callable] = []
         self.close_events: List[Callable] = []
```

### Comparing `eggella-0.0.3/eggella/command/arg_caster.py` & `eggella-0.0.4/eggella/command/arg_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/command/handler.py` & `eggella-0.0.4/eggella/command/handler.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/command/objects.py` & `eggella-0.0.4/eggella/command/objects.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 import inspect
 from typing import Any, Callable, Dict, List, NamedTuple, Optional, Tuple
 
+from prompt_toolkit.completion.nested import NestedDict
+
 from eggella.command.abc import ABCCommandHandler
 from eggella.command.handler import CommandHandler
 
 
 class Command(NamedTuple):
     fn: Callable[..., Any]
     key: str
     handler: ABCCommandHandler = CommandHandler()
     usage: Optional[str] = None
     short_description: Optional[str] = None
+    nested_completions: Optional[NestedDict] = None
+    nested_meta: Dict[str, Any] = {}
 
     def handle(self, command_text: str) -> Tuple[Tuple[Any, ...], Dict[str, Any]]:
         args, kwargs = self.handler.handle(self.fn, command_text)
         return self.fn(*args, **kwargs)
 
     @property
     def arguments(self) -> List[str]:
@@ -23,21 +27,23 @@
 
     @property
     def docstring(self) -> str:
         return inspect.getdoc(self.fn) or ""
 
     @property
     def short_desc(self):
-        arg_list = " ".join(f"[{arg}]" for arg in self.arguments)
+        arg_list = ", ".join(f"{arg}" for arg in self.arguments)
         if self.short_description:
-            return f"({arg_list}) - {self.short_description}"
+            if arg_list:
+                return f"({arg_list}) - {self.short_description}"
+            return self.short_description
         elif self.docstring:
             short_desc = self.docstring.split("\n")[0]
-            return f"{arg_list} - {short_desc}"
-        return f"{arg_list}"
+            return f"({arg_list}) - {short_desc}" if arg_list else short_desc
+        return f"({arg_list})"
 
     @property
     def completion(self) -> Tuple[str, str]:
         return self.key, self.short_desc
 
     @property
     def help(self):
```

### Comparing `eggella-0.0.3/eggella/events/events.py` & `eggella-0.0.4/eggella/events/events.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/fsm/fsm.py` & `eggella-0.0.4/eggella/fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/shortcuts/cmd_shortcuts.py` & `eggella-0.0.4/eggella/shortcuts/cmd_shortcuts.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/shortcuts/help_pager.py` & `eggella-0.0.4/eggella/shortcuts/help_pager.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/eggella/tools/type_caster.py` & `eggella-0.0.4/eggella/tools/type_caster.py`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/.gitignore` & `eggella-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/README.md` & `eggella-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/pyproject.toml` & `eggella-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eggella-0.0.3/PKG-INFO` & `eggella-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eggella
-Version: 0.0.3
+Version: 0.0.4
 Summary: Create awesome command line applications with less effort
 Project-URL: Documentation, https://github.com/unknown/eggella#readme
 Project-URL: Issues, https://github.com/unknown/eggella/issues
 Project-URL: Source, https://github.com/unknown/eggella
 Author: georgiy
 License-Expression: MIT
 Classifier: Development Status :: 4 - Beta
```

