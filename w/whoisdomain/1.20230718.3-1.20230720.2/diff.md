# Comparing `tmp/whoisdomain-1.20230718.3.tar.gz` & `tmp/whoisdomain-1.20230720.2.tar.gz`

## Comparing `whoisdomain-1.20230718.3.tar` & `whoisdomain-1.20230720.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     4549 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10089 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    13856 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18029 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/main.py
--rw-r--r--   0        0        0   132545 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/.gitignore
--rw-r--r--   0        0        0    10056 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/pyproject.toml
--rw-r--r--   0        0        0    10979 2020-02-02 00:00:00.000000 whoisdomain-1.20230718.3/PKG-INFO
+-rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_0_init_tld.py
+-rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_1_query.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_2_parse.py
+-rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_3_adjust.py
+-rw-r--r--   0        0        0    14196 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/__init__.py
+-rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/exceptions.py
+-rwxr-xr-x   0        0        0    18420 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/main.py
+-rw-r--r--   0        0        0   132995 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/tld_regexpr.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/.gitignore
+-rw-r--r--   0        0        0    10341 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/README.md
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/pyproject.toml
+-rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/PKG-INFO
```

### Comparing `whoisdomain-1.20230718.3/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230720.2/whoisdomain/_0_init_tld.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,18 +124,18 @@
     for name in zz:
         # print(name)
         z = zz[name]
         for key in z:
             if key is None:
                 continue
 
-            if key.startswith("_"):
+            if key.startswith("_"):  # skip meta keys, they are not regexes
                 continue
 
-            if key in ["extend"]:
+            if key in ["extend"]:  # this actually should have been a meta key: "_extend"
                 continue
 
             if key not in regCollection:
                 regCollection[key] = {}
 
             reg = z[key]
             if reg is None:
```

### Comparing `whoisdomain-1.20230718.3/whoisdomain/_1_query.py` & `whoisdomain-1.20230720.2/whoisdomain/_1_query.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230718.3/whoisdomain/_2_parse.py` & `whoisdomain-1.20230720.2/whoisdomain/_2_parse.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,26 +23,26 @@
 
 Verbose: bool = True
 
 NONESTRINGS: List[str] = [
     "the domain has not been registered",
     "no match found for",
     "no matching record",
+    "no match",
     "not found",
     "no data found",
     "no entries found",
-    "status: free",
+    # "status: free", # we should not interprete the result if there is a result
     "no such domain",
     "the queried object does not exist",
     "domain you requested is not known",
-    "status: available",
+    # "status: available", # we should not interprete the result if there is a result
     "no whois server is known for this kind of object",
     "nameserver not found",
     "malformed request",  # this means this domain is not in whois as it is on top of a registered domain
-    "no match",
     "registration of this domain is restricted",
     "restricted",
     "this domain is currently available",
 ]
 
 QUOTASTRINGS: List[str] = [
     "limit exceeded",
@@ -282,24 +282,24 @@
 
         tmp2.append(line.strip("\r"))
 
     return "\n".join(tmp2)
 
 
 def NoneStrings() -> List[str]:
-    return sorted(NONESTRINGS)
+    return NONESTRINGS
 
 
 def NoneStringsAdd(aString: str) -> None:
     if aString and isinstance(aString, str) and len(aString) > 0:
         NONESTRINGS.append(aString)
 
 
 def QuotaStrings() -> List[str]:
-    return sorted(QUOTASTRINGS)
+    return QUOTASTRINGS
 
 
 def QuotaStringsAdd(aString: str) -> None:
     if aString and isinstance(aString, str) and len(aString) > 0:
         NONESTRINGS.append(aString)
```

### Comparing `whoisdomain-1.20230718.3/whoisdomain/_3_adjust.py` & `whoisdomain-1.20230720.2/whoisdomain/_3_adjust.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230718.3/whoisdomain/__init__.py` & `whoisdomain-1.20230720.2/whoisdomain/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,14 +73,15 @@
     "query",
     # from parse
     "NoneStrings",
     "NoneStringsAdd",
     "QuotaStrings",
     "QuotaStringsAdd",
     "cleanupWhoisResponse",
+    "getTestHint",
 ]
 
 WHOISDOMAIN: str = ""
 if os.getenv("WHOISDOMAIN"):
     WHOISDOMAIN = str(os.getenv("WHOISDOMAIN"))
 
 WD = WHOISDOMAIN.upper().split(":")
@@ -174,14 +175,15 @@
 
 def _doServerHintsForThisTld(
     tld: str,
     thisTld: Dict[str, Any],
     server: Optional[str],
     verbose: bool = False,
 ) -> Optional[str]:
+    # note _server hints currently are not passes down when using "extend", that may have been my error during the initial implementation
     # allow server hints using "_server" from the tld_regexpr.py file
     thisTldServer = thisTld.get("_server")
     if server is None and thisTldServer:
         server = thisTldServer
         if verbose:
             print(f"using _server hint {server} for tld: {tld}", file=sys.stderr)
     return server
