# Comparing `tmp/virl2_client-2.5.0.tar.gz` & `tmp/virl2_client-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "virl2_client-2.5.0.tar", max compression
+gzip compressed data, was "virl2_client-2.6.0.tar", max compression
```

## Comparing `virl2_client-2.5.0.tar` & `virl2_client-2.6.0.tar`

### file list

```diff
@@ -1,25 +1,30 @@
--rw-r--r--   0        0        0    11358 2022-03-15 08:41:23.934137 virl2_client-2.5.0/LICENSE
--rw-r--r--   0        0        0     4751 2023-03-06 13:51:37.777721 virl2_client-2.5.0/README.md
--rw-r--r--   0        0        0     3850 2022-03-15 08:41:23.934137 virl2_client-2.5.0/examples/demo.ipynb
--rw-r--r--   0        0        0     4760 2023-03-06 13:51:37.777721 virl2_client-2.5.0/examples/licensing.py
--rw-r--r--   0        0        0     3391 2023-03-06 13:51:37.777721 virl2_client-2.5.0/examples/link_conditioning.py
--rw-r--r--   0        0        0     3512 2023-03-06 13:51:37.777721 virl2_client-2.5.0/examples/sample.py
--rw-r--r--   0        0        0     1521 2023-03-06 13:51:37.777721 virl2_client-2.5.0/pyproject.toml
--rw-r--r--   0        0        0     1045 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/__init__.py
--rw-r--r--   0        0        0     1293 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/exceptions.py
--rw-r--r--   0        0        0     1542 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/__init__.py
--rw-r--r--   0        0        0     4139 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/authentication.py
--rw-r--r--   0        0        0     4546 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/cl_pyats.py
--rw-r--r--   0        0        0     4302 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/groups.py
--rw-r--r--   0        0        0     7037 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/interface.py
--rw-r--r--   0        0        0    46887 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/lab.py
--rw-r--r--   0        0        0    11657 2023-03-06 13:51:37.781721 virl2_client-2.5.0/virl2_client/models/licensing.py
--rw-r--r--   0        0        0     9836 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/link.py
--rw-r--r--   0        0        0    19199 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/node.py
--rw-r--r--   0        0        0     8346 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/node_image_definitions.py
--rw-r--r--   0        0        0    12787 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/resource_pools.py
--rw-r--r--   0        0        0     7787 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/system.py
--rw-r--r--   0        0        0     4544 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/models/users.py
--rw-r--r--   0        0        0    25750 2023-03-06 13:51:37.785721 virl2_client-2.5.0/virl2_client/virl2_client.py
--rw-r--r--   0        0        0     5701 1970-01-01 00:00:00.000000 virl2_client-2.5.0/setup.py
--rw-r--r--   0        0        0     5882 1970-01-01 00:00:00.000000 virl2_client-2.5.0/PKG-INFO
+-rw-r--r--   0        0        0    11358 2023-05-11 03:48:26.877583 virl2_client-2.6.0/LICENSE
+-rw-r--r--   0        0        0     4751 2023-06-27 05:16:05.743312 virl2_client-2.6.0/README.md
+-rw-r--r--   0        0        0     3850 2023-07-03 08:34:36.076232 virl2_client-2.6.0/examples/demo.ipynb
+-rw-r--r--   0        0        0     4760 2023-07-03 08:34:36.076232 virl2_client-2.6.0/examples/licensing.py
+-rw-r--r--   0        0        0     3391 2023-07-03 08:34:36.076232 virl2_client-2.6.0/examples/link_conditioning.py
+-rw-r--r--   0        0        0     3514 2023-07-03 08:34:36.076232 virl2_client-2.6.0/examples/sample.py
+-rw-r--r--   0        0        0     1552 2023-07-20 17:26:48.808615 virl2_client-2.6.0/pyproject.toml
+-rw-r--r--   0        0        0     1045 2023-06-27 05:16:30.776998 virl2_client-2.6.0/virl2_client/__init__.py
+-rw-r--r--   0        0        0     9428 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/event_handling.py
+-rw-r--r--   0        0        0     5665 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/event_listening.py
+-rw-r--r--   0        0        0     1394 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/exceptions.py
+-rw-r--r--   0        0        0     1608 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/__init__.py
+-rw-r--r--   0        0        0    11405 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/auth_management.py
+-rw-r--r--   0        0        0     4210 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/authentication.py
+-rw-r--r--   0        0        0     6296 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/cl_pyats.py
+-rw-r--r--   0        0        0     2962 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/configuration.py
+-rw-r--r--   0        0        0     4363 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/groups.py
+-rw-r--r--   0        0        0     8040 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/models/interface.py
+-rw-r--r--   0        0        0    51401 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/models/lab.py
+-rw-r--r--   0        0        0    11656 2023-07-09 17:37:31.247357 virl2_client-2.6.0/virl2_client/models/licensing.py
+-rw-r--r--   0        0        0    10761 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/models/link.py
+-rw-r--r--   0        0        0    20194 2023-07-09 17:37:31.258191 virl2_client-2.6.0/virl2_client/models/node.py
+-rw-r--r--   0        0        0    10157 2023-07-09 17:37:31.258191 virl2_client-2.6.0/virl2_client/models/node_image_definitions.py
+-rw-r--r--   0        0        0    12787 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/models/resource_pools.py
+-rw-r--r--   0        0        0    14702 2023-07-03 08:34:36.076232 virl2_client-2.6.0/virl2_client/models/system.py
+-rw-r--r--   0        0        0     4683 2023-07-09 17:37:31.258191 virl2_client-2.6.0/virl2_client/models/users.py
+-rw-r--r--   0        0        0     4229 2023-07-09 17:37:31.258191 virl2_client-2.6.0/virl2_client/utils.py
+-rw-r--r--   0        0        0    28905 2023-07-09 17:37:31.258191 virl2_client-2.6.0/virl2_client/virl2_client.py
+-rw-r--r--   0        0        0     5717 2023-07-20 17:38:40.625321 virl2_client-2.6.0/setup.py
+-rw-r--r--   0        0        0     5791 2023-07-20 17:38:40.626136 virl2_client-2.6.0/PKG-INFO
```

### Comparing `virl2_client-2.5.0/LICENSE` & `virl2_client-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/README.md` & `virl2_client-2.6.0/README.md`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/examples/demo.ipynb` & `virl2_client-2.6.0/examples/demo.ipynb`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/examples/licensing.py` & `virl2_client-2.6.0/examples/licensing.py`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/examples/link_conditioning.py` & `virl2_client-2.6.0/examples/link_conditioning.py`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/examples/sample.py` & `virl2_client-2.6.0/examples/sample.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,15 +82,15 @@
 
 # this must remove the link between s1 and s2
 lab.remove_node(s2)
 
 lab.sync_states()
 for node in lab.nodes():
     print(node, node.state)
-    for iface in node.interfaces:
+    for iface in node.interfaces():
         print(iface, iface.state)
 
 assert [link for link in lab.links() if link.state is not None] == []
 
 # in case you's like to deregister after you're done
 status = cl.licensing.deregister()
 cl.licensing.remove_certificate()
```

### Comparing `virl2_client-2.5.0/pyproject.toml` & `virl2_client-2.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "virl2_client"
-version = "2.5.0"
+version = "2.6.0"
 description = "VIRL2 Client Library"
 authors = ["Simon Knight <simknigh@cisco.com>", "Ralph Schmieder <rschmied@cisco.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/ciscodevnet/virl2-client"
 repository = "https://github.com/ciscodevnet/virl2-client"
 include = ["examples/*"]
@@ -16,36 +16,38 @@
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3.8",
     "Topic :: System :: Networking",
 ]
 
 [tool.poetry.dependencies]
-python = "^3.8.0"
-httpx = "^0.23.0"
+python = "^3.8.1"
+httpx = "^0.24.0"
+
+# optional package for events
+aiohttp = {version = "*", optional = true}
 
 # optional pyATS package
 # (this pulls in a lot more dependencies)
 # it does not pull in genie, need to specify extras=["full"] for pyATS.
-# pyats = {extras=["full"], version = "^22.4", optional = true}
-pyats = {version = "^22.4", optional = true}
+# pyats = {extras=["full"], version = "^23", optional = true}
+pyats = {version = "^23", optional = true}
 
 # needed to build documentation, technically, this is a dev-dependency
 # https://github.com/python-poetry/poetry/pull/606 -- no support
 sphinx_rtd_theme = {version="^1", optional = true}
-sphinx =  {version="^5", optional = true}
-
+sphinx =  {version="^6", optional = true}
 
 [tool.poetry.dev-dependencies]
-# flake8 version 6 is available but requires python>=3.8.1
-flake8 = "^5"
-pre-commit = "^2.17.0"
+flake8 = "^6"
+pre-commit = "^3"
 pytest = "*"
 respx = "^0.20.0"
 
 [tool.poetry.extras]
+events = ["aiohttp"]
 pyats = ["pyats"]
 docs = ["sphinx", "sphinx_rtd_theme"]
 
 [build-system]
 requires = ["poetry>=1.1.8"]
-build-backend = "poetry.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `virl2_client-2.5.0/virl2_client/__init__.py` & `virl2_client-2.6.0/virl2_client/__init__.py`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/virl2_client/exceptions.py` & `virl2_client-2.6.0/virl2_client/exceptions.py`

 * *Files 10% similar despite different names*

```diff
@@ -51,13 +51,21 @@
     pass
 
 
 class DesynchronizedError(VirlException):
     pass
 
 
+class InvalidContentType(VirlException):
+    pass
+
+
 class InvalidImageFile(VirlException):
     pass
 
 
 class InvalidProperty(VirlException):
     pass
+
+
+class MethodNotActive(VirlException):
+    pass
```

### Comparing `virl2_client-2.5.0/virl2_client/models/__init__.py` & `virl2_client-2.6.0/virl2_client/models/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 # limitations under the License.
 #
 """This package contains the VIRL2 client library models for
 labs, nodes, interfaces and links. It also contains classes for
 node and image definition and helper classes for automation
 and authentication."""
 
+from .auth_management import AuthManagement
 from .authentication import TokenAuth
 from .groups import GroupManagement
 from .interface import Interface
 from .lab import Lab
 from .licensing import Licensing
 from .link import Link
 from .node import Node
@@ -42,8 +43,9 @@
     "NodeImageDefinitions",
     "Licensing",
     "SystemManagement",
     "UserManagement",
     "GroupManagement",
     "TokenAuth",
     "ResourcePoolManagement",
+    "AuthManagement",
 )
```

### Comparing `virl2_client-2.5.0/virl2_client/models/authentication.py` & `virl2_client-2.6.0/virl2_client/models/authentication.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 #
 
 from __future__ import annotations
 
 import json
 import logging
 from typing import TYPE_CHECKING, Generator, Optional
+from uuid import uuid4
 
 import httpx
 
 _LOGGER = logging.getLogger(__name__)
 
 if TYPE_CHECKING:
     from ..virl2_client import ClientLibrary
@@ -71,15 +72,14 @@
     @token.setter
     def token(self, value: Optional[str]):
         self._token = value
 
     def auth_flow(
         self, request: httpx.Request
     ) -> Generator[httpx.Request, httpx.Response, None]:
-
         request.headers["Authorization"] = "Bearer {}".format(self.token)
         response = yield request
 
         if response.status_code == 401:
             _LOGGER.warning("re-auth called on 401 unauthorized")
             self.token = None
             request.headers["Authorization"] = "Bearer {}".format(self.token)
@@ -119,8 +119,9 @@
 def make_session(base_url: str, ssl_verify: bool = True) -> httpx.Client:
     return httpx.Client(
         base_url=base_url,
         verify=ssl_verify,
         auth=BlankAuth(),
         follow_redirects=True,
         timeout=None,
+        headers={"X-Client-UUID": str(uuid4())},
     )
```

### Comparing `virl2_client-2.5.0/virl2_client/models/groups.py` & `virl2_client-2.6.0/virl2_client/models/groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # limitations under the License.
 #
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Optional
 
+from ..utils import UNCHANGED
+
 if TYPE_CHECKING:
     import httpx
 
 
 class GroupManagement:
     def __init__(self, session: httpx.Client) -> None:
         self._session = session
@@ -86,36 +88,36 @@
         }
         return self._session.post(self.base_url, json=data).json()
 
     def update_group(
         self,
         group_id: str,
         name: Optional[str] = None,
-        description: Optional[str] = None,
-        members: Optional[list[str]] = None,
-        labs: Optional[list[dict[str, str]]] = None,
+        description: Optional[str] = UNCHANGED,
+        members: Optional[list[str]] = UNCHANGED,
+        labs: Optional[list[dict[str, str]]] = UNCHANGED,
     ) -> dict:
         """
         Updates a group.
 
         :param group_id: group uuid4
         :param name: new group name
         :param description: group description
         :param members: group members
         :param labs: group labs
         :return: updated group object
         """
         data: dict[str, str | list] = {}
         if name is not None:
             data["name"] = name
-        if description is not None:
+        if description is not UNCHANGED:
             data["description"] = description
-        if members is not None:
+        if members is not UNCHANGED:
             data["members"] = members
