# Comparing `tmp/otpauth-2.0.0.tar.gz` & `tmp/otpauth-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpauth-2.0.0.tar", last modified: Fri Mar 24 13:57:14 2023, max compression
+gzip compressed data, was "otpauth-2.1.0.tar", last modified: Thu Jul 20 14:42:33 2023, max compression
```

## Comparing `otpauth-2.0.0.tar` & `otpauth-2.1.0.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:57:14.700894 otpauth-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-24 13:57:05.000000 otpauth-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-24 13:57:14.700894 otpauth-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      607 2023-03-24 13:57:05.000000 otpauth-2.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-24 13:57:05.000000 otpauth-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-24 13:57:14.700894 otpauth-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:57:14.700894 otpauth-2.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:57:14.700894 otpauth-2.0.0/src/otpauth/
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-24 13:57:05.000000 otpauth-2.0.0/src/otpauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2516 2023-03-24 13:57:05.000000 otpauth-2.0.0/src/otpauth/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-03-24 13:57:05.000000 otpauth-2.0.0/src/otpauth/rfc4226.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-03-24 13:57:05.000000 otpauth-2.0.0/src/otpauth/rfc6238.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:57:14.700894 otpauth-2.0.0/src/otpauth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3411 2023-03-24 13:57:14.000000 otpauth-2.0.0/src/otpauth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-03-24 13:57:14.000000 otpauth-2.0.0/src/otpauth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 13:57:14.000000 otpauth-2.0.0/src/otpauth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-24 13:57:14.000000 otpauth-2.0.0/src/otpauth.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 13:57:14.700894 otpauth-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-24 13:57:05.000000 otpauth-2.0.0/tests/test_hotp.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-03-24 13:57:05.000000 otpauth-2.0.0/tests/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-03-24 13:57:05.000000 otpauth-2.0.0/tests/test_totp.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:33.133108 otpauth-2.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-07-20 14:42:23.000000 otpauth-2.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-20 14:42:33.133108 otpauth-2.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-07-20 14:42:23.000000 otpauth-2.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-07-20 14:42:23.000000 otpauth-2.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-20 14:42:33.133108 otpauth-2.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:33.129108 otpauth-2.1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:33.133108 otpauth-2.1.0/src/otpauth/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-07-20 14:42:23.000000 otpauth-2.1.0/src/otpauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-07-20 14:42:23.000000 otpauth-2.1.0/src/otpauth/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:23.000000 otpauth-2.1.0/src/otpauth/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-07-20 14:42:23.000000 otpauth-2.1.0/src/otpauth/rfc4226.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-07-20 14:42:23.000000 otpauth-2.1.0/src/otpauth/rfc6238.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:33.133108 otpauth-2.1.0/src/otpauth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1916 2023-07-20 14:42:33.000000 otpauth-2.1.0/src/otpauth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-07-20 14:42:33.000000 otpauth-2.1.0/src/otpauth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-20 14:42:33.000000 otpauth-2.1.0/src/otpauth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-07-20 14:42:33.000000 otpauth-2.1.0/src/otpauth.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-20 14:42:33.133108 otpauth-2.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-07-20 14:42:23.000000 otpauth-2.1.0/tests/test_hotp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-07-20 14:42:23.000000 otpauth-2.1.0/tests/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-07-20 14:42:23.000000 otpauth-2.1.0/tests/test_totp.py
```

### Comparing `otpauth-2.0.0/LICENSE` & `otpauth-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `otpauth-2.0.0/pyproject.toml` & `otpauth-2.1.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [project]
 name = "otpauth"
 description = "Implements one time password of HOTP/TOTP"
 authors = [{name = "Hsiaoming Yang", email="me@lepture.com"}]
 dependencies = []
-license = {file = "LICENSE"}
+license = {text = "BSD-3-Clause"}
 requires-python = ">=3.7"
 dynamic = ["version"]
 readme = "README.rst"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "Environment :: Web Environment",
@@ -25,27 +25,30 @@
   "Programming Language :: Python :: 3.11",
   "Programming Language :: Python :: Implementation :: CPython",
   "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 [project.urls]
 Documentation = "https://otp.authlib.org/"
-Donate = "https://github.com/sponsors/lepture"
+Donate = "https://github.com/sponsors/authlib"
 Blog = "https://blog.authlib.org/"
 
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [tool.setuptools.dynamic]
 version = {attr = "otpauth.__version__"}
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
+[tool.setuptools.package-data]
+"otpauth" = ["py.typed"]
+
 [tool.pytest.ini_options]
 pythonpath = ["src"]
 testpaths = ["tests"]
 filterwarnings = ["error"]
 
 [tool.coverage.run]
 branch = true
@@ -56,7 +59,14 @@
 
 [tool.coverage.report]
 exclude_lines = [
   "pragma: no cover",
   "raise NotImplementedError",
   "@(abc\\.)?abstractmethod",
 ]
+
+[tool.mypy]
+strict = true
+python_version = "3.8"
+files = ["src/otpauth"]
+show_error_codes = true
+pretty = true
```

