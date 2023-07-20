# Comparing `tmp/herta_villa_sdk-0.7.0.tar.gz` & `tmp/herta_villa_sdk-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.7.0.tar", last modified: Thu Jul 20 08:28:02 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.8.0.tar", last modified: Thu Jul 20 12:20:02 2023, max compression
```

## Comparing `herta_villa_sdk-0.7.0.tar` & `herta_villa_sdk-0.8.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     1068 2023-07-20 08:27:23.075545 herta_villa_sdk-0.7.0/LICENSE
--rw-r--r--   0        0        0     4548 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/README.md
--rw-r--r--   0        0        0      850 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0     1485 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/audit.py
--rw-r--r--   0        0        0      782 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1739 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0      701 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/img.py
--rw-r--r--   0        0        0     2174 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2693 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4405 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     8820 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/bot.py
--rw-r--r--   0        0        0     6282 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/event.py
--rw-r--r--   0        0        0     1952 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     5141 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1398 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/model.py
--rw-r--r--   0        0        0      928 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/__init__.py
--rw-r--r--   0        0        0      788 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/_lifespan.py
--rw-r--r--   0        0        0     1977 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/aiohttp.py
--rw-r--r--   0        0        0     2342 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/fastapi.py
--rw-r--r--   0        0        0     3333 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/internal.py
--rw-r--r--   0        0        0      564 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-20 08:27:23.191552 herta_villa_sdk-0.7.0/hertavilla/version.py
--rw-r--r--   0        0        0     2292 2023-07-20 08:28:02.046027 herta_villa_sdk-0.7.0/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-20 08:27:23.083545 herta_villa_sdk-0.7.0/tests/test_utils.py
--rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 herta_villa_sdk-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/LICENSE
+-rw-r--r--   0        0        0     4548 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/README.md
+-rw-r--r--   0        0        0     1023 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0     1485 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/audit.py
+-rw-r--r--   0        0        0      782 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1739 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0      701 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/img.py
+-rw-r--r--   0        0        0     2174 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2693 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4405 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-20 12:19:30.798672 herta_villa_sdk-0.8.0/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     9836 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     6282 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/event.py
+-rw-r--r--   0        0        0     1952 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     3271 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     5141 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1398 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/model.py
+-rw-r--r--   0        0        0      928 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0      788 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/server/_lifespan.py
+-rw-r--r--   0        0        0     1977 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     2342 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     3333 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      564 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-20 12:19:30.882672 herta_villa_sdk-0.8.0/hertavilla/version.py
+-rw-r--r--   0        0        0     2292 2023-07-20 12:20:02.958901 herta_villa_sdk-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-20 12:19:30.802672 herta_villa_sdk-0.8.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 herta_villa_sdk-0.8.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.7.0/LICENSE` & `herta_villa_sdk-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/README.md` & `herta_villa_sdk-0.8.0/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ```
 
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
-from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
+from hertavilla import MessageChain, SendMessageEvent, VillaBot, run, StartswithResult
 from hertavilla.server import init_backend
 
 
 PUB_KEY = """-----BEGIN PUBLIC KEY-----
 aaa
 bbb
 ccc
@@ -49,19 +49,17 @@
     "bot_secret",  # 这里填写 secret
     "/",  # bot 回调 endpoint
     PUB_KEY,  # 开放平台提供的 pub_key
 )
 
 
 @bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
-async def _(event: SendMessageEvent, bot: VillaBot):
-    message = event.message
-    if str(message[1]) == "/hello":
-        chain = MessageChain()
-        chain.append("world")
+async def _(event: SendMessageEvent, bot: VillaBot, match_result: StartswithResult):
+    if match_result.text == "hello":
+        chain = MessageChain("world")
         await bot.send(event.villa_id, event.room_id, chain)
 
 
 init_backend()  # 初始化后端
 run(bot)  # 运行 bot
 ```
```

### Comparing `herta_villa_sdk-0.7.0/hertavilla/__init__.py` & `herta_villa_sdk-0.8.0/hertavilla/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,14 +6,20 @@
     AuditCallbackEvent as AuditCallbackEvent,
     CreateRobotEvent as CreateRobotEvent,
     DeleteRobotEvent as DeleteRobotEvent,
     Event as Event,
     JoinVillaEvent as JoinVillaEvent,
     SendMessageEvent as SendMessageEvent,
 )
