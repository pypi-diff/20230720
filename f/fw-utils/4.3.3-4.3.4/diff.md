# Comparing `tmp/fw_utils-4.3.3-py3-none-any.whl.zip` & `tmp/fw_utils-4.3.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 22170 bytes, number of entries: 14
+Zip file size: 22302 bytes, number of entries: 14
 -rw-r--r--  2.0 unx     1747 b- defN 80-Jan-01 00:00 fw_utils/__init__.py
--rw-r--r--  2.0 unx     2914 b- defN 80-Jan-01 00:00 fw_utils/datetime.py
+-rw-r--r--  2.0 unx     3217 b- defN 80-Jan-01 00:00 fw_utils/datetime.py
 -rw-r--r--  2.0 unx     3095 b- defN 80-Jan-01 00:00 fw_utils/dicts.py
 -rw-r--r--  2.0 unx     5436 b- defN 80-Jan-01 00:00 fw_utils/files.py
 -rw-r--r--  2.0 unx     9209 b- defN 80-Jan-01 00:00 fw_utils/filters.py
 -rw-r--r--  2.0 unx    10502 b- defN 80-Jan-01 00:00 fw_utils/formatters.py
 -rw-r--r--  2.0 unx    15077 b- defN 80-Jan-01 00:00 fw_utils/parsers.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 fw_utils/py.typed
 -rw-r--r--  2.0 unx     4382 b- defN 80-Jan-01 00:00 fw_utils/state.py
 -rw-r--r--  2.0 unx     3063 b- defN 80-Jan-01 00:00 fw_utils/testing.py
--rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.3.3.dist-info/LICENSE
--rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.3.3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.3.3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.3.3.dist-info/RECORD
-14 files, 59567 bytes uncompressed, 20458 bytes compressed:  65.7%
+-rw-r--r--  2.0 unx     1078 b- defN 80-Jan-01 00:00 fw_utils-4.3.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1922 b- defN 80-Jan-01 00:00 fw_utils-4.3.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 fw_utils-4.3.4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1054 b- defN 16-Jan-01 00:00 fw_utils-4.3.4.dist-info/RECORD
+14 files, 59870 bytes uncompressed, 20590 bytes compressed:  65.6%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: fw_utils/state.py
 Comment: 
 
 Filename: fw_utils/testing.py
 Comment: 
 
-Filename: fw_utils-4.3.3.dist-info/LICENSE
+Filename: fw_utils-4.3.4.dist-info/LICENSE
 Comment: 
 
-Filename: fw_utils-4.3.3.dist-info/METADATA
+Filename: fw_utils-4.3.4.dist-info/METADATA
 Comment: 
 
-Filename: fw_utils-4.3.3.dist-info/WHEEL
+Filename: fw_utils-4.3.4.dist-info/WHEEL
 Comment: 
 
-Filename: fw_utils-4.3.3.dist-info/RECORD
+Filename: fw_utils-4.3.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fw_utils/datetime.py

```diff
@@ -20,15 +20,15 @@
 
 
 def format_datetime(dt: datetime):
     """Return ISO-formatted datetime with millisecond precision."""
     return dt.isoformat(timespec="milliseconds")
 
 
-def get_datetime(
+def get_datetime(  # noqa: PLR0912
     value: t.Union[str, int, float, datetime] = "now",
     *,
     sub: t.Union[t.Tuple[str, str], t.List[t.Tuple[str, str]]] = None,
     fmt: t.Union[str, t.List[str]] = None,
     tz: t.Union[str, tzinfo] = None,
 ) -> datetime:
     """Return datetime object parsed from a string/number (or now w/o value)."""
@@ -53,14 +53,18 @@
         return set_tz(value)
     # apply substitutions if specified
     sub = sub or []
     if len(sub) == 2 and isinstance(sub[0], str):
         sub = [t.cast(t.Tuple[str, str], sub)]
     for pattern, repl in t.cast(t.List[t.Tuple[str, str]], sub):
         value = re.sub(pattern, repl, value)
+    # add built-in compatibility for time separators other than colon
+    compat_re = re.compile(r"\d\d\d\d-\d\d-\d\d[T ]\d\d[ _-]\d\d[ _-]\d\d")
+    if isinstance(value, str) and compat_re.match(value):
+        value = re.sub(r"^(.{11}\d\d)[ _-](\d\d)[ _-](\d\d)", r"\1:\2:\3", value)
     # parse with dateutil parser when no format is specified
     if not fmt:
         default = datetime(1970, 1, 1, 0, 0, 0)
         try:
             return set_tz(dt_parser.parse(value, default=default))
         except dt_parser.ParserError:
             raise ValueError(f"Can't parse {value!r} with dateutil") from None
```

