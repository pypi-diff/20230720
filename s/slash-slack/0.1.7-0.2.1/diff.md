# Comparing `tmp/slash-slack-0.1.7.tar.gz` & `tmp/slash-slack-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "slash-slack-0.1.7.tar", last modified: Wed Mar  8 19:37:37 2023, max compression
+gzip compressed data, was "slash-slack-0.2.1.tar", last modified: Thu Jul 20 20:58:01 2023, max compression
```

## Comparing `slash-slack-0.1.7.tar` & `slash-slack-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-08 19:37:37.949305 slash-slack-0.1.7/
--rw-r--r--   0 henryjones   (501) staff       (20)    35149 2023-03-08 16:32:42.000000 slash-slack-0.1.7/LICENSE
--rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-03-08 19:37:37.949036 slash-slack-0.1.7/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)     8873 2023-03-08 16:32:44.000000 slash-slack-0.1.7/README.md
--rw-r--r--   0 henryjones   (501) staff       (20)      890 2023-03-08 19:37:12.000000 slash-slack-0.1.7/pyproject.toml
--rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-03-08 19:37:37.949398 slash-slack-0.1.7/setup.cfg
--rw-r--r--   0 henryjones   (501) staff       (20)      253 2023-03-08 16:32:44.000000 slash-slack-0.1.7/setup.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-08 19:37:37.945192 slash-slack-0.1.7/slash_slack/
--rw-r--r--   0 henryjones   (501) staff       (20)      164 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/__init__.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1853 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/arg_functions.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5853 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/arg_types.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1823 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/blocks.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1050 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/exceptions.py
--rwxr-xr-x   0 henryjones   (501) staff       (20)     3709 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/mock_slack.py
--rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/py.typed
--rw-r--r--   0 henryjones   (501) staff       (20)     2573 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/signature_verifier.py
--rw-r--r--   0 henryjones   (501) staff       (20)    12568 2023-03-08 19:36:49.000000 slash-slack-0.1.7/slash_slack/slash_slack.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5435 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/slash_slack_command.py
--rw-r--r--   0 henryjones   (501) staff       (20)      468 2023-03-08 16:32:44.000000 slash-slack-0.1.7/slash_slack/slash_slack_request.py
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-08 19:37:37.947062 slash-slack-0.1.7/slash_slack.egg-info/
--rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/PKG-INFO
--rw-r--r--   0 henryjones   (501) staff       (20)      731 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/SOURCES.txt
--rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/dependency_links.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       59 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/entry_points.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       16 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/requires.txt
--rw-r--r--   0 henryjones   (501) staff       (20)       12 2023-03-08 19:37:37.000000 slash-slack-0.1.7/slash_slack.egg-info/top_level.txt
-drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-03-08 19:37:37.948637 slash-slack-0.1.7/tests/
--rw-r--r--   0 henryjones   (501) staff       (20)     5247 2023-03-08 16:32:44.000000 slash-slack-0.1.7/tests/test_arg_types.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     4120 2023-03-08 16:32:44.000000 slash-slack-0.1.7/tests/test_parse_command_text.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     6827 2023-03-08 16:32:44.000000 slash-slack-0.1.7/tests/test_parse_func_params.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     1231 2023-03-08 16:32:44.000000 slash-slack-0.1.7/tests/test_slash_slack.test.py
--rw-r--r--   0 henryjones   (501) staff       (20)     5848 2023-03-08 16:32:44.000000 slash-slack-0.1.7/tests/test_slash_slack_command.test.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.214772 slash-slack-0.2.1/
+-rw-r--r--   0 henryjones   (501) staff       (20)    35149 2023-07-20 20:35:07.000000 slash-slack-0.2.1/LICENSE
+-rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-07-20 20:58:01.214528 slash-slack-0.2.1/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)     8873 2023-07-20 20:35:07.000000 slash-slack-0.2.1/README.md
+-rw-r--r--   0 henryjones   (501) staff       (20)      890 2023-07-20 20:57:31.000000 slash-slack-0.2.1/pyproject.toml
+-rw-r--r--   0 henryjones   (501) staff       (20)       38 2023-07-20 20:58:01.214856 slash-slack-0.2.1/setup.cfg
+-rw-r--r--   0 henryjones   (501) staff       (20)      253 2023-07-20 20:35:07.000000 slash-slack-0.2.1/setup.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.212773 slash-slack-0.2.1/slash_slack/
+-rw-r--r--   0 henryjones   (501) staff       (20)      164 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/__init__.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1853 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/arg_functions.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5853 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/arg_types.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1823 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/blocks.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1050 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/exceptions.py
+-rwxr-xr-x   0 henryjones   (501) staff       (20)     3709 2023-07-20 20:54:10.000000 slash-slack-0.2.1/slash_slack/mock_slack.py
+-rw-r--r--   0 henryjones   (501) staff       (20)        0 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/py.typed
+-rw-r--r--   0 henryjones   (501) staff       (20)     2573 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/signature_verifier.py
+-rw-r--r--   0 henryjones   (501) staff       (20)    13334 2023-07-20 20:48:23.000000 slash-slack-0.2.1/slash_slack/slash_slack.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5477 2023-07-20 20:38:46.000000 slash-slack-0.2.1/slash_slack/slash_slack_command.py
+-rw-r--r--   0 henryjones   (501) staff       (20)      468 2023-07-20 20:35:07.000000 slash-slack-0.2.1/slash_slack/slash_slack_request.py
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.213654 slash-slack-0.2.1/slash_slack.egg-info/
+-rw-r--r--   0 henryjones   (501) staff       (20)     9629 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/PKG-INFO
+-rw-r--r--   0 henryjones   (501) staff       (20)      731 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)        1 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       59 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/entry_points.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       16 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/requires.txt
+-rw-r--r--   0 henryjones   (501) staff       (20)       12 2023-07-20 20:58:01.000000 slash-slack-0.2.1/slash_slack.egg-info/top_level.txt
+drwxr-xr-x   0 henryjones   (501) staff       (20)        0 2023-07-20 20:58:01.214329 slash-slack-0.2.1/tests/
+-rw-r--r--   0 henryjones   (501) staff       (20)     5247 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_arg_types.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     4120 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_parse_command_text.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     6827 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_parse_func_params.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     1231 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_slash_slack.test.py
+-rw-r--r--   0 henryjones   (501) staff       (20)     5848 2023-07-20 20:35:07.000000 slash-slack-0.2.1/tests/test_slash_slack_command.test.py
```

### Comparing `slash-slack-0.1.7/LICENSE` & `slash-slack-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/PKG-INFO` & `slash-slack-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slash-slack
-Version: 0.1.7
+Version: 0.2.1
 Summary: A python framework for slack slash bots.
 Home-page: https://github.com/henryivesjones/slash-slack
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: slack,fastapi,bot,slash command
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `slash-slack-0.1.7/README.md` & `slash-slack-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/pyproject.toml` & `slash-slack-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "slash-slack"
-version = "0.1.7"
+version = "0.2.1"
 authors = [
   { name="Henry Jones", email="henryivesjones@gmail.com" },
 ]
 description = "A python framework for slack slash bots."
 readme = "README.md"
 requires-python = ">=3.6"
 license = {text="GPL-3.0-or-later"}
```