### Comparing `otpauth-2.0.0/src/otpauth/core.py` & `otpauth-2.1.0/src/otpauth/core.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,82 +1,95 @@
 import base64
 import typing as t
 from urllib.parse import quote
 from abc import ABCMeta, abstractmethod
 
+SupportedAlgorithms = t.Literal["SHA1", "SHA256", "SHA512"]
+Self = t.TypeVar("Self", bound="OTP")
 
-class OTP(object, metaclass=ABCMeta):
-    TYPE: str
+
+class OTP(metaclass=ABCMeta):
+    TYPE: t.ClassVar[str]
 
     #: The supportted algorithms
-    ALGORITHMS = ["SHA1", "SHA256", "SHA512"]
+    ALGORITHMS: t.ClassVar[t.List[str]] = ["SHA1", "SHA256", "SHA512"]
 
-    def __init__(self, secret: bytes, digit: int = 6, algorithm: str = "SHA1"):
+    def __init__(self, secret: bytes, digit: int = 6, algorithm: SupportedAlgorithms = "SHA1"):
         assert 0 < digit < 11
         assert algorithm in self.ALGORITHMS
 
         self.secret = secret
         self.digit = digit
         self.algorithm = algorithm
-        self._b32_secret = None
+        self._b32_secret: t.Optional[str] = None
 
     @property
     def b32_secret(self) -> str:
         if self._b32_secret:
             return self._b32_secret
 
         secret = base64.b32encode(self.secret)
-        self._b32_secret = secret.rstrip(b'=').decode("ascii")
+        self._b32_secret = secret.rstrip(b"=").decode("ascii")
         return self._b32_secret
 
     @classmethod
-    def from_b32encode(cls, secret: t.AnyStr, digit: int = 6, algorithm: str = "SHA1"):
+    def from_b32encode(
+            cls: t.Type[Self],
+            secret: t.Union[bytes, str],
+            digit: int = 6,
+            algorithm: SupportedAlgorithms = "SHA1") -> Self:
         """Create the instance with a base32 encoded secret.
 
         :param secret: A base32 encoded secret string or bytes.
         :param digit: Number of digits in the OTP code.
         :param algorithm: Hash algorithm used in HOTP.
         """
         if isinstance(secret, str):
             secret = secret.encode("utf-8")
 
-        b32_secret = secret.rstrip(b'=')
+        b32_secret = secret.rstrip(b"=")
 
         # add padding back
-        secret += b'=' * (-len(secret) % 8)
+        secret += b"=" * (-len(secret) % 8)
         raw_secret = base64.b32decode(secret)
 
         obj = cls(raw_secret, digit, algorithm)
         obj._b32_secret = b32_secret.decode("ascii")
         return obj
 
     def _get_base_uri(self, label: str, issuer: str) -> str:
         label = quote(label, safe="/@:")
         issuer = quote(issuer, safe="")
         _type = self.TYPE.lower()