## Comparing `fw_utils-4.3.3.dist-info/LICENSE` & `fw_utils-4.3.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fw_utils-4.3.3.dist-info/METADATA` & `fw_utils-4.3.4.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fw-utils
-Version: 4.3.3
+Version: 4.3.4
 Summary: Common Flywheel helper utilities.
 Home-page: https://gitlab.com/flywheel-io/tools/lib/fw-utils
 License: MIT
 Keywords: Flywheel,helper,utility
 Author: Flywheel
 Author-email: support@flywheel.io
 Requires-Python: >=3.8,<4.0
```

## Comparing `fw_utils-4.3.3.dist-info/RECORD` & `fw_utils-4.3.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 fw_utils/__init__.py,sha256=0toIsVaBlF-X0TBUQjj9fmkIU6HDGJ_MQJzjk4D89oU,1747
-fw_utils/datetime.py,sha256=8KSueLgg0OfqVNTTtqJRZI8mFrkR8aMGUyj0bT89aEg,2914
+fw_utils/datetime.py,sha256=zrWtYNXLRWj7Igibp8wGH_jBeXSBYq9A2Vn80zZxRVc,3217
 fw_utils/dicts.py,sha256=Xh08WlC-cyJuxLsm3mNHI0x8GUfUfMBXgA6vT3mnVKA,3095
 fw_utils/files.py,sha256=Jck1ZRDXkBxXeqMcKxeywPu-SzRnxQyw--WH8J8OEL8,5436
 fw_utils/filters.py,sha256=jCNhsNnpZYgIk6yDFh_6VM9aL8bqK70iXJTwPgGJEHQ,9209
 fw_utils/formatters.py,sha256=Kb4ae5XLhjX1uNZJHSCLe9KjznhuMzulZ9gkp0S_oeE,10502
 fw_utils/parsers.py,sha256=S0g7fQpudkNq8xz8BgCwgnoLnsqatFUq61PwhpSrNCA,15077
 fw_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 fw_utils/state.py,sha256=wsa1p60kVaoy-wLxMy5XjEmZO_A2CUjRLMgkrhgdVts,4382
 fw_utils/testing.py,sha256=e3qjGfECyiEk3BspMYTW85ZqRozxoDJjZTVu2qBdq3Y,3063
-fw_utils-4.3.3.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
-fw_utils-4.3.3.dist-info/METADATA,sha256=Q7z8RgMhVsMUE6Ns0TBsu3Gg8ZFIdiz6NC-TIMmJN0g,1922
-fw_utils-4.3.3.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
-fw_utils-4.3.3.dist-info/RECORD,,
+fw_utils-4.3.4.dist-info/LICENSE,sha256=l6rSIY1z68PIZljFVsWf7vH6pbhZay7Yz2EKgbsR8q0,1078
+fw_utils-4.3.4.dist-info/METADATA,sha256=dr9TCnwdCc0vNSCpTKnVQrivMEvbFs6wt3jLt2FjOew,1922
+fw_utils-4.3.4.dist-info/WHEEL,sha256=Zb28QaM1gQi8f4VCBhsUklF61CTlNYfs9YAZn-TOGFk,88
+fw_utils-4.3.4.dist-info/RECORD,,
```