### Comparing `slash-slack-0.1.7/slash_slack/arg_functions.py` & `slash-slack-0.2.1/slash_slack/arg_functions.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/arg_types.py` & `slash-slack-0.2.1/slash_slack/arg_types.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/blocks.py` & `slash-slack-0.2.1/slash_slack/blocks.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/exceptions.py` & `slash-slack-0.2.1/slash_slack/exceptions.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/mock_slack.py` & `slash-slack-0.2.1/slash_slack/mock_slack.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/signature_verifier.py` & `slash-slack-0.2.1/slash_slack/signature_verifier.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/slash_slack/slash_slack.py` & `slash-slack-0.2.1/slash_slack/slash_slack.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 import logging
 import re
 from typing import Any, Callable, Coroutine, Dict, List, Optional, Set, Tuple, Union
 from urllib.parse import parse_qsl
 
-from fastapi import BackgroundTasks, FastAPI, HTTPException, Request, Response
+from fastapi import BackgroundTasks, FastAPI, HTTPException, Request
+from fastapi.responses import JSONResponse
 from pydantic import ValidationError
 
 from slash_slack.arg_types import (
     BaseArgType,
     FlagType,
     FloatType,
     IntType,
@@ -24,14 +25,16 @@
     NoSigningSecretException,
     ParamAfterUnknownLengthListException,
 )
 from slash_slack.signature_verifier import SignatureVerifier
 from slash_slack.slash_slack_command import SlashSlackCommand
 from slash_slack.slash_slack_request import SlashSlackRequest
 
+logger = logging.getLogger("slash_slack")
+
 
 class SlashSlack:
     """
     A framework for building python response servers for Slack slash bot.
     """
 
     global_flags = {"visible", "help"}
@@ -39,37 +42,43 @@
     description: str
     contact: Optional[str] = None
     app: FastAPI
     commands: Dict[str, SlashSlackCommand]
     dev: bool
     signature_verifier: SignatureVerifier
     before_request_functions: List[Callable]
+    acknowledge_response: Optional[dict]
 
     def __init__(
         self,
         dev: bool = False,
         signing_secret: Optional[str] = None,
-        url_path="/slash_slack",
-        description="",
-        contact=None,
+        url_path: str = "/slash_slack",
+        description: str = "",
+        contact: Optional[str] = None,
+        acknowledge_response: Union[None, str, dict] = None,
     ):
         """
         Create a Slash Slack app.
         To disable signature verification set dev=True
+
+        To respond to the initial request with a non-blank response pass in a value for `acknowledge_response`
+        The value will be passed into `blocks._make_block_message` and should be formatted as such.
         """
         self.url_path = url_path
         self.description = description
         self.app = FastAPI(title="SlashSlack", openapi_url=None)
         self.commands = {}
         self.dev = dev
         self.contact = contact