-        return f"otpauth://{_type}/{label}?secret={self.b32_secret}&issuer={issuer}&algorithm={self.algorithm}&digits={self.digit}"
+        url = (
+            f"otpauth://{_type}/{label}"
+            f"?secret={self.b32_secret}"
+            f"&issuer={issuer}"
+            f"&algorithm={self.algorithm}"
+            f"&digits={self.digit}"
+        )
+        return url
 
     def string_code(self, code: int) -> str:
         """Add leading 0 if the code length does not match the defined length.
 
         For instance, parameter ``digit=6``, but ``code=123``, this method would
         return ``000123``::
 
             >>> otp.string_code(123)
             '000123'
 
         :param code: The number that this OTP generated.
         """
-        code = str(code)
-        return "0" * (self.digit - len(code)) + code
+        return "{code:0{w}}".format(code=code, w=self.digit)
 
     @abstractmethod
-    def generate(self, *args, **kwargs) -> int:
+    def generate(self, *args: t.Any, **kwargs: t.Any) -> int:
         ...
 
     @abstractmethod
-    def verify(self, code: int, *args, **kwargs) -> bool:
+    def verify(self, code: int, *args: t.Any, **kwargs: t.Any) -> bool:
         ...
 
     @abstractmethod
-    def to_uri(self, label: str, issuer: str, *args, **kwargs) -> str:
+    def to_uri(self, label: str, issuer: str, *args: t.Any, **kwargs: t.Any) -> str:
         ...
```

### Comparing `otpauth-2.0.0/src/otpauth/rfc4226.py` & `otpauth-2.1.0/src/otpauth/rfc4226.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,64 +1,66 @@
+import typing as t
 import struct
 import hmac
 import hashlib
-from .core import OTP
+from .core import OTP, SupportedAlgorithms
 
 
 class HOTP(OTP):
     """Implementation of RFC4226, An HMAC-Based One-Time Password Algorithm.
 
     :param secret: A secret in bytes
     :param digit: Number of digits in the HOTP code.
     :param algorithm: Hash algorithm used in HOTP.
     """
 
-    TYPE = "HOTP"
+    TYPE: t.ClassVar[str] = "HOTP"
 
     def generate(self, counter: int) -> int:
         """Generate a HOTP code. The returning result is an integer.
         To convert it into string with the correct digit length, developers
         can use :meth:`string_code`::
 
             int_code = hotp.generate(4)
             str_code = hotp.string_code(int_code)
 
         :param counter: HOTP is a counter based algorithm.
         """
         return generate_hotp(self.secret, counter, self.digit, self.algorithm)
 
-    def verify(self, code: int, counter: int) -> bool:
+    def verify(self, code: int, counter: int) -> bool:  # type: ignore[override]
         """Valid a HOTP code at the given counter.
 
         :param code: A number to be verified.
         :param counter: The counter HOTP code based on.
         """
         if len(str(code)) > self.digit:
             return False
         return hmac.compare_digest(bytes(self.generate(counter)), bytes(code))
 
-    def to_uri(self, label: str, issuer: str, counter: int) -> str:
+    def to_uri(self, label: str, issuer: str, counter: int) -> str:  # type: ignore[override]
         """Generate the otpauth protocal string for HOTP.
 
         :param label: Label of the identifier.
         :param issuer: The company, the organization or something else.
         :param counter: Initial counter of the HOTP algorithm.
         """
         uri = self._get_base_uri(label, issuer)
         return uri + f"&counter={counter}"
 
 
-def generate_hotp(secret: bytes, counter: int, digit: int=6, algorithm: str = "SHA1") -> int:
+def generate_hotp(secret: bytes, counter: int, digit: int = 6, algorithm: SupportedAlgorithms = "SHA1") -> int:
     """Generate a HOTP code.
 
     :param secret: A secret token for the authentication.
     :param counter: HOTP is a counter based algorithm.
     :param digit: Number of digits in the HOTP code.
     :param algorithm: Hash algorithm used in HOTP.
     """
     hash_alg = getattr(hashlib, algorithm.lower())
-    msg = struct.pack('>Q', counter)
+    msg = struct.pack(">Q", counter)
     digest = hmac.new(secret, msg, hash_alg).digest()
