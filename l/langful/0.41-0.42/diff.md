# Comparing `tmp/langful-0.41-py3-none-any.whl.zip` & `tmp/langful-0.42-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 5653 bytes, number of entries: 8
+Zip file size: 5771 bytes, number of entries: 8
 -rw-rw-rw-  2.0 fat      166 b- defN 23-Jul-30 07:47 langful/__init__.py
 -rw-rw-rw-  2.0 fat      382 b- defN 23-Jul-30 12:15 langful/errors.py
--rw-rw-rw-  2.0 fat     8308 b- defN 23-Jul-30 12:55 langful/lang.py
--rw-rw-rw-  2.0 fat     1066 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2984 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        8 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      600 b- defN 23-Jul-30 12:57 langful-0.41.dist-info/RECORD
-8 files, 13606 bytes uncompressed, 4613 bytes compressed:  66.1%
+-rw-rw-rw-  2.0 fat     8961 b- defN 23-Aug-04 11:05 langful/lang.py
+-rw-rw-rw-  2.0 fat     1066 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     2984 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        8 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      600 b- defN 23-Aug-04 11:07 langful-0.42.dist-info/RECORD
+8 files, 14259 bytes uncompressed, 4731 bytes compressed:  66.8%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: langful/errors.py
 Comment: 
 
 Filename: langful/lang.py
 Comment: 
 
-Filename: langful-0.41.dist-info/LICENSE
+Filename: langful-0.42.dist-info/LICENSE
 Comment: 
 
-Filename: langful-0.41.dist-info/METADATA
+Filename: langful-0.42.dist-info/METADATA
 Comment: 
 
-Filename: langful-0.41.dist-info/WHEEL
+Filename: langful-0.42.dist-info/WHEEL
 Comment: 
 
-Filename: langful-0.41.dist-info/top_level.txt
+Filename: langful-0.42.dist-info/top_level.txt
 Comment: 
 
-Filename: langful-0.41.dist-info/RECORD
+Filename: langful-0.42.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## langful/lang.py

```diff
@@ -4,15 +4,15 @@
 
 from . import errors
 
 import json
 import os
 
 __all__ = [ "__version__" , "to_json" , "to_lang" , "getdefaultlocale" , "lang" ]
-__version__ = "0.41"
+__version__ = "0.42"
 
 def to_json( text : str ) -> dict[ str , str ] :
     from re import split
     ret = {}
     for line in text.split( "\n" ) :
         try :
             ret.update( dict( [ split( "\\s=\\s" , line.split( "#" )[ 0 ] , 1 ) ] ) )
@@ -28,24 +28,23 @@
     getdefaultlocale will deprecated so use this
     """
     from locale import getlocale
     from sys import platform
     if platform == "win32" :
         code = __import__( "_locale" )._getdefaultlocale()[ 0 ]
         if code and code[ : 2 ] == "0x" :
-            from locale import windows_locale
-            code = windows_locale.get( int( code , 0 ) )
+            code = __import__( "locale" ).windows_locale.get( int( code , 0 ) )
     else :
         code = getlocale()[ 0 ]
     return code.replace( "-" , "_" ).lower()
 
 class lang :
 
     locale_system = getdefaultlocale()
-    __slots__ = [ "locale_default" , "locale_use" , "languages" , "path" , "configs" , "types" ]
+    __slots__ = [ "locale_default" , "locale_use" , "languages" , "configs" , "types" , "path" ]
 
     @property
     def locale( self ) -> str :
         for locale in [ self.locale_use , self.locale_system , self.locale_default ] :
             if locale and locale in self.locales :
                 return locale
         raise errors.LocaleError( f"no such locale '{ self.locale_system }' or '{ self.locale_default }'" )
@@ -71,26 +70,41 @@
 
     def __setitem__( self , key , value ) -> None :
         self.set( key , value )
 
     def __delitem__( self , key ) -> None :
         self.remove( key )
 
-    def __str__( self ) -> str :
-        return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.configs[ "separators" ] )
+    def __contains__( self , item ) -> bool :
+        return item in self.languages
 
-    def __len__( self ) -> int :
-        return len( self.language )
+    def __enter__( self ) -> dict[ str , str ] :
+        return self.languages
+
+    def __iter__( self ) -> tuple[ dict[ str , str ] ] :
+        return iter( self.keys() )
+
+    def __exit__( self , *args ) -> None :
+        self.save() if all( item is None for item in args ) else ...
 
     def __bool__( self ) -> bool :
         return self.locale_system in self.languages
 
+    def __repr__( self ) -> str :
+        return str( self.languages )
+
     def __call__( self ) -> None :
         self.init()
 
+    def __str__( self ) -> str :
+        return json.dumps( self.languages , indent = 4 , ensure_ascii = False , separators = self.configs[ "separators" ] )
+
+    def __len__( self ) -> int :
+        return len( self.language )
+
     def __init__( self , path : str | dict = "lang" , locale_default : str = "en_us" , json_first : bool = True ) -> None :
         """
         path: lang files dir, if use dict to set that to a dictionary or False
         locale_default: default locale
         load: is load json file first
         """
         self.configs = { "separators" : [ " ," , ": " ] , "replace" : "%" , "load" : json_first , "file" : False }
@@ -146,22 +160,30 @@
         self.configs[ "file" ] = False
         self.languages = language
         self.path = language
 
     def to_dict( self ) :
         self.types = { key : ".json" for key in self.languages.keys() }
         self.configs[ "file" ] = False
-        self.path = self.languages
 
     def to_file( self , path ) :
         if not os.path.exists( path ) :
             os.makedirs( path )
         self.configs[ "file" ] = True
         self.path = path
 
+    def values( self ) -> tuple[ dict[ str , str ] ] :
+        return self.languages.values()
+
+    def items( self ) -> tuple[ str , dict[ str , str ] ] :
+        return self.languages.items()
+
+    def keys( self ) -> tuple[ str ] :
+        return self.languages.keys()
+
     def locale_get( self , locale : str = None ) -> str :
         return locale if locale else self.locale
 
     def locale_set( self , locale : str = None  ) -> None :
         if locale and locale not in self.locales :
             raise errors.LocaleError( f"no such locale '{ locale }'" )
         self.locale_use = locale
@@ -189,16 +211,15 @@
         self.languages[ self.locale_get( locale ) ][ key ] = value
 
     def remove( self , key : str , locale : str = None ) -> None :
         del self.languages[ self.locale_get( locale ) ][ key ]
 
     def merge( self , locale : str = None , args : list[ str ] = [] ) -> dict[ str , str ] :
         ret = self.lang_get( locale )
-        for locale_key in args :
-            ret.update( self.lang_get( locale_key ) )
+        [ ret.update( self.lang_get( key ) ) for key in args ]
         return ret
 
     def save( self ) -> dict[ str , str ] :
         if self.configs[ "file" ] :
             for key , value in self.languages.items() :
                 suffix = self.types[ key ]
                 with open( os.path.join( self.path , key + suffix ) , "w" , encoding = "utf-8" ) as file :
```

