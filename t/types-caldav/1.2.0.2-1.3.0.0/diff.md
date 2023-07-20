# Comparing `tmp/types-caldav-1.2.0.2.tar.gz` & `tmp/types-caldav-1.3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-caldav-1.2.0.2.tar", last modified: Wed May 10 15:23:54 2023, max compression
+gzip compressed data, was "types-caldav-1.3.0.0.tar", last modified: Thu Jul 20 15:21:52 2023, max compression
```

## Comparing `types-caldav-1.2.0.2.tar` & `types-caldav-1.3.0.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1894 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/caldav-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     3371 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/davclient.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/elements/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/base.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/cdav.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/dav.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/elements/ical.pyi
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/caldav-stubs/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/error.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/namespace.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      916 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/url.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/lib/vcal.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    10217 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/objects.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-05-10 15:19:44.000000 types-caldav-1.2.0.2/caldav-stubs/requests.pyi
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-10 15:23:54.014937 types-caldav-1.2.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-10 15:23:54.010938 types-caldav-1.2.0.2/types_caldav.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-10 15:23:53.000000 types-caldav-1.2.0.2/types_caldav.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2087 2023-07-20 15:21:51.000000 types-caldav-1.3.0.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-07-20 15:21:51.000000 types-caldav-1.3.0.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/caldav-stubs/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-07-20 15:21:51.000000 types-caldav-1.3.0.0/caldav-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/davclient.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/caldav-stubs/elements/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/elements/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/elements/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/elements/cdav.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/elements/dav.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/elements/ical.pyi
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/caldav-stubs/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/lib/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/lib/error.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/lib/namespace.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      916 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/lib/url.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/lib/vcal.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    10767 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/objects.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-07-20 15:15:13.000000 types-caldav-1.3.0.0/caldav-stubs/requests.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-07-20 15:21:51.000000 types-caldav-1.3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 15:21:52.105273 types-caldav-1.3.0.0/types_caldav.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-07-20 15:21:52.000000 types-caldav-1.3.0.0/types_caldav.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-07-20 15:21:52.000000 types-caldav-1.3.0.0/types_caldav.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 15:21:52.000000 types-caldav-1.3.0.0/types_caldav.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-07-20 15:21:52.000000 types-caldav-1.3.0.0/types_caldav.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-20 15:21:52.000000 types-caldav-1.3.0.0/types_caldav.egg-info/top_level.txt
```

### Comparing `types-caldav-1.2.0.2/CHANGELOG.md` & `types-caldav-1.3.0.0/CHANGELOG.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+## 1.3.0.0 (2023-07-20)
+
+Add an upstream_repository field to METADATA.toml (#10487)
+
+Closes: #10478
+
+Update `caldav` to `1.3.*` (#10485)
+
+Co-authored-by: Alex Waygood <Alex.Waygood@Gmail.com>
+
 ## 1.2.0.2 (2023-05-10)
 
 Add `partial_stub` metadata field (#10157)
 
 ## 1.2.0.1 (2023-03-27)
 
 Add defaults for third-party stubs A-D (#9952)
```

### Comparing `types-caldav-1.2.0.2/PKG-INFO` & `types-caldav-1.3.0.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-caldav
-Version: 1.2.0.2
+Version: 1.3.0.0
 Summary: Typing stubs for caldav
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-caldav-1.2.0.2/caldav-stubs/davclient.pyi` & `types-caldav-1.3.0.0/caldav-stubs/davclient.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,16 @@
 
 class DAVResponse:
     reason: str
     tree: _Element | None
     status: int
     headers: CaseInsensitiveDict[str]
     objects: dict[str, dict[str, str]]  # only defined after call to find_objects_and_props()
-    def __init__(self, response: Response) -> None: ...
+    huge_tree: bool
+    def __init__(self, response: Response, davclient: DAVClient | None = None) -> None: ...
     @property
     def raw(self) -> str: ...
     def validate_status(self, status: str) -> None: ...
     def find_objects_and_props(self) -> None: ...
     def expand_simple_props(
         self, props: Iterable[Incomplete] = [], multi_value_props: Iterable[Incomplete] = [], xpath: str | None = None
     ) -> dict[str, dict[str, str]]: ...
@@ -35,25 +36,27 @@
     headers: dict[str, str]
     username: str | None
     password: str | None
     auth: AuthBase | None
     timeout: _Timeout | None
     ssl_verify_cert: bool | str
     ssl_cert: str | tuple[str, str] | None
+    huge_tree: bool
     def __init__(
         self,
         url: str,
         proxy: str | None = None,
         username: str | None = None,
         password: str | None = None,
         auth: AuthBase | None = None,
         timeout: _Timeout | None = None,
         ssl_verify_cert: bool | str = True,
         ssl_cert: str | tuple[str, str] | None = None,
         headers: dict[str, str] = {},
+        huge_tree: bool = False,
     ) -> None: ...
     def __enter__(self) -> Self: ...
     def __exit__(
         self, exc_type: type[BaseException] | None, exc_value: BaseException | None, traceback: TracebackType | None
     ) -> None: ...
     def principal(self, *, url: str | ParseResult | SplitResult | URL | None = ...) -> Principal: ...
     def calendar(
```

### Comparing `types-caldav-1.2.0.2/caldav-stubs/elements/base.pyi` & `types-caldav-1.3.0.0/caldav-stubs/elements/base.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.2/caldav-stubs/elements/cdav.pyi` & `types-caldav-1.3.0.0/caldav-stubs/elements/cdav.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.2/caldav-stubs/elements/dav.pyi` & `types-caldav-1.3.0.0/caldav-stubs/elements/dav.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.2/caldav-stubs/lib/error.pyi` & `types-caldav-1.3.0.0/caldav-stubs/lib/error.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.2/caldav-stubs/lib/url.pyi` & `types-caldav-1.3.0.0/caldav-stubs/lib/url.pyi`

 * *Files identical despite different names*

### Comparing `types-caldav-1.2.0.2/caldav-stubs/objects.pyi` & `types-caldav-1.3.0.0/caldav-stubs/objects.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import datetime
 from _typeshed import Incomplete
-from collections.abc import Iterable, Iterator, Mapping, Sequence
-from typing import TypeVar, overload
+from collections import defaultdict
+from collections.abc import Callable, Container, Iterable, Iterator, Mapping, Sequence
+from typing import Any, TypeVar, overload
 from typing_extensions import Literal, Self, TypeAlias
 from urllib.parse import ParseResult, SplitResult
 
 from vobject.base import VBase
 
 from .davclient import DAVClient
-from .elements.cdav import CalendarQuery, CompFilter, ScheduleInboxURL, ScheduleOutboxURL
+from .elements.cdav import CalendarData, CalendarQuery, CompFilter, ScheduleInboxURL, ScheduleOutboxURL
 from .lib.url import URL
 
 _CC = TypeVar("_CC", bound=CalendarObjectResource)
 # Actually "type[Todo] | type[Event] | type[Journal]", but mypy doesn't like that.
 _CompClass: TypeAlias = type[CalendarObjectResource]
 _VCalAddress: TypeAlias = Incomplete  # actually icalendar.vCalAddress
 
@@ -121,57 +122,62 @@
         self,
         xml: None = None,
         comp_class: None = None,
         todo: bool | None = None,
         include_completed: bool = False,
         sort_keys: Sequence[str] = (),
         split_expanded: bool = True,
+        props: list[CalendarData] | None = None,
         **kwargs,
     ) -> list[CalendarObjectResource]: ...
     @overload
     def search(
         self,
         xml,
         comp_class: type[_CC],
         todo: bool | None = None,
         include_completed: bool = False,
         sort_keys: Sequence[str] = (),
         split_expanded: bool = True,
+        props: list[CalendarData] | None = None,
         **kwargs,
     ) -> list[_CC]: ...
     @overload
     def search(
         self,
         *,
         comp_class: type[_CC],
         todo: bool | None = None,
         include_completed: bool = False,
         sort_keys: Sequence[str] = (),
         split_expanded: bool = True,
+        props: list[CalendarData] | None = None,
         **kwargs,
     ) -> list[_CC]: ...
     def build_search_xml_query(
         self,
         comp_class: _CompClass | None = None,
         todo: bool | None = None,
         ignore_completed1: bool | None = None,
         ignore_completed2: bool | None = None,
         ignore_completed3: bool | None = None,
         event: bool | None = None,
         filters: list[Incomplete] | None = None,
         expand: bool | None = None,
         start: datetime.datetime | None = None,
         end: datetime.datetime | None = None,
+        props: list[CalendarData] | None = None,
         *,
         uid=...,
         summary=...,
         comment=...,
         description=...,
         location=...,
         status=...,
+        **kwargs: str,
     ) -> tuple[CalendarQuery, _CompClass]: ...
     def freebusy_request(self, start: datetime.datetime, end: datetime.datetime) -> FreeBusy: ...
     def todos(
         self, sort_keys: Iterable[str] = ("due", "priority"), include_completed: bool = False, sort_key: str | None = None
     ) -> list[Todo]: ...
     def event_by_url(self, href, data: Incomplete | None = None) -> Event: ...
     def object_by_uid(self, uid: str, comp_filter: CompFilter | None = None, comp_class: _CompClass | None = None) -> Event: ...
@@ -217,14 +223,21 @@
         parent: Incomplete | None = None,
         id: Incomplete | None = None,
         props: Incomplete | None = None,
     ) -> None: ...
     def add_organizer(self) -> None: ...
     def split_expanded(self) -> list[Self]: ...
     def expand_rrule(self, start: datetime.datetime, end: datetime.datetime) -> None: ...
+    def get_relatives(
+        self,
+        reltypes: Container[str] | None = None,
+        relfilter: Callable[[Any], bool] | None = None,
+        fetch_objects: bool = True,
+        ignore_missing: bool = True,
+    ) -> defaultdict[str, set[str]]: ...
     def add_attendee(self, attendee, no_default_parameters: bool = False, **parameters) -> None: ...
     def is_invite_request(self) -> bool: ...
     def accept_invite(self, calendar: Incomplete | None = None) -> None: ...
     def decline_invite(self, calendar: Incomplete | None = None) -> None: ...
     def tentatively_accept_invite(self, calendar: Incomplete | None = None) -> None: ...
     def copy(self, keep_uid: bool = False, new_parent: Incomplete | None = None) -> Self: ...
     def load(self, only_if_unloaded: bool = False) -> Self: ...
```

### Comparing `types-caldav-1.2.0.2/setup.py` & `types-caldav-1.3.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,33 +11,39 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
 '''.lstrip()
 
 setup(name=name,
-      version="1.2.0.2",
+      version="1.3.0.0",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md",
           "Issue tracker": "https://github.com/python/typeshed/issues",
           "Chat": "https://gitter.im/python/typing",
       },
       install_requires=['types-requests', 'types-vobject'],
       packages=['caldav-stubs'],
-      package_data={'caldav-stubs': ['__init__.pyi', 'davclient.pyi', 'elements/__init__.pyi', 'elements/base.pyi', 'elements/cdav.pyi', 'elements/dav.pyi', 'elements/ical.pyi', 'lib/__init__.pyi', 'lib/error.pyi', 'lib/namespace.pyi', 'lib/url.pyi', 'lib/vcal.pyi', 'objects.pyi', 'requests.pyi', 'METADATA.toml']},
+      package_data={'caldav-stubs': ['__init__.pyi', 'davclient.pyi', 'elements/__init__.pyi', 'elements/base.pyi', 'elements/cdav.pyi', 'elements/dav.pyi', 'elements/ical.pyi', 'lib/__init__.pyi', 'lib/error.pyi', 'lib/namespace.pyi', 'lib/url.pyi', 'lib/vcal.pyi', 'objects.pyi', 'requests.pyi', 'METADATA.toml', 'py.typed']},
       license="Apache-2.0 license",
       classifiers=[
           "License :: OSI Approved :: Apache Software License",
           "Programming Language :: Python :: 3",
           "Typing :: Stubs Only",
       ]
 )
```

### Comparing `types-caldav-1.2.0.2/types_caldav.egg-info/PKG-INFO` & `types-caldav-1.3.0.0/types_caldav.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-caldav
-Version: 1.2.0.2
+Version: 1.3.0.0
 Summary: Typing stubs for caldav
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/caldav.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -21,9 +21,15 @@
 [pyright](https://github.com/microsoft/pyright),
 [pytype](https://github.com/google/pytype/),
 PyCharm, etc. to check code that uses
 `caldav`. The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/caldav. All fixes for
 types and metadata should be contributed there.
 
+This stub package is marked as [partial](https://peps.python.org/pep-0561/#partial-stub-packages).
+If you find that annotations are missing, feel free to contribute and help complete them.
+
+
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `d1bfd08b4bc843227d097decfd99d70272a1f804`.
+This package was generated from typeshed commit `afe18e95a9592434e93b648de5194cfe54443f84` and was tested
+with mypy 1.4.1, pyright 1.1.318, and
+pytype 2023.6.16.
```

### Comparing `types-caldav-1.2.0.2/types_caldav.egg-info/SOURCES.txt` & `types-caldav-1.3.0.0/types_caldav.egg-info/SOURCES.txt`

 * *Files identical despite different names*

