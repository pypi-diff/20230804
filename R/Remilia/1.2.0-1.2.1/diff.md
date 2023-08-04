# Comparing `tmp/remilia-1.2.0.tar.gz` & `tmp/remilia-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "remilia-1.2.0.tar", last modified: Sun Jul 30 03:02:46 2023, max compression
+gzip compressed data, was "remilia-1.2.1.tar", last modified: Fri Aug  4 09:29:35 2023, max compression
```

## Comparing `remilia-1.2.0.tar` & `remilia-1.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1063 2023-07-30 03:02:06.674510 remilia-1.2.0/LICENSE
--rw-r--r--   0        0        0     1063 2023-07-30 03:02:06.674510 remilia-1.2.0/LICENSE
--rw-r--r--   0        0        0     1009 2023-07-30 03:02:06.674510 remilia-1.2.0/README.md
--rw-r--r--   0        0        0     1009 2023-07-30 03:02:06.674510 remilia-1.2.0/README.md
--rw-r--r--   0        0        0     1282 2023-07-30 03:02:46.158661 remilia-1.2.0/pyproject.toml
--rw-r--r--   0        0        0      185 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/__init__.py
--rw-r--r--   0        0        0       21 2023-07-30 03:02:46.154661 remilia-1.2.0/src/Remilia/__version__.py
--rw-r--r--   0        0        0      102 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/__init__.py
--rw-r--r--   0        0        0      113 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/exceptions.py
--rw-r--r--   0        0        0      695 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/models.py
--rw-r--r--   0        0        0     1920 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/base/rtypes.py
--rw-r--r--   0        0        0     5161 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/log.py
--rw-r--r--   0        0        0    13515 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/mixin.py
--rw-r--r--   0        0        0     5280 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/res.py
--rw-r--r--   0        0        0     5182 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/shadow.py
--rw-r--r--   0        0        0      518 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/signs.py
--rw-r--r--   0        0        0     5797 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/structdb.py
--rw-r--r--   0        0        0      151 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/__init__.py
--rw-r--r--   0        0        0      628 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/cli/__init__.py
--rw-r--r--   0        0        0        0 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/cli/prompts_extension/__init__.py
--rw-r--r--   0        0        0      413 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/misc.py
--rw-r--r--   0        0        0     6579 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/pixiv.py
--rw-r--r--   0        0        0     4163 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/Timeout.py
--rw-r--r--   0        0        0      242 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/__init__.py
--rw-r--r--   0        0        0     1149 2023-07-30 03:02:06.678510 remilia-1.2.0/src/Remilia/utils/thread/terminable_thread.py
--rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 remilia-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-08-04 09:29:03.200227 remilia-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1063 2023-08-04 09:29:03.200227 remilia-1.2.1/LICENSE
+-rw-r--r--   0        0        0     1009 2023-08-04 09:29:03.200227 remilia-1.2.1/README.md
+-rw-r--r--   0        0        0     1009 2023-08-04 09:29:03.200227 remilia-1.2.1/README.md
+-rw-r--r--   0        0        0     1282 2023-08-04 09:29:35.076794 remilia-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0      185 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/__init__.py
+-rw-r--r--   0        0        0       21 2023-08-04 09:29:35.072794 remilia-1.2.1/src/Remilia/__version__.py
+-rw-r--r--   0        0        0      102 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/base/__init__.py
+-rw-r--r--   0        0        0      153 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/base/exceptions.py
+-rw-r--r--   0        0        0      695 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/base/models.py
+-rw-r--r--   0        0        0     1920 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/base/rtypes.py
+-rw-r--r--   0        0        0     5659 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/log.py
+-rw-r--r--   0        0        0    21471 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/mixin.py
+-rw-r--r--   0        0        0     5280 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/res.py
+-rw-r--r--   0        0        0     5182 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/shadow.py
+-rw-r--r--   0        0        0      518 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/signs.py
+-rw-r--r--   0        0        0     5797 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/structdb.py
+-rw-r--r--   0        0        0      151 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/utils/__init__.py
+-rw-r--r--   0        0        0      628 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/utils/cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/utils/cli/prompts_extension/__init__.py
+-rw-r--r--   0        0        0      413 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/utils/misc.py
+-rw-r--r--   0        0        0     6579 2023-08-04 09:29:03.200227 remilia-1.2.1/src/Remilia/utils/pixiv.py
+-rw-r--r--   0        0        0     4163 2023-08-04 09:29:03.204228 remilia-1.2.1/src/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0        0        0      242 2023-08-04 09:29:03.204228 remilia-1.2.1/src/Remilia/utils/thread/__init__.py
+-rw-r--r--   0        0        0     1149 2023-08-04 09:29:03.204228 remilia-1.2.1/src/Remilia/utils/thread/terminable_thread.py
+-rw-r--r--   0        0        0     3219 1970-01-01 00:00:00.000000 remilia-1.2.1/PKG-INFO
```

### Comparing `remilia-1.2.0/LICENSE` & `remilia-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/README.md` & `remilia-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/pyproject.toml` & `remilia-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 ]
 dependencies = [
     "colorama",
     "pyyaml",
     "pydantic",
     "typing_extensions",
 ]