## Comparing `langful-0.41.dist-info/LICENSE` & `langful-0.42.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `langful-0.41.dist-info/METADATA` & `langful-0.42.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: langful
-Version: 0.41
+Version: 0.42
 Summary: Help to localization
 Home-page: https://github.com/cueavy/langful
 Author: cueavyqwp
 Author-email: cueavyqwp@outlook.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

## Comparing `langful-0.41.dist-info/RECORD` & `langful-0.42.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 langful/__init__.py,sha256=BSJ-BT1Yr3Xz-SFnmZu7QvgV5pgg2WEqUO42oM3Py2w,166
 langful/errors.py,sha256=2Ag2tnAPSzozEIzye5U-mnyvSmvk5X8ZqB3kwLhGOIs,382
-langful/lang.py,sha256=0fEXuuM2--rtU-plANTXtEJDCQG6qnzbKdw9GVXQ77o,8308
-langful-0.41.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
-langful-0.41.dist-info/METADATA,sha256=VrZQbsdkCLGISKnVVIPYwh_k3uW9whNuWxsAURjCmpY,2984
-langful-0.41.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
-langful-0.41.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
-langful-0.41.dist-info/RECORD,,
+langful/lang.py,sha256=vxWyvoqf2zMMscimKBNUlBm2_7nkLzSIc_fUvgHdr14,8961
+langful-0.42.dist-info/LICENSE,sha256=JrQca6fL66RGTmf-hkJU9UEX64JB0yE9gKNsOhpmZVE,1066
+langful-0.42.dist-info/METADATA,sha256=8K6zixJvXukIPEtxZr2d7nCSDqkL60FBjfofOg7oUXI,2984
+langful-0.42.dist-info/WHEEL,sha256=AtBG6SXL3KF_v0NxLf0ehyVOh0cold-JbJYXNGorC6Q,92
+langful-0.42.dist-info/top_level.txt,sha256=EkKV_WnIZfE3A6EhWwDIt2uwZhMVHWXTUueKJL6K15w,8
+langful-0.42.dist-info/RECORD,,
```

