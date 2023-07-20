# Comparing `tmp/hyload-0.2.1-py3-none-any.whl.zip` & `tmp/hyload-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 26033 bytes, number of entries: 17
+Zip file size: 26034 bytes, number of entries: 17
 -rw-rw-rw-  2.0 fat      171 b- defN 23-Jul-19 05:41 hyload/__init__.py
--rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-17 05:11 hyload/cfg.py
+-rw-rw-rw-  2.0 fat       17 b- defN 23-Jul-20 14:20 hyload/cfg.py
 -rw-rw-rw-  2.0 fat    15612 b- defN 23-Jul-20 02:58 hyload/httpclient.py
 -rw-rw-rw-  2.0 fat     2439 b- defN 23-Jul-08 14:54 hyload/logger.py
--rw-rw-rw-  2.0 fat    10770 b- defN 23-Jul-20 03:23 hyload/stats.py
+-rw-rw-rw-  2.0 fat    10760 b- defN 23-Jul-20 12:34 hyload/stats.py
 -rw-rw-rw-  2.0 fat      979 b- defN 23-Jul-08 14:54 hyload/util.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jul-08 14:54 hyload/tools/__init__.py
 -rw-rw-rw-  2.0 fat     3667 b- defN 23-Jul-08 14:54 hyload/tools/plotperf.py
 -rw-rw-rw-  2.0 fat     2802 b- defN 23-Jul-08 14:54 hyload/tools/plotresource.py
 -rw-rw-rw-  2.0 fat    39521 b- defN 23-Jul-08 14:54 hyload/tools/puttyagents.py
 -rw-rw-rw-  2.0 fat     3940 b- defN 23-Jul-20 08:38 hyload/tools/remoteop.py
 -rw-rw-rw-  2.0 fat     7493 b- defN 23-Jul-14 12:12 hyload/tools/statshub.py
--rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-20 11:21 hyload-0.2.1.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat     1482 b- defN 23-Jul-20 11:21 hyload-0.2.1.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 11:21 hyload-0.2.1.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-20 11:21 hyload-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-20 11:21 hyload-0.2.1.dist-info/RECORD
-17 files, 91403 bytes uncompressed, 23909 bytes compressed:  73.8%
+-rw-rw-rw-  2.0 fat     1100 b- defN 23-Jul-20 14:21 hyload-0.2.2.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat     1482 b- defN 23-Jul-20 14:21 hyload-0.2.2.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 14:21 hyload-0.2.2.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        7 b- defN 23-Jul-20 14:21 hyload-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1311 b- defN 23-Jul-20 14:21 hyload-0.2.2.dist-info/RECORD
+17 files, 91393 bytes uncompressed, 23910 bytes compressed:  73.8%
```

## zipnote {}

```diff
@@ -30,23 +30,23 @@
 
 Filename: hyload/tools/remoteop.py
 Comment: 
 
 Filename: hyload/tools/statshub.py
 Comment: 
 
-Filename: hyload-0.2.1.dist-info/LICENSE.txt
+Filename: hyload-0.2.2.dist-info/LICENSE.txt
 Comment: 
 
-Filename: hyload-0.2.1.dist-info/METADATA
+Filename: hyload-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: hyload-0.2.1.dist-info/WHEEL
+Filename: hyload-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: hyload-0.2.1.dist-info/top_level.txt
+Filename: hyload-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: hyload-0.2.1.dist-info/RECORD
+Filename: hyload-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## hyload/cfg.py

```diff
@@ -1 +1 @@
-Version = '0.2.1'
+Version = '0.2.2'
```

## hyload/stats.py

```diff
@@ -144,16 +144,16 @@
                       table,
                       tableName,
                       action,
                       statsOneSecond):
 
         # 如果前1秒 有记录， 打印出记录，并且加入发送给console的信息里
         if lastSecond in table:
-            if not cls.runFlag:
-                print(f'{strLastSecond}> {action} {table[lastSecond]:6}')
+            if cls.runFlag:
+                print(f'{strLastSecond} {action} {table[lastSecond]:6}')
             statsOneSecond[tableName] = table[lastSecond]
             table.pop(lastSecond)
         else:
             statsOneSecond[tableName] = 0
 
 
     # 一秒结束后的统计处理
@@ -185,16 +185,16 @@
         # eps
         cls._statsOneTable(strLastSecond,lastSecond,cls.errorTable, 'eps','error',statsOneSecond)
 
         # tps、respTimeSum 、 avgRespTime
         if lastSecond in cls.tpsTable:
             count = cls.tpsTable[lastSecond]
             avgRespTime = cls.responseTimeTable[lastSecond]/count  
-            if not cls.runFlag:
-                print(f'{strLastSecond}> recv {count:6} | avg lantency {avgRespTime:.4f}')
+            if cls.runFlag:
+                print(f'{strLastSecond} recv {count:6} | avg lantency {avgRespTime:.4f}')
 
             statsOneSecond['tps'] = count
             statsOneSecond['respTimeSum'] = round(cls.responseTimeTable[lastSecond],4)
             statsOneSecond['avgRespTime'] = round(avgRespTime,4)
 
             cls.tpsTable.pop(lastSecond)
             cls.responseTimeTable.pop(lastSecond)
```