@@ -491,7 +493,18 @@
 
 # Add get function to support return result in dictionary form
 get = _result2dict(query)
 
 
 def getVersion() -> str:
     return VERSION
+
+
+def getTestHint(tld: str) -> Optional[str]:
+    if tld not in ZZ:
+        return None
+
+    k: str = "_test"
+    if k not in ZZ[tld]:
+        return None
+
+    return str(ZZ[tld][k])
```

### Comparing `whoisdomain-1.20230718.3/whoisdomain/exceptions.py` & `whoisdomain-1.20230720.2/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230718.3/whoisdomain/main.py` & `whoisdomain-1.20230720.2/whoisdomain/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 PrintJson: bool = False
 Verbose: bool = False
 PrintGetRawWhoisResult: bool = False
 Ruleset: bool = False
 
 Failures: Dict[str, Any] = {}
 IgnoreReturncode: bool = False
+TestAllTld: bool = False
 
 
 class ResponseCleaner:
     data: str
     rDict: Dict[str, Any] = {}
 
     def __init__(
@@ -204,14 +205,15 @@
 def testItem(
     d: str,
     printgetRawWhoisResult: bool = False,
 ) -> None:
     global PrintGetRawWhoisResult
     global SIMPLISTIC
     global WithRedacted
+    global TestAllTld
 
     timeout = 30  # seconds
 
     w = whois.query(
         d,
         ignore_returncode=IgnoreReturncode,
         verbose=Verbose,
@@ -345,21 +347,34 @@
     return whois.validTlds()
 
 
 def makeMetaAllCurrentTld(
     allHaving: Optional[str] = None,
     allRegex: Optional[str] = None,
 ) -> List[str]:
+    global TestAllTld
+
+    def appendHint(
+        allRegex: Optional[str],
+        tld: str,
+    ) -> None:
+        if TestAllTld is True:
+            hint = whois.getTestHint(tld)
+            hint = hint if hint else f"meta.{tld}"
+            rr.append(f"{hint}")
+        else:
+            rr.append(f"meta.{tld}")
+
     rr: List[str] = []
     for tld in getAllCurrentTld():
         if allRegex:
             if re.search(allRegex, tld):
-                rr.append(f"meta.{tld}")
+                appendHint(allRegex, tld)
         else:
-            rr.append(f"meta.{tld}")
+            appendHint(allRegex, tld)
 
     return rr
 
 
 def showAllCurrentTld() -> None:
     print("Tld's currently supported")
     for tld in getAllCurrentTld():
@@ -473,14 +488,15 @@
     global PrintJson
     global Verbose
     global IgnoreReturncode
     global PrintGetRawWhoisResult
     global Ruleset
     global SIMPLISTIC
     global WithRedacted
+    global TestAllTld
 
     name: str = os.path.basename(sys.argv[0])
     if name == "test2.py":
         SIMPLISTIC = False
     else:
         SIMPLISTIC = True
 
@@ -506,15 +522,15 @@
                 "withRedacted",
             ],
         )
     except getopt.GetoptError:
         usage()
         sys.exit(2)
 
-    testAllTld: bool = False
+    # TestAllTld: bool = False
 
     allHaving: Optional[str] = None  # from all supported tld only process the ones having this :: TODO ::
     allRegex: Optional[str] = None  # from all supported tld process only the ones matching this regex
 
     directory: Optional[str] = None
     dirs: List[str] = []
 
@@ -540,22 +556,22 @@
             usage()
             sys.exit(0)
 
         if opt in ("--withRedacted"):
             WithRedacted = True
 
         if opt in ("-a", "--all"):
-            testAllTld = True
+            TestAllTld = True
 
         if opt in ("-H", "--having"):
-            testAllTld = True
+            TestAllTld = True
             allHaving = str(arg)
 
         if opt in ("-r", "--reg"):
-            testAllTld = True
+            TestAllTld = True
             allRegex = str(arg)
 
         if opt in ("-v", "--verbose"):
             Verbose = True
 
         if opt in ("-p", "--print"):
             PrintGetRawWhoisResult = True
@@ -590,30 +606,30 @@
             isFile = os.path.isfile(filename)
             if isFile is False:
                 print(f"{filename} cannot be found or is not a file", file=sys.stderr)
                 sys.exit(101)
 
             if filename not in files:
                 files.append(filename)
-                testAllTld = False
+                TestAllTld = False
 
         if opt in ("-d", "--domain"):
             domain = arg
             if domain not in domains:
                 domains.append(domain)
 
     if Verbose:
         print(f"{name} SIMPLISTIC: {SIMPLISTIC}", file=sys.stderr)
 
     if Ruleset is True and len(domains):
         for domain in domains:
             ShowRuleset(domain)
         sys.exit(0)
 
-    if testAllTld:
+    if TestAllTld:
         allMetaTld = makeMetaAllCurrentTld(allHaving, allRegex)
         testDomains(allMetaTld)
         showFailures()
         sys.exit(0)
 
     if len(dirs):
         fileData = {}