+        self.acknowledge_response = _make_block_message(acknowledge_response)
         self.before_request_functions = []
 
         if self.dev:
-            logging.info("Running in DEV MODE. Signature verification is disabled.")
+            logger.info("Running in DEV MODE. Signature verification is disabled.")
         else:
             if signing_secret is None:
                 raise NoSigningSecretException(
                     "No signing secret provided. Either disable signature verification by running in dev mode, or provide the signing secret."
                 )
             self.signature_verifier = SignatureVerifier(signing_secret)
 
@@ -88,19 +97,19 @@
                     raise HTTPException(
                         status_code=403,
                         detail="Unable to verify request signature.",
                     )
             try:
                 request_form_data = dict(parse_qsl(request_body.decode()))
                 if request_form_data.get("ssl_check") == 1:
-                    return Response(status_code=200)
+                    return self.make_success_acknowledge_response()
                 try:
                     slash_slack_request = SlashSlackRequest(**request_form_data)
                 except ValidationError as e:
-                    logging.error(e)
+                    logger.error(e)
                     raise HTTPException(
                         status_code=422, detail="Validation of request body failed."
                     )
                 for fn in self.before_request_functions:
                     background_tasks.add_task(fn, slash_slack_request)
                 command, args, flags = _parse_command_text(
                     slash_slack_request.text.strip()
@@ -134,21 +143,27 @@
                     self.commands[command].execute,
                     parsed_args,
                     flags.difference(self.global_flags),
                     global_flags,
                     slash_slack_request,
                 )
 
-                return Response(status_code=200)
+                return self.make_success_acknowledge_response()
             except Exception as e:
-                logging.error(e)
+                logger.error(e)
                 return _make_block_message(
                     self._unable_to_respond(), visible_in_channel=False
                 )
 
+    def make_success_acknowledge_response(self):
+        kwargs: dict = {"status_code": 200}
+        if self.acknowledge_response is not None:
+            kwargs["content"] = self.acknowledge_response
+        return JSONResponse(**kwargs)
+
     def get_fast_api(self):
         """
         Get the underlying fast_api app which should be exported to be run by a wsgi worker (uvicorn).
         """
         return self.app
 
     def add_before_request_function(
```

### Comparing `slash-slack-0.1.7/slash_slack/slash_slack_command.py` & `slash-slack-0.2.1/slash_slack/slash_slack_command.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     UnknownLengthListType,
 )
 from slash_slack.blocks import _make_block_message
 from slash_slack.slash_slack_request import SlashSlackRequest
 
 _NL = "\n"
 
+logger = logging.getLogger("slash_slack")
+
 
 class SlashSlackCommand:
     """
     Abstraction for running command functions. Input parsing, command execution, and command help live here.
     """
 
     command: str
@@ -112,15 +114,15 @@
             async with session.post(
                 slash_slack_request.response_url,
                 json=_make_block_message(
                     response, visible_in_channel="visible" in global_flags
                 ),
             ) as resp:
                 if resp.status != 200:
-                    logging.error(
+                    logger.error(
                         f"Received an error when sending request to callback ({resp.status}): {await resp.text()}"
                     )
 
     def _help(
         self, slash_slack_request: SlashSlackRequest, visible_in_channel: bool = False
     ):
         """
```

### Comparing `slash-slack-0.1.7/slash_slack.egg-info/PKG-INFO` & `slash-slack-0.2.1/slash_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: slash-slack
-Version: 0.1.7
+Version: 0.2.1
 Summary: A python framework for slack slash bots.
 Home-page: https://github.com/henryivesjones/slash-slack
 Author-email: Henry Jones <henryivesjones@gmail.com>
 License: GPL-3.0-or-later
 Keywords: slack,fastapi,bot,slash command
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
```

### Comparing `slash-slack-0.1.7/slash_slack.egg-info/SOURCES.txt` & `slash-slack-0.2.1/slash_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/tests/test_arg_types.test.py` & `slash-slack-0.2.1/tests/test_arg_types.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/tests/test_parse_command_text.test.py` & `slash-slack-0.2.1/tests/test_parse_command_text.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/tests/test_parse_func_params.test.py` & `slash-slack-0.2.1/tests/test_parse_func_params.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/tests/test_slash_slack.test.py` & `slash-slack-0.2.1/tests/test_slash_slack.test.py`

 * *Files identical despite different names*

### Comparing `slash-slack-0.1.7/tests/test_slash_slack_command.test.py` & `slash-slack-0.2.1/tests/test_slash_slack_command.test.py`

 * *Files identical despite different names*