## Comparing `hyload-0.2.1.dist-info/LICENSE.txt` & `hyload-0.2.2.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `hyload-0.2.1.dist-info/METADATA` & `hyload-0.2.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyload
-Version: 0.2.1
+Version: 0.2.2
 Summary: Framework for load testing
 Home-page: http://www.byhy.net
 Download-URL: https://pypi.python.org/pypi/hyload
 Author: baiyueheiyu 白月黑羽
 Author-email: jcyrss@gmail.com
 License: Apache License 2.0
 Keywords: hyload loadtesting
```

## Comparing `hyload-0.2.1.dist-info/RECORD` & `hyload-0.2.2.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 hyload/__init__.py,sha256=wXjdLCvcOlQV8a7Mku2cQbyWRXheGf7dGkHfjvBqKu8,171
-hyload/cfg.py,sha256=uisuY7nIEXhRqibyun63mFNRLab56cOQt7UjyfyPwrs,17
+hyload/cfg.py,sha256=5FDM-eOsLqzqxqtXBwnVdT4vctBDStFcdQ__igt6HEw,17
 hyload/httpclient.py,sha256=xsbuhB5Pg1to47J-lMcxSh3N2-bFqezK8KsfInoRYOk,15612
 hyload/logger.py,sha256=JR8uUXypCp9eaWvKZRT_pqtUYRbATkC2XCKIB9R_ptM,2439
-hyload/stats.py,sha256=x3JS7ZjYw3_1ecnaQc5pIMvnrNZN4lG5YlIffd3BecQ,10770
+hyload/stats.py,sha256=emUBJSTzSWh4mJJBFxzKTY-1ByLcCLsDZoLlqyBYp3M,10760
 hyload/util.py,sha256=lNKVVW4vYFueXcvOC4HoIMIiXFUz6skR9shSA7iPsWU,979
 hyload/tools/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 hyload/tools/plotperf.py,sha256=H1OszxmfgAYAxX4YEp-_aX66w6slynz9tjDGdpraMMo,3667
 hyload/tools/plotresource.py,sha256=9ydos2xFSA__ANhQ4b_fr5ORJPwWVLCgXoYnYdO5cA4,2802
 hyload/tools/puttyagents.py,sha256=NvL3VhYYka69kh7QTdRzjm7dLN3dB5MuU__K1GmGsW8,39521
 hyload/tools/remoteop.py,sha256=yyySauc3rSc03jsJ1n_6dKuIv-Vlo6W-TSC5EOI-VEQ,3940
 hyload/tools/statshub.py,sha256=bPyj9h6eewxRJSJmQpqtkx3DFbvoYbQsWpcFvATFang,7493
-hyload-0.2.1.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
-hyload-0.2.1.dist-info/METADATA,sha256=lFbcQoVIvxFCmzzUQKRg4ewnzlzYINYc4Ac3SPCxr5Y,1482
-hyload-0.2.1.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-hyload-0.2.1.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
-hyload-0.2.1.dist-info/RECORD,,
+hyload-0.2.2.dist-info/LICENSE.txt,sha256=OGhxEO0MAMle3LEQV8Us5uo4C8pk-jWmCBKyQ7U_gCE,1100
+hyload-0.2.2.dist-info/METADATA,sha256=TG_Iioma4bo34bSb4pafU3Ti5L5eecia4LTT4uRj0HM,1482
+hyload-0.2.2.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+hyload-0.2.2.dist-info/top_level.txt,sha256=ivEyc-v2p5WU0itBl-u9QARFubEqBlHfczIhYbuD_U8,7
+hyload-0.2.2.dist-info/RECORD,,
```

