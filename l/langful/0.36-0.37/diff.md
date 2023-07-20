# Comparing `tmp/langful-0.36-py3-none-any.whl.zip` & `tmp/langful-0.37-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 5528 bytes, number of entries: 7
+Zip file size: 5561 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-06 06:25 langful/__init__.py
--rw-rw-rw-  2.0 fat     9860 b- defN 23-Jul-18 02:04 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     3074 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      527 b- defN 23-Jul-18 02:05 langful-0.36.dist-info/RECORD
-7 files, 14793 bytes uncompressed, 4598 bytes compressed:  68.9%
+-rw-rw-rw-  2.0 fat    10023 b- defN 23-Jul-20 12:41 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     3050 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      528 b- defN 23-Jul-20 12:47 langful-0.37.dist-info/RECORD
+7 files, 14933 bytes uncompressed, 4631 bytes compressed:  69.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: langful/__init__.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.36.dist-info/LICENSE
+Filename: langful-0.37.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.36.dist-info/METADATA
+Filename: langful-0.37.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.36.dist-info/WHEEL
+Filename: langful-0.37.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.36.dist-info/top_level.txt
+Filename: langful-0.37.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.36.dist-info/RECORD
+Filename: langful-0.37.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -1,21 +1,21 @@
 """
 # lang
 """
 
 import json
 import os
-import re
 
 __all__ = [ "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
 
 def to_json( lang_file : str ) -> dict :
     """
     .lang -> .json
     """
+    import re
     ret = {}
     for line in lang_file.split( "\n" ) :
         text = re.split( "([^#^=^\\s]+|)(\\s+=\\s+|\\s+=|=\\s+|=|)([^#^\\n]+|)" , line )
         index = 0
         for value in text :
             if "=" in value :
                 ret[ "".join( text[ :index ] ) ] = "".join( text[ index + 1: ] )
@@ -28,14 +28,23 @@
     .json -> .lang
     """
     ret = ""
     for key , value in dict_file.items() :
         ret += f"{ key } = { value }\n"
     return ret
 
+def to_list( args : str | list ) -> list :
+    """
+    only use it in this file don't add it in __all__ list
+    """
+    if isinstance( args , list ) :
+        return args
+    else :
+        return [ args ]
+
 def getdefaultlocale() -> str :
     """
     getdefaultlocale will deprecated so use this
     """
     import locale
     import sys
     if sys.platform == "win32" :
@@ -273,47 +282,47 @@
         locale = self.locale_get( locale )
         del self.languages[ locale ][ key ]
 
     def merge( self , locale : str = None , args : str | list = [] ) -> dict :
         """
         merge
         """
-        if isinstance( args , str ) :
-            args = [ args ]
+        args = to_list( args )
         ret = self.lang_get( self.locale_get( locale ) )
         for locale_key in args :
             for key , value in self.lang_get( locale_key ).items() :
                 ret[ key ] = value
         return ret
 
     def save( self , separators : list = [ " ," , ": " ] ) -> dict :
         """
         save file when is_file variable is true
         """
-        if isinstance( self.lang_dir , str ) :
+        if self.is_file :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
                 with open( os.path.join( self.lang_dir , key + suffix ) , "w" , encoding = "utf-8" ) as file :
                     if suffix == ".json" :
-                        file.write( json.dumps( value , indent = 4 , separators = separators , ensure_ascii = False ) )
+                        json.dump( value , file , indent = 4 , separators = separators , ensure_ascii = False )
                     elif suffix == ".lang" :
                         file.write( to_lang( value ) )
         return self.languages
 
     def replace( self , key : str = None , args : str | list  = None , locale : str = None , replace_letter : str = None ) -> str :
         """
         replace
         """
         replace_letter = self.replace_letter_get( replace_letter )
         locale = self.locale_get( locale )
-        if isinstance( args , str ) :
-            args = [ args ]
+        args = to_list( args )
         index = 0
         ret = ""
-        for text in re.split( f"({ replace_letter }+)" , self.get( key , locale ) ) :
-            if text != replace_letter :
-                ret += text
+        for text in self.get( key , locale ) :
+            if text == replace_letter :
+                if len( ret ) and ret[ -1 ] == "\\" :
+                    ret = ret[ : -1 ] + replace_letter
+                else :
+                    ret += str( args[ index ] )
+                    index += index < len( args ) - 1
             else :
-                ret += text.replace( replace_letter , str( args[ index ] ) )
-                if index + 1 < len( args ) :
-                    index += 1
+                ret += text
         return ret
```

## Comparing `langful-0.36.dist-info/LICENSE` & `langful-0.37.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.36.dist-info/METADATA` & `langful-0.37.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.36
+Version: 0.37
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -61,15 +61,17 @@
     "key": "value" ,
     "..." : "..."
 }
 ```
 
 .lang
 
-> if you need highlight, you can install `vscode-langful` : [GitHub](https://github.com/cueavy/vscode-langful) [VSCode](https://marketplace.visualstudio.com/items?itemName=cueavyqwp.langful)
+> if you need highlight, you can install `vscode-langful` :
+[GitHub](https://github.com/cueavy/vscode-langful)
+[VSCode](https://marketplace.visualstudio.com/items?itemName=cueavyqwp.langful)
 
 ```
 key = value # hi, this is a example
 # hi, I am a example, too
 ... = ...
 ```
 
@@ -113,18 +115,17 @@
 
 ## function
 
 ### replace
 
 ```python
 lang = langful.lang( False )
-lang.replace_letter = "&"
 lang.init_dict( {
     "en_us" : {
-        "test" : "&.&%"
+        "test" : "%.%\%"
     }
 } )
 print( lang.replace( "test" , [ 33 , 3 ] ) )
 ```
 
 ### merge
```

