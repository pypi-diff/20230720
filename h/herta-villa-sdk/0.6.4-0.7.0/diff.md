# Comparing `tmp/herta_villa_sdk-0.6.4.tar.gz` & `tmp/herta_villa_sdk-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "herta_villa_sdk-0.6.4.tar", last modified: Thu Jul 20 06:54:46 2023, max compression
+gzip compressed data, was "herta_villa_sdk-0.7.0.tar", last modified: Thu Jul 20 08:28:02 2023, max compression
```

## Comparing `herta_villa_sdk-0.6.4.tar` & `herta_villa_sdk-0.7.0.tar`

### file list

```diff
@@ -1,35 +1,36 @@
--rw-r--r--   0        0        0     1068 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/LICENSE
--rw-r--r--   0        0        0     4497 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/README.md
--rw-r--r--   0        0        0      668 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/__init__.py
--rw-r--r--   0        0        0        0 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/__init__.py
--rw-r--r--   0        0        0      782 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/auth.py
--rw-r--r--   0        0        0     1739 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/base.py
--rw-r--r--   0        0        0      520 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/emoticon.py
--rw-r--r--   0        0        0      701 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/img.py
--rw-r--r--   0        0        0     2174 2023-07-20 06:54:07.133764 herta_villa_sdk-0.6.4/hertavilla/apis/member.py
--rw-r--r--   0        0        0     2693 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/apis/message.py
--rw-r--r--   0        0        0     4405 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/apis/role.py
--rw-r--r--   0        0        0     4190 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/apis/room.py
--rw-r--r--   0        0        0      645 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/apis/villa.py
--rw-r--r--   0        0        0     7869 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/bot.py
--rw-r--r--   0        0        0     5398 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/event.py
--rw-r--r--   0        0        0     1952 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/exception.py
--rw-r--r--   0        0        0     1481 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/match.py
--rw-r--r--   0        0        0      353 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/__init__.py
--rw-r--r--   0        0        0     5141 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/chain.py
--rw-r--r--   0        0        0     1398 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/image.py
--rw-r--r--   0        0        0      927 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/post.py
--rw-r--r--   0        0        0     6289 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/text.py
--rw-r--r--   0        0        0      442 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/message/types.py
--rw-r--r--   0        0        0     6280 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/model.py
--rw-r--r--   0        0        0      928 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/server/__init__.py
--rw-r--r--   0        0        0      788 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/server/_lifespan.py
--rw-r--r--   0        0        0     1977 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/server/aiohttp.py
--rw-r--r--   0        0        0     2342 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/server/fastapi.py
--rw-r--r--   0        0        0     3333 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/server/internal.py
--rw-r--r--   0        0        0      564 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/typing.py
--rw-r--r--   0        0        0      563 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/hertavilla/utils.py
--rw-r--r--   0        0        0       58 2023-07-20 06:54:07.233765 herta_villa_sdk-0.6.4/hertavilla/version.py
--rw-r--r--   0        0        0     2292 2023-07-20 06:54:46.070185 herta_villa_sdk-0.6.4/pyproject.toml
--rw-r--r--   0        0        0      528 2023-07-20 06:54:07.137764 herta_villa_sdk-0.6.4/tests/test_utils.py
--rw-r--r--   0        0        0     5279 1970-01-01 00:00:00.000000 herta_villa_sdk-0.6.4/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-07-20 08:27:23.075545 herta_villa_sdk-0.7.0/LICENSE
+-rw-r--r--   0        0        0     4548 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/README.md
+-rw-r--r--   0        0        0      850 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/__init__.py
+-rw-r--r--   0        0        0        0 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/__init__.py
+-rw-r--r--   0        0        0     1485 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/audit.py
+-rw-r--r--   0        0        0      782 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/auth.py
+-rw-r--r--   0        0        0     1739 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/base.py
+-rw-r--r--   0        0        0      520 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/emoticon.py
+-rw-r--r--   0        0        0      701 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/img.py
+-rw-r--r--   0        0        0     2174 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/member.py
+-rw-r--r--   0        0        0     2693 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/message.py
+-rw-r--r--   0        0        0     4405 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/role.py
+-rw-r--r--   0        0        0     4190 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/room.py
+-rw-r--r--   0        0        0      645 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/apis/villa.py
+-rw-r--r--   0        0        0     8820 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/bot.py
+-rw-r--r--   0        0        0     6282 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/event.py
+-rw-r--r--   0        0        0     1952 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/exception.py
+-rw-r--r--   0        0        0     1481 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/match.py
+-rw-r--r--   0        0        0      353 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/__init__.py
+-rw-r--r--   0        0        0     5141 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/chain.py
+-rw-r--r--   0        0        0     1398 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/image.py
+-rw-r--r--   0        0        0      927 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/post.py
+-rw-r--r--   0        0        0     6289 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/text.py
+-rw-r--r--   0        0        0      442 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/message/types.py
+-rw-r--r--   0        0        0     6280 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/model.py
+-rw-r--r--   0        0        0      928 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/__init__.py
+-rw-r--r--   0        0        0      788 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/_lifespan.py
+-rw-r--r--   0        0        0     1977 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/aiohttp.py
+-rw-r--r--   0        0        0     2342 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/fastapi.py
+-rw-r--r--   0        0        0     3333 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/server/internal.py
+-rw-r--r--   0        0        0      564 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/typing.py
+-rw-r--r--   0        0        0      563 2023-07-20 08:27:23.079545 herta_villa_sdk-0.7.0/hertavilla/utils.py
+-rw-r--r--   0        0        0       58 2023-07-20 08:27:23.191552 herta_villa_sdk-0.7.0/hertavilla/version.py
+-rw-r--r--   0        0        0     2292 2023-07-20 08:28:02.046027 herta_villa_sdk-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0      528 2023-07-20 08:27:23.083545 herta_villa_sdk-0.7.0/tests/test_utils.py
+-rw-r--r--   0        0        0     5330 1970-01-01 00:00:00.000000 herta_villa_sdk-0.7.0/PKG-INFO
```

### Comparing `herta_villa_sdk-0.6.4/LICENSE` & `herta_villa_sdk-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/README.md` & `herta_villa_sdk-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -99,24 +99,26 @@
   - [x] 创建身份组 `/createMemberRole`
   - [x] 编辑身份组 `/editMemberRole`
   - [x] 删除身份组 `/deleteMemberRole`
   - [x] 获取身份组 `/getMemberRoleInfo`
   - [x] 获取大别野下所有身份组 `/getVillaMemberRoles`
 - [x] 表态表情
   - [x] 获取全量表情 `/getAllEmoticons`