+from .match import (
+    EndswithResult as EndswithResult,
+    KeywordsResult as KeywordsResult,
+    RegexResult as RegexResult,
+    StartswithResult as StartswithResult,
+)
 from .message import (
     Image as Image,
     Link as Link,
     MentionedAll as MentionedAll,
     MentionedRobot as MentionedRobot,
     MentionedUser as MentionedUser,
     MessageChain as MessageChain,
```

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/audit.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/audit.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/auth.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/auth.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/base.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/base.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/emoticon.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/img.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/img.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/member.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/member.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/message.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/message.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/role.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/role.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/room.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/room.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/apis/villa.py` & `herta_villa_sdk-0.8.0/hertavilla/apis/villa.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/bot.py` & `herta_villa_sdk-0.8.0/hertavilla/bot.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,44 +4,53 @@
 import base64
 from dataclasses import dataclass
 import logging
 import re
 from typing import (
     TYPE_CHECKING,
     Any,
+    Awaitable,
     Callable,
     Coroutine,
     Generic,
-    NamedTuple,
     TypeVar,
 )
 import urllib.parse
 
 from hertavilla.apis.auth import AuthAPIMixin
 from hertavilla.apis.img import ImgAPIMixin
 from hertavilla.apis.member import MemberAPIMixin
 from hertavilla.apis.message import MessageAPIMixin
 from hertavilla.apis.role import RoleAPIMixin
 from hertavilla.apis.room import RoomAPIMixin
 from hertavilla.apis.villa import VillaAPIMixin
-from hertavilla.match import Endswith, Keywords, Match, Regex, Startswith
+from hertavilla.match import (
+    Endswith,
+    EndswithResult,
+    Keywords,
+    KeywordsResult,
+    Match,
+    MatchResult,
+    Regex,
+    RegexResult,
+    Startswith,
+    StartswithResult,
+    current_match_result,
+)
 
 import rsa
 
 if TYPE_CHECKING:
     from hertavilla.event import Command, Event, SendMessageEvent, Template
     from hertavilla.message import MessageChain
 
 
 TE = TypeVar("TE", bound="Event")
+TR = TypeVar("TR", bound="MatchResult")
 
-MessageHandlerFunc = Callable[
-    ["SendMessageEvent", "VillaBot"],
-    Coroutine[Any, Any, None],
-]
 
 logger = logging.getLogger("hertavilla.bot")
 
 
 @dataclass
 class Handler(Generic[TE]):
     event: type[TE]
@@ -51,26 +60,48 @@
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def __eq__(self, __value: Event) -> bool:
         return isinstance(__value, self.event)
 
 
-class MessageHandler(NamedTuple):
+@dataclass
+class MessageHandler(Generic[TR]):
     match: Match
-    func: Callable[["SendMessageEvent", VillaBot], Coroutine[Any, Any, None]]
+    func: Callable[["SendMessageEvent", "VillaBot", TR], Awaitable[Any]]
     temp: bool = False
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def check(self, chain: MessageChain) -> bool:
         return self.match.check(chain)
 
 
+RegexHandlerFunc = Callable[
+    ["SendMessageEvent", "VillaBot", RegexResult],
+    Awaitable[Any],
+]
+
+StartswithHandlerFunc = Callable[
+    ["SendMessageEvent", "VillaBot", StartswithResult],
+    Awaitable[Any],
+]
+
+EndswithHandlerFunc = Callable[
+    ["SendMessageEvent", "VillaBot", EndswithResult],
+    Awaitable[Any],
+]
+
+KeywordsHandlerFunc = Callable[
+    ["SendMessageEvent", "VillaBot", KeywordsResult],
+    Awaitable[Any],
+]
+
+
 class VillaBot(
     AuthAPIMixin,
     MemberAPIMixin,
     MessageAPIMixin,
     RoomAPIMixin,
     VillaAPIMixin,
     RoleAPIMixin,
@@ -222,95 +253,110 @@
         for handler in need_remove_handlers:
             self.handlers.remove(handler)
             logger.debug(f"Removed handler for {event.__class__.__name__}")
 
     # message handle
     @staticmethod
     async def message_handler(event: "SendMessageEvent", bot: "VillaBot"):
-        handlers = list(
-            filter(
-                lambda x: x.check(event.message),
-                bot.message_handlers,
-            ),
+        await asyncio.gather(
+            *[
+                bot._run_message_handler(event, bot, handler)  # noqa: SLF001
+                for handler in bot.message_handlers
+            ],
         )
-        need_remove_handlers = filter(lambda x: x.temp, handlers)
-        await asyncio.gather(*[handler(event, bot) for handler in handlers])
-        for handler in need_remove_handlers:
+
+    @staticmethod
+    async def _run_message_handler(
+        event: "SendMessageEvent",
+        bot: "VillaBot",
+        handler: MessageHandler,
+    ):
+        if not handler.check(event.message):
+            return
+        result = current_match_result.get()
+        await handler(event, bot, result)
+        if handler.temp:
             bot.message_handlers.remove(handler)
             logger.debug(f"Removed message handler with {handler.match}")
 
     def register_msg_handler(
         self,
         match: Match,
-        func: MessageHandlerFunc,
+        func: Callable[["SendMessageEvent", "VillaBot", TR], Awaitable[Any]],
         temp: bool = False,
     ):
-        self.message_handlers.append(MessageHandler(match, func, temp))
+        self.message_handlers.append(MessageHandler[TR](match, func, temp))
         logger.info(
             f"Registered the handler {func} with {match} (temp: {temp})",
         )
         return func
 
     def match(
         self,
         match: Match,
         temp: bool = False,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+    ) -> Callable[
+        [Callable[["SendMessageEvent", "VillaBot", TR], Awaitable[Any]]],
+        Callable[["SendMessageEvent", "VillaBot", TR], Awaitable[Any]],
+    ]:
         def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
+            func: Callable[
+                ["SendMessageEvent", "VillaBot", TR],
+                Awaitable[Any],
+            ],
+        ) -> Callable[["SendMessageEvent", "VillaBot", TR], Awaitable[Any]]:
             self.register_msg_handler(match, func, temp)
             return func
 
         return wrapper
 
     def regex(
         self,
         pattern: str | re.Pattern,
         temp: bool = False,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+    ) -> Callable[[RegexHandlerFunc], RegexHandlerFunc]:
         def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
+            func: RegexHandlerFunc,
+        ) -> RegexHandlerFunc:
             self.register_msg_handler(Regex(pattern), func, temp)
             return func
 
         return wrapper
 
     def startswith(
         self,
         prefix: str,
         temp: bool = False,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+    ) -> Callable[[StartswithHandlerFunc], StartswithHandlerFunc]:
         def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
+            func: StartswithHandlerFunc,
+        ) -> StartswithHandlerFunc:
             self.register_msg_handler(Startswith(prefix), func, temp)
             return func
 
         return wrapper
 
     def endswith(
         self,
         suffix: str,
         temp: bool = False,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+    ) -> Callable[[EndswithHandlerFunc], EndswithHandlerFunc]:
         def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
+            func: EndswithHandlerFunc,
+        ) -> EndswithHandlerFunc:
             self.register_msg_handler(Endswith(suffix), func, temp)
             return func
 
         return wrapper
 
     def keyword(
         self,
         *keywords: str,
         temp: bool = False,
-    ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
+    ) -> Callable[[KeywordsHandlerFunc], KeywordsHandlerFunc]:
         def wrapper(
-            func: MessageHandlerFunc,
-        ) -> MessageHandlerFunc:
+            func: KeywordsHandlerFunc,
+        ) -> KeywordsHandlerFunc:
             self.register_msg_handler(Keywords(*keywords), func, temp)
             return func
 
         return wrapper
```

### Comparing `herta_villa_sdk-0.7.0/hertavilla/event.py` & `herta_villa_sdk-0.8.0/hertavilla/event.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/exception.py` & `herta_villa_sdk-0.8.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/message/chain.py` & `herta_villa_sdk-0.8.0/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/message/image.py` & `herta_villa_sdk-0.8.0/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/message/post.py` & `herta_villa_sdk-0.8.0/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/message/text.py` & `herta_villa_sdk-0.8.0/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/model.py` & `herta_villa_sdk-0.8.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/server/__init__.py` & `herta_villa_sdk-0.8.0/hertavilla/server/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/server/_lifespan.py` & `herta_villa_sdk-0.8.0/hertavilla/server/_lifespan.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/server/aiohttp.py` & `herta_villa_sdk-0.8.0/hertavilla/server/aiohttp.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/server/fastapi.py` & `herta_villa_sdk-0.8.0/hertavilla/server/fastapi.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/server/internal.py` & `herta_villa_sdk-0.8.0/hertavilla/server/internal.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/typing.py` & `herta_villa_sdk-0.8.0/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/hertavilla/utils.py` & `herta_villa_sdk-0.8.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/pyproject.toml` & `herta_villa_sdk-0.8.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 keywords = [
     "mihoyo",
     "miyoushe",
     "bot",
     "villa",
 ]
 dynamic = []