```

### Comparing `whoisdomain-1.20230718.3/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230720.2/whoisdomain/tld_regexpr.py`

 * *Files 0% similar despite different names*

```diff
@@ -283,32 +283,41 @@
     "status": r"Status:\s?(.+)",
 }
 
 ZZ["com.au"] = {
     "extend": "au",
 }
 
+ZZ["tr"] = {"extend": "_privateReg"}  # whois.nic.tr is an alias for whois.trabis.gov.tr.
+
 ZZ["com.tr"] = {
     "extend": "com",
     "domain_name": r"\*\* Domain Name:\s?(.+)",
     "registrar": r"Organization Name\s+:\s?(.+)",
     "registrant": r"\*\* Registrant:\s+?(.+)",
     "registrant_country": None,
     "creation_date": r"Created on\.+:\s?(.+).",
     "expiration_date": r"Expires on\.+:\s?(.+).",  # note the trailing . on both dates fields
     "updated_date": "",
-    "name_servers": r"\*\* Domain Servers:\n(?:(\S+)\n)(?:(\S+)\n)?(?:(\S+)\n)?(?:(\S+)\n)?(?:(\S+)\n)?(?:(\S+)\n)\n?",
+    "name_servers": r"\*\* Domain Servers:\n(?:(\S+).*\n)?(?:(\S+).*\n)?(?:(\S+).*\n)?(?:(\S+).*\n)?",  # allow for ip addresses after the name server
     "status": None,
+    "_server": "whois.trabis.gov.tr",
+    "_test": "google.com.tr",
 }
 
-ZZ["edu.tr"] = {"extend": "com.tr"}
+ZZ["gov.tr"] = {
+    "extend": "com.tr",
+    "_server": "whois.trabis.gov.tr",
+    "_test": "www.turkiye.gov.tr",
+}
 
-ZZ["org.tr"] = {"extend": "com.tr"}
+ZZ["edu.tr"] = {"extend": "com.tr", "_server": "whois.trabis.gov.tr", "_test": "anadolu.edu.tr"}
+ZZ["org.tr"] = {"extend": "com.tr", "_server": "whois.trabis.gov.tr", "_test": "dergipark.org.tr"}
+ZZ["net.tr"] = {"extend": "com.tr", "_server": "whois.trabis.gov.tr", "_test": "trt.net.tr"}
 
-ZZ["net.tr"] = {"extend": "com.tr"}
 
 ZZ["co.il"] = {
     "extend": "com",
     "domain_name": r"domain:\s*(.+)",
     "registrar": r"registrar name:\s*(.+)",
     "registrant": None,
     "registrant_country": None,
@@ -2068,15 +2077,14 @@
 ZZ["realestate"] = {"_server": "whois.nic.realestate", "extend": "com"}
 ZZ["ph"] = {"extend": "_privateReg"}
 ZZ["com.ph"] = {"extend": "ph"}
 ZZ["org.ph"] = {"extend": "ph"}
 ZZ["net.ph"] = {"extend": "ph"}
 ZZ["zm"] = {"extend": "com"}
 ZZ["sy"] = {"extend": "_privateReg", "_server": "whois.tld.sy"}
-ZZ["tr"] = {"extend": "_privateReg"}
 ZZ["onl"] = {"extend": "com"}
 ZZ["blue"] = {"extend": "com"}
 ZZ["garden"] = {"extend": "com", "_server": "whois.nic.garden"}
 ZZ["promo"] = {"extend": "com", "_server": "whois.nic.promo"}
 
 ZZ["pyc"] = {"extend": "com"}
```

### Comparing `whoisdomain-1.20230718.3/.gitignore` & `whoisdomain-1.20230720.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230718.3/README.md` & `whoisdomain-1.20230720.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -209,8 +209,10 @@
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
   * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
   * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
-  * 1.20230718.2 fix typo in whois server hint for tld: ru
+  * 1.20230718.3 fix typo in whois server hint for tld: ru
+  * 1.20230720.1 add gov.tr; switch off status:available and status:free as None response, we should not interprete the result by default (we can add a option later)
+  * 1.20230720.2 fix server hints for derived second level "xxx.tr", add processing "_test" hints during 'test2.py -a'
```

### Comparing `whoisdomain-1.20230718.3/pyproject.toml` & `whoisdomain-1.20230720.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230718.3/PKG-INFO` & `whoisdomain-1.20230720.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230718.3
+Version: 1.20230720.2
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -230,8 +230,10 @@
 ## Updates
   * 1.20230627.2 add Kenia proper whois server and known second level domains
   * 1.20230627.3 add rw tld proper whois server and second level ; restore mistakenly deleted .toml file
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
   * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
   * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
-  * 1.20230718.2 fix typo in whois server hint for tld: ru
+  * 1.20230718.3 fix typo in whois server hint for tld: ru
+  * 1.20230720.1 add gov.tr; switch off status:available and status:free as None response, we should not interprete the result by default (we can add a option later)
+  * 1.20230720.2 fix server hints for derived second level "xxx.tr", add processing "_test" hints during 'test2.py -a'
```