-        if labs is not None:
+        if labs is not UNCHANGED:
             data["labs"] = labs
         url = self.base_url + "/{}".format(group_id)
         return self._session.patch(url, json=data).json()
 
     def group_members(self, group_id: str) -> list[str]:
         """
         Gets group members.
```

### Comparing `virl2_client-2.5.0/virl2_client/models/interface.py` & `virl2_client-2.6.0/virl2_client/models/interface.py`

 * *Files 7% similar despite different names*

```diff
@@ -21,14 +21,17 @@
 from __future__ import annotations
 
 import logging
 import warnings
 from functools import total_ordering
 from typing import TYPE_CHECKING, Optional
 
+from ..utils import check_stale
+from ..utils import property_s as property
+
 if TYPE_CHECKING:
     import httpx
 
     from .link import Link
     from .node import Node
 
 _LOGGER = logging.getLogger(__name__)
@@ -49,21 +52,22 @@
 
         :param iid: interface ID
         :param node: node object
         :param label: the label of the interface
         :param slot: the slot of the interface
         :param iface_type: the type of the interface, defaults to "physical"
         """
-        self.id = iid
-        self.node = node
-        self.type = iface_type
-        self.label = label
-        self.slot = slot
+        self._id = iid
+        self._node = node
+        self._type = iface_type
+        self._label = label
+        self._slot = slot
         self._state: Optional[str] = None
         self._session: httpx.Client = node.lab.session
+        self._stale = False
         self.statistics = {
             "readbytes": 0,
             "readpackets": 0,
             "writebytes": 0,
             "writepackets": 0,
         }
         self.ip_snooped_info: dict[str, Optional[str]] = {
@@ -71,59 +75,82 @@
             "ipv4": None,
             "ipv6": None,
         }
 
     def __eq__(self, other):
         if not isinstance(other, Interface):
             return False
-        return self.id == other.id
+        return self._id == other._id
 
     def __lt__(self, other):
         if not isinstance(other, Interface):
             return False
-        return int(self.id) < int(other.id)
+        return self._id < other._id
 
     def __str__(self):
-        return "Interface: {}".format(self.label)
+        return f"Interface: {self._label}{' (STALE)' if self._stale else ''}"
 
     def __repr__(self):
         return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
             self.__class__.__name__,
-            self.id,
-            self.node,
-            self.label,
-            self.slot,
-            self.type,
+            self._id,
+            self._node,
+            self._label,
+            self._slot,
+            self._type,
         )
 
     def __hash__(self):
-        return hash(self.id)
+        return hash(self._id)
 
     @property
     def lab_base_url(self) -> str:
         return self.node.lab_base_url
 
     @property
     def _base_url(self) -> str:
         return self.lab_base_url + "/interfaces/{}".format(self.id)
 
     @property
+    def id(self) -> str:
+        return self._id
+
+    @property
+    def node(self) -> Node:
+        return self._node
+
+    @property
+    def type(self) -> str:
+        return self._type
+
+    @property
+    def label(self) -> str:
+        return self._label
+
+    @property
+    def slot(self) -> Optional[int]:
+        return self._slot
+
+    @property
     def physical(self) -> bool:
         """Whether the interface is physical."""
         self.node.lab.sync_topology_if_outdated()
         return self.type == "physical"
 
     @property
     def connected(self) -> bool:
         """Whether the interface is connected to a link."""
         return self.link is not None
 
     @property
     def state(self) -> Optional[str]:
         self.node.lab.sync_states_if_outdated()
+        if self._state is None:
+            url = self._base_url + "/state"
+            self._state = self._session.get(url).json()["state"]
         return self._state
 
     @property
     def link(self) -> Optional[Link]:
         """Is link if connected, otherwise None."""
         self.node.lab.sync_topology_if_outdated()
         for link in self.node.lab.links():
@@ -198,24 +225,37 @@
         :returns: A Link
         """
         link = self.link
         if link is not None and other_interface in link.interfaces:
             return link
         return None
 
-    def remove_on_server(self) -> None:
-        _LOGGER.info("Removing interface %s", self)
+    def remove(self) -> None:
+        self.node.lab.remove_interface(self)
 
+    @check_stale
+    def _remove_on_server(self) -> None:
+        _LOGGER.info("Removing interface %s", self)
         url = self._base_url
         self._session.delete(url)
 
+    def remove_on_server(self) -> None:
+        warnings.warn(
+            "'Interface.remove_on_server()' is deprecated, "
+            "use 'Interface.remove()' instead.",
+            DeprecationWarning,
+        )
+        self._remove_on_server()
+
+    @check_stale
     def bring_up(self) -> None:
         url = self._base_url + "/state/start"
         self._session.put(url)
 
+    @check_stale
     def shutdown(self) -> None:
         url = self._base_url + "/state/stop"
         self._session.put(url)
 
     def peer_interfaces(self):
         warnings.warn("Deprecated, use .peer_interface instead.", DeprecationWarning)
         return {self.peer_interface}
```

### Comparing `virl2_client-2.5.0/virl2_client/models/lab.py` & `virl2_client-2.6.0/virl2_client/models/lab.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,14 +32,16 @@
     ElementAlreadyExists,
     InterfaceNotFound,
     LabNotFound,
     LinkNotFound,
     NodeNotFound,
     VirlException,
 )
+from ..utils import check_stale, locked
+from ..utils import property_s as property
 from .cl_pyats import ClPyats
 from .interface import Interface
 from .link import Link
 from .node import Node
 
 if TYPE_CHECKING:
     import httpx
@@ -86,17 +88,18 @@
 
         self.username = username
         self.password = password
 
         self._title = title
         self._description = ""
         self._notes = ""
-        self._lab_id = lab_id
+        self._id = lab_id
         self._session = session
         self._owner = username
+        self._state = None
         self._nodes: dict[str, Node] = {}
         """
         Dictionary containing all nodes in the lab.
         It maps node identifier to `models.Node`
         """
         self._links: dict[str, Link] = {}
         """
@@ -128,71 +131,82 @@
         if resource_pool_manager is None:
             raise VirlException(
                 f"Lab object for lab {title or lab_id} cannot be created "
                 "because it is missing a resource pool manager."
             )
         self._resource_pool_manager = resource_pool_manager
         self._resource_pools = []
+        self._stale = False
 
     def __len__(self):
         return len(self._nodes)
 
     def __str__(self):
-        return "Lab: {}".format(self._title)
+        return f"Lab: {self._title}{' (STALE)' if self._stale else ''}"
 
     def __repr__(self):
         return "{}({!r}, {!r}, {!r}, {!r}, {!r}, {!r})".format(
             self.__class__.__name__,
             self._title,
-            self._lab_id,
+            self._id,
             self._session.base_url.path,
             self.auto_sync,
             self.auto_sync_interval,
             self.wait_for_convergence,
         )
 
     def need_to_wait(self, local_wait: Optional[bool]) -> bool:
         if local_wait is None:
             return self.wait_for_convergence
         if not isinstance(local_wait, bool):
             raise ValueError
         return local_wait
 
+    @check_stale
+    @locked
     def sync_statistics_if_outdated(self) -> None:
         timestamp = time.time()
         if (
             self.auto_sync
             and timestamp - self._last_sync_statistics_time > self.auto_sync_interval
         ):
             self.sync_statistics()
 
+    @check_stale
+    @locked
     def sync_states_if_outdated(self) -> None:
         timestamp = time.time()
         if (
             self.auto_sync
             and timestamp - self._last_sync_state_time > self.auto_sync_interval
         ):
             self.sync_states()
 
+    @check_stale
+    @locked
     def sync_l3_addresses_if_outdated(self) -> None:
         timestamp = time.time()
         if (
             self.auto_sync
             and timestamp - self._last_sync_l3_address_time > self.auto_sync_interval
         ):
             self.sync_layer3_addresses()
 
+    @check_stale
+    @locked
     def sync_topology_if_outdated(self) -> None:
         timestamp = time.time()
         if (
             self.auto_sync
             and timestamp - self._last_sync_topology_time > self.auto_sync_interval
         ):
             self._sync_topology(exclude_configurations=True)
 
+    @check_stale
+    @locked
     def sync_operational_if_outdated(self) -> None:
         timestamp = time.time()
         if (
             self.auto_sync
             and timestamp - self._last_sync_operational_time > self.auto_sync_interval
         ):
             self.sync_operational()
@@ -201,15 +215,15 @@
     def id(self) -> str:
         """
         Returns the ID of the lab (a 6 digit hex string).
 
         :returns: The Lab ID
         """
 
-        return self._lab_id
+        return self._id
 
     @property
     def title(self) -> Optional[str]:
         """
         Returns the title of the lab.
 
         :returns: The lab name
@@ -220,17 +234,15 @@
     @title.setter
     def title(self, value: str) -> None:
         """
         Set the title of the lab.
 
         :param value: The new lab title
         """
-        url = self.lab_base_url
-        self._session.patch(url, json={"title": value})
-        self._title = value
+        self._set_property("title", value)
 
     @property
     def notes(self) -> str:
         """
         Returns the notes of the lab.
 
         :returns: The lab name
@@ -241,17 +253,15 @@
     @notes.setter
     def notes(self, value: str) -> None:
         """
         Set the notes of the lab.
 
         :param value: The new lab notes
         """
-        url = self.lab_base_url
-        self._session.patch(url, json={"notes": value})
-        self._notes = value
+        self._set_property("notes", value)
 
     @property
     def description(self) -> str:
         """
         Returns the description of the lab.
 
         :returns: The lab name
@@ -262,17 +272,22 @@
     @description.setter
     def description(self, value: str) -> None:
         """
         Set the description of the lab.
 
         :param value: The new lab description
         """
+        self._set_property("description", value)
+
+    @check_stale
+    @locked
+    def _set_property(self, prop: str, value: Any):
         url = self.lab_base_url
-        self._session.patch(url, json={"description": value})
-        self._description = value
+        self._session.patch(url, json={prop: value})
+        setattr(self, f"_{prop}", value)
 
     @property
     def session(self) -> httpx.Client:
         """
         Returns the API client session object.
 
         :returns: The session object
@@ -319,17 +334,18 @@
         :returns: A list of Interface objects
         """
         self.sync_topology_if_outdated()
         return list(self._interfaces.values())
 
     @property
     def lab_base_url(self) -> str:
-        return "labs/{}".format(self._lab_id)
+        return "labs/{}".format(self._id)
 
     @property
+    @locked
     def statistics(self) -> dict:
         """
         Returns some statistics about the lab.
 
         :returns: A dictionary with stats of the lab
         """
         return {
@@ -444,14 +460,16 @@
 
         :param tag: tag of the nodes to be returned
         :returns: a list of nodes
         """
         self.sync_topology_if_outdated()
         return [node for node in self.nodes() if tag in node.tags()]
 
