# Comparing `tmp/gulf_id_scanner-0.1.0b0.tar.gz` & `tmp/gulf_id_scanner-0.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gulf_id_scanner-0.1.0b0.tar", max compression
+gzip compressed data, was "gulf_id_scanner-0.1.0b1.tar", max compression
```

## Comparing `gulf_id_scanner-0.1.0b0.tar` & `gulf_id_scanner-0.1.0b1.tar`

### file list

```diff
@@ -1,14 +1,9 @@
--rw-r--r--   0        0        0     1344 2023-07-20 06:55:01.071294 gulf_id_scanner-0.1.0b0/README.md
--rw-r--r--   0        0        0        0 2023-07-14 07:54:09.650522 gulf_id_scanner-0.1.0b0/gulf_id_scanner/__init__.py
--rw-r--r--   0        0        0      498 2023-07-19 13:41:46.282752 gulf_id_scanner-0.1.0b0/gulf_id_scanner/__main__.py
--rw-r--r--   0        0        0     9292 2023-07-19 13:47:12.592803 gulf_id_scanner-0.1.0b0/gulf_id_scanner/client.py
--rw-r--r--   0        0        0     6655 2023-07-14 07:38:59.670502 gulf_id_scanner-0.1.0b0/gulf_id_scanner/eid/test.py
--rw-r--r--   0        0        0      450 2023-07-19 12:58:44.044128 gulf_id_scanner-0.1.0b0/gulf_id_scanner/execptions.py
--rw-r--r--   0        0        0     2388 2023-07-17 10:52:00.698819 gulf_id_scanner-0.1.0b0/gulf_id_scanner/gulf_ids/client.py
--rw-r--r--   0        0        0     3621 2023-07-17 08:02:33.141257 gulf_id_scanner-0.1.0b0/gulf_id_scanner/gulf_ids/models.py
--rw-r--r--   0        0        0    23959 2023-07-14 13:48:36.963663 gulf_id_scanner-0.1.0b0/gulf_id_scanner/gulf_ids/response.json
--rw-r--r--   0        0        0     6655 2023-07-14 13:32:44.483959 gulf_id_scanner-0.1.0b0/gulf_id_scanner/gulf_ids/test.py
--rw-r--r--   0        0        0    19462 2023-07-20 06:12:41.792522 gulf_id_scanner-0.1.0b0/gulf_id_scanner/models.py
--rw-r--r--   0        0        0        0 2023-07-13 09:22:18.378843 gulf_id_scanner-0.1.0b0/gulf_id_scanner/tests/__init__.py
--rw-r--r--   0        0        0      657 2023-07-20 07:00:32.335039 gulf_id_scanner-0.1.0b0/pyproject.toml
--rw-r--r--   0        0        0     2113 1970-01-01 00:00:00.000000 gulf_id_scanner-0.1.0b0/PKG-INFO
+-rw-r--r--   0        0        0     1314 2023-07-20 11:39:48.504207 gulf_id_scanner-0.1.0b1/README.md
+-rw-r--r--   0        0        0      207 2023-07-20 11:39:12.042176 gulf_id_scanner-0.1.0b1/gulf_id_scanner/__init__.py
+-rw-r--r--   0        0        0      460 2023-07-20 11:39:12.042176 gulf_id_scanner-0.1.0b1/gulf_id_scanner/__main__.py
+-rw-r--r--   0        0        0     9519 2023-07-20 12:52:08.860980 gulf_id_scanner-0.1.0b1/gulf_id_scanner/client.py
+-rw-r--r--   0        0        0      464 2023-07-20 11:22:47.326789 gulf_id_scanner-0.1.0b1/gulf_id_scanner/exceptions.py
+-rw-r--r--   0        0        0    20112 2023-07-20 12:51:56.240980 gulf_id_scanner-0.1.0b1/gulf_id_scanner/models.py
+-rw-r--r--   0        0        0        0 2023-07-13 09:22:18.378843 gulf_id_scanner-0.1.0b1/gulf_id_scanner/tests/__init__.py
+-rw-r--r--   0        0        0      657 2023-07-20 13:01:49.033475 gulf_id_scanner-0.1.0b1/pyproject.toml
+-rw-r--r--   0        0        0     2083 1970-01-01 00:00:00.000000 gulf_id_scanner-0.1.0b1/PKG-INFO
```

### Comparing `gulf_id_scanner-0.1.0b0/README.md` & `gulf_id_scanner-0.1.0b1/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -6,16 +6,15 @@
 
 - Install the card reader service on a windows machine
 - Ensure the services are running
 - Get the IP of the machine
 
 ```python
 import aiohttp
-from gulf_id_scanner.client import Client
-from .execptions import ServiceError
+from gulf_id_scanner import Client, ServiceError
 
 session = aiohttp.ClientSession()
 client = Client(host="192.168.3.45", web_session=session)
 # validate connection
 try:
     await client.connect()
 except ServiceError as err:
```