-- [ ] 审核 `/audit`
+- [x] 图片
+  - [x] 图片转存 `/transferImage`
+- [x] 审核 `/audit`
 
 ## 支持的事件
 
 - [x] [JoinVilla](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###JoinVilla) 有新用户加入大别野
 - [x] [SendMessage](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage) 用户@机器人发送消息
 - [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
 - [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
 - [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
-- [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
+- [x] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
 
 ## Bug 反馈及建议
 
 大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
 
 ## 相关项目
```

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/auth.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/auth.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/base.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/base.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/emoticon.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/emoticon.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/img.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/img.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/member.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/member.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/message.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/message.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/role.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/role.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/room.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/room.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/apis/villa.py` & `herta_villa_sdk-0.7.0/hertavilla/apis/villa.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/bot.py` & `herta_villa_sdk-0.7.0/hertavilla/bot.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,25 +42,27 @@
 logger = logging.getLogger("hertavilla.bot")
 
 
 @dataclass
 class Handler(Generic[TE]):
     event: type[TE]
     func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]]
+    temp: bool = False
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def __eq__(self, __value: Event) -> bool:
         return isinstance(__value, self.event)
 
 
 class MessageHandler(NamedTuple):
     match: Match
     func: Callable[["SendMessageEvent", VillaBot], Coroutine[Any, Any, None]]
+    temp: bool = False
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         return self.func(*args, **kwargs)
 
     def check(self, chain: MessageChain) -> bool:
         return self.match.check(chain)
 
@@ -178,110 +180,137 @@
 
     # event handle
 
     def register_handler(
         self,
         event: type[TE],
         func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
+        temp: bool = False,
     ):
-        self.handlers.append(Handler[TE](event, func))
-        logger.info(f"Registered the handler {func} for {event.__name__}")
+        self.handlers.append(Handler[TE](event, func, temp))
+        logger.info(
+            f"Registered the handler {func} "
+            f"for {event.__name__} (temp: {temp})",
+        )
         return func
 
     def listen(
         self,
         event: type[TE],
+        temp: bool = False,
     ) -> Callable[
         [Callable[[TE, VillaBot], Coroutine[Any, Any, None]]],
         Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
     ]:
         def wrapper(
             func: Callable[[TE, VillaBot], Coroutine[Any, Any, None]],
         ) -> Callable[[TE, VillaBot], Coroutine[Any, Any, None]]:
-            self.register_handler(event, func)
+            self.register_handler(event, func, temp)
             return func
 
         return wrapper
 
     async def handle_event(self, event: Event) -> None:
-        handlers = filter(lambda x: x == event, self.handlers)
+        handlers = list(filter(lambda x: x == event, self.handlers))
         logger.info(f"Handling event {event.__class__.__name__}")
+        need_remove_handlers = filter(lambda x: x.temp, handlers)
         try:
             await asyncio.gather(
                 *[handler(event, self) for handler in handlers],
             )
         except Exception:
             logger.exception("Raised exceptions while handling event.")
+        for handler in need_remove_handlers:
+            self.handlers.remove(handler)
+            logger.debug(f"Removed handler for {event.__class__.__name__}")
 
     # message handle
     @staticmethod
     async def message_handler(event: "SendMessageEvent", bot: "VillaBot"):
-        handlers = filter(
-            lambda x: x.check(event.message),
-            bot.message_handlers,
+        handlers = list(
+            filter(
+                lambda x: x.check(event.message),
+                bot.message_handlers,
+            ),
         )
+        need_remove_handlers = filter(lambda x: x.temp, handlers)
         await asyncio.gather(*[handler(event, bot) for handler in handlers])
+        for handler in need_remove_handlers:
+            bot.message_handlers.remove(handler)
+            logger.debug(f"Removed message handler with {handler.match}")
 
-    def register_msg_handler(self, match: Match, func: MessageHandlerFunc):
-        self.message_handlers.append(MessageHandler(match, func))
-        logger.info(f"Registered the handler {func} with {match}")
+    def register_msg_handler(
+        self,
+        match: Match,
+        func: MessageHandlerFunc,
+        temp: bool = False,
+    ):
+        self.message_handlers.append(MessageHandler(match, func, temp))
+        logger.info(
+            f"Registered the handler {func} with {match} (temp: {temp})",
+        )
         return func
 
     def match(
         self,
         match: Match,
+        temp: bool = False,
     ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
         def wrapper(
             func: MessageHandlerFunc,
         ) -> MessageHandlerFunc:
-            self.register_msg_handler(match, func)
+            self.register_msg_handler(match, func, temp)
             return func
 
         return wrapper
 
     def regex(
         self,
         pattern: str | re.Pattern,
+        temp: bool = False,
     ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
         def wrapper(
             func: MessageHandlerFunc,
         ) -> MessageHandlerFunc:
-            self.register_msg_handler(Regex(pattern), func)
+            self.register_msg_handler(Regex(pattern), func, temp)
             return func
 
         return wrapper
 
     def startswith(
         self,
         prefix: str,
+        temp: bool = False,
     ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
         def wrapper(
             func: MessageHandlerFunc,
         ) -> MessageHandlerFunc:
-            self.register_msg_handler(Startswith(prefix), func)
+            self.register_msg_handler(Startswith(prefix), func, temp)
             return func
 
         return wrapper
 
     def endswith(
         self,
         suffix: str,
+        temp: bool = False,
     ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
         def wrapper(
             func: MessageHandlerFunc,
         ) -> MessageHandlerFunc:
-            self.register_msg_handler(Endswith(suffix), func)
+            self.register_msg_handler(Endswith(suffix), func, temp)
             return func
 
         return wrapper
 
     def keyword(
         self,
         *keywords: str,
+        temp: bool = False,
     ) -> Callable[[MessageHandlerFunc], MessageHandlerFunc]:
         def wrapper(
             func: MessageHandlerFunc,
         ) -> MessageHandlerFunc:
-            self.register_msg_handler(Keywords(*keywords), func)
+            self.register_msg_handler(Keywords(*keywords), func, temp)
             return func
 
         return wrapper
```

### Comparing `herta_villa_sdk-0.6.4/hertavilla/event.py` & `herta_villa_sdk-0.7.0/hertavilla/event.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # ruff: noqa: A003
 from __future__ import annotations
 
+from enum import IntEnum
 import json
 import sys
 from typing import Any, List, Literal, Optional, Type
 
 from hertavilla.message import (
     MessageChain,
 )
@@ -220,14 +221,48 @@
     bot_msg_id: str
     """如果被回复的消息从属于机器人，则该字段不为空字符串"""
 
     is_cancel: bool = False
     """是否是取消表情"""
 
 
+class AuditResult(IntEnum):
+    COMPATIBLE = 0
+    APPROVED = 1
+    REJECTED = 2
+
+
+class AuditCallbackEvent(Event):
+    type: Literal[6]
+
+    audit_id: str
+    """审核事件 id"""
+
+    bot_tpl_id: str
+    """机器人 id"""
+
+    room_id: int
+    """房间 id（和审核接口调用方传入的值一致）"""
+
+    user_id: int
+    """用户 id（和审核接口调用方传入的值一致）"""
+
+    pass_through: Optional[str] = None
+    """透传数据（和审核接口调用方传入的值一致）"""
+
+    audit_result: AuditResult
+    """审核结果，0作兼容，1审核通过，2审核驳回"""
+
+    def __bool__(self) -> bool:
+        return self.audit_result != AuditResult.REJECTED
+
+    def compare(self, audit_id: str, pass_through: str | None = None) -> bool:
+        return self.audit_id == audit_id and self.pass_through == pass_through
+
+
 def parse_event(payload: dict[str, Any]) -> Event:
     type_: int = payload["type"]
     cls_, name = events[type_]
     data = payload["extend_data"]["EventData"][name]
     payload.pop("extend_data")
     payload |= data
     return cls_.parse_obj(payload)
```

### Comparing `herta_villa_sdk-0.6.4/hertavilla/exception.py` & `herta_villa_sdk-0.7.0/hertavilla/exception.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/match.py` & `herta_villa_sdk-0.7.0/hertavilla/match.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/message/chain.py` & `herta_villa_sdk-0.7.0/hertavilla/message/chain.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/message/image.py` & `herta_villa_sdk-0.7.0/hertavilla/message/image.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/message/post.py` & `herta_villa_sdk-0.7.0/hertavilla/message/post.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/message/text.py` & `herta_villa_sdk-0.7.0/hertavilla/message/text.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/model.py` & `herta_villa_sdk-0.7.0/hertavilla/model.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/server/__init__.py` & `herta_villa_sdk-0.7.0/hertavilla/server/__init__.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/server/_lifespan.py` & `herta_villa_sdk-0.7.0/hertavilla/server/_lifespan.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/server/aiohttp.py` & `herta_villa_sdk-0.7.0/hertavilla/server/aiohttp.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/server/fastapi.py` & `herta_villa_sdk-0.7.0/hertavilla/server/fastapi.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/server/internal.py` & `herta_villa_sdk-0.7.0/hertavilla/server/internal.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/typing.py` & `herta_villa_sdk-0.7.0/hertavilla/typing.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/hertavilla/utils.py` & `herta_villa_sdk-0.7.0/hertavilla/utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/pyproject.toml` & `herta_villa_sdk-0.7.0/pyproject.toml`

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
-version = "0.6.4"
+version = "0.7.0"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Homepage = "https://github.com/Herta-villa/Herta-villa-SDK"
 Documentation = "https://github.com/Herta-villa/Herta-villa-SDK"
```

### Comparing `herta_villa_sdk-0.6.4/tests/test_utils.py` & `herta_villa_sdk-0.7.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `herta_villa_sdk-0.6.4/PKG-INFO` & `herta_villa_sdk-0.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: herta-villa-sdk
-Version: 0.6.4
+Version: 0.7.0
 Summary: 大别野「黑塔」Python SDK
 Keywords: mihoyo miyoushe bot villa
 Author-Email: MingxuanGame <MingxuanGame@outlook.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Documentation, https://github.com/Herta-villa/Herta-villa-SDK
 Project-URL: Repository, https://github.com/Herta-villa/Herta-villa-SDK
@@ -119,24 +119,26 @@
   - [x] 创建身份组 `/createMemberRole`
   - [x] 编辑身份组 `/editMemberRole`
   - [x] 删除身份组 `/deleteMemberRole`
   - [x] 获取身份组 `/getMemberRoleInfo`
   - [x] 获取大别野下所有身份组 `/getVillaMemberRoles`
 - [x] 表态表情
   - [x] 获取全量表情 `/getAllEmoticons`
-- [ ] 审核 `/audit`
+- [x] 图片
+  - [x] 图片转存 `/transferImage`
+- [x] 审核 `/audit`
 
 ## 支持的事件
 
 - [x] [JoinVilla](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###JoinVilla) 有新用户加入大别野
 - [x] [SendMessage](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###SendMessage) 用户@机器人发送消息
 - [x] [CreateRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###CreateRobot) 大别野添加机器人实例
 - [x] [DeleteRobot](https://webstatic.mihoyo.com/vila/bot/doc/callback.html###DeleteRobot) 大别野删除机器人实例
 - [x] [AddQuickEmoticon](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AddQuickEmoticon) 用户使用表情回复消息表态
-- [ ] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
+- [x] [AuditCallback](https://webstatic.mihoyo.com/vila/bot/doc/callback.html#AuditCallback) 审核结果回调
 
 ## Bug 反馈及建议
 
 大别野 Bot 和 Herta SDK 均处于开发状态中，如遇到问题或有相关建议可通过 [Issue](https://github.com/Herta-villa/Herta-villa-SDK/issues/new) 提出，感谢支持！
 
 ## 相关项目
```