-    offset = digest[19] & 0xf
-    bin_code: int = struct.unpack('>I', digest[offset:offset + 4])[0]
-    base = bin_code & 0x7fffffff
-    return base % (10 ** digit)
+    offset = digest[19] & 0xF
+    bin_code: int = struct.unpack(">I", digest[offset: offset + 4])[0]
+    total: int = bin_code & 0x7FFFFFFF
+    power: int = 10 ** digit
+    return total % power
```

### Comparing `otpauth-2.0.0/src/otpauth/rfc6238.py` & `otpauth-2.1.0/src/otpauth/rfc6238.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,66 +1,72 @@
+import typing as t
 import time
 import hmac
-from .core import OTP
+from .core import OTP, SupportedAlgorithms
 from .rfc4226 import generate_hotp
 
 
 class TOTP(OTP):
     """Implementation of RFC6238, Time-Based One-Time Password Algorithm.
 
     :param secret: A secret in bytes
     :param digit: Number of digits in the HOTP code.
     :param algorithm: Hash algorithm used in HOTP.
     :param period: The password valid in "period" seconds.
     """
 
-    TYPE = "TOTP"
+    TYPE: t.ClassVar[str] = "TOTP"
 
-    def __init__(self, secret: bytes, digit: int = 6, algorithm: str = "SHA1", period: int = 30):
+    def __init__(self, secret: bytes, digit: int = 6, algorithm: SupportedAlgorithms = "SHA1", period: int = 30):
         super().__init__(secret, digit, algorithm)
         self.period = period
 
-    def generate(self, timestamp: int = None) -> int:
+    def generate(self, timestamp: t.Optional[int] = None) -> int:
         """Generate a TOTP code. The returning result is an integer.
         To convert it into string with the correct digit length, developers
         can use :meth:`string_code`::
 
             int_code = totp.generate()
             str_code = totp.string_code(int_code)
 
         :param timestamp: Create TOTP at this given timestamp, default is now.
         """
         return generate_totp(self.secret, self.period, timestamp, self.digit, self.algorithm)
 
-    def verify(self, code: int, timestamp: int = None) -> bool:
+    def verify(self, code: int, timestamp: t.Optional[int] = None) -> bool:  # type: ignore[override]
         """Valid a TOTP code for the given timestamp.
 
         :param code: A number to be verified.
         :param timestamp: Validate TOTP at this given timestamp, default is now.
         """
         if len(str(code)) > self.digit:
             return False
         return hmac.compare_digest(bytes(self.generate(timestamp)), bytes(code))
 
-    def to_uri(self, label: str, issuer: str) -> str:
+    def to_uri(self, label: str, issuer: str) -> str:  # type: ignore[override]
         """Generate the otpauth protocal string for TOTP.
 
         :param label: Label of the identifier.
         :param issuer: The company, the organization or something else.
         """
         uri = self._get_base_uri(label, issuer)
         return uri + f"&period={self.period}"
 
 
-def generate_totp(secret: bytes, period: int=30, timestamp: int=None, digit: int = 6, algorithm: str = "SHA1"):
+def generate_totp(
+        secret: bytes,
+        period: int = 30,
+        timestamp: t.Optional[int] = None,
+        digit: int = 6,
+        algorithm: SupportedAlgorithms = "SHA1") -> int:
     """Generate a TOTP code.
 
     A TOTP code is an extension of TOTP algorithm.
 
     :param secret: A secret token for the authentication.
     :param period: A period that a TOTP code is valid in seconds
     :param timestamp: Create TOTP at this given timestamp, default is now.
     """
     if timestamp is None:
-        timestamp = time.time()
+        timestamp = int(time.time())
     counter = int(timestamp) // period
     return generate_hotp(secret, counter, digit, algorithm)
```

### Comparing `otpauth-2.0.0/tests/test_hotp.py` & `otpauth-2.1.0/tests/test_hotp.py`

 * *Files identical despite different names*

### Comparing `otpauth-2.0.0/tests/test_misc.py` & `otpauth-2.1.0/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `otpauth-2.0.0/tests/test_totp.py` & `otpauth-2.1.0/tests/test_totp.py`

 * *Files identical despite different names*

