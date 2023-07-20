# Comparing `tmp/panda_client_light-1.5.62-py2.py3-none-any.whl.zip` & `tmp/panda_client_light-1.5.63-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 156203 bytes, number of entries: 36
+Zip file size: 156204 bytes, number of entries: 36
 -rw-r--r--  2.0 unx    63478 b- defN 20-Feb-02 00:00 pandaclient/AthenaUtils.py
 -rw-r--r--  2.0 unx     2276 b- defN 20-Feb-02 00:00 pandaclient/BookConfig.py
 -rwxr-xr-x  2.0 unx    32382 b- defN 20-Feb-02 00:00 pandaclient/BookGUI.py
 -rwxr-xr-x  2.0 unx    64256 b- defN 20-Feb-02 00:00 pandaclient/Client.py
 -rwxr-xr-x  2.0 unx     3118 b- defN 20-Feb-02 00:00 pandaclient/FileSpec.py
 -rw-r--r--  2.0 unx     4175 b- defN 20-Feb-02 00:00 pandaclient/Group_argparse.py
 -rwxr-xr-x  2.0 unx    27030 b- defN 20-Feb-02 00:00 pandaclient/JobSpec.py
@@ -28,11 +28,11 @@
 -rw-r--r--  2.0 unx     4163 b- defN 20-Feb-02 00:00 pandaclient/localSpecs.py
 -rw-r--r--  2.0 unx    10226 b- defN 20-Feb-02 00:00 pandaclient/openidc_utils.py
 -rw-r--r--  2.0 unx    10528 b- defN 20-Feb-02 00:00 pandaclient/panda_api.py
 -rw-r--r--  2.0 unx     4975 b- defN 20-Feb-02 00:00 pandaclient/panda_gui.py
 -rw-r--r--  2.0 unx     4025 b- defN 20-Feb-02 00:00 pandaclient/panda_jupyter.py
 -rw-r--r--  2.0 unx     7280 b- defN 20-Feb-02 00:00 pandaclient/pcontainer_core.py
 -rw-r--r--  2.0 unx     4281 b- defN 20-Feb-02 00:00 pandaclient/queryPandaMonUtils.py
-?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.62.dist-info/METADATA
-?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.62.dist-info/WHEEL
-?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.62.dist-info/RECORD
-36 files, 660506 bytes uncompressed, 151483 bytes compressed:  77.1%
+?rw-r--r--  2.0 unx      894 b- defN 20-Feb-02 00:00 panda_client_light-1.5.63.dist-info/METADATA
+?rw-r--r--  2.0 unx      105 b- defN 20-Feb-02 00:00 panda_client_light-1.5.63.dist-info/WHEEL
+?rw-r--r--  2.0 unx     2992 b- defN 20-Feb-02 00:00 panda_client_light-1.5.63.dist-info/RECORD
+36 files, 660506 bytes uncompressed, 151484 bytes compressed:  77.1%
```

## zipnote {}

```diff
@@ -93,17 +93,17 @@
 
 Filename: pandaclient/pcontainer_core.py
 Comment: 
 
 Filename: pandaclient/queryPandaMonUtils.py
 Comment: 
 
-Filename: panda_client_light-1.5.62.dist-info/METADATA
+Filename: panda_client_light-1.5.63.dist-info/METADATA
 Comment: 
 
-Filename: panda_client_light-1.5.62.dist-info/WHEEL
+Filename: panda_client_light-1.5.63.dist-info/WHEEL
 Comment: 
 
-Filename: panda_client_light-1.5.62.dist-info/RECORD
+Filename: panda_client_light-1.5.63.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pandaclient/PandaToolsPkgInfo.py

```diff
@@ -1 +1 @@
-release_version = "1.5.62"
+release_version = "1.5.63"
```