### Comparing `gulf_id_scanner-0.1.0b0/gulf_id_scanner/client.py` & `gulf_id_scanner-0.1.0b1/gulf_id_scanner/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 """Websocket client for Emirates ID."""
 
-import asyncio
 import json
 import logging
 from enum import Enum
-from typing import Any, AsyncIterator, Iterable
+from typing import Any, AsyncIterator, cast
 
 import aiohttp
 
-from .execptions import (
+from .exceptions import (
     ReadError,
+    ReaderNotFound,
     ServiceDisconnected,
     ServiceUnavailable,
 )
 from .models import (
     CardData,
     EIDCardData,
-    EIDContext,
-    EIDRequest,
-    EstablishContext,
+    Request,
     GCCIDCardData,
-    GCCIDRequest,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 PROTOCOLS = ["eida-toolkit"]
 
 
@@ -51,29 +48,28 @@
     ) -> None:
         """Initiate class."""
         self.host = host
         self.eid_url = f"ws{'s' if use_ssl else ''}://{host}:{eid_ws_port}"
         self.gcc_id_url = f"ws{'s' if use_ssl else ''}://{host}:{gcc_ws_port}/SCardRead"
         self.ssl = use_ssl
         self.web_session = web_session
-        self.request: EIDRequest | None = None
-        self.context = EIDContext()
+        self.request = Request()
         self.eid_ws_state = ServiceState.DISCONNECTED
         self.gcc_ws_state = ServiceState.DISCONNECTED
 
     @staticmethod
     async def _list_readers(readers: list[str]) -> list[str]:
         """List connected ID card readers."""
         return [reader for reader in readers if "Windows Hello" not in reader]
 
     async def _async_ws_request(
         self,
         url: str,
         request: str | dict[str, Any] | None = None,
-        protocols: Iterable[str] = (),
+        protocols: list[str] = [],
     ) -> dict[str, Any] | bool:
         """Send request over ws and return response."""
         async with self.web_session.ws_connect(url, protocols=protocols) as ws:
             if isinstance(request, dict):
                 await ws.send_json(request)
             elif isinstance(request, str):
                 await ws.send_str(request)
@@ -84,20 +80,24 @@
                         if request is None:
                             return True
                         continue
                     else:
                         try:
                             return msg.json()
                         except json.JSONDecodeError:
-                            return msg.data
+                            raise ValueError(f"Data received is not json. {msg.data}")
+        return False
 
     async def _async_eid_request(self, request: dict[str, Any]) -> dict[str, Any]:
         """Send a ws request to EID service and return the response."""
         try:
-            return await self._async_ws_request(self.eid_url, request, PROTOCOLS)
+            return cast(
+                dict[str, Any],
+                await self._async_ws_request(self.eid_url, request, PROTOCOLS),
+            )
         except aiohttp.ClientConnectionError as err:
             self.eid_ws_state = ServiceState.DISCONNECTED
             raise ServiceDisconnected("EID reader service is disconnected.") from err
 
     async def _async_gcc_id_request(
         self, request: str | None = None
     ) -> dict[str, Any] | bool:
@@ -109,95 +109,99 @@
             raise ServiceDisconnected("GCC ID reader service is disconnected.") from err
 
     async def _connect_reader_with_eid(self) -> bool:
         """Connect to the card reading holding EID."""
         if self.eid_ws_state == ServiceState.DISCONNECTED:
             raise ServiceDisconnected("EID service is disconnected.")
         try:
-            response = await self._async_eid_request(self.request.reader_with_eid())
+            response = await self._async_eid_request(self.request.reader_with_eid)
         except ServiceDisconnected:
             return False
         if response["status"] != "success":
             return False
-        response = await self._async_eid_request(
-            self.request.connect_to_reader(response["smartcard_reader"])
-        )
-        self.context.eid_card_context = response["card_context"]
+        self.request.context.card_reader_name = response["smartcard_reader"]
+        response = await self._async_eid_request(self.request.connect_to_reader)
+        self.request.context.eid_card_context = response["card_context"]
         self.eid_ws_state = ServiceState.READY
         return True
 
-    async def get_connected_reader(self) -> bool:
+    async def _connect_reader_with_gccid(self) -> bool:
         """Get list of connected readers."""
         if self.gcc_ws_state == ServiceState.DISCONNECTED:
             raise ServiceDisconnected("GCC ID service is disconnected.")
-        response = await self._async_gcc_id_request("GetReaderNames")
-        if card_readers := await self._list_readers(response["ReaderNames"]):
-            self.context.card_reader_name = card_readers[0]
-            self.gcc_ws_state = ServiceState.READY
+        response = cast(
+            dict[str, Any], await self._async_gcc_id_request("GetReaderNames")
+        )
+        if not (card_readers := await self._list_readers(response["ReaderNames"])):
+            return False
+        self.request.context.card_reader_name = card_readers[0]
+        self.gcc_ws_state = ServiceState.READY
+        return True
 
     async def connect(self) -> None:
         """Connect to the scanner services and set context."""
         if self.gcc_ws_state == ServiceState.DISCONNECTED:
             try:
                 if await self._async_gcc_id_request():
                     self.gcc_ws_state = ServiceState.CONNECTED
             except ServiceDisconnected:
                 self.gcc_ws_state = ServiceState.UNAVAILABLE
 
         if self.eid_ws_state == ServiceState.DISCONNECTED:
             try:
                 response: dict[str, Any] = await self._async_eid_request(
-                    str(EstablishContext())
+                    Request.establish_context()
                 )
                 if response.get("status") == "success":
-                    self.context.service_context = response["service_context"]
-                    self.request = EIDRequest(self.context)
+                    self.request.context.service_context = response["service_context"]
                     self.eid_ws_state = ServiceState.CONNECTED
             except ServiceDisconnected:
                 self.eid_ws_state = ServiceState.UNAVAILABLE
         if self.gcc_ws_state == self.eid_ws_state == ServiceState.UNAVAILABLE:
             raise ServiceUnavailable(
                 f"No smart card service detected on host {self.host}"
             )
 
     async def _read_eid_card_data(self) -> EIDCardData | None:
         """Read data from EID card."""
         if self.eid_ws_state != ServiceState.READY:
             if not await self._connect_reader_with_eid():
                 _LOGGER.debug("No EID smart card detected.")
                 return None
-        await asyncio.sleep(10)
         try:
-            response = await self._async_eid_request(self.request.read_card_data())
+            response = await self._async_eid_request(self.request.read_eid_card)
         except ServiceDisconnected as err:
             raise ReadError("Failed to read EID card.") from err
         if response["status"] != "success":
             raise ReadError("Failed to read EID card.")
-        card_data = EIDCardData.from_xml(response["toolkit_response"])
+        card_data = EIDCardData(xml_data=response["toolkit_response"])
         return card_data
 
-    async def _read_gcc_card_data(self) -> GCCIDCardData | None:
+    async def _read_gcc_card_data(self) -> GCCIDCardData:
         """Read data from other Gulf ID cards."""
         if self.gcc_ws_state != ServiceState.READY:
-            await self.get_connected_reader()
+            if not await self._connect_reader_with_gccid():
+                raise ReaderNotFound("No compatible reader detected.")
 
-        request = GCCIDRequest()
-        request.ReaderName = self.context.card_reader_name
-        response = await self._async_gcc_id_request(str(request))
-        if response["MessageType"] == "Data":
-            return GCCIDCardData(**response["CardData"])
-        raise ReadError("Failed to read GCC card")
+        response = cast(
+            dict[str, Any], await self._async_gcc_id_request(self.request.read_gcc_card)
+        )
+        if response["MessageType"] == "Error":
+            raise ReadError("Failed to read GCC card: %s", response["ErrorDescription"])
+        return GCCIDCardData(**response["CardData"])
 
-    async def async_read_card(self) -> CardData | None:
+    async def async_read_card(self) -> CardData:
         """Return data from Gulf ID card."""
         card_data: EIDCardData | GCCIDCardData | None = None
         if self.eid_ws_state != ServiceState.UNAVAILABLE:
-            card_data = await self._read_eid_card_data()
-        if card_data is None and self.gcc_ws_state != ServiceState.UNAVAILABLE:
-            card_data = await self._read_gcc_card_data()
+            if card_data := await self._read_eid_card_data():
+                return CardData(card_data)
+        if self.gcc_ws_state == ServiceState.UNAVAILABLE:
+            raise ReadError("Can't read inserted card")
+        card_data = await self._read_gcc_card_data()
         return CardData(card_data)
 
     async def async_detect_card(
         self,
     ) -> AsyncIterator[CardData | None]:
         """List to card inserted events and read card data."""
         if self.gcc_ws_state == ServiceState.UNAVAILABLE:
@@ -214,19 +218,19 @@
                     if msg.data == "Connected to WebSockets Server!":
                         continue
                     try:
                         response: dict[str, Any] = msg.json()
                     except json.JSONDecodeError:
                         return
                     if response.get("EventName") == "CardMonitorStarted":
-                        self.context.card_reader_name = response["ReaderName"]
+                        self.request.context.card_reader_name = response["ReaderName"]
                         continue
                     if response.get("EventName") == "CardInserted":
                         _LOGGER.debug("Card inserted")
                         yield await self.async_read_card()
                         continue
                     if response.get("EventName") == "CardRemoved":
                         _LOGGER.debug("Card removed")
                         continue
         if ws.closed:
-            self.gcc_ws_state == ServiceState.DISCONNECTED
+            self.gcc_ws_state = ServiceState.DISCONNECTED
             raise ServiceDisconnected("GCC service disconnected.")
```

### Comparing `gulf_id_scanner-0.1.0b0/gulf_id_scanner/models.py` & `gulf_id_scanner-0.1.0b1/gulf_id_scanner/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,25 @@
 
 import base64
 import json
 import random
 import string
 import xml.etree.ElementTree as ET
 from collections.abc import Callable
-from dataclasses import dataclass, field, fields
+from dataclasses import InitVar, dataclass, field, fields
 from datetime import datetime
 from enum import IntEnum
+from typing import Any
 
 from typing_extensions import Self
 
 NS = {"ns": "http://www.emiratesid.ae/toolkit"}
-# library command classes
 
 
+# library command classes
 class CMD(IntEnum):
     """List of commands."""
 
     ESTABLISH_CONTEXT = 1
     CLEANUP_CONETEXT = 2
     LIST_READERS = 3
     CONNECT_READER = 4
@@ -40,103 +41,117 @@
     GET_INTERFACE = 19
     CSN = 20
     CARD_VERSION = 21
     FAMILY_BOOK_DATA_REQUEST = 22
     CARD_GENUINE = 24
     GET_READER_WITH_EID = 54
 
-    def __str__(self):
-        return str(self.value)
-
-
-@dataclass(frozen=True)
-class EstablishContext:
-    """Establish context request."""
-
-    cmd: CMD = CMD.ESTABLISH_CONTEXT.value
-    config_params: str = ""
-    user_agent: str = "Chrome 114.0.0.0"
-
-    def __str__(self):
-        return repr(self.__dict__)
-
 
 @dataclass
 class EIDContext:
     """class for storing context."""
 
-    service_context: str = ""
+    service_context: int = 0
     eid_card_context: str = ""
     card_reader_name: str = ""
     request_id: str = ""
 
-    def gen_request_id(self) -> str:
+    def gen_request_id(self) -> None:
         """Generate a new request_id."""
         letters = string.ascii_letters + string.digits
         random_str = "".join(random.choice(letters) for _ in range(40))
         self.request_id = base64.b64encode(random_str.encode("utf-8")).decode("utf-8")
 
 
-class EIDRequest:
+class Request:
     """Reqeust base class."""
 
-    def __init__(self, context: EIDContext) -> None:
+    def __init__(self) -> None:
         """Initialize request object."""
-        self.context = context
-        self.request: dict[str, str] = {"service_context": context.service_context}
+        self.context = EIDContext()
+
+    @classmethod
+    def establish_context(cls) -> dict[str, str | int]:
+        """Request to establish context."""
+        return {
+            "cmd": CMD.ESTABLISH_CONTEXT.value,
+            "config_params": "",
+            "user_agent": "Chrome 114.0.0.0",
+        }
+
+    @property
+    def request(self) -> dict[str, str | int]:
+        return {"service_context": self.context.service_context}
 
-    def list_readers(self) -> dict[str, str]:
+    @property
+    def list_readers(self) -> dict[str, str | int]:
         """List connected readers."""
         request = self.request.copy()
-        request["cmd"] = CMD.LIST_READERS
+        request["cmd"] = CMD.LIST_READERS.value
         return request
 
-    def reader_with_eid(self) -> dict[str, str]:
+    @property
+    def reader_with_eid(self) -> dict[str, str | int]:
         """Request reader with EID inserted."""
         request = self.request.copy()
-        request["cmd"] = CMD.GET_READER_WITH_EID
+        request["cmd"] = CMD.GET_READER_WITH_EID.value
         return request
 
-    def connect_to_reader(self, reader_name: str) -> dict[str, str]:
+    @property
+    def connect_to_reader(self) -> dict[str, str | int]:
         """Connect to selected reader."""
         request = self.request.copy()
-        request["cmd"] = CMD.CONNECT_READER
-        request["smartcard_reader"] = reader_name
+        request["cmd"] = CMD.CONNECT_READER.value
+        request["smartcard_reader"] = self.context.card_reader_name
         return request
 
-    def read_card_data(self) -> dict[str, str]:
-        """Read card data."""
+    @property
+    def read_eid_card(self) -> dict[str, str | int]:
+        """Request for reading EID card."""
         request = self.request.copy()
         self.context.gen_request_id()
         request.update(
             {
-                "cmd": CMD.READ_PUBLIC_DATA,
+                "cmd": CMD.READ_PUBLIC_DATA.value,
                 "card_context": self.context.eid_card_context,
                 "read_photography": True,
                 "read_non_modifiable_data": True,
                 "read_modifiable_data": True,
                 "request_id": self.context.request_id,
                 "signature_image": True,
                 "address": True,
             }
         )
         return request
 
+    @property
+    def read_gcc_card(self) -> str:
+        """Request for reading GCC card."""
+        params = {
+            "ReaderName": self.context.card_reader_name,
+            "ReaderIndex": -1,
+            "OutputFormat": "JSON",
+            "SilentReading": True,
+        }
+        return f"ReadCard{json.dumps(params)}"
+
 
 # EID Card data classes
+@dataclass
 class BaseClass:
     """Base class for card data classes."""
 
     @classmethod
     def from_xml_element(cls, root: ET.Element) -> Self:
         """Construct class from xml element."""
         _cls = object.__new__(cls)
         for cls_field in fields(_cls):
             element = root.find(f".ns:{cls_field.name}", NS)
-            setattr(_cls, cls_field.name, element.text)
+            if element is not None:
+                setattr(_cls, cls_field.name, element.text)
         return _cls
 
 
 @dataclass(init=False)
 class NonModifiableData(BaseClass):
     IdType: str
     IssueDate: str
@@ -230,85 +245,63 @@
     EmiratesDescEnglish: str
     CityCode: str
     CityDescArabic: str
     CityDescEnglish: str
     StreetArabic: str
     StreetEnglish: str
     POBOX: str
-    StreetArabic: str
-    StreetEnglish: str
     AreaCode: str
     AreaDescArabic: str
     AreaDescEnglish: str
     BuildingNameArabic: str
     BuildingNameEnglish: str
     LandPhoneNumber: str
     MobilePhoneNumber: str
     Email: str
 
 
 @dataclass
 class EIDCardData:
-    IdNumber: str
-    CardNumber: str
-    NonModifiableData: NonModifiableData
-    ModifiableData: ModifiableData
-    HomeAddress: HomeAddress
-    WorkAddress: WorkAddress
-    CardHolderPhoto: str
-    HolderSignatureImage: str
-
-    @classmethod
-    def from_xml(cls, data: str) -> EIDCardData:
-        """Construct class from xml data."""
-        root = ET.fromstring(data)
-        return EIDCardData(
-            IdNumber=root.find(".//ns:IdNumber", NS).text,
-            CardNumber=root.find(".//ns:CardNumber", NS).text,
-            NonModifiableData=NonModifiableData.from_xml_element(
-                root.find(".//ns:NonModifiableData", NS)
-            ),
-            ModifiableData=ModifiableData.from_xml_element(
-                root.find(".//ns:ModifiableData", NS)
-            ),
-            HomeAddress=HomeAddress.from_xml_element(
-                root.find(".//ns:HomeAddress", NS)
-            ),
-            WorkAddress=WorkAddress.from_xml_element(
-                root.find(".//ns:WorkAddress", NS)
-            ),
-            CardHolderPhoto=root.find(".//ns:CardHolderPhoto", NS).text,
-            HolderSignatureImage=root.find(".//ns:HolderSignatureImage", NS).text,
-        )
+    xml_data: InitVar[str]
+    IdNumber: str | None = field(init=False)
+    CardNumber: str | None = field(init=False)
+    NonModifiableData: NonModifiableData = field(init=False)
+    ModifiableData: ModifiableData = field(init=False)
+    HomeAddress: HomeAddress = field(init=False)
+    WorkAddress: WorkAddress = field(init=False)
+    CardHolderPhoto: str | None = field(init=False)
+    HolderSignatureImage: str | None = field(init=False)
+
+    def __post_init__(self, xml_data: str) -> None:
+        """Fill attribute values from xml_data."""
+        root = ET.fromstring(xml_data)
+        body = root.find(".//ns:PublicData", NS)
+        if body is None:
+            return
+        for child in body:
+            if "IdNumber" in child.tag:
+                self.IdNumber = child.text
+            if "CardNumber" in child.tag:
+                self.CardNumber = child.text
+            if "NonModifiableData" in child.tag:
+                self.NonModifiableData = NonModifiableData.from_xml_element(child)
+            if "ModifiableData" in child.tag:
+                self.ModifiableData = ModifiableData.from_xml_element(child)
+            if "HomeAddress" in child.tag:
+                self.HomeAddress = HomeAddress.from_xml_element(child)
+            if "WorkAddress" in child.tag:
+                self.WorkAddress = WorkAddress.from_xml_element(child)
+            if "CardHolderPhoto" in child.tag:
+                self.CardHolderPhoto = child.text
+            if "HolderSignatureImage" in child.tag:
+                self.HolderSignatureImage = child.text
 
 
 # GCC ID related classes
 @dataclass
-class GCCIDRequest:
-    """Gulf ID read request."""
-
-    ReadCardInfo: bool = True
-    ReadPersonalInfo: bool = True
-    ReadAddressDetails: bool = True
-    ReadBiometrics: bool = True
-    ReadEmploymentInfo: bool = True
-    ReadImmigrationDetails: bool = True
-    ReadTrafficDetails: bool = True
-    ReaderName: str = ""
-    ReaderIndex: int = -1
-    OutputFormat: str = "JSON"
-    ValidateCard: bool = False
-    SilentReading: bool = True
-
-    def __repr__(self) -> str:
-        """Return request string."""
-        return f"ReadCard{json.dumps(self.__dict__)}"
-
-
-@dataclass
 class MiscellaneousTextData:
     FirstNameArabic: str
     LastNameArabic: str
     MiddleName1Arabic: str
     MiddleName2Arabic: str
     MiddleName3Arabic: str
     MiddleName4Arabic: str
@@ -449,24 +442,27 @@
     SignB64Encoded: str
     SponserId: str
     SponserNameArabic: str
     SponserNameEnglish: str
     ErrorDescription: str
 
     def __post_init__(self) -> None:
-        self.MiscellaneousTextData = MiscellaneousTextData(**self.MiscellaneousTextData)
+        if isinstance(self.MiscellaneousTextData, dict):
+            self.MiscellaneousTextData = MiscellaneousTextData(
+                **self.MiscellaneousTextData
+            )
 
 
 @dataclass
 class CardDataField:
     """Class to represent Card data field."""
 
     name: str
     value_fn: Callable[  # noqa: E731
-        [EIDCardData | GCCIDCardData], str
+        [EIDCardData | GCCIDCardData], Any
     ] = lambda val: val
 
 
 CARDDATA_FIELDS: tuple[CardDataField, ...] = (
     CardDataField(name="IdNumber", value_fn=lambda val: val.IdNumber),
     CardDataField(
         name="IssueDate",
@@ -621,27 +617,35 @@
         value_fn=lambda val: val.ModifiableData.PassportNumber
         if isinstance(val, EIDCardData)
         else val.PassportNumber,
     ),
     CardDataField(
         name="PassportIssueDate",
         value_fn=lambda val: datetime.strptime(
-            val.ModifiableData.PassportIssueDate  # TODO check if value is not there
-            if isinstance(val, EIDCardData)
-            else val.PassportIssueDate,
-            "%d/%m/%Y",
+            val.ModifiableData.PassportIssueDate, "%d/%m/%Y"
+        )
+        if isinstance(val, EIDCardData)
+        and val.ModifiableData.PassportIssueDate is not None
+        else (
+            datetime.strptime(val.PassportIssueDate, "%d/%m/%Y")
+            if isinstance(val, GCCIDCardData) and val.PassportIssueDate is not None
+            else None
         ),
     ),
     CardDataField(
         name="PassportExpiryDate",
         value_fn=lambda val: datetime.strptime(
-            val.ModifiableData.PassportExpiryDate
-            if isinstance(val, EIDCardData)
-            else val.PassportExpiryDate,
-            "%d/%m/%Y",
+            val.ModifiableData.PassportExpiryDate, "%d/%m/%Y"
+        )
+        if isinstance(val, EIDCardData)
+        and val.ModifiableData.PassportExpiryDate is not None
+        else (
+            datetime.strptime(val.PassportExpiryDate, "%d/%m/%Y")
+            if isinstance(val, GCCIDCardData) and val.PassportExpiryDate is not None
+            else None
         ),
     ),
     CardDataField(
         name="Photo",
         value_fn=lambda val: val.CardHolderPhoto
         if isinstance(val, EIDCardData)
         else val.PhotoB64Encoded,
@@ -669,16 +673,14 @@
     NationalityEnglish: str = ""
     NationalityArabic: str = ""
     PlaceOfBirthEnglish: str = ""
     PlaceOfBirthArabic: str = ""
     OccupationEnglish: str = ""
     OccupationArabic: str = ""
     CompanyNameEnglish: str = ""
-    OccupationArabic: str = ""
-    CompanyNameEnglish: str = ""
     CompanyNameArabic: str = ""
     SponsorUnifiedNumber: str = ""
     SponsorName: str = ""
     PassportNumber: str = ""
     PassportIssueDate: datetime | None = None
     PassportExpiryDate: datetime | None = None
     Photo: str = ""
```

### Comparing `gulf_id_scanner-0.1.0b0/pyproject.toml` & `gulf_id_scanner-0.1.0b1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gulf-id-scanner"
-version = "0.1.0b0"
+version = "0.1.0b1"
 description = "Python websocket client for reading Gulf IDs"
 authors = ["Rami Mousleh <engrbm87@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://github.com/Gallagher-ME/gulf_id_scanner"
 repository = "https://github.com/Gallagher-ME/gulf_id_scanner/releases"
 packages = [{include = "gulf_id_scanner"}]
```

### Comparing `gulf_id_scanner-0.1.0b0/PKG-INFO` & `gulf_id_scanner-0.1.0b1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gulf-id-scanner
-Version: 0.1.0b0
+Version: 0.1.0b1
 Summary: Python websocket client for reading Gulf IDs
 Home-page: https://github.com/Gallagher-ME/gulf_id_scanner
 License: MIT
 Author: Rami Mousleh
 Author-email: engrbm87@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -26,16 +26,15 @@
 
 - Install the card reader service on a windows machine
 - Ensure the services are running
 - Get the IP of the machine
 
 ```python
 import aiohttp
-from gulf_id_scanner.client import Client
-from .execptions import ServiceError
+from gulf_id_scanner import Client, ServiceError
 
 session = aiohttp.ClientSession()
 client = Client(host="192.168.3.45", web_session=session)
 # validate connection
 try:
     await client.connect()
 except ServiceError as err:
```

