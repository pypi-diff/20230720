# Comparing `tmp/slash-slack-0.2.1.tar.gz` & `tmp/slash-slack-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slash-slack-0.2.1.tar", last modified: Thu Jul 20 20:58:01 2023, max compression
+gzip compressed data, was "slash-slack-0.2.2.tar", last modified: Thu Jul 20 21:23:37 2023, max compression
```

## Comparing `slash-slack-0.2.1.tar` & `slash-slack-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.214772 slash-slack-0.2.1/
--rw-r--r--   0 henryjones   (501) staff       (20)    35149 2023-07-20 20:35:07.000000 slash-slack-0.2.1/LICENSE
--rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-07-20 20:58:01.214528 slash-slack-0.2.1/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)     8873 2023-07-20 20:35:07.000000 slash-slack-0.2.1/README.md
--rw-r--r--   0 henryjones   (501) staff       (20)      890 2023-07-20 20:57:31.000000 slash-slack-0.2.1/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-07-20 20:58:01.214856 slash-slack-0.2.1/setup.cfg
--rw-r--r--   0 henryjones   (501) staff       (20)      253 2023-07-20 20:35:07.000000 slash-slack-0.2.1/setup.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.212773 slash-slack-0.2.1/slash_slack/
--rw-r--r--   0 henryjones   (501) staff       (20)      164 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1853 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/arg_functions.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5853 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/arg_types.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1823 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/blocks.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1050 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/exceptions.py
--rwxr-xr-x   0 henryjones   (501) staff       (20)     3709 2023-07-20 20:54:10.000000 slash-slack-0.2.1/slash_slack/mock_slack.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)     2573 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/signature_verifier.py
--rw-r--r--   0 henryjones   (501) staff       (20)    13334 2023-07-20 20:48:23.000000 slash-slack-0.2.1/slash_slack/slash_slack.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5477 2023-07-20 20:38:46.000000 slash-slack-0.2.1/slash_slack/slash_slack_command.py
--rw-r--r--   0 henryjones   (501) staff       (20)      468 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/slash_slack_request.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.213654 slash-slack-0.2.1/slash_slack.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      731 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       59 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       16 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       12 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/top_level.txt
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.214329 slash-slack-0.2.1/tests/
--rw-r--r--   0 henryjones   (501) staff       (20)     5247 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_arg_types.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     4120 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_parse_command_text.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     6827 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_parse_func_params.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1231 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_slash_slack.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5848 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_slash_slack_command.test.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 21:23:37.041106 slash-slack-0.2.2/
+-rw-r--r--   0 henryjones   (501) staff       (20)    35149 2023-07-20 20:35:07.000000 slash-slack-0.2.2/LICENSE
+-rw-r--r--   0 henryjones   (501) staff       (20)    10309 2023-07-20 21:23:37.040933 slash-slack-0.2.2/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)     9553 2023-07-20 21:21:38.000000 slash-slack-0.2.2/README.md
+-rw-r--r--   0 henryjones   (501) staff       (20)      890 2023-07-20 21:21:50.000000 slash-slack-0.2.2/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-07-20 21:23:37.041158 slash-slack-0.2.2/setup.cfg
+-rw-r--r--   0 henryjones   (501) staff       (20)      253 2023-07-20 20:35:07.000000 slash-slack-0.2.2/setup.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 21:23:37.038234 slash-slack-0.2.2/slash_slack/
+-rw-r--r--   0 henryjones   (501) staff       (20)      164 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1853 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/arg_functions.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5853 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/arg_types.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1823 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/blocks.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1050 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/exceptions.py
+-rwxr-xr-x   0 henryjones   (501) staff       (20)     3709 2023-07-20 20:54:10.000000 slash-slack-0.2.2/slash_slack/mock_slack.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)     2573 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/signature_verifier.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    13817 2023-07-20 21:22:24.000000 slash-slack-0.2.2/slash_slack/slash_slack.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5776 2023-07-20 21:22:12.000000 slash-slack-0.2.2/slash_slack/slash_slack_command.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      468 2023-07-20 20:35:07.000000 slash-slack-0.2.2/slash_slack/slash_slack_request.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 21:23:37.039420 slash-slack-0.2.2/slash_slack.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)    10309 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      731 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       59 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       16 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       12 2023-07-20 21:23:37.000000 slash-slack-0.2.2/slash_slack.egg-info/top_level.txt
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 21:23:37.040657 slash-slack-0.2.2/tests/
+-rw-r--r--   0 henryjones   (501) staff       (20)     5247 2023-07-20 20:35:07.000000 slash-slack-0.2.2/tests/test_arg_types.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     4120 2023-07-20 20:35:07.000000 slash-slack-0.2.2/tests/test_parse_command_text.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     6827 2023-07-20 20:35:07.000000 slash-slack-0.2.2/tests/test_parse_func_params.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1231 2023-07-20 20:35:07.000000 slash-slack-0.2.2/tests/test_slash_slack.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5848 2023-07-20 20:35:07.000000 slash-slack-0.2.2/tests/test_slash_slack_command.test.py
```

### Comparing `slash-slack-0.2.1/LICENSE` & `slash-slack-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/PKG-INFO` & `slash-slack-0.2.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slash-slack
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python framework for slack slash bots.
 Home-page: https://github.com/henryivesjones/slash-slack
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: slack,fastapi,bot,slash command
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -60,14 +60,21 @@
 ## Command Response Timeout/Async responses
 Slack requires that the slash bot webhook be responded to within 3 seconds.
 
 Often times the action being taken by the bot will depend on external services which might not respond within 3 seconds.
 
 `slash-slack` sends an immediate `200` response to the webhook request, and runs the command function in the background. When the command function finishes, the response is sent back to slack using the `response_url` from the request.
 