-version = "0.7.0"
+version = "0.8.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Herta-villa/Herta-villa-SDK"
 Documentation = "https://github.com/Herta-villa/Herta-villa-SDK"
```

### Comparing `herta_villa_sdk-0.7.0/tests/test_utils.py` & `herta_villa_sdk-0.8.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.7.0/PKG-INFO` & `herta_villa_sdk-0.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.7.0
+Version: 0.8.0
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
@@ -46,15 +46,15 @@
 ```
 
 ## 快速开始
 
 你需要拥有一个[大别野](https://dby.miyoushe.com/chat)机器人。可前往大别野[「机器人开发者社区」](https://dby.miyoushe.com/chat/463/20020)（`OpenVilla`）申请。
 
 ```python
-from hertavilla import MessageChain, SendMessageEvent, VillaBot, run
+from hertavilla import MessageChain, SendMessageEvent, VillaBot, run, StartswithResult
 from hertavilla.server import init_backend
 
 
 PUB_KEY = """-----BEGIN PUBLIC KEY-----
 aaa
 bbb
 ccc
@@ -69,19 +69,17 @@
     "bot_secret",  # 这里填写 secret
     "/",  # bot 回调 endpoint
     PUB_KEY,  # 开放平台提供的 pub_key
 )
 
 
 @bot.startswith("/")  # 注册一个消息匹配器，匹配前缀为 / 的消息
-async def _(event: SendMessageEvent, bot: VillaBot):
-    message = event.message
-    if str(message[1]) == "/hello":
-        chain = MessageChain()
-        chain.append("world")
+async def _(event: SendMessageEvent, bot: VillaBot, match_result: StartswithResult):
+    if match_result.text == "hello":
+        chain = MessageChain("world")
         await bot.send(event.villa_id, event.room_id, chain)
 
 
 init_backend()  # 初始化后端
 run(bot)  # 运行 bot
 ```
```