## Comparing `panda_client_light-1.5.62.dist-info/METADATA` & `panda_client_light-1.5.63.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: panda-client-light
-Version: 1.5.62
+Version: 1.5.63
 Summary: Lightweight PanDA Client Package installed on PanDA server
 Project-URL: Homepage, https://panda-wms.readthedocs.io/en/latest/
 Author-email: PanDA Team <atlas-adc-panda@cern.ch>
 License-Expression: Apache-2.0
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 2.7
```

## Comparing `panda_client_light-1.5.62.dist-info/RECORD` & `panda_client_light-1.5.63.dist-info/RECORD`

 * *Files 7% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 pandaclient/LocalJobSpec.py,sha256=rVMgk4KVhMY1hjWnsaIL9cWVAZMEKVOnE4vQqz7cHWU,13691
 pandaclient/LocalJobsetSpec.py,sha256=nYQMhKrbCtzm68ZWnEXCs_-mWvATm9XClm514aJ-7cU,11007
 pandaclient/MiscUtils.py,sha256=SQWcqhHOW_tmahjb1zbO62zP-uBcB51SJB4ERyYtt5Y,10225
 pandaclient/MyproxyUtils.py,sha256=7eNIdr6Vt8phcW5FVbt5mZ10I4tZH0n-xAuKBk-GcQI,15025
 pandaclient/PBookCore.py,sha256=134Ubc_RG2SMjmgeNs6s_op-3zpyFFOcNLMqd89f8bs,17679
 pandaclient/PBookScript.py,sha256=zgH4LHQeXkyeM1rxtQ64KN0lFDM3wAqpsRf5QVYzp_I,19506
 pandaclient/PLogger.py,sha256=1R0xMlWsHLdptyb-ewt_o6NVveK07ENmKBoE-NKtyJw,1167
-pandaclient/PandaToolsPkgInfo.py,sha256=DgpK_Vd51wh3kvj-UKRqYIckaSiSmSvK_9oGXxHm1_0,27
+pandaclient/PandaToolsPkgInfo.py,sha256=SELeZK15mRUTGxxNBkyyIMb8Pf7X-GMOEe84MJ0q5jw,27
 pandaclient/ParseJobXML.py,sha256=GWdiTXhRZOVIqxUT4laZZ13WQ5HZs4V2PgichtyQ4Ec,15441
 pandaclient/PathenaScript.py,sha256=LcUwCNrAmN2m2DOdhJqPjRlJiMPN8SRkSn5fOX-u-AM,104988
 pandaclient/PchainScript.py,sha256=QyQS6i_Espb-BwajMyGTfngQJdvqUZICPUDnhKpZnkI,11696
 pandaclient/PcontainerScript.py,sha256=J7EiyUfBmMPHXvdwbPE7t9redP6JhdWmCZa3Yg27fRQ,247
 pandaclient/PdbUtils.py,sha256=TNsmCb___D1JevvocLWMUUKajA10Zo62VjdqDx4-Law,24834
 pandaclient/PhpoScript.py,sha256=9CyzSvppDrcDYyAJ1aHNzOMRgGIY2gRuibCK9wim6E8,27466
 pandaclient/PrunScript.py,sha256=MtceatuP1BqxAEq0n0GtA2C5W_SnseQaNfe93JumK3E,104655
@@ -27,10 +27,10 @@
 pandaclient/localSpecs.py,sha256=Cx9ZNTaOvFIWbk_u9f7Xg9s_4zJdhyksAeMWNwHKbt0,4163
 pandaclient/openidc_utils.py,sha256=nV4cq1n9jDgGXn8FqoERBDHDnFEJMTYuZ7HqIbWKqaU,10226
 pandaclient/panda_api.py,sha256=eNLVvzBiqjANFbqED_AX-K3UI7tASl0fHml8SAMuIkw,10528
 pandaclient/panda_gui.py,sha256=5nW5RsYaXuDcgsxj8SCXvnrZrC117bg70OBZRXqjIvY,4975
 pandaclient/panda_jupyter.py,sha256=buiC8kGSA_KCaZ9TF6XLbfi0hwHi9d6_npDXitRlkCA,4025
 pandaclient/pcontainer_core.py,sha256=k_HjWhLtGPVtnRgK1yaMzEY0XgiBz3XHZt-rVoLf04c,7280
 pandaclient/queryPandaMonUtils.py,sha256=7NqvwjMAgpJC9re4qKe7W6Zn9E7CRzyL1yHmp9yndsg,4281
-panda_client_light-1.5.62.dist-info/METADATA,sha256=qYH6pXiwMYPMInRRHZIQXwK7Uy2u70HV1-NlQeScruU,894
-panda_client_light-1.5.62.dist-info/WHEEL,sha256=fagL_Tj29mg80flwlxJNW45nBDbboxF04Tnbc_jt3Bg,105
-panda_client_light-1.5.62.dist-info/RECORD,,
+panda_client_light-1.5.63.dist-info/METADATA,sha256=hIkUWohO2YydTbpJuCk2HhZDykDZlooNL6ws89NeQWI,894
+panda_client_light-1.5.63.dist-info/WHEEL,sha256=fagL_Tj29mg80flwlxJNW45nBDbboxF04Tnbc_jt3Bg,105
+panda_client_light-1.5.63.dist-info/RECORD,,
```