-version = "1.2.0"
+version = "1.2.1"
 
 [project.license]
 file = "LICENSE"
 
 [project.urls]
 Homepage = "https://pypi.org/project/Remilia/"
 Repository = "https://github.com/H2Sxxa/Remilia"
```

### Comparing `remilia-1.2.0/src/Remilia/base/models.py` & `remilia-1.2.1/src/Remilia/base/models.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/base/rtypes.py` & `remilia-1.2.1/src/Remilia/base/rtypes.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/log.py` & `remilia-1.2.1/src/Remilia/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,162 +1,198 @@
 from functools import partial
 from pathlib import Path
 from colorama import Fore, Back, Style, Cursor
 from colorama import init as initcolor
-from typing import Callable, Dict, List, Optional,TYPE_CHECKING, Union
+from typing import Callable, Dict, List, Optional, TYPE_CHECKING, Union
 from typing_extensions import Self
-from time import strftime,localtime
+from time import strftime, localtime
 
 from .res import rFile, rPath
 from .base.models import Ruler
 from .base.rtypes import Pair
 
 from platform import system
 import inspect
- 
+
 if TYPE_CHECKING:
+
     class _CallMethod:
         def __call__(self, *args: str) -> None:
             ...
 
 
 try:
     if system() == "Windows":
         initcolor(wrap=True)
     else:
         initcolor(wrap=False)
 except:
     pass
 
+
 class Log:
-    def __init__(self,name:str,location:str,logs:tuple=(),ruler:Ruler=Ruler()) -> None:
+    def __init__(
+        self, name: str, location: str, logs: tuple = (), ruler: Ruler = Ruler()
+    ) -> None:
         super().__init__()
-        self.ruler=ruler
-        self.location=location
-        self.logs=[str(log) for log in logs]
-        self.name=name.upper()
-    
+        self.ruler = ruler
+        self.location = location
+        self.logs = [str(log) for log in logs]
+        self.name = name.upper()
+
     @property
     def color(self) -> str:
-        #colorama stuff
-        fore=Fore
-        style=Style
-        cursor=Cursor
-        back=Back
-        #base
-        location=self.location
-        ruler=self.ruler
-        name=self.name
-        text=" ".join(self.logs)
-        time=strftime(
-            self.ruler.timeformat,
-            localtime()
-            )
-        __all__=[ruler,location,name,text,time,fore,style,cursor,back]
+        # colorama stuff
+        fore = Fore
+        style = Style
+        cursor = Cursor
+        back = Back
+        # base
+        location = self.location
+        ruler = self.ruler
+        name = self.name
+        text = " ".join(self.logs)
+        time = strftime(self.ruler.timeformat, localtime())
+        __all__ = [ruler, location, name, text, time, fore, style, cursor, back]
         return eval(self.ruler.excolor)
-    
+
     @property
     def plain(self) -> str:
-        location=self.location
-        ruler=self.ruler
-        name=self.name
-        text=" ".join(self.logs)
-        time=strftime(
-            self.ruler.timeformat,
-            localtime()
-            )
-        __all__=[ruler,location,name,text,time]
+        location = self.location
+        ruler = self.ruler
+        name = self.name
+        text = " ".join(self.logs)
+        time = strftime(self.ruler.timeformat, localtime())
+        __all__ = [ruler, location, name, text, time]
         return eval(self.ruler.explain)
 
 
 class LogCat:
-    all_logs:List[Log]
-    all_subs:List[Pair[Callable[[Log],bool],rFile]]
+    all_logs: List[Log]
+    all_subs: List[Pair[Callable[[Log], bool], rFile]]
+
     def __init__(self) -> None:
-        self.all_logs=[]
-        self.all_subs=[]
-          
-    def get_logs(self,filter:Callable[[Log],bool]=lambda _:True) -> List[Log]:
+        self.all_logs = []
+        self.all_subs = []
+
+    def get_logs(self, filter: Callable[[Log], bool] = lambda _: True) -> List[Log]:
         return [log for log in self.all_logs if filter(log)]
-    
-    def record(self,*logs:Log) -> Self:
+
+    def record(self, *logs: Log) -> Self:
         self.all_logs.extend(logs)
         self._subwrite(*logs)
         return self
-    
-    def export(self,path:Union[rFile,rPath,Path,str],filter:Callable[[Log],bool]=lambda _:True,mode:str="w") -> Self:
-        rflog=rFile(path) if not isinstance(path,rFile) else path
-        rflog.write(data='\n'.join([log.plain for log in self.get_logs(filter)]),mode=mode)
-        return self
-    
-    def subscribe(self,*pairs:Pair[Callable[[Log],bool],Union[rFile,rPath,Path,str]]) -> Self:
-        subs=[Pair(pair.name,rFile(pair.value) if not isinstance(pair.value,rFile) else pair.value) for pair in pairs]
+
+    def export(
+        self,
+        path: Union[rFile, rPath, Path, str],
+        filter: Callable[[Log], bool] = lambda _: True,
+        mode: str = "w",
+    ) -> Self:
+        rflog = rFile(path) if not isinstance(path, rFile) else path
+        rflog.write(
+            data="\n".join([log.plain for log in self.get_logs(filter)]), mode=mode
+        )
+        return self
+
+    def subscribe(
+        self, *pairs: Pair[Callable[[Log], bool], Union[rFile, rPath, Path, str]]
+    ) -> Self:
+        subs = [
+            Pair(
+                pair.name,
+                rFile(pair.value) if not isinstance(pair.value, rFile) else pair.value,
+            )
+            for pair in pairs
+        ]
         self.all_subs.extend(subs)
         return self
-    
-    def _subwrite(self,*logs:Log) -> None:
+
+    def _subwrite(self, *logs: Log) -> None:
         for sub in self.all_subs:
-            mode ="a" if sub.value.exists() else "w"
+            mode = "a" if sub.value.exists() else "w"
             for log in logs:
                 if sub.name(log):
-                    sub.value.write(data=log.plain+"\n",mode=mode)
-            
-    
+                    sub.value.write(data=log.plain + "\n", mode=mode)
+
+
 class Logger:
-    def __init__(self,logcat:LogCat=LogCat(),ruler_map:Optional[Dict[str,Ruler]]={},model:str="'%s[ '+name+' '+time+' '+location+'] %s'+text") -> None:
-        self.ruler_map={
-            "DEBUG":Ruler(level=3).exgenerate(model,Fore.CYAN,Style.RESET_ALL),
-            "INFO":Ruler(level=5).exgenerate(model,Fore.LIGHTGREEN_EX,Style.RESET_ALL),
-            "WARN":Ruler(level=6).exgenerate(model,Fore.LIGHTYELLOW_EX,Style.RESET_ALL),
-            "ERROR":Ruler(level=7).exgenerate(model,Fore.LIGHTRED_EX,Style.RESET_ALL),
+    def __init__(
+        self,
+        logcat: LogCat = LogCat(),
+        ruler_map: Optional[Dict[str, Ruler]] = {},
+        model: str = "'%s[ '+name+' '+time+' '+location+'] %s'+text",
+    ) -> None:
+        self.ruler_map = {
+            "DEBUG": Ruler(level=3).exgenerate(model, Fore.CYAN, Style.RESET_ALL),
+            "INFO": Ruler(level=5).exgenerate(
+                model, Fore.LIGHTGREEN_EX, Style.RESET_ALL
+            ),
+            "WARN": Ruler(level=6).exgenerate(
+                model, Fore.LIGHTYELLOW_EX, Style.RESET_ALL
+            ),
+            "ERROR": Ruler(level=7).exgenerate(
+                model, Fore.LIGHTRED_EX, Style.RESET_ALL
+            ),
         }
         self.ruler_map.update(ruler_map)
-        self.logcat=logcat
-        self.handle_out=print
-        self.vlevel=5
+        self.logcat = logcat
+        self.handle_out = print
+        self.vlevel = 5
         global instance
-        instance=self
-    
-    def set_vlevel(self,vlevel:int) -> Self:
-        self.vlevel=vlevel
-        return self
-    
-    
-    def ex_ruler(self,model:str,**colors:Dict[str,tuple]) -> Self:
-        for n,c in colors.items():
-            self.to_ruler(n,self.get_ruler(n).exgenerate(model,*c))
-        return self
-    
-    def to_ruler(self,name:str,ruler:Ruler) -> Self:
-        self.ruler_map.update({name.upper():ruler})
+        instance = self
+
+    def set_vlevel(self, vlevel: int) -> Self:
+        self.vlevel = vlevel
+        return self
+
+    def ex_ruler(self, model: str, **colors: Dict[str, tuple]) -> Self:
+        for n, c in colors.items():
+            self.to_ruler(n, self.get_ruler(n).exgenerate(model, *c))
         return self
-    
-    def get_ruler(self,name:str) -> Ruler:
+
+    def to_ruler(self, name: str, ruler: Ruler) -> Self:
+        self.ruler_map.update({name.upper(): ruler})
+        return self
+
+    def get_ruler(self, name: str) -> Ruler:
         try:
             return self.ruler_map[name.upper()]
         except:
             return Ruler()
-        
-    def print(self,name:str,*log:Log) -> None:
-        clog=Log(name,inspect.getmodule(inspect.stack()[1][0]).__name__,log,self.get_ruler(name))
+
+    def print(self, name: str, *log: Log) -> None:
+        clog = Log(
+            name,
+            inspect.getmodule(inspect.stack()[1][0]).__name__,
+            log,
+            self.get_ruler(name),
+        )
         self.logcat.record(clog)
         if self.vlevel >= clog.ruler.level:
             self.handle_out(clog.color)
-    
-    def __getattr__(self,name) -> "_CallMethod":
+
+    def __getattr__(self, name) -> "_CallMethod":
         if name.startswith("__") and name.endswith("__"):
             raise AttributeError(
                 f"'{self.__class__.__name__}' object has no attribute '{name}'"
             )
-        return partial(self.print,name)
-    
-instance:Logger
-def get_logger(*args,**kwargs) -> Logger:
-    '''
+        return partial(self.print, name)
+
+
+instance: Logger
+
+
+def get_logger(*args, **kwargs) -> Logger:
+    """
     args & kwargs only work under (instance == None)
-    '''
+    """
     global instance
-    if instance != None:
-        return instance
-    else:
-        instance=Logger(*args,**kwargs)
+    try:
+        if instance != None:
+            return instance
+        else:
+            instance = Logger(*args, **kwargs)
+            return instance
+    except:
+        instance = Logger(*args, **kwargs)
         return instance
```

### Comparing `remilia-1.2.0/src/Remilia/res.py` & `remilia-1.2.1/src/Remilia/res.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/shadow.py` & `remilia-1.2.1/src/Remilia/shadow.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/signs.py` & `remilia-1.2.1/src/Remilia/signs.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/structdb.py` & `remilia-1.2.1/src/Remilia/structdb.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/utils/cli/__init__.py` & `remilia-1.2.1/src/Remilia/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/utils/pixiv.py` & `remilia-1.2.1/src/Remilia/utils/pixiv.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/utils/thread/Timeout.py` & `remilia-1.2.1/src/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/src/Remilia/utils/thread/terminable_thread.py` & `remilia-1.2.1/src/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

### Comparing `remilia-1.2.0/PKG-INFO` & `remilia-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remilia
-Version: 1.2.0
+Version: 1.2.1
 Summary: Use python with next generation api
 Author-Email: H2Sxxa <H2Sxxa0w0@gmail.com>
 License: MIT License
         
         Copyright (c) 2022 H2Sxxa
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