+    @check_stale
+    @locked
     def create_node(
         self,
         label: str,
         node_definition: str,
         x: int = 0,
         y: int = 0,
         wait: Optional[bool] = None,
@@ -492,18 +510,28 @@
         for key in ("image_definition", "configuration"):
             if key not in kwargs:
                 kwargs[key] = None
 
         if "compute_id" in kwargs:
             kwargs.pop("compute_id")
         kwargs["resource_pool"] = None
-        node = self.add_node_local(node_id, **kwargs)
+        node = self._create_node_local(node_id, **kwargs)
         return node
 
-    def add_node_local(
+    def add_node_local(self, *args, **kwargs):
+        warnings.warn(
+            "Deprecated. You probably want .create_node instead; "
+            "if you really want to create a node locally only, "
+            "use ._create_node_local.",
+            DeprecationWarning,
+        )
+        return self._create_node_local(*args, **kwargs)
+
+    @locked
+    def _create_node_local(
         self,
         node_id: str,
         label: str,
         node_definition: str,
         image_definition: Optional[str],
         configuration: Optional[str],
         x: int,
@@ -543,171 +571,218 @@
             resource_pool,
         )
         if compute_id is not None:
             node._compute_id = compute_id
         self._nodes[node.id] = node
         return node
 
-    def remove_node(self, node: Node, wait: Optional[bool] = None) -> None:
+    @check_stale
+    @locked
+    def remove_node(self, node: Node | str, wait: Optional[bool] = None) -> None:
         """
         Removes a node from the lab.
 
-        :param node: the node
+        If you have a node object, you can also simply do::
+
+            node.remove()
+
+
+        :param node: the node object or ID
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
-        node.remove_on_server()
-        for iface in node.interfaces():
-            if iface.link is not None:
-                try:
-                    del self._links[iface.link.id]
-                except KeyError:
-                    # element may already have been deleted on server,
-                    # and removed locally due to auto-sync
-                    pass
-            try:
-                del self._interfaces[iface.id]
-            except KeyError:
-                # element may already have been deleted on server,
-                # and removed locally due to auto-sync
-                pass
+        if isinstance(node, str):
+            node = self.get_node_by_id(node)
+        node._remove_on_server()
+        self._remove_node_local(node)
+
+        if self.need_to_wait(wait):
+            self.wait_until_lab_converged()
+        _LOGGER.debug("%s node removed from lab %s", node._id, self._id)
+
+    @locked
+    def _remove_node_local(self, node: Node) -> None:
+        """Helper function to remove a node from the client library."""
+        for iface in tuple(self._interfaces.values()):
+            if iface._node is node:
+                self._remove_interface_local(iface)
         try:
-            del self._nodes[node.id]
+            del self._nodes[node._id]
+            node._stale = True
         except KeyError:
             # element may already have been deleted on server,
             # and removed locally due to auto-sync
             pass
 
-        if self.need_to_wait(wait):
-            self.wait_until_lab_converged()
-        _LOGGER.debug("%s node removed from lab %s", node.id, self._lab_id)
-
+    @locked
     def remove_nodes(self, wait: Optional[bool] = None) -> None:
         """
         Remove all nodes from the lab.
 
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
         # TODO: see if this is used - in testing?
         for node in list(self._nodes.values()):
             self.remove_node(node, wait=False)
 
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
-        _LOGGER.debug("all nodes removed from lab %s", self._lab_id)
+        _LOGGER.debug("all nodes removed from lab %s", self._id)
 
-    def remove_link(self, link: Link, wait: Optional[bool] = None) -> None:
+    @check_stale
+    @locked
+    def remove_link(self, link: Link | str, wait: Optional[bool] = None) -> None:
         """
         Removes a link from the lab.
 
-        :param link: the link
+        If you have a link object, you can also simply do::
+
+            link.remove()
+
+        :param link: the link object or ID
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
-        link.remove_on_server()
+        if isinstance(link, str):
+            link = self.get_link_by_id(link)
+        link._remove_on_server()
+        self._remove_link_local(link)
+
+        if self.need_to_wait(wait):
+            self.wait_until_lab_converged()
+        _LOGGER.debug("link %s removed from lab %s", link._id, self._id)
+
+    @locked
+    def _remove_link_local(self, link: Link) -> None:
+        """Helper function to remove a link from the client library."""
         try:
-            del self._links[link.id]
+            del self._links[link._id]
+            link._stale = True
         except KeyError:
             # element may already have been deleted on server,
             # and removed locally due to auto-sync
             pass
 
-        if self.need_to_wait(wait):
-            self.wait_until_lab_converged()
-        _LOGGER.debug("link %s removed from lab %s", link.id, self._lab_id)
-
-    def remove_interface(self, iface: Interface, wait: Optional[bool] = None) -> None:
+    @check_stale
+    @locked
+    def remove_interface(
+        self, iface: Interface | str, wait: Optional[bool] = None
+    ) -> None:
         """
         Removes an interface from the lab.
 
-        :param iface: the interface
+        If you have an interface object, you can also simply do::
+
+            interface.remove()
+
+        :param iface: the interface object or ID
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
-        iface.remove_on_server()
-        if iface.link is not None:
-            try:
-                del self._links[iface.link.id]
-            except KeyError:
-                # element may already have been deleted on server, and removed
-                # locally due to auto-sync
-                pass
+        if isinstance(iface, str):
+            iface = self.get_interface_by_id(iface)
+        iface._remove_on_server()
+
+        self._remove_interface_local(iface)
+
+        if self.need_to_wait(wait):
+            self.wait_until_lab_converged()
+        _LOGGER.debug("interface %s removed from lab %s", iface._id, self._id)
+
+    @locked
+    def _remove_interface_local(self, iface: Interface) -> None:
+        """Helper function to remove an interface from the client library."""
+        for link in tuple(self._links.values()):
+            if iface in link.interfaces:
+                self._remove_link_local(link)
+                break
         try:
-            del self._interfaces[iface.id]
+            del self._interfaces[iface._id]
+            iface._stale = True
         except KeyError:
             # element may already have been deleted on server, and removed
             # locally due to auto-sync
             pass
 
-        if self.need_to_wait(wait):
-            self.wait_until_lab_converged()
-        _LOGGER.debug("interface %s removed from lab %s", iface.id, self._lab_id)
-
+    @check_stale
+    @locked
     def create_link(
-        self, i1: Interface, i2: Interface, wait: Optional[bool] = None
+        self, i1: Interface | str, i2: Interface | str, wait: Optional[bool] = None
     ) -> Link:
         """
         Creates a link between two interfaces
 
-        :param i1: the first interface object
-        :param i2: the second interface object
+        :param i1: the first interface object or ID
+        :param i2: the second interface object or ID
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         :returns: the created link
         """
+        if isinstance(i1, str):
+            i1 = self.get_interface_by_id(i1)
+        if isinstance(i2, str):
+            i2 = self.get_interface_by_id(i2)
         url = self.lab_base_url + "/links"
         data = {
             "src_int": i1.id,
             "dst_int": i2.id,
         }
         response = self._session.post(url, json=data)
         result = response.json()
         link_id = result["id"]
         label = result.get("label")
 
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
 
-        link = self.create_link_local(i1, i2, link_id, label)
+        link = self._create_link_local(i1, i2, link_id, label)
         return link
 
+    @check_stale
+    @locked
+    def _create_link_local(
+        self, i1: Interface, i2: Interface, link_id: str, label: Optional[str] = None
+    ) -> Link:
+        """Helper function to create a link in the client library."""
+        link = Link(self, link_id, i1, i2, label)
+        self._links[link_id] = link
+        return link
+
+    @check_stale
+    @locked
     def connect_two_nodes(self, node1: Node, node2: Node) -> Link:
         """
         Convenience method to connect two nodes within a lab.
 
         :param node1: the first node object
         :param node2: the second node object
         :returns: the created link
         """
         iface1 = node1.next_available_interface() or node1.create_interface()
         iface2 = node2.next_available_interface() or node2.create_interface()
         return self.create_link(iface1, iface2)
 
-    def create_link_local(
-        self, i1: Interface, i2: Interface, link_id: str, label: Optional[str] = None
-    ) -> Link:
-        """Helper function to create a link in the client library."""
-        link = Link(self, link_id, i1, i2, label)
-        self._links[link_id] = link
-        return link
-
+    @check_stale
+    @locked
     def create_interface(
-        self, node: Node, slot: Optional[int] = None, wait: Optional[bool] = None
+        self, node: Node | str, slot: Optional[int] = None, wait: Optional[bool] = None
     ) -> Interface:
         """
         Create an interface in the next available slot, or, if a slot is specified,
         in all available slots up to and including the specified slot.
 
         :param node: The node on which the interface is created
         :param slot: (optional)
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         :returns: The newly created interface
         """
+        if isinstance(node, str):
+            node = self.get_node_by_id(node)
         url = self.lab_base_url + "/interfaces"
         payload: dict[str, str | int] = {"node": node.id}
         if slot is not None:
             payload["slot"] = slot
         result = self._session.post(url, json=payload).json()
         if isinstance(result, dict):
             # in case API returned just one interface, pack it into the list:
@@ -715,15 +790,15 @@
 
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
 
         # TODO: need to import the topology then
         desired_interface: Optional[Interface] = None
         for iface in result:
-            lab_interface = self.create_interface_local(
+            lab_interface = self._create_interface_local(
                 iface_id=iface["id"],
                 label=iface["label"],
                 node=node,
                 slot=iface["slot"],
             )
             if slot == iface["slot"] or slot is None:
                 desired_interface = lab_interface
@@ -731,40 +806,45 @@
         if desired_interface is None:
             # Shouldn't happen, but type checkers complain about desired_interface
             # possibly being None otherwise
             raise InterfaceNotFound
 
         return desired_interface
 
-    def create_interface_local(
+    @check_stale
+    @locked
+    def _create_interface_local(
         self,
         iface_id: str,
         label: str,
         node: Node,
         slot: Optional[int],
         iface_type: str = "physical",
     ) -> Interface:
         """Helper function to create an interface in the client library."""
         if iface_id not in self._interfaces:
             iface = Interface(iface_id, node, label, slot, iface_type)
             self._interfaces[iface_id] = iface
         else:  # update the interface if it already exists:
-            self._interfaces[iface_id].node = node
-            self._interfaces[iface_id].label = label
-            self._interfaces[iface_id].slot = slot
-            self._interfaces[iface_id].type = iface_type
-        return self._interfaces[iface_id]
+            iface = self._interfaces[iface_id]
+            iface._node = node
+            iface._label = label
+            iface._slot = slot
+            iface._type = iface_type
+        return iface
 
     @staticmethod
     def _get_element_from_data(data: dict, element: str) -> int:
         try:
             return int(data[element])
         except (TypeError, KeyError):
             return 0
 
+    @check_stale
+    @locked
     def sync_statistics(self) -> None:
         """Retrieve the simulation statistic data from the back end server."""
         url = self.lab_base_url + "/simulation_stats"
         states: dict[str, dict[str, dict]] = self._session.get(url).json()
         node_statistics = states.get("nodes", {})
         link_statistics = states.get("links", {})
         for node_id, node_data in node_statistics.items():
@@ -791,70 +871,68 @@
             link.statistics = {
                 "readbytes": readbytes,
                 "readpackets": readpackets,
                 "writebytes": writebytes,
                 "writepackets": writepackets,
             }
 
-            iface_a = link.interface_a
-            iface_a.statistics = {
-                "readbytes": readbytes,
-                "readpackets": readpackets,
-                "writebytes": writebytes,
-                "writepackets": writepackets,
-            }
+            link.interface_a.statistics = link.statistics
+
             # reverse for other interface
-            iface_b = link.interface_b
-            iface_b.statistics = {
+            link.interface_b.statistics = {
                 "readbytes": writebytes,
                 "readpackets": writepackets,
                 "writebytes": readbytes,
                 "writepackets": readpackets,
             }
 
         self._last_sync_statistics_time = time.time()
 
+    @check_stale
+    @locked
     def sync_states(self) -> None:
         """
         Sync all the states of the various elements with the back end server.
         """
         url = self.lab_base_url + "/lab_element_state"
         states: dict[str, dict[str, str]] = self._session.get(url).json()
         for node_id, node_state in states["nodes"].items():
-            self._nodes[node_id].state = node_state
-
+            self._nodes[node_id]._state = node_state
+        ifaces = self._interfaces.copy()
         for interface_id, interface_state in states["interfaces"].items():
             try:
-                iface = self._interfaces[interface_id]
+                iface = ifaces.pop(interface_id)
             except KeyError:
                 # TODO: handle loopbacks created server-side
                 # check how the UI handles these created today
                 # - extra call after node created?
                 pass
             else:
                 iface._state = interface_state
-
+        for stale_iface in ifaces:
+            ifaces[stale_iface]._stale = True
         for link_id, link_state in states["links"].items():
             self._links[link_id]._state = link_state
 
         self._last_sync_state_time = time.time()
 
+    @check_stale
     def wait_until_lab_converged(
         self, max_iterations: Optional[int] = None, wait_time: Optional[int] = None
     ) -> None:
         """Wait until lab converges."""
         max_iter = (
             self.wait_max_iterations if max_iterations is None else max_iterations
         )
         wait_time = self.wait_time if wait_time is None else wait_time
-        _LOGGER.info("Waiting for lab %s to converge", self._lab_id)
+        _LOGGER.info("Waiting for lab %s to converge", self._id)
         for index in range(max_iter):
             converged = self.has_converged()
             if converged:
-                _LOGGER.info("Lab %s has booted", self._lab_id)
+                _LOGGER.info("Lab %s has booted", self._id)
                 return
 
             if index % 10 == 0:
                 _LOGGER.info(
                     "Lab has not converged, attempt %s/%s, waiting...",
                     index,
                     max_iter,
@@ -868,121 +946,140 @@
         _LOGGER.error(msg)
         # after maximum retries are exceeded and lab has not converged
         # error must be raised - it makes no sense to just log info
         # and let client fail with something else if wait is explicitly
         # specified
         raise RuntimeError(msg)
 
+    @check_stale
     def has_converged(self) -> bool:
         url = self.lab_base_url + "/check_if_converged"
         converged = self._session.get(url).json()
         return converged
 
+    @check_stale
     def start(self, wait: Optional[bool] = None) -> None:
         """
         Start all the nodes and links in the lab.
 
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
-        :type wait: bool
         """
         url = self.lab_base_url + "/start"
         self._session.put(url)
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
-        _LOGGER.debug("started lab: %s", self._lab_id)
+        _LOGGER.debug("started lab: %s", self._id)
 
+    @check_stale
     def state(self) -> str:
         """
         Returns the state of the lab.
 
         :returns: The state as text
         """
-        url = self.lab_base_url + "/state"
-        response = self._session.get(url)
-        _LOGGER.debug("lab state: %s -> %s", self._lab_id, response.text)
-        return response.json()
+        if self._state is None or getattr(self._session, "lock", None) is None:
+            # no lock == event listening not enabled
+            url = self.lab_base_url + "/state"
+            response = self._session.get(url)
+            self._state = response.json()
+
+        _LOGGER.debug("lab state: %s -> %s", self._id, self._state)
+        return self._state
 
     def is_active(self) -> bool:
         """
         Returns whether the lab is started.
 
         :returns: Whether the lab is started
         """
         return self.state() == "STARTED"
 
+    @check_stale
     def details(self) -> dict[str, str | list | int]:
         """
         Returns the lab details (including state) of the lab.
 
         :returns: The detailed lab state
         """
         url = self.lab_base_url
         response = self._session.get(url)
-        _LOGGER.debug("lab state: %s -> %s", self._lab_id, response.text)
+        _LOGGER.debug("lab state: %s -> %s", self._id, response.text)
         return response.json()
 
+    @check_stale
     def stop(self, wait: Optional[bool] = None) -> None:
         """
         Stops all the nodes and links in the lab.
 
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
         url = self.lab_base_url + "/stop"
         self._session.put(url)
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
-        _LOGGER.debug("stopped lab: %s", self._lab_id)
+        _LOGGER.debug("stopped lab: %s", self._id)
 
+    @check_stale
     def wipe(self, wait: Optional[bool] = None) -> None:
         """
         Wipe all the nodes and links in the lab.
 
         :param wait: Wait for convergence (if left at default,
             the lab wait property takes precedence)
         """
         url = self.lab_base_url + "/wipe"
         self._session.put(url)
         if self.need_to_wait(wait):
             self.wait_until_lab_converged()
-        _LOGGER.debug("wiped lab: %s", self._lab_id)
+        _LOGGER.debug("wiped lab: %s", self._id)
 
     def remove(self) -> None:
         """
         Removes the lab from the server. The lab has to
         be stopped and wiped for this to work.
 
         Use carefully, it removes current lab::
 
             lab.remove()
 
         """
-        # TODO: mark as disconnected
+        self._remove_on_server()
+        self._stale = True
+
+    @check_stale
+    def _remove_on_server(self):
         url = self.lab_base_url
         response = self._session.delete(url)
         _LOGGER.debug("removed lab: %s", response.text)
 
-    def sync_events(self) -> None:
-        # TODO: return a boolean if events have changed since last run
+    @check_stale
+    @locked
+    def sync_events(self) -> bool:
         url = self.lab_base_url + "/events"
         result = self._session.get(url).json()
+        changed = self.events != result
         self.events = result
+        return changed
 
+    @check_stale
     def build_configurations(self) -> None:
         """
         Build basic configurations for all nodes in the lab which
         do not already have a configuration and also do support
         configuration building.
         """
-        url = "build_configurations?lab_id=" + self._lab_id
+        url = "build_configurations?lab_id=" + self._id
         self._session.get(url)
         # sync to get the updated configs
         self.sync_topology_if_outdated()
 
+    @check_stale
+    @locked
     def sync(
         self,
         topology_only=True,
         with_node_configurations: Optional[bool] = None,
         exclude_configurations=False,
     ) -> None:
         """
@@ -1008,14 +1105,15 @@
         self._sync_topology(exclude_configurations)
 
         if not topology_only:
             self.sync_statistics()
             self.sync_layer3_addresses()
             self.sync_operational()
 
+    @locked
     def _sync_topology(self, exclude_configurations=False) -> None:
         """Helper function to sync topologies from the backend server."""
         # TODO: check what happens if call twice
         url = self.lab_base_url + "/topology"
         params = {"exclude_configurations": exclude_configurations}
         try:
             result = self._session.get(url, params=params)
@@ -1024,31 +1122,38 @@
             try:
                 # Get the error message from the API's JSON error object.
                 error_msg = json.loads(error_msg)["description"]
             except (ValueError, TypeError, KeyError):
                 # response.text was empty, not a JSON object, or not the expected
                 # JSON schema. Use the raw result text.
                 pass
+            if (
+                exc.response.status_code == 404
+                and f"Lab not found: {self._id}" in exc.response.text
+            ):
+                self._stale = True
             raise LabNotFound("Error syncing lab: {}".format(error_msg))
             # TODO: get the error message from response/headers also?
         topology = result.json()
         if self._initialized:
             self.update_lab(topology, exclude_configurations)
         else:
             self.import_lab(topology)
             self._initialized = True
         self._last_sync_topology_time = time.time()
 
+    @locked
     def import_lab(self, topology: dict) -> None:
         self._import_lab(topology)
 
         self._handle_import_nodes(topology)
         self._handle_import_interfaces(topology)
         self._handle_import_links(topology)
 
+    @locked
     def _import_lab(self, topology: dict[str, Any]) -> None:
         """Replaces lab properties. Will raise KeyError if any property is missing."""
         lab_dict = topology.get("lab")
         if lab_dict is None:
             warnings.warn(
                 "Labs created in older CML releases (schema version 0.0.5 or lower) "
                 "are deprecated. Use labs with schema version 0.1.0 or higher instead.",
@@ -1060,14 +1165,15 @@
             self._owner = topology.get("lab_owner", self.username)
         else:
             self._title = lab_dict["title"]
             self._description = lab_dict["description"]
             self._notes = lab_dict["notes"]
             self._owner = lab_dict.get("owner", self.username)
 
+    @locked
     def _handle_import_nodes(self, topology: dict) -> None:
         for node in topology["nodes"]:
             node_id = node["id"]
             if node_id in self._nodes:
                 raise ElementAlreadyExists("Node already exists")
             interfaces = node.pop("interfaces", [])
             self._import_node(node_id, node)
@@ -1077,65 +1183,76 @@
 
             for iface in interfaces:
                 iface_id = iface["id"]
                 if iface_id in self._interfaces:
                     raise ElementAlreadyExists("Interface already exists")
                 self._import_interface(iface_id, node_id, iface)
 
+    @locked
     def _handle_import_interfaces(self, topology: dict) -> None:
         if "interfaces" in topology:
             for iface in topology["interfaces"]:
                 iface_id = iface["id"]
                 node_id = iface["node"]
                 if iface_id in self._interfaces:
                     raise ElementAlreadyExists("Interface already exists")
                 self._import_interface(iface_id, node_id, iface)
 
+    @locked
     def _handle_import_links(self, topology: dict) -> None:
         for link in topology["links"]:
             link_id = link["id"]
             if link_id in self._links:
                 raise ElementAlreadyExists("Link already exists")
             iface_a_id = link["interface_a"]
             iface_b_id = link["interface_b"]
             label = link.get("label")
             self._import_link(link_id, iface_b_id, iface_a_id, label)
 
+    @locked
     def _import_link(
         self,
         link_id: str,
         iface_b_id: str,
         iface_a_id: str,
         label: Optional[str] = None,
     ) -> Link:
         iface_a = self._interfaces[iface_a_id]
         iface_b = self._interfaces[iface_b_id]
-        return self.create_link_local(iface_a, iface_b, link_id, label)
+        return self._create_link_local(iface_a, iface_b, link_id, label)
 
+    @locked
     def _import_interface(
         self, iface_id: str, node_id: str, iface_data: dict
     ) -> Interface:
         if "data" in iface_data:
             iface_data = iface_data["data"]
         label = iface_data["label"]
         slot = iface_data.get("slot")
         iface_type = iface_data["type"]
         node = self._nodes[node_id]
-        return self.create_interface_local(iface_id, label, node, slot, iface_type)
+        return self._create_interface_local(iface_id, label, node, slot, iface_type)
 
+    @locked
     def _import_node(self, node_id: str, node_data: dict) -> Node:
         if "data" in node_data:
             node_data = node_data["data"]
         node_data.pop("id", None)
-        node_data.pop("state", None)
+        state = node_data.pop("state", None)
+        node_data.pop("lab_id", None)
+        node_data.pop("boot_progress", None)
+
         for key in ("image_definition", "configuration"):
             if key not in node_data:
                 node_data[key] = None
-        return self.add_node_local(node_id, **node_data)
+        node = self._create_node_local(node_id, **node_data)
+        node._state = state
+        return node
 
+    @locked
     def update_lab(self, topology: dict, exclude_configurations: bool) -> None:
         self._import_lab(topology)
 
         # add in order: node -> interface -> link
         # remove in reverse, eg link -> interface -> node
         existing_node_keys = set(self._nodes)
         existing_link_keys = set(self._links)
@@ -1169,35 +1286,37 @@
         # kept elements
         kept_nodes = update_node_keys.intersection(existing_node_keys)
         # kept_links = update_link_keys.intersection(existing_link_keys)
         # kept_interfaces = update_interface_keys.intersection(existing_interface_keys)
 
         self._update_elements(topology, kept_nodes, exclude_configurations)
 
+    @locked
     def _remove_elements(
         self,
         removed_nodes: Iterable[str],
         removed_links: Iterable[str],
         removed_interfaces: Iterable[str],
     ) -> None:
         for link_id in removed_links:
-            link = self._links[link_id]
+            link = self._links.pop(link_id)
             _LOGGER.info("Removed link %s", link)
-            del self._links[link_id]
+            link._stale = True
 
         for interface_id in removed_interfaces:
-            interface = self._interfaces[interface_id]
+            interface = self._interfaces.pop(interface_id)
             _LOGGER.info("Removed interface %s", interface)
-            del self._interfaces[interface_id]
+            interface._stale = True
 
         for node_id in removed_nodes:
-            node = self._nodes[node_id]
+            node = self._nodes.pop(node_id)
             _LOGGER.info("Removed node %s", node)
-            del self._nodes[node_id]
+            node._stale = True
 
+    @locked
     def _add_elements(
         self,
         topology: dict,
         new_nodes: Iterable[str],
         new_links: Iterable[str],
         new_interfaces: Iterable[str],
     ) -> None:
@@ -1228,14 +1347,15 @@
             link_data = self._find_link_in_topology(link_id, topology)
             iface_a_id = link_data["interface_a"]
             iface_b_id = link_data["interface_b"]
             label = link_data.get("label")
             link = self._import_link(link_id, iface_b_id, iface_a_id, label)
             _LOGGER.info("Added link %s", link)
 
+    @locked
     def _update_elements(
         self, topology: dict, kept_nodes: Iterable[str], exclude_configurations: bool
     ) -> None:
         for node_id in kept_nodes:
             node = self._find_node_in_topology(node_id, topology)
             lab_node = self._nodes[node_id]
             lab_node.update(node, exclude_configurations)
@@ -1244,14 +1364,24 @@
         # for interface_id in kept_interfaces:
         #     interface_data = self._find_interface_in_topology(interface_id, topology)
 
         # For now, can't update link data server-side, this will change with tags
         # for link_id in kept_links:
         #     link_data = self._find_link_in_topology(link_id, topology)
 
+    @locked
+    def update_lab_properties(self, properties: dict[str, Any]):
+        """Updates lab properties. Will not modify unspecified properties.
+        Is not compatible with schema version 0.0.5."""
+        # TODO: Should it be?
+        self._title = properties.get("title", self._title)
+        self._description = properties.get("description", self._description)
+        self._notes = properties.get("notes", self._notes)
+        self._owner = properties.get("owner", self._owner)
+
     @staticmethod
     def _find_link_in_topology(link_id: str, topology: dict) -> dict:
         for link in topology["links"]:
             if link["id"] == link_id:
                 return link
         # if it cannot be found, it is an internal structure error
         raise LinkNotFound
@@ -1269,14 +1399,15 @@
     def _find_node_in_topology(node_id: str, topology: dict) -> dict:
         for node in topology["nodes"]:
             if node["id"] == node_id:
                 return node
         # if it cannot be found, it is an internal structure error
         raise NodeNotFound
 
+    @check_stale
     def get_pyats_testbed(self, hostname: Optional[str] = None) -> str:
         """
         Return lab's pyATS YAML testbed. Example usage::
 
             from pyats.topology import loader
 
             lab = client_library.join_existing_lab("lab_1")
@@ -1295,31 +1426,35 @@
         url = self.lab_base_url + "/pyats_testbed"
         params = {}
         if hostname is not None:
             params["hostname"] = hostname
         result = self._session.get(url, params=params)
         return result.text
 
+    @check_stale
     def sync_pyats(self) -> None:
         self.pyats.sync_testbed(self.username, self.password)
 
+    def cleanup_pyats_connections(self) -> None:
+        """Closes and cleans up connection that pyATS might still hold."""
+        self.pyats.cleanup()
+
+    @check_stale
+    @locked
     def sync_layer3_addresses(self) -> None:
         """Syncs all layer 3 IP addresses from the backend server."""
         url = self.lab_base_url + "/layer3_addresses"
         result: dict[str, dict] = self._session.get(url).json()
         for node_id, node_data in result.items():
             node = self.get_node_by_id(node_id)
             mapping = node_data.get("interfaces", {})
             node.map_l3_addresses_to_interfaces(mapping)
         self._last_sync_l3_address_time = time.time()
 
-    def cleanup_pyats_connections(self) -> None:
-        """Closes and cleans up connection that pyATS might still hold."""
-        self.pyats.cleanup()
-
+    @check_stale
     def download(self) -> str:
         """
         Download the lab from the server in YAML format.
 
         :returns: The lab in YAML format
         """
         url = self.lab_base_url + "/download"
@@ -1331,26 +1466,57 @@
         Returns the groups this lab is associated with.
 
         :return: associated groups
         """
         url = self.lab_base_url + "/groups"
         return self._session.get(url).json()
 
+    @check_stale
     def update_lab_groups(
         self, group_list: list[dict[str, str]]
     ) -> list[dict[str, str]]:
         """
         Modifies lab / group association
 
         :param group_list: list of objects consisting of group id and permission
         :return: updated objects consisting of group id and permission
         """
         url = self.lab_base_url + "/groups"
         return self._session.put(url, json=group_list).json()
 
+    @property
+    def connector_mappings(self) -> list[dict[str, Any]]:
+        """Retrieve lab's external connector mappings
+
+        Returns a list of mappings; each mapping has a key, which is used
+        as the configuration of external connector nodes, and a device name,
+        used to uniquely identify the controller host's bridge to use.
+        If unset, the mapping is invalid and nodes using it cannot start.
+        """
+        url = self.lab_base_url + "/connector_mappings"
+        return self._session.get(url).json()
+
+    def update_connector_mappings(
+        self, updates: list[dict[str, str]]
+    ) -> list[dict[str, str]]:
+        """Update lab's external connector mappings
+
+        Accepts a list of mappings, each with a key to add or modify,
+        and the associated device name (bridge) of the controller host.
+        If no running external connector node uses this key, the device_name
+        value may be None to disassociate the bridge from the key; if no node
+        uses this key in its configuration, the mapping entry is removed.
+
+        Returns all connector mappings after updates were applied.
+        """
+        url = self.lab_base_url + "/connector_mappings"
+        return self._session.patch(url, json=updates).json()
+
+    @check_stale
+    @locked
     def sync_operational(self) -> None:
         url = self.lab_base_url + "/resource_pools"
         response = self._session.get(url).json()
         res_pools = self._resource_pool_manager.get_resource_pools_by_ids(response)
         self._resource_pools = list(res_pools.values())
         self._last_sync_operational_time = time.time()
```

### Comparing `virl2_client-2.5.0/virl2_client/models/licensing.py` & `virl2_client-2.6.0/virl2_client/models/licensing.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
 _LOGGER = logging.getLogger(__name__)
 
 DEFAULT_PROXY_SERVER = None
 DEFAULT_PROXY_PORT = None
 
 
 class Licensing:
-
     max_wait = 30
     wait_interval = 1.5
 
     def __init__(self, session: httpx.Client) -> None:
         self._session = session
 
     @property
```

### Comparing `virl2_client-2.5.0/virl2_client/models/link.py` & `virl2_client-2.6.0/virl2_client/models/link.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,17 +18,21 @@
 # limitations under the License.
 #
 
 from __future__ import annotations
 
 import logging
 import time
+import warnings
 from functools import total_ordering
 from typing import TYPE_CHECKING, Optional
 
+from ..utils import check_stale, locked
+from ..utils import property_s as property
+
 if TYPE_CHECKING:
     import httpx
 
     from .interface import Interface
     from .lab import Lab
     from .node import Node
 
@@ -51,31 +55,74 @@
 
         :param lab: the lab object
         :param lid: the link ID
         :param iface_a: the first interface of the link
         :param iface_b: the second interface of the link
         :param label: the link label
         """
-        self.id = lid
-        self.interface_a = iface_a
-        self.interface_b = iface_b
+        self._id = lid
+        self._interface_a = iface_a
+        self._interface_b = iface_b
         self._label = label
         self.lab = lab
         self._session: httpx.Client = lab.session
         self._state: Optional[str] = None
+        self._stale = False
         self.statistics = {
             "readbytes": 0,
             "readpackets": 0,
             "writebytes": 0,
             "writepackets": 0,
         }
 
+    def __str__(self):
+        return f"Link: {self._label}{' (STALE)' if self._stale else ''}"
+
+    def __repr__(self):
+        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
+            self.__class__.__name__,
+            str(self.lab),
+            self._id,
+            self._interface_a,
+            self._interface_b,
+            self._label,
+        )
+
+    def __eq__(self, other: object):
+        if not isinstance(other, Link):
+            return False
+        return self._id == other._id
+
+    def __lt__(self, other: object):
+        if not isinstance(other, Link):
+            return False
+        return self._id < other._id
+
+    def __hash__(self):
+        return hash(self._id)
+
     @property
+    def id(self):
+        return self._id
+
+    @property
+    def interface_a(self):
+        return self._interface_a
+
+    @property
+    def interface_b(self):
+        return self._interface_b
+
+    @property
+    @locked
     def state(self) -> Optional[str]:
         self.lab.sync_states_if_outdated()
+        if self._state is None:
+            url = self.base_url
+            self._state = self._session.get(url).json()["state"]
         return self._state
 
     @property
     def readbytes(self) -> int:
         self.lab.sync_statistics_if_outdated()
         return self.statistics["readbytes"]
 
@@ -90,66 +137,43 @@
         return self.statistics["writebytes"]
 
     @property
     def writepackets(self) -> int:
         self.lab.sync_statistics_if_outdated()
         return self.statistics["writepackets"]
 
-    def __str__(self):
-        return "Link: {}".format(self.id)
-
-    def __repr__(self):
-        return "{}({!r}, {!r}, {!r}, {!r}, {!r})".format(
-            self.__class__.__name__,
-            str(self.lab),
-            self.id,
-            self.interface_a,
-            self.interface_b,
-            self.label,
-        )
-
-    def __eq__(self, other: object):
-        if not isinstance(other, Link):
-            return False
-        return self.id == other.id
-
-    def __lt__(self, other: object):
-        if not isinstance(other, Link):
-            return False
-        return int(self.id) < int(other.id)
-
-    def __hash__(self):
-        return hash(self.id)
-
     @property
     def node_a(self) -> Node:
         self.lab.sync_topology_if_outdated()
         return self.interface_a.node
 
     @property
     def node_b(self) -> Node:
         self.lab.sync_topology_if_outdated()
         return self.interface_b.node
 
     @property
+    @locked
     def nodes(self) -> tuple[Node, Node]:
         """Return nodes this link connects."""
         self.lab.sync_topology_if_outdated()
         return self.node_a, self.node_b
 
     @property
+    @locked
     def interfaces(self) -> tuple[Interface, Interface]:
         self.lab.sync_topology_if_outdated()
         return self.interface_a, self.interface_b
 
     @property
     def label(self) -> Optional[str]:
         self.lab.sync_topology_if_outdated()
         return self._label
 
+    @locked
     def as_dict(self) -> dict[str, str]:
         return {
             "id": self.id,
             "interface_a": self.interface_a.id,
             "interface_b": self.interface_b.id,
         }
 
@@ -157,19 +181,30 @@
     def lab_base_url(self) -> str:
         return self.lab.lab_base_url
 
     @property
     def base_url(self) -> str:
         return self.lab_base_url + "/links/{}".format(self.id)
 
-    def remove_on_server(self) -> None:
+    def remove(self):
+        self.lab.remove_link(self)
+
+    @check_stale
+    def _remove_on_server(self) -> None:
         _LOGGER.info("Removing link %s", self)
         url = self.base_url
         self._session.delete(url)
 
+    def remove_on_server(self) -> None:
+        warnings.warn(
+            "'Link.remove_on_server()' is deprecated, use 'Link.remove()' instead.",
+            DeprecationWarning,
+        )
+        self._remove_on_server()
+
     def wait_until_converged(
         self, max_iterations: Optional[int] = None, wait_time: Optional[int] = None
     ) -> None:
         _LOGGER.info("Waiting for link %s to converge", self.id)
         max_iter = (
             self.lab.wait_max_iterations if max_iterations is None else max_iterations
         )
@@ -195,71 +230,73 @@
         _LOGGER.error(msg)
         # after maximum retries are exceeded and link has not converged
         # error must be raised - it makes no sense to just log info
         # and let client fail with something else if wait is explicitly
         # specified
         raise RuntimeError(msg)
 
+    @check_stale
     def has_converged(self) -> bool:
         url = self.base_url + "/check_if_converged"
         converged = self._session.get(url).json()
         return converged
 
+    @check_stale
     def start(self, wait: Optional[bool] = None) -> None:
         url = self.base_url + "/state/start"
         self._session.put(url)
         if self.lab.need_to_wait(wait):
             self.wait_until_converged()
 
+    @check_stale
     def stop(self, wait: Optional[bool] = None) -> None:
         url = self.base_url + "/state/stop"
         self._session.put(url)
         if self.lab.need_to_wait(wait):
             self.wait_until_converged()
 
+    @check_stale
     def set_condition(
         self, bandwidth: int, latency: int, jitter: int, loss: float
     ) -> None:
         """
         Applies conditioning to this link.
 
         :param bandwidth: desired bandwidth, 0-10000000 kbps
-        :type bandwidth: int
         :param latency: desired latency, 0-10000 ms
-        :type latency: int
         :param jitter: desired jitter, 0-10000 ms
-        :type jitter: int
         :param loss: desired loss, 0-100%
-        :type loss: float
         """
         url = self.base_url + "/condition"
         data = {
             "bandwidth": bandwidth,
             "latency": latency,
             "jitter": jitter,
             "loss": loss,
         }
         self._session.patch(url, json=data)
 
-    def get_condition(self) -> Optional[dict]:
+    @check_stale
+    def get_condition(self) -> dict:
         """
         Retrieves the current condition on this link.
-        If there is no link condition specified, None is returned.
+        If there is no link condition applied, an empty dictionary is returned.
+
+        (Note: this used to (erroneously) say None would be returned
+        when no condition is applied, but that was never the case.)
 
         :return: the applied link condition
         """
         url = self.base_url + "/condition"
         condition = self._session.get(url).json()
-        if condition is None:
-            return None
-
         keys = ["bandwidth", "latency", "jitter", "loss"]
         result = {k: v for (k, v) in condition.items() if k in keys}
         return result
 
+    @check_stale
     def remove_condition(self) -> None:
         """
         Removes link conditioning.
         If there's no condition applied then this is a no-op for the controller.
         """
         url = self.base_url + "/condition"
         self._session.delete(url)
```

### Comparing `virl2_client-2.5.0/virl2_client/models/node.py` & `virl2_client-2.6.0/virl2_client/models/node.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 #
+#
 # This file is part of VIRL 2
 # Copyright (c) 2019-2023, Cisco Systems, Inc.
 # All rights reserved.
 #
 # Python bindings for the Cisco VIRL 2 Network Simulation Platform
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
@@ -23,14 +24,16 @@
 import logging
 import time
 import warnings
 from functools import total_ordering
 from typing import TYPE_CHECKING, Any, Optional
 
 from ..exceptions import InterfaceNotFound
+from ..utils import check_stale, locked
+from ..utils import property_s as property
 
 if TYPE_CHECKING:
     import httpx
 
     from .interface import Interface
     from .lab import Lab
     from .link import Link
@@ -79,15 +82,15 @@
         :param data_volume: Size in GiB of 2nd HDD (if > 0)
         :param boot_disk_size: Size in GiB of boot disk (will expand to this size)
         :param hide_links: Whether node's links should be hidden in UI visualization
         :param tags: List of tags
         :param resource_pool: A resource pool ID if the node is in a resource pool
         """
         self.lab = lab
-        self.id = nid
+        self._id = nid
         self._label = label
         self._node_definition = node_definition
         self._x = x
         self._y = y
         self._state: Optional[str] = None
         self._session: httpx.Client = lab.session
         self._image_definition = image_definition
@@ -97,31 +100,32 @@
         self._cpu_limit = cpu_limit
         self._data_volume = data_volume
         self._boot_disk_size = boot_disk_size
         self._hide_links = hide_links
         self._tags = tags
         self._compute_id: Optional[str] = None
         self._resource_pool = resource_pool
+        self._stale = False
 
         self.statistics: dict[str, int | float] = {
             "cpu_usage": 0,
             "disk_read": 0,
             "disk_write": 0,
         }
 
     def __str__(self):
-        return "Node: {}".format(self._label)
+        return f"Node: {self._label}{' (STALE)' if self._stale else ''}"
 
     def __repr__(self):
         return (
             "{}({!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, "
             "{!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r}, {!r})".format(
                 self.__class__.__name__,
                 str(self.lab),
-                self.id,
+                self._id,
                 self._label,
                 self._node_definition,
                 self._image_definition,
                 self._configuration,
                 self._x,
                 self._y,
                 self._ram,
@@ -133,160 +137,176 @@
                 self._tags,
             )
         )
 
     def __eq__(self, other):
         if not isinstance(other, Node):
             return False
-        return self.id == other.id
+        return self._id == other._id
 
     def __lt__(self, other):
         if not isinstance(other, Node):
             return False
-        return int(self.id) < int(other.id)
+        return self._id < other._id
 
     def __hash__(self):
-        return hash(self.id)
+        return hash(self._id)
 
     @property
+    @locked
     def state(self) -> Optional[str]:
         self.lab.sync_states_if_outdated()
         if self._state is None:
             url = self._base_url + "/state"
             self._state = self._session.get(url).json()["state"]
         return self._state
 
-    @state.setter
-    def state(self, value: Optional[str]) -> None:
-        self._state = value
-
+    @check_stale
+    @locked
     def interfaces(self) -> list[Interface]:
-        self.lab.sync_topology_if_outdated()
+        # self.lab.sync_topology_if_outdated()
         return [iface for iface in self.lab.interfaces() if iface.node is self]
 
+    @locked
     def physical_interfaces(self) -> list[Interface]:
-        self.lab.sync_topology_if_outdated()
+        # self.lab.sync_topology_if_outdated()
         return [iface for iface in self.interfaces() if iface.physical]
 
+    @check_stale
+    @locked
     def create_interface(
         self, slot: Optional[int] = None, wait: bool = False
     ) -> Interface:
         """
         Create an interface in the specified slot or, if no slot is given, in the
         next available slot.
 
         :param slot: (optional)
         :param wait: Wait for the creation
         :returns: The newly created interface
-        :rtype: models.Interface
         """
         return self.lab.create_interface(self, slot, wait=wait)
 
+    @locked
     def next_available_interface(self) -> Optional[Interface]:
         """
         Returns the next available physical interface on this node.
 
         Note: On XR 9000v, the first two physical interfaces are marked
         as "do not use"... Only the third physical interface can be used
         to connect to other nodes!
 
         :returns: an interface or None, if all existing ones are connected
-        :rtype: models.Interface
         """
         for iface in self.interfaces():
             if not iface.connected and iface.physical:
                 return iface
         return None
 
+    @locked
     def peer_interfaces(self) -> list[Interface]:
         peer_ifaces = []
         for iface in self.interfaces():
             peer_iface = iface.peer_interface
             if peer_iface is not None and peer_iface not in peer_ifaces:
                 peer_ifaces.append(peer_iface)
         return peer_ifaces
 
+    @locked
     def peer_nodes(self) -> list[Node]:
         return list({iface.node for iface in self.peer_interfaces()})
 
+    @locked
     def links(self) -> list[Link]:
         return list(
             {link for iface in self.interfaces() if (link := iface.link) is not None}
         )
 
+    @locked
     def degree(self) -> int:
         self.lab.sync_topology_if_outdated()
         return len(self.links())
 
     @property
+    def id(self) -> str:
+        return self._id
+
+    @property
     def label(self) -> str:
         self.lab.sync_topology_if_outdated()
         return self._label
 
     @label.setter
+    @locked
     def label(self, value: str) -> None:
         self._set_node_property("label", value)
         self._label = value
 
     @property
     def x(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._x
 
     @x.setter
+    @locked
     def x(self, value: int) -> None:
         self._set_node_property("x", value)
         self._x = value
 
     @property
     def y(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._y
 
     @y.setter
+    @locked
     def y(self, value: int) -> None:
         self._set_node_property("y", value)
         self._y = value
 
     @property
     def ram(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._ram
 
     @ram.setter
+    @locked
     def ram(self, value: int) -> None:
         self._set_node_property("ram", value)
         self._ram = value
 
     @property
     def cpus(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._cpus
 
     @cpus.setter
+    @locked
     def cpus(self, value: int) -> None:
         self._set_node_property("cpus", value)
         self._cpus = value
 
     @property
     def cpu_limit(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._cpu_limit
 
     @cpu_limit.setter
+    @locked
     def cpu_limit(self, value: int) -> None:
         self._set_node_property("cpu_limit", value)
         self._cpu_limit = value
 
     @property
     def data_volume(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._data_volume
 
     @data_volume.setter
+    @locked
     def data_volume(self, value: int) -> None:
         self._set_node_property("data_volume", value)
         self._data_volume = value
 
     @property
     def hide_links(self) -> bool:
         self.lab.sync_topology_if_outdated()
@@ -299,14 +319,15 @@
 
     @property
     def boot_disk_size(self) -> int:
         self.lab.sync_topology_if_outdated()
         return self._boot_disk_size
 
     @boot_disk_size.setter
+    @locked
     def boot_disk_size(self, value: int) -> None:
         self._set_node_property("boot_disk_size", value)
         self._boot_disk_size = value
 
     @property
     def configuration(self) -> Optional[str]:
         # TODO: auto sync if out of date
@@ -319,24 +340,26 @@
 
     @property
     def config(self) -> Optional[str]:
         warnings.warn(CONFIG_WARNING, DeprecationWarning)
         return self.configuration
 
     @config.setter
+    @locked
     def config(self, value: str) -> None:
         warnings.warn(CONFIG_WARNING, DeprecationWarning)
         self.configuration = value
 
     @property
     def image_definition(self) -> Optional[str]:
         self.lab.sync_topology_if_outdated()
         return self._image_definition
 
     @image_definition.setter
+    @locked
     def image_definition(self, value: str) -> None:
         self.lab.sync_topology_if_outdated()
         self._set_node_property("image_definition", value)
         self._image_definition = value
 
     @property
     def node_definition(self) -> str:
@@ -372,20 +395,22 @@
         return round(self.statistics["disk_read"] / 1048576)
 
     @property
     def disk_write(self) -> int:
         self.lab.sync_statistics_if_outdated()
         return round(self.statistics["disk_write"] / 1048576)
 
+    @locked
     def get_interface_by_label(self, label: str) -> Interface:
         for iface in self.interfaces():
             if iface.label == label:
                 return iface
         raise InterfaceNotFound("{}:{}".format(label, self))
 
+    @locked
     def get_interface_by_slot(self, slot: int) -> Interface:
         for iface in self.interfaces():
             if iface.slot == slot:
                 return iface
         raise InterfaceNotFound("{}:{}".format(slot, self))
 
     def get_links_to(self, other_node: Node) -> list[Link]:
@@ -409,14 +434,15 @@
         :returns: a link, if one exists
         """
         for link in self.links():
             if other_node in link.nodes:
                 return link
         return None
 
+    @check_stale
     def wait_until_converged(
         self, max_iterations: Optional[int] = None, wait_time: Optional[int] = None
     ) -> None:
         _LOGGER.info("Waiting for node %s to converge", self.id)
         max_iter = (
             self.lab.wait_max_iterations if max_iterations is None else max_iterations
         )
@@ -442,69 +468,91 @@
         _LOGGER.error(msg)
         # after maximum retries are exceeded and node has not converged
         # error must be raised - it makes no sense to just log info
         # and let client fail with something else if wait is explicitly
         # specified
         raise RuntimeError(msg)
 
+    @check_stale
     def has_converged(self) -> bool:
         url = self._base_url + "/check_if_converged"
         return self._session.get(url).json()
 
+    @check_stale
     def start(self, wait=False) -> None:
         url = self._base_url + "/state/start"
         self._session.put(url)
         if self.lab.need_to_wait(wait):
             self.wait_until_converged()
 
+    @check_stale
     def stop(self, wait=False) -> None:
         url = self._base_url + "/state/stop"
         self._session.put(url)
         if self.lab.need_to_wait(wait):
             self.wait_until_converged()
 
+    @check_stale
     def wipe(self, wait=False) -> None:
         url = self._base_url + "/wipe_disks"
         self._session.put(url)
         if self.lab.need_to_wait(wait):
             self.wait_until_converged()
 
+    @check_stale
     def extract_configuration(self) -> None:
         url = self._base_url + "/extract_configuration"
         self._session.put(url)
 
+    @check_stale
     def console_logs(self, console_id: int, lines: Optional[int] = None) -> dict:
         query = "?lines=%d" % lines if lines else ""
         url = self._base_url + "/consoles/%d/log%s" % (console_id, query)
         return self._session.get(url).json()
 
+    @check_stale
     def console_key(self) -> str:
         url = self._base_url + "/keys/console"
         return self._session.get(url).json()
 
+    @check_stale
     def vnc_key(self) -> str:
         url = self._base_url + "/keys/vnc"
         return self._session.get(url).json()
 
-    def remove_on_server(self) -> None:
+    def remove(self) -> None:
+        self.lab.remove_node(self)
+
+    @check_stale
+    def _remove_on_server(self) -> None:
         _LOGGER.info("Removing node %s", self)
         url = self._base_url
         self._session.delete(url)
 
+    def remove_on_server(self) -> None:
+        warnings.warn(
+            "'Node.remove_on_server()' is deprecated, use 'Node.remove()' instead.",
+            DeprecationWarning,
+        )
+        self._remove_on_server()
+
+    @check_stale
     def tags(self) -> list[str]:
         """Returns the tags set on this node"""
         self.lab.sync_topology_if_outdated()
         return self._tags
 
+    @locked
     def add_tag(self, tag: str) -> None:
         current = self.tags()
         if tag not in current:
             current.append(tag)
             self._set_node_property("tags", current)
 
+    @locked
     def remove_tag(self, tag: str) -> None:
         current = self.tags()
         current.remove(tag)
         self._set_node_property("tags", current)
 
     def run_pyats_command(self, command: str) -> str:
         """Run a pyATS command in exec mode.
@@ -520,52 +568,61 @@
 
         :param command: the command (like "interface gi0")
         :returns: the output from the device
         """
         label = self.label
         return self.lab.pyats.run_config_command(label, command)
 
+    @check_stale
+    @locked
     def sync_layer3_addresses(self) -> None:
         """Acquire all L3 addresses from the controller. For this
         to work, the device has to be attached to the external network
         in bridge mode and must run DHCP to acquire an IP address.
         """
         # TODO: can optimise the sync of l3 to only be for the node
         # rather than whole lab
         url = self._base_url + "/layer3_addresses"
         result = self._session.get(url).json()
         interfaces = result.get("interfaces", {})
         self.map_l3_addresses_to_interfaces(interfaces)
 
+    @check_stale
+    @locked
     def sync_operational(self, response: dict[str, Any] = None):
         if response is None:
             url = self._base_url + "?operational=true"
             response = self._session.get(url).json()
         operational = response.get("operational", {})
         self._compute_id = operational.get("compute_id")
         self._resource_pool = operational.get("resource_pool")
 
+    @check_stale
+    @locked
     def map_l3_addresses_to_interfaces(
         self, mapping: dict[str, dict[str, str]]
     ) -> None:
         for mac_address, entry in mapping.items():
             label = entry.get("label")
             if not label:
                 continue
             ipv4 = entry.get("ip4")
             ipv6 = entry.get("ip6")
-            iface = self.get_interface_by_label(label)
-            if not iface:
+            try:
+                iface = self.get_interface_by_label(label)
+            except InterfaceNotFound:
                 continue
             iface.ip_snooped_info = {
                 "mac_address": mac_address,
                 "ipv4": ipv4,
                 "ipv6": ipv6,
             }
 
+    @check_stale
+    @locked
     def update(
         self,
         node_data: dict[str, Any],
         exclude_configurations: bool,
         push_to_server: bool = False,
     ) -> None:
         if push_to_server:
@@ -588,9 +645,10 @@
     def is_booted(self) -> bool:
         return self.state == "BOOTED"
 
     def _set_node_property(self, key: str, val: Any) -> None:
         _LOGGER.debug("Setting node property %s %s: %s", self, key, val)
         self._set_node_properties({key: val})
 
+    @check_stale
     def _set_node_properties(self, node_data: dict[str, Any]) -> None:
         self._session.patch(url=self._base_url, json=node_data)
```

### Comparing `virl2_client-2.5.0/virl2_client/models/node_image_definitions.py` & `virl2_client-2.6.0/virl2_client/models/node_image_definitions.py`

 * *Files 17% similar despite different names*

```diff
@@ -16,30 +16,26 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 from __future__ import annotations
 
-import logging
 import os
 import pathlib
 import time
 import warnings
 from typing import TYPE_CHECKING, BinaryIO, Callable, Optional
 
-from virl2_client.exceptions import InvalidImageFile
+from virl2_client.exceptions import InvalidContentType, InvalidImageFile
 
 if TYPE_CHECKING:
     import httpx
 
 
-_LOGGER = logging.getLogger(__name__)
-
-
 class NodeImageDefinitions:
     def __init__(self, session: httpx.Client) -> None:
         """
         VIRL2 Definition classes to specify a node VM and associated disk images.
 
         :param session: httpx Client session
         """
@@ -82,41 +78,83 @@
 
         :param definition_id: node definition id
         :returns: list of image definition objects
         """
         url = "node_definitions/" + definition_id + "/image_definitions"
         return self._session.get(url).json()
 
-    def upload_node_definition(self, body, json: bool = False) -> str:
+    def set_image_definition_read_only(
+        self, definition_id: str, read_only: bool
+    ) -> dict:
+        """
+        Set the read-only attribute of the image definition with the given ID.
+
+        :param definition_id: The ID of the image definition.
+        :param read_only: The new value of the read-only attribute.
+        :returns: The modified image definition.
+        """
+        url = f"image_definitions/{definition_id}/read_only"
+        return self._session.put(url, json=read_only).json()
+
+    def set_node_definition_read_only(
+        self, definition_id: str, read_only: bool
+    ) -> dict:
+        """
+        Set the read-only attribute of the node definition with the given ID.
+
+        :param definition_id: The ID of the node definition.
+        :param read_only: The new value of the read-only attribute.
+        :returns: The modified node definition.
+        """
+        url = f"node_definitions/{definition_id}/read_only"
+        return self._session.put(url, json=read_only).json()
+
+    def upload_node_definition(self, body: str | dict, json: bool | None = None) -> str:
         """
-        Upload new node definition.
+        Uploads a new node definition.
 
         :param body: node definition (yaml or json)
-        :type: str or dict
-        :param json: whether we are sending json data
+        :param json: DEPRECATED, replaced with type check
         :return: "Success"
         """
+        is_json = _is_json_content(body)
+        if json is not None:
+            warnings.warn(
+                'The argument "json" is deprecated as the content type is determined '
+                "from the provided body",
+                DeprecationWarning,
+            )
+            is_json = True
         url = "node_definitions/"
-        if json:
+        if is_json:
             return self._session.post(url, json=body).json()
         else:
             # YAML
             return self._session.post(url, content=body).json()
 
-    def upload_image_definition(self, body, json: bool = False) -> str:
+    def upload_image_definition(
+        self, body: str | dict, json: bool | None = None
+    ) -> str:
         """
-        Upload new image definition.
+        Uploads a new image definition.
 
         :param body: image definition (yaml or json)
-        :type: str or dict
-        :param json: whether we are sending json data
+        :param json: DEPRECATED, replaced with type check
         :return: "Success"
         """
+        is_json = _is_json_content(body)
+        if json is not None:
+            warnings.warn(
+                'The argument "json" is deprecated as the content type is determined '
+                "from the provided body",
+                DeprecationWarning,
+            )
+            is_json = True
         url = "image_definitions/"
-        if json:
+        if is_json:
             return self._session.post(url, json=body).json()
         else:
             # YAML
             return self._session.post(url, content=body).json()
 
     def download_node_definition(self, definition_id: str) -> str:
         """
@@ -263,7 +301,15 @@
     print(
         "\r |{}| {}/{} {}% {}".format(bar, cur, total, percent, elapsed),
         end="",
         flush=True,
     )
     if cur == total:
         print()
+
+
+def _is_json_content(content: dict | str) -> bool:
+    if isinstance(content, dict):
+        return True
+    elif isinstance(content, str):
+        return False
+    raise InvalidContentType(type(content))
```

### Comparing `virl2_client-2.5.0/virl2_client/models/resource_pools.py` & `virl2_client-2.6.0/virl2_client/models/resource_pools.py`

 * *Files identical despite different names*

### Comparing `virl2_client-2.5.0/virl2_client/models/users.py` & `virl2_client-2.6.0/virl2_client/models/users.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,16 @@
 # limitations under the License.
 #
 
 from __future__ import annotations
 
 from typing import TYPE_CHECKING, Any, Optional
 
+from ..utils import UNCHANGED
+
 if TYPE_CHECKING:
     import httpx
 
 
 class UserManagement:
     def __init__(self, session: httpx.Client) -> None:
         self._session = session
@@ -94,45 +96,45 @@
         }
         url = self.base_url
         return self._session.post(url, json=data).json()
 
     def update_user(
         self,
         user_id: str,
-        fullname: str = "",
-        description: str = "",
-        groups: list[str] = None,
+        fullname: Optional[str] = UNCHANGED,
+        description: Optional[str] = UNCHANGED,
+        groups: Optional[list[str]] = UNCHANGED,
         admin: Optional[bool] = None,
-        password_dict: dict[str, str] = None,
-        resource_pool: Optional[str] = None,
+        password_dict: Optional[dict[str, str]] = None,
+        resource_pool: Optional[str] = UNCHANGED,
     ) -> dict:
         """
         Updates user.
 
         :param user_id: user uuid4
         :param fullname: full name
         :param description: description
         :param admin: whether to create admin user
         :param groups: adds user to groups specified
         :param password_dict: dict containing old and new passwords
         :param resource_pool: adds user to resource pool specified
         :return: user object
         """
         data: dict[str, Any] = {}
-        if fullname:
+        if fullname is not UNCHANGED:
             data["fullname"] = fullname
-        if description:
+        if description is not UNCHANGED:
             data["description"] = description
         if admin is not None:
             data["admin"] = admin
-        if groups is not None:
+        if groups is not UNCHANGED:
             data["groups"] = groups
         if password_dict is not None:
             data["password"] = password_dict
-        if resource_pool is not None:
+        if resource_pool is not UNCHANGED:
             data["resource_pool"] = resource_pool
 
         url = self.base_url + "/{}".format(user_id)
         return self._session.patch(url, json=data).json()
 
     def user_groups(self, user_id: str) -> list[str]:
         """
```

### Comparing `virl2_client-2.5.0/virl2_client/virl2_client.py` & `virl2_client-2.6.0/virl2_client/virl2_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,31 +23,35 @@
 import json
 import logging
 import os
 import re
 import time
 from functools import lru_cache
 from pathlib import Path
+from threading import RLock
 from typing import Any, NamedTuple, Optional
 from urllib.parse import urljoin, urlsplit, urlunsplit
 
 import httpx
 
 from .exceptions import InitializationError, LabNotFound
 from .models import (
+    AuthManagement,
     GroupManagement,
     Lab,
     Licensing,
     NodeImageDefinitions,
     ResourcePoolManagement,
     SystemManagement,
     TokenAuth,
     UserManagement,
 )
 from .models.authentication import make_session
+from .models.configuration import get_configuration
+from .utils import locked
 
 _LOGGER = logging.getLogger(__name__)
 cached = lru_cache(maxsize=None)  # cache results forever
 
 
 class Version:
     __slots__ = ("version_str", "major", "minor", "patch")
@@ -130,39 +134,41 @@
 
     url: Optional[str] = None
     username: Optional[str] = None
     password: Optional[str] = None
     ssl_verify: bool | str = True
     allow_http: bool = False
     auto_sync: float = 1.0
+    events: bool = False
     raise_for_auth_failure: bool = True
     convergence_wait_max_iter: int = 500
     convergence_wait_time: int | float = 5
 
     def make_client(self) -> ClientLibrary:
         client = ClientLibrary(
             url=self.url,
             username=self.username,
             password=self.password,
             ssl_verify=self.ssl_verify,
             raise_for_auth_failure=self.raise_for_auth_failure,
             allow_http=self.allow_http,
             convergence_wait_max_iter=self.convergence_wait_max_iter,
             convergence_wait_time=self.convergence_wait_time,
+            events=self.events,
         )
-        client.auto_sync = self.auto_sync >= 0.0
         client.auto_sync_interval = self.auto_sync
+        client.auto_sync = self.auto_sync >= 0.0 and not self.events
         return client
 
 
 class ClientLibrary:
     """Python bindings for the REST API of a CML controller."""
 
     # current client version
-    VERSION = Version("2.5.0")
+    VERSION = Version("2.6.0")
     # list of Version objects
     INCOMPATIBLE_CONTROLLER_VERSIONS = [
         Version("2.0.0"),
         Version("2.0.1"),
         Version("2.1.0"),
         Version("2.1.1"),
         Version("2.1.2"),
@@ -177,66 +183,60 @@
         username: Optional[str] = None,
         password: Optional[str] = None,
         ssl_verify: bool | str = True,
         raise_for_auth_failure: bool = False,
         allow_http: bool = False,
         convergence_wait_max_iter: int = 500,
         convergence_wait_time: int | float = 5,
+        events: bool = False,
     ) -> None:
         """
         Initializes a ClientLibrary instance. Note that ssl_verify can
         also be a string that points to a cert (see class documentation).
 
         :param url: URL of controller. It's also possible to pass the
-            URL via the ``VIRL2_URL`` environment variable. If no protocol
-            scheme is provided, "https:" is used.
-        :param username: Username of the user to authenticate
-        :param password: Password of the user to authenticate
+            URL via the ``VIRL2_URL`` or ``VIRL_HOST`` environment variable.
+            If no protocol scheme is provided, "https:" is used.
+        :param username: Username of the user to authenticate. It's also possible
+            to pass the username via ``VIRL2_USER`` or ``VIRL_USERNAME`` variable.
+        :param password: Password of the user to authenticate. It's also possible
+            to pass the password via ``VIRL2_PASS`` or ``VIRL_PASSWORD`` variable.
         :param ssl_verify: Path SSL controller certificate, or True to load
-            from ``CA_BUNDLE`` environment variable, or False to disable
+            from ``CA_BUNDLE`` or ``CML_VERIFY_CERT`` environment variable,
+            or False to disable.
         :param raise_for_auth_failure: Raise an exception if unable
-            to connect to controller (use for scripting scenarios)
+            to connect to controller (use for scripting scenarios).
         :param allow_http: If set, a https URL will not be enforced
         :param convergence_wait_max_iter: maximum number of iterations to wait for
-            lab to converge
+            lab to converge.
         :param convergence_wait_time: wait interval in seconds to wait during one
-            iteration during lab convergence wait
+            iteration during lab convergence wait.
+        :param events: whether to use events - event listeners for state updates and
+            event handlers for custom handling.
         :raises InitializationError: If no URL is provided,
-            authentication fails or host can't be reached
+            authentication fails or host can't be reached.
         """
-
-        url = self._environ_get("VIRL2_URL", url)
-        if url is None or len(url) == 0:
-            message = "no URL provided"
-            raise InitializationError(message)
+        url, username, password, cert = get_configuration(
+            url, username, password, ssl_verify
+        )
+        if cert is not None:
+            ssl_verify = cert
 
         url, base_url = prepare_url(url, allow_http)
-
-        # check environment for username
-        username = self._environ_get("VIRL2_USER", username)
-        if username is None or len(username) == 0:
-            message = "no username provided"
-            raise InitializationError(message)
         self.username: str = username
-
-        # check environment for password
-        password = self._environ_get("VIRL2_PASS", password)
-        if password is None or len(password) == 0:
-            message = "no password provided"
-            raise InitializationError(message)
         self.password: str = password
 
-        if ssl_verify is True:
-            ssl_verify = self._environ_get("CA_BUNDLE", default=True)
-
         if ssl_verify is False:
             _LOGGER.warning("SSL Verification disabled")
 
         self._ssl_verify = ssl_verify
-        self._session = make_session(base_url, ssl_verify)
+        try:
+            self._session = make_session(base_url, ssl_verify)
+        except httpx.InvalidURL as exc:
+            raise InitializationError(exc) from None
         # checks version from system_info against self.VERSION
         self.check_controller_version()
 
         self._session.auth = TokenAuth(self)
         # Note: session.auth is defined in the httpx module to be of type Auth,
         #  which has no logout function; this TokenAuth function will, therefore,
         #  not be visible to a type checker, causing warnings.
@@ -266,24 +266,36 @@
             auto_sync_interval=self.auto_sync_interval,
         )
         self.resource_pool_management = ResourcePoolManagement(
             self._session,
             auto_sync=self.auto_sync,
             auto_sync_interval=self.auto_sync_interval,
         )
+        self.auth_management = AuthManagement(
+            self._session,
+            auto_sync=self.auto_sync,
+            auto_sync_interval=self.auto_sync_interval,
+        )
 
         try:
             self._make_test_auth_call()
         except InitializationError as exc:
             if raise_for_auth_failure:
                 raise
             else:
                 _LOGGER.warning(exc)
                 return
 
+        self.event_listener = None
+        self.session.lock = None
+        if events:
+            # http-based auto sync should be off by default when using events
+            self.auto_sync = False
+            self.start_event_listening()
+
     def __repr__(self):
         return "{}({!r}, {!r}, {!r}, {!r}, {!r}, {!r})".format(
             self.__class__.__name__,
             self.url,
             self.username,
             self.password,
             self._ssl_verify,
@@ -329,14 +341,23 @@
         """
         Returns the used `httpx` client session object.
 
         :returns: The session object
         """
         return self._session
 
+    @property
+    def uuid(self) -> str:
+        """
+        Returns the UUID4 that identifies this client to the server.
+
+        :returns: the UUID4 string
+        """
+        return self._session.headers["X-Client-UUID"]
+
     def logout(self, clear_all_sessions: bool = False) -> None:
         """
         Invalidate current token.
         """
         return self._session.auth.logout(  # type: ignore
             clear_all_sessions=clear_all_sessions
         )
@@ -432,14 +453,40 @@
 
     @staticmethod
     def is_virl_1x(path: Path) -> bool:
         if path.suffix == ".virl":
             return True
         return False
 
+    @locked
+    def start_event_listening(self):
+        """
+        Starts listening for and parsing websocket events.
+
+        To replace the default event handling mechanism,
+        subclass `event_handling.EventHandler` (or `EventHandlerBase` if necessary),
+        then do:
+            self.websockets = event_listening.EventListener(self)
+            self.websockets._event_handler = handler
+        """
+        from .event_listening import EventListener
+
+        if self.event_listener is None:
+            self.event_listener = EventListener(self)
+        if not self.event_listener:
+            self._session.lock = RLock()
+            self.event_listener.start_listening()
+
+    @locked
+    def stop_event_listening(self):
+        if self.event_listener:
+            self.session.lock = None
+            self.event_listener.stop_listening()
+
+    @locked
     def import_lab(
         self,
         topology: str,
         title: Optional[str] = None,
         offline: bool = False,
         virl_1x: bool = False,
     ) -> Lab:
@@ -491,14 +538,15 @@
             topology_dict["lab"]["owner"] = self.user_management.user_id(self.username)
             lab.import_lab(topology_dict)
         else:
             lab.sync()
         self._labs[lab_id] = lab
         return lab
 
+    @locked
     def import_lab_from_path(self, path: str, title: Optional[str] = None) -> Lab:
         """
         Imports an existing topology from a file / path.
 
         :param path: Topology filename / path
         :param title: Title of the lab
         :returns: A Lab instance
@@ -518,56 +566,66 @@
         Returns a dictionary with information about all sample labs available on host.
 
         :returns: A dictionary of sample lab information, where keys are titles
         """
         url = "sample/labs"
         return self._session.get(url).json()
 
+    @locked
     def import_sample_lab(self, title: str) -> Lab:
         """
         Imports a built-in sample lab.
 
         :param title: sample lab name, as returned by get_sample_labs
         :returns: a Lab instance
         """
 
         url = "sample/labs/" + title
         lab_id = self._session.put(url).json()
         return self.join_existing_lab(lab_id)
 
+    @locked
     def all_labs(self, show_all: bool = False) -> list[Lab]:
         """
-        Retrieves a list of all defined labs.
+        Joins all labs owned by this user (or all labs period) and returns their list.
 
         :param show_all: Whether to get only labs owned by the admin or all user labs
         :returns: A list of lab objects
-        :rtype: list[models.Lab]
         """
-        # TODO: integrate this further with local labs - check if already exist
         url = "labs"
         if show_all:
             url += "?show_all=true"
         lab_ids = self._session.get(url).json()
         result = []
         for lab_id in lab_ids:
             lab = self.join_existing_lab(lab_id)
             result.append(lab)
 
         return result
 
+    @locked
+    def _remove_stale_labs(self):
+        for lab in list(self._labs.values()):
+            if lab._stale:
+                self._remove_lab_local(lab)
+
+    @locked
     def local_labs(self) -> list[Lab]:
-        # TODO: first sync with controller to pull all possible labs
-        return [lab for lab in self._labs.values()]
+        self._remove_stale_labs()
+        return list(self._labs.values())
 
+    @locked
     def get_local_lab(self, lab_id: str) -> Lab:
+        self._remove_stale_labs()
         try:
             return self._labs[lab_id]
         except KeyError:
             raise LabNotFound(lab_id)
 
+    @locked
     def create_lab(self, title: Optional[str] = None) -> Lab:
         """
         Creates an empty lab with the given name. If no name is given, then
         the created lab ID is set as the name.
 
         Note that the lab will be auto-syncing according to the Client Library's
         auto-sync setting when created. The lab has a property to override this
@@ -598,27 +656,55 @@
             wait_max_iterations=self.convergence_wait_max_iter,
             wait_time=self.convergence_wait_time,
             resource_pool_manager=self.resource_pool_management,
         )
         self._labs[lab_id] = lab
         return lab
 
-    def remove_lab(self, lab_id: str) -> None:
+    @locked
+    def remove_lab(self, lab_id: str | Lab) -> None:
         """
         Use carefully, it removes a given lab::
 
             client_library.remove_lab("1f6cd7")
 
-        :param lab_id: The lab ID to be removed.
-        :type lab_id: str
+        If you have a lab object, you can also simply do:
+
+            lab.remove()
+
+        :param lab_id: the lab ID or object
         """
+        self._remove_stale_labs()
+        if isinstance(lab_id, Lab):
+            lab_id.remove()
+            self._remove_lab_local(lab_id)
+        elif lab_id in self._labs:
+            self._labs[lab_id].remove()
+            self._remove_lab_local(self._labs[lab_id])
+
+        else:
+            self._remove_unjoined_lab(lab_id)
+
+    @locked
+    def _remove_lab_local(self, lab: Lab) -> None:
+        """Helper function to remove a lab from the client library."""
+        try:
+            del self._labs[lab._id]
+            lab._stale = True
+        except KeyError:
+            # element may already have been deleted on server,
+            # and removed locally due to auto-sync
+            pass
+
+    def _remove_unjoined_lab(self, lab_id: str):
         url = "labs/{}".format(lab_id)
-        self._session.delete(url)
-        self._labs.pop(lab_id, None)
+        response = self._session.delete(url)
+        _LOGGER.debug("removed lab: %s", response.text)
 
+    @locked
     def join_existing_lab(self, lab_id: str, sync_lab: bool = True) -> Lab:
         """
         Creates a new ClientLibrary lab instance that is retrieved
         from the controller.
 
         If `sync_lab` is set to true, then synchronize current lab
         by applying the changes that were done in UI or in another
@@ -628,39 +714,52 @@
 
             lab = client_library.join_existing_lab("2e6a18")
 
         :param lab_id: The lab ID to be joined.
         :param sync_lab: Synchronize changes.
         :returns: A Lab instance
         """
-        # TODO: check if lab exists through REST call
-        title = None
-        # TODO: sync lab name
+        self._remove_stale_labs()
+        if lab_id in self._labs:
+            return self._labs[lab_id]
+        topology = {}
+        if sync_lab:
+            try:
+                # check if lab exists through REST call
+                topology = self.session.get(f"labs/{lab_id}/topology").json()
+            except httpx.HTTPStatusError as exc:
+                if exc.response.status_code == 404:
+                    raise LabNotFound("No lab with the given ID exists on the host.")
+                raise
+            title = topology.get("lab", {}).get("title")
+        else:
+            title = None
+
         lab = Lab(
             title,
             lab_id,
             self._session,
             self.username,
             self.password,
             auto_sync=self.auto_sync,
             auto_sync_interval=self.auto_sync_interval,
             resource_pool_manager=self.resource_pool_management,
         )
         if sync_lab:
-            lab.sync()
+            lab.import_lab(topology)
+            lab._initialized = True
 
         self._labs[lab_id] = lab
         return lab
 
     def get_diagnostics(self) -> dict:
         """
         Returns the controller diagnostic data as JSON
 
         :returns: diagnostic data
-        :rtype: dict
         """
         url = "diagnostics"
         return self._session.get(url).json()
 
     def get_system_health(self) -> dict:
         """
         Returns the controller system health data as JSON
@@ -675,14 +774,15 @@
         Returns the controller resource statistics as JSON
 
         :returns: system resource statistics
         """
         url = "system_stats"
         return self._session.get(url).json()
 
+    @locked
     def find_labs_by_title(self, title: str) -> list[Lab]:
         """
         Return a list of labs which match the given title.
 
         :param title: The title to search for
         :returns: A list of lab objects which match the title specified
         """
@@ -709,17 +809,15 @@
         return matched_labs
 
     def get_lab_list(self, show_all: bool = False) -> list[str]:
         """
         Returns list of all lab IDs.
 
         :param show_all: Whether to get only labs owned by the admin or all user labs
-        :type show_all: bool
         :returns: a list of Lab IDs
-        :rtype: list[str]
         """
         url = "labs"
         if show_all:
             url += "?show_all=true"
         return self._session.get(url).json()
```

### Comparing `virl2_client-2.5.0/setup.py` & `virl2_client-2.6.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,32 +4,33 @@
 packages = \
 ['virl2_client', 'virl2_client.models']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
-['httpx>=0.23.0,<0.24.0']
+['httpx>=0.24.0,<0.25.0']
 
 extras_require = \
-{'docs': ['sphinx_rtd_theme>=1,<2', 'sphinx>=5,<6'],
- 'pyats': ['pyats>=22.4,<23.0']}
+{'docs': ['sphinx_rtd_theme>=1,<2', 'sphinx>=6,<7'],
+ 'events': ['aiohttp'],
+ 'pyats': ['pyats>=23,<24']}
 
 setup_kwargs = {
     'name': 'virl2-client',
-    'version': '2.5.0',
+    'version': '2.6.0',
     'description': 'VIRL2 Client Library',
     'long_description': '[![CI](https://github.com/CiscoDevNet/virl2-client/actions/workflows/main.yml/badge.svg)](https://github.com/CiscoDevNet/virl2-client/actions/workflows/main.yml)\n\n# VIRL 2 Client Library\n\n> **Note:** The product has been renamed from *VIRL* to *Cisco Modeling Labs* /\n> CML 2.  References to VIRL still exist in the product documentation and within\n> code or examples.\n>\n> The name of the package itself has not been changed.  Throughout the\n> documentation it is referred to as "virl2_client",  "Python Client Library" or\n> "PCL".\n\n## Introduction\n\nThis is the client library for the *Cisco Modeling Labs* Platform\n(`virl2_client`). It provides a Python package to programmatically create,\nedit, delete and control network simulations on a CML 2 controller.\n\nIt is a pure Python implementation that requires Python 3. We\'ve tested and\nwritten the package with Python 3.8.10.\n\nThe status of the package can be considered **stable**.  Issues with the\nsoftware should be raised via the [GitHub issue\ntracker](https://github.com/CiscoDevNet/virl2-client/issues).\n\n## Use Case Description\n\nThe client library provides a convenient interface to control the life-cycle of\na network simulation. This can be used for automation scripts directly in\nPython but also for third party integrations / plugins which need to integrate\nwith a simulated network. Examples already existing are an [Ansible\nplugin](https://github.com/CiscoDevNet/ansible-virl).\n\n## Installation\n\nThe package comes in form of a wheel that is downloadable from the CML\n2 controller. The package can be installed either from PyPI using\n\n    pip3 install virl2_client\n\nIf you want to interact with devices via the client library, you need to\nalso install the pyATS library. This can be achieved in one go using\n\n```\npip3 install "virl2_client[pyats]"\n```\n\nNote that this does *not* pull in the full pyATS package... See below how that is achieved.\n\nor, alternatively, the version that is bundled with the CML 2 controller can\nbe downloaded to the local filesystem and then directly installed via\n\n    pip3 install ./virl2_client-*.whl\n\nThe bundled version is available on the index site of the docs when viewed\ndirectly on the CML 2 controller.\n\nEnsure to replace and/or use the correct file name, replacing the wildcard with the\nproper version/build information. For example\n\n    pip3 install virl2_client-2.0.0b10-py3-none-any.whl\n\nWe recommend the use of a virtual environment for installation.\n\nIf you require the full version of the pyATS library including things like Genie\nthen you need to do this in a subsequent step like shown here:\n\n    pip3 install "pyats[full]"\n\n> **IMPORTANT**: The version of the Python client library  must be compatible\n> with the version of the controller.  If you are running an older controller\n> version then it\'s likely that the latest client library version from PyPI can\n> **not** be used.  In this case, you need to either use the version available\n> from the controller itself or by specifying a version constraint.\n>\n> Example: When on a controller version 2.2.x, then you\'d need to install with\n> `pip3 install "virl2-client<2.3.0"`. This will ensure that the version\n> installed is compatible with 2.2.x.\n\n## Usage\n\nThe package itself is fairly well documented using *docstrings*. In addition, the\ndocumentation is available in HTML format on the controller itself, via the\n"Tools -> Client Library" menu.\n\n## Compatibility\n\nThis package and the used API is specific to CML 2. It is not\nbackwards compatible with VIRL 1.x and therefore can not be used with VIRL\n1.x. If you are looking for a convenient tool to interface with the VIRL 1 API\nthen the [CML Utils tool](https://github.com/CiscoDevNet/virlutils) is\nrecommended.\n\n## Known Issues\n\nThere are no major known issues at this point. See the comment in the *Introduction*\nsection.  Also, see the *Issues* section in GitHub to learn about known issues or raise new ones, if needed.  Also see [CHANGES](CHANGES.md).\n\n## Getting Help\n\nIf you have questions, concerns, bug reports, etc., please create an issue\nagainst the [repository on\nGitHub](https://github.com/CiscoDevNet/virl2-client/)\n\n## Getting Involved\n\nWe welcome contributions. Whether you fixed a bug, added a new feature or\ncorrected a typo, all contributions are welcome. General instructions on how to\ncontribute can be found in the [CONTRIBUTING](CONTRIBUTING.md) file.\n\n## Licensing Info\n\nThis code is licensed under the Apache 2.0 License. See [LICENSE](LICENSE) for\ndetails.\n\n## References\n\nThis package is part of the CML 2 Network Simulation platform. For details, go\nto <https://developer.cisco.com/modeling-labs>. Additional documentation for the\nproduct is available at <https://developer.cisco.com/docs/modeling-labs>\n',
     'author': 'Simon Knight',
     'author_email': 'simknigh@cisco.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
+    'maintainer': None,
+    'maintainer_email': None,
     'url': 'https://github.com/ciscodevnet/virl2-client',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
     'extras_require': extras_require,
-    'python_requires': '>=3.8.0,<4.0.0',
+    'python_requires': '>=3.8.1,<4.0.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `virl2_client-2.5.0/PKG-INFO` & `virl2_client-2.6.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,32 +1,31 @@
 Metadata-Version: 2.1
 Name: virl2-client
-Version: 2.5.0
+Version: 2.6.0
 Summary: VIRL2 Client Library
 Home-page: https://github.com/ciscodevnet/virl2-client
 License: Apache-2.0
 Author: Simon Knight
 Author-email: simknigh@cisco.com
-Requires-Python: >=3.8.0,<4.0.0
+Requires-Python: >=3.8.1,<4.0.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Topic :: System :: Networking
 Provides-Extra: docs
+Provides-Extra: events
 Provides-Extra: pyats
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
-Requires-Dist: pyats (>=22.4,<23.0); extra == "pyats"
-Requires-Dist: sphinx (>=5,<6); extra == "docs"
+Requires-Dist: aiohttp; extra == "events"
+Requires-Dist: httpx (>=0.24.0,<0.25.0)
+Requires-Dist: pyats (>=23,<24); extra == "pyats"
+Requires-Dist: sphinx (>=6,<7); extra == "docs"
 Requires-Dist: sphinx_rtd_theme (>=1,<2); extra == "docs"
 Project-URL: Repository, https://github.com/ciscodevnet/virl2-client
 Description-Content-Type: text/markdown
 
 [![CI](https://github.com/CiscoDevNet/virl2-client/actions/workflows/main.yml/badge.svg)](https://github.com/CiscoDevNet/virl2-client/actions/workflows/main.yml)
 
 # VIRL 2 Client Library
```