+You can optionally add content to the immediate response to let your user know that something is being
+done in the background. A global/default response can be set with the `acknowledge_response` parameter on
+the `SlashSlack` class, or at the command level with the `acknowledge_response` parameter on the `command` decorator.
+The value passed to `acknowledge_response` will be passed to `blocks._make_block_message` and can be a `str`, `block`, `list[str]`, or `list[block]`
+where a `block` is a [block kit block](https://api.slack.com/block-kit/building#getting_started).
+See the [example](https://github.com/henryivesjones/slash-slack/blob/main/example.py) for example usage.
+
 ## Input Arg/Flag parsing
 `slash-slack` takes care of parsing command input into pre-defined args and flags which let you focus on writing the command function, and not wrangling the content into the format that you need.
 
 ## Auto-generated help
 `slash-slack` provides help dialog auto-generated from your commands, args, and flags. Additional details can be embedded directly into the command decorator and arg/flag initializers.
 
 To request global help:
```

### Comparing `slash-slack-0.2.1/README.md` & `slash-slack-0.2.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -41,14 +41,21 @@
 ## Command Response Timeout/Async responses
 Slack requires that the slash bot webhook be responded to within 3 seconds.
 
 Often times the action being taken by the bot will depend on external services which might not respond within 3 seconds.
 
 `slash-slack` sends an immediate `200` response to the webhook request, and runs the command function in the background. When the command function finishes, the response is sent back to slack using the `response_url` from the request.
 
+You can optionally add content to the immediate response to let your user know that something is being
+done in the background. A global/default response can be set with the `acknowledge_response` parameter on
+the `SlashSlack` class, or at the command level with the `acknowledge_response` parameter on the `command` decorator.
+The value passed to `acknowledge_response` will be passed to `blocks._make_block_message` and can be a `str`, `block`, `list[str]`, or `list[block]`
+where a `block` is a [block kit block](https://api.slack.com/block-kit/building#getting_started).
+See the [example](https://github.com/henryivesjones/slash-slack/blob/main/example.py) for example usage.
+
 ## Input Arg/Flag parsing
 `slash-slack` takes care of parsing command input into pre-defined args and flags which let you focus on writing the command function, and not wrangling the content into the format that you need.
 
 ## Auto-generated help
 `slash-slack` provides help dialog auto-generated from your commands, args, and flags. Additional details can be embedded directly into the command decorator and arg/flag initializers.
 
 To request global help:
```

### Comparing `slash-slack-0.2.1/pyproject.toml` & `slash-slack-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slash-slack"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="Henry Jones", email="henryivesjones@gmail.com" },
 ]
 description = "A python framework for slack slash bots."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text="GPL-3.0-or-later"}
```

### Comparing `slash-slack-0.2.1/slash_slack/arg_functions.py` & `slash-slack-0.2.2/slash_slack/arg_functions.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/arg_types.py` & `slash-slack-0.2.2/slash_slack/arg_types.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/blocks.py` & `slash-slack-0.2.2/slash_slack/blocks.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/exceptions.py` & `slash-slack-0.2.2/slash_slack/exceptions.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/mock_slack.py` & `slash-slack-0.2.2/slash_slack/mock_slack.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/signature_verifier.py` & `slash-slack-0.2.2/slash_slack/signature_verifier.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/slash_slack/slash_slack.py` & `slash-slack-0.2.2/slash_slack/slash_slack.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import inspect
 import logging
 import re
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Set, Tuple, Union
 from urllib.parse import parse_qsl
 
-from fastapi import BackgroundTasks, FastAPI, HTTPException, Request
+from fastapi import BackgroundTasks, FastAPI, HTTPException, Request, Response
 from fastapi.responses import JSONResponse
 from pydantic import ValidationError
 
 from slash_slack.arg_types import (
     BaseArgType,
     FlagType,
     FloatType,
@@ -42,15 +42,15 @@
     description: str
     contact: Optional[str] = None
     app: FastAPI
     commands: Dict[str, SlashSlackCommand]
     dev: bool
     signature_verifier: SignatureVerifier
     before_request_functions: List[Callable]
-    acknowledge_response: Optional[dict]
+    acknowledge_response: Optional[dict] = None
 
     def __init__(
         self,
         dev: bool = False,
         signing_secret: Optional[str] = None,
         url_path: str = "/slash_slack",
         description: str = "",
@@ -66,15 +66,19 @@
         """
         self.url_path = url_path
         self.description = description
         self.app = FastAPI(title="SlashSlack", openapi_url=None)
         self.commands = {}
         self.dev = dev
         self.contact = contact
-        self.acknowledge_response = _make_block_message(acknowledge_response)
+        if acknowledge_response is not None:
+            self.acknowledge_response = _make_block_message(
+                acknowledge_response, visible_in_channel=False
+            )
+
         self.before_request_functions = []
 
         if self.dev:
             logger.info("Running in DEV MODE. Signature verification is disabled.")
         else:
             if signing_secret is None:
                 raise NoSigningSecretException(
@@ -97,15 +101,15 @@
                     raise HTTPException(
                         status_code=403,
                         detail="Unable to verify request signature.",
                     )
             try:
                 request_form_data = dict(parse_qsl(request_body.decode()))
                 if request_form_data.get("ssl_check") == 1:
-                    return self.make_success_acknowledge_response()
+                    return Response(status_code=200)
                 try:
                     slash_slack_request = SlashSlackRequest(**request_form_data)
                 except ValidationError as e:
                     logger.error(e)
                     raise HTTPException(
                         status_code=422, detail="Validation of request body failed."
                     )
@@ -143,25 +147,30 @@
                     self.commands[command].execute,
                     parsed_args,
                     flags.difference(self.global_flags),
                     global_flags,
                     slash_slack_request,
                 )
 
-                return self.make_success_acknowledge_response()
+                return self.make_success_acknowledge_response(command)
             except Exception as e:
                 logger.error(e)
                 return _make_block_message(
                     self._unable_to_respond(), visible_in_channel=False
                 )
 
-    def make_success_acknowledge_response(self):
+    def make_success_acknowledge_response(self, command: str):
         kwargs: dict = {"status_code": 200}
         if self.acknowledge_response is not None:
             kwargs["content"] = self.acknowledge_response
+        if (
+            command in self.commands
+            and self.commands[command].acknowledge_response is not None
+        ):
+            kwargs["content"] = self.commands[command].acknowledge_response
         return JSONResponse(**kwargs)
 
     def get_fast_api(self):
         """
         Get the underlying fast_api app which should be exported to be run by a wsgi worker (uvicorn).
         """
         return self.app
@@ -175,15 +184,19 @@
 
         This function should take one argument of the type `SlashSlackRequest` and return None.
 
         """
         self.before_request_functions.append(func)
 
     def command(
-        self, command: str, help: Optional[str] = None, summary: Optional[str] = None
+        self,
+        command: str,
+        help: Optional[str] = None,
+        summary: Optional[str] = None,
+        acknowledge_response: Union[None, str, dict] = None,
     ):
         """
         Decorator for defining a command within a SlashSlack app.
 
         command (str): The first word used for routing between commands within a SlashSlack app.
         help    (str): The help content for this command.
         summary (str): The summary/title for this command.
@@ -203,14 +216,15 @@
                 func=func,
                 flags=flags,
                 args_type=params,
                 request_arg=request_arg,
                 help=help,
                 summary=summary,
                 is_async=is_async,
+                acknowledge_response=acknowledge_response,
             )
             return func
 
         return decorator_command
 
     def _global_help(
         self, slash_slack_request: SlashSlackRequest, visible_in_channel: bool = False
```

### Comparing `slash-slack-0.2.1/slash_slack/slash_slack_command.py` & `slash-slack-0.2.2/slash_slack/slash_slack_command.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import logging
-from typing import Any, Callable, List, Optional, Set, Tuple
+from typing import Any, Callable, List, Optional, Set, Tuple, Union
 
 import aiohttp
 
 from slash_slack.arg_types import (
     BaseArgType,
     FlagType,
     StringType,
@@ -26,34 +26,40 @@
     help: Optional[str] = None
     summary: Optional[str] = None
     func: Callable
     flags: List[Tuple[str, FlagType, int]]
     args_type: List[Tuple[str, BaseArgType, int]]
     request_arg: Optional[Tuple[str, int]] = None
     is_async: bool
+    acknowledge_response: Optional[dict] = None
 
     def __init__(
         self,
         command: str,
         func: Callable,
         flags: List[Tuple[str, FlagType, int]],
         args_type: List[Tuple[str, BaseArgType, int]],
         request_arg: Optional[Tuple[str, int]],
         help: Optional[str] = None,
         summary: Optional[str] = None,
         is_async: bool = False,
+        acknowledge_response: Union[None, str, dict] = None,
     ):
         self.command = command
         self.func = func
         self.flags = flags
         self.args_type = args_type
         self.request_arg = request_arg
         self.help = help
         self.summary = summary
         self.is_async = is_async
+        if acknowledge_response is not None:
+            self.acknowledge_response = _make_block_message(
+                acknowledge_response, visible_in_channel=False
+            )
 
     def parse_args(self, args: str):
         """
         Parse input text for this command utilizing this commands flag and arg schema.
         """
         if len(self.args_type) == 1 and isinstance(self.args_type[0][1], StringType):
             p = self.args_type[0][1].parse(args)
```

### Comparing `slash-slack-0.2.1/slash_slack.egg-info/PKG-INFO` & `slash-slack-0.2.2/slash_slack.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slash-slack
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python framework for slack slash bots.
 Home-page: https://github.com/henryivesjones/slash-slack
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: slack,fastapi,bot,slash command
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
@@ -60,14 +60,21 @@
 ## Command Response Timeout/Async responses
 Slack requires that the slash bot webhook be responded to within 3 seconds.
 
 Often times the action being taken by the bot will depend on external services which might not respond within 3 seconds.
 
 `slash-slack` sends an immediate `200` response to the webhook request, and runs the command function in the background. When the command function finishes, the response is sent back to slack using the `response_url` from the request.
 
+You can optionally add content to the immediate response to let your user know that something is being
+done in the background. A global/default response can be set with the `acknowledge_response` parameter on
+the `SlashSlack` class, or at the command level with the `acknowledge_response` parameter on the `command` decorator.
+The value passed to `acknowledge_response` will be passed to `blocks._make_block_message` and can be a `str`, `block`, `list[str]`, or `list[block]`
+where a `block` is a [block kit block](https://api.slack.com/block-kit/building#getting_started).
+See the [example](https://github.com/henryivesjones/slash-slack/blob/main/example.py) for example usage.
+
 ## Input Arg/Flag parsing
 `slash-slack` takes care of parsing command input into pre-defined args and flags which let you focus on writing the command function, and not wrangling the content into the format that you need.
 
 ## Auto-generated help
 `slash-slack` provides help dialog auto-generated from your commands, args, and flags. Additional details can be embedded directly into the command decorator and arg/flag initializers.
 
 To request global help:
```

### Comparing `slash-slack-0.2.1/slash_slack.egg-info/SOURCES.txt` & `slash-slack-0.2.2/slash_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/tests/test_arg_types.test.py` & `slash-slack-0.2.2/tests/test_arg_types.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/tests/test_parse_command_text.test.py` & `slash-slack-0.2.2/tests/test_parse_command_text.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/tests/test_parse_func_params.test.py` & `slash-slack-0.2.2/tests/test_parse_func_params.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/tests/test_slash_slack.test.py` & `slash-slack-0.2.2/tests/test_slash_slack.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.2.1/tests/test_slash_slack_command.test.py` & `slash-slack-0.2.2/tests/test_slash_slack_command.test.py`

 * *Files identical despite different names*

