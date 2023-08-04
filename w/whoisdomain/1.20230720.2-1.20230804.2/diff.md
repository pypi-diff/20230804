# Comparing `tmp/whoisdomain-1.20230720.2.tar.gz` & `tmp/whoisdomain-1.20230804.2.tar.gz`

## Comparing `whoisdomain-1.20230720.2.tar` & `whoisdomain-1.20230804.2.tar`

### file list

```diff
@@ -1,13 +1,18 @@
--rw-r--r--   0        0        0     4645 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_0_init_tld.py
--rw-r--r--   0        0        0     6901 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_1_query.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_2_parse.py
--rw-r--r--   0        0        0     9507 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/_3_adjust.py
--rw-r--r--   0        0        0    14196 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/__init__.py
--rw-r--r--   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/exceptions.py
--rwxr-xr-x   0        0        0    18420 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/main.py
--rw-r--r--   0        0        0   132995 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/tld_regexpr.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/whoisdomain/version.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/.gitignore
--rw-r--r--   0        0        0    10341 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/README.md
--rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/pyproject.toml
--rw-r--r--   0        0        0    11264 2020-02-02 00:00:00.000000 whoisdomain-1.20230720.2/PKG-INFO
+-rwxr-xr-x   0        0        0     4823 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/_0_init_tld.py
+-rwxr-xr-x   0        0        0     2261 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/__init__.py
+-rwxr-xr-x   0        0        0    10362 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doParse.py
+-rw-r--r--   0        0        0    10047 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doQuery.py
+-rwxr-xr-x   0        0        0     6427 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/doWhoisCommand.py
+-rwxr-xr-x   0        0        0     4753 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/domain.py
+-rwxr-xr-x   0        0        0      544 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/exceptions.py
+-rw-r--r--   0        0        0     5149 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/handleDateStrings.py
+-rwxr-xr-x   0        0        0    19563 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/main.py
+-rwxr-xr-x   0        0        0     6022 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/parameterContext.py
+-rwxr-xr-x   0        0        0     1744 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/simpleCacheBase.py
+-rwxr-xr-x   0        0        0     2279 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/simpleCacheWithFile.py
+-rwxr-xr-x   0        0        0   131854 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/tld_regexpr.py
+-rwxr-xr-x   0        0        0       25 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/whoisdomain/version.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/.gitignore
+-rw-r--r--   0        0        0    10918 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/README.md
+-rw-r--r--   0        0        0     1699 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/pyproject.toml
+-rw-r--r--   0        0        0    11841 2020-02-02 00:00:00.000000 whoisdomain-1.20230804.2/PKG-INFO
```

### Comparing `whoisdomain-1.20230720.2/whoisdomain/_0_init_tld.py` & `whoisdomain-1.20230804.2/whoisdomain/_0_init_tld.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,62 +8,34 @@
 )
 
 from .tld_regexpr import ZZ
 from .exceptions import (
     UnknownTld,
 )
 
+# from .parameterContext import ParameterContext # not needed yet here
+
 Verbose: bool = False
 TLD_RE: Dict[str, Dict[str, Any]] = {}
 REG_COLLECTION_BY_KEY: Dict[str, Any] = {}
 
 
-def validTlds() -> List[str]:
-    return sorted(TLD_RE.keys())
-
-
-def filterTldToSupportedPattern(
-    domain: str,
-    d: List[str],
-    verbose: bool = False,
-) -> str:
-    # we have max 2 levels so first check if the last 2 are in our list
-    tld = f"{d[-2]}.{d[-1]}"
-    if tld in ZZ:
-        if verbose:
-            print(f"we have {tld}", file=sys.stderr)
-        return tld
-
-    # if not check if the last item  we have
-    tld = f"{d[-1]}"
-    if tld in ZZ:
-        if verbose:
-            print(f"we have {tld}", file=sys.stderr)
-        return tld
-
-    if verbose:
-        print(f"we DONT have {tld}", file=sys.stderr)
-
-    # if not fail
-    a = f"The TLD {tld} is currently not supported by this package."
-    b = "Use validTlds() to see what toplevel domains are supported."
-    msg = f"{a} {b}"
-    raise UnknownTld(msg)
-
-
-def get_tld_re(tld: str, override: bool = False) -> Dict[str, Any]:
+def _get_tld_re(
+    tld: str,
+    override: bool = False,
+) -> Dict[str, Any]:
     if override is False:
         if tld in TLD_RE:
             return TLD_RE[tld]
 
     v = ZZ[tld]
 
     extend = v.get("extend")
     if extend:
-        e = get_tld_re(extend)  # call recursive
+        e = _get_tld_re(extend)  # call recursive
         tmp = e.copy()
         tmp.update(v)  # and merge results in tmp with caller data in v
         # The update() method updates the dictionary with the elements
         # from another dictionary object or from an iterable of key/value pairs.
     else:
         tmp = v
 
@@ -83,45 +55,39 @@
     # meta domains start with _: examples _centralnic and _donuts
     if tld[0] != "_":
         TLD_RE[tld] = tld_re
 
     return tld_re
 
 
-def mergeExternalDictWithRegex(aDict: Dict[str, Any] = {}) -> None:
-    # merge in ZZ, this extends ZZ with new tld's and overrides existing tld's
-    for tld in aDict.keys():
-        ZZ[tld] = aDict[tld]
-
-    # reprocess te regexes we newly defined or overrode
-    override = True
-    for tld in aDict.keys():
-        initOne(tld, override)
-
-
-def initOne(tld: str, override: bool = False) -> None:
+def _initOne(
+    tld: str,
+    override: bool = False,
+) -> None:
     if tld[0] == "_":  # skip meta domain patterns , these are not domains just handles we reuse
         return
 
-    what = get_tld_re(tld, override)
+    what = _get_tld_re(tld, override)
 
     # test if the string is identical after idna conversion
     d = tld.split(".")
     j = [k.encode("idna").decode() or k for k in d]
     tld2 = ".".join(j)
     if tld == tld2:
         return
 
     # also automatically see if we can internationalize the domains to the official ascii string
     TLD_RE[tld2] = what
     if Verbose:
         print(f"{tld} -> {tld2}", file=sys.stderr)
 
 
-def buildRegCollection(zz: Dict[str, Any]) -> Dict[str, Any]:
+def _buildRegCollection(
+    zz: Dict[str, Any],
+) -> Dict[str, Any]:
     regCollection: Dict[str, Any] = {}
 
     # get all regexes
     for name in zz:
         # print(name)
         z = zz[name]
         for key in z:
@@ -148,19 +114,69 @@
             regCollection[key][reg] = None
             if isinstance(reg, str):
                 regCollection[key][reg] = re.compile(reg, flags=re.IGNORECASE)
 
     return regCollection
 
 
-def initOnImport() -> None:
+def _initOnImport() -> None:
     global REG_COLLECTION_BY_KEY
     # here we run the import processing
     # we load all tld's on import so we dont lose time later
     # we keep ZZ so we can later reuse it if we want to aoverrid or update tld's
-    REG_COLLECTION_BY_KEY = buildRegCollection(ZZ)
+    REG_COLLECTION_BY_KEY = _buildRegCollection(ZZ)
     override = False
     for tld in ZZ.keys():
-        initOne(tld, override)
+        _initOne(tld, override)
+
+
+# ========================================
+# external use
+
+
+def filterTldToSupportedPattern(
+    domain: str,
+    d: List[str],
+    verbose: bool = False,
+) -> str:
+    # we have max 2 levels so first check if the last 2 are in our list
+    tld = f"{d[-2]}.{d[-1]}"
+    if tld in ZZ:
+        if verbose:
+            print(f"we have {tld}", file=sys.stderr)
+        return tld
+
+    # if not check if the last item  we have
+    tld = f"{d[-1]}"
+    if tld in ZZ:
+        if verbose:
+            print(f"we have {tld}", file=sys.stderr)
+        return tld
+
+    if verbose:
+        print(f"we DONT have {tld}", file=sys.stderr)
+
+    # if not fail
+    a = f"The TLD {tld} is currently not supported by this package."
+    b = "Use validTlds() to see what toplevel domains are supported."
+    msg = f"{a} {b}"
+    raise UnknownTld(msg)
+
+
+def mergeExternalDictWithRegex(
+    aDict: Dict[str, Any] = {},
+) -> None:
+    # merge in ZZ, this extends ZZ with new tld's and overrides existing tld's
+    for tld in aDict.keys():
+        ZZ[tld] = aDict[tld]
+
+    # reprocess te regexes we newly defined or overrode
+    override = True
+    for tld in aDict.keys():
+        _initOne(tld, override)
+
+
+def validTlds() -> List[str]:
+    return sorted(TLD_RE.keys())
 
 
-initOnImport()
+_initOnImport()
```

### Comparing `whoisdomain-1.20230720.2/whoisdomain/_1_query.py` & `whoisdomain-1.20230804.2/whoisdomain/doWhoisCommand.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,243 +1,232 @@
+#!  /usr/bin/env python3
+
 import subprocess
 import time
 import sys
 import os
 import platform
-import json
 import shutil
-from .exceptions import WhoisCommandFailed, WhoisCommandTimeout
-
-from typing import Dict, List, Optional, Tuple
-
-
-# PYTHON_VERSION = sys.version_info[0]
-CACHE: Dict[str, Tuple[int, str]] = {}
-CACHE_MAX_AGE = 60 * 60 * 48  # 48h
 
-IS_WINDOWS = platform.system() == "Windows"
-
-if not IS_WINDOWS and shutil.which("stdbuf"):
-    STDBUF_OFF_CMD = ["stdbuf", "-o0"]
-else:
-    STDBUF_OFF_CMD = []
+from .exceptions import (
+    WhoisCommandFailed,
+    WhoisCommandTimeout,
+)
 
+from .simpleCacheBase import SimpleCacheBase
+from .simpleCacheWithFile import SimpleCacheWithFile
 
-def _cache_load(cf: str) -> None:
-    if not os.path.isfile(cf):
-        return
+from typing import (
+    # Dict,
+    List,
+    Optional,
+    # Tuple,
+    Any,
+)
 
-    global CACHE
-    f = open(cf, "r")
+from .parameterContext import ParameterContext
 
-    try:
-        CACHE = json.load(f)
-    except Exception as e:
-        print(f"ignore lson load err: {e}", file=sys.stderr)
 
-    f.close()
+IS_WINDOWS: bool = platform.system() == "Windows"
 
+STDBUF_OFF_CMD: List[str] = []
+if not IS_WINDOWS and shutil.which("stdbuf"):
+    STDBUF_OFF_CMD = ["stdbuf", "-o0"]
 
-def _cache_save(cf: str) -> None:
-    global CACHE
+# actually also whois uses cache, so if you really dont want to use cache
+# you should also pass the --force-lookup flag (on linux)
 
-    f = open(cf, "w")
-    json.dump(CACHE, f)
-    f.close()
+CACHE_STUB: Any = None
 
 
 def _testWhoisPythonFromStaticTestData(
-    dl: List[str],
-    ignore_returncode: bool,
-    server: Optional[str] = None,
-    verbose: bool = False,
+    dList: List[str],
+    pc: ParameterContext,
 ) -> str:
-    domain = ".".join(dl)
+    domain = ".".join(dList)
     testDir = os.getenv("TEST_WHOIS_PYTHON")
     pathToTestFile = f"{testDir}/{domain}/input"
     if os.path.exists(pathToTestFile):
         with open(pathToTestFile, mode="rb") as f:  # switch to binary mode as that is what Popen uses
             # make sure the data is treated exactly the same as the output of Popen
             return f.read().decode(errors="ignore")
 
     raise WhoisCommandFailed("")
 
 
 def _tryInstallMissingWhoisOnWindows(
-    verbose: bool = False,
+    pc: ParameterContext,
 ) -> None:
     """
     Windows 'whois' command wrapper
     https://docs.microsoft.com/en-us/sysinternals/downloads/whois
     """
     folder = os.getcwd()
     copy_command = r"copy \\live.sysinternals.com\tools\whois.exe " + folder
-    if verbose:
+    if pc.verbose:
         print("downloading dependencies", file=sys.stderr)
         print(copy_command, file=sys.stderr)
 
     subprocess.call(
         copy_command,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
         shell=True,
     )
 
 
 def _makeWhoisCommandToRun(
-    dl: List[str],
-    server: Optional[str] = None,
-    verbose: bool = False,
-    wh: str = "whois",
+    dList: List[str],
+    pc: ParameterContext,
 ) -> List[str]:
-    domain = ".".join(dl)
+    domain = ".".join(dList)
 
-    if " " in wh:
-        whList = wh.split(" ")
-    else:
-        whList = [wh]
+    whList: List[str] = [pc.cmd]
+    if " " in pc.cmd:
+        whList = pc.cmd.split(" ")
 
     if IS_WINDOWS:
-        if wh == "whois":  # only if the use did not specify what whois to use
-            if os.path.exists("whois.exe"):
-                wh = r".\whois.exe"
+        if pc.cmd == "whois":  # only if the use did not specify what whois to use
+            k: str = "whois.exe"
+            if os.path.exists(k):
+                pc.cmd = os.path.join(".", k)
             else:
                 find = False
                 paths = os.environ["path"].split(";")
                 for path in paths:
-                    wpath = os.path.join(path, "whois.exe")
+                    wpath = os.path.join(path, k)
                     if os.path.exists(wpath):
-                        wh = wpath
+                        pc.cmd = wpath
                         find = True
                         break
 
                 if not find:
-                    _tryInstallMissingWhoisOnWindows(verbose)
-        whList = [wh]
+                    _tryInstallMissingWhoisOnWindows(
+                        pc=pc,
+                    )
+        whList = [pc.cmd]
 
-        if server:
-            return whList + ["-v", "-nobanner", domain, server]
+        if pc.server:
+            return whList + ["-v", "-nobanner", domain, pc.server]
         return whList + ["-v", "-nobanner", domain]
 
     # not windows
-    if server:
-        return whList + [domain, "-h", server]
+    if pc.server:
+        return whList + [domain, "-h", pc.server]
     return whList + [domain]
 
 
-def _do_whois_query(
-    dl: List[str],
-    ignore_returncode: bool,
-    server: Optional[str] = None,
-    verbose: bool = False,
-    timeout: Optional[float] = None,
-    parse_partial_response: bool = False,
-    wh: str = "whois",
-    simplistic: bool = False,
+def _execute_whois_query(
+    dList: List[str],
+    pc: ParameterContext,
 ) -> str:
     # if getenv[TEST_WHOIS_PYTON] fake whois by reading static data from a file
     # this wasy we can actually implemnt a test run with known data in and expected data out
     if os.getenv("TEST_WHOIS_PYTHON"):
-        return _testWhoisPythonFromStaticTestData(dl, ignore_returncode, server, verbose)
+        return _testWhoisPythonFromStaticTestData(
+            dList,
+            pc=pc,
+        )
 
     cmd = _makeWhoisCommandToRun(
-        dl=dl,
-        server=server,
-        verbose=verbose,
-        wh=wh,
+        dList=dList,
+        pc=pc,
     )
-    if verbose:
-        print(cmd, wh, file=sys.stderr)
+    if pc.verbose:
+        print(cmd, pc.cmd, file=sys.stderr)
+
+    if pc.slow_down:
+        # slow down before so we can force individual domains at a slower tempo
+        time.sleep(pc.slow_down)
 
     # LANG=en is added to make the ".jp" output consist across all environments
     p = subprocess.Popen(
         # STDBUF_OFF_CMD needed to not lose data on kill
         STDBUF_OFF_CMD + cmd,
         stdout=subprocess.PIPE,
         stderr=subprocess.STDOUT,
-        env={"LANG": "en"} if dl[-1] in ".jp" else None,
+        env={"LANG": "en"} if dList[-1] in ".jp" else None,
     )
 
     try:
-        r = p.communicate(timeout=timeout)[0].decode(errors="ignore")
+        r = p.communicate(timeout=pc.timeout,)[
+            0
+        ].decode(errors="ignore")
     except subprocess.TimeoutExpired:
         # Kill the child process & flush any output buffers
         p.kill()
         r = p.communicate()[0].decode(errors="ignore")
         # In most cases whois servers returns partial domain data really fast
         # after that delay occurs (probably intentional) before returning contact data.
         # Add this option to cover those cases
-        if not parse_partial_response or not r:
-            raise WhoisCommandTimeout(f"timeout: query took more then {timeout} seconds")
+        if not pc.parse_partial_response or not r:
+            raise WhoisCommandTimeout(f"timeout: query took more then {pc.timeout} seconds")
 
-    if verbose:
+    if pc.verbose:
         print(r, file=sys.stderr)
 
-    if ignore_returncode is False and p.returncode not in [0, 1]:
-        # network error, "fgets: Connection reset by peer" fix, ignore
+    if pc.ignore_returncode is False and p.returncode not in [0, 1]:
         if "fgets: Connection reset by peer" in r:
             return r.replace("fgets: Connection reset by peer", "")
-        # connect: Connection refused
-        elif "connect: Connection refused" in r:
+
+        if "connect: Connection refused" in r:
             return r.replace("connect: Connection refused", "")
 
-        if simplistic:
+        if pc.simplistic:
             return r
 
         raise WhoisCommandFailed(r)
 
     return r
 
 
 # PUBLIC
 
-
-def do_query(
-    dl: List[str],
-    force: bool = False,
-    cache_file: Optional[str] = None,
-    cache_age: int = CACHE_MAX_AGE,
-    slow_down: int = 0,
-    ignore_returncode: bool = False,
-    server: Optional[str] = None,
-    verbose: bool = False,
-    timeout: Optional[float] = None,
-    parse_partial_response: bool = False,
-    wh: str = "whois",
-    simplistic: bool = False,
+# future: use decorator for caching
+def doWhoisAndReturnString(
+    dList: List[str],
+    pc: ParameterContext,
 ) -> str:
-    k = ".".join(dl)
+    global CACHE_STUB
 
-    if cache_file:
-        if verbose:
-            print(f"using cache file: {cache_file}", file=sys.stderr)
-        _cache_load(cache_file)
-
-    # actually also whois uses cache, so if you really dont want to use cache
-    # you should also pass the --force-lookup flag (on linux)
-    if force or k not in CACHE or CACHE[k][0] < time.time() - cache_age:
-        if verbose:
-            print(f"force = {force}", file=sys.stderr)
+    # here you can override caching, if someone else already defined CACHE_STUB by this time, we use their caching
+    if CACHE_STUB is None:
+        CACHE_STUB = SimpleCacheWithFile(
+            verbose=pc.verbose,
+            cacheFilePath=pc.cache_file,
+            cacheMaxAge=pc.cache_age,
+        )
 
-        # slow down before so we can force individual domains at a slower tempo
-        if slow_down:
-            time.sleep(slow_down)
+    # allways test CACHE_STUB is a subclass of SimpleCacheBase
+    assert isinstance(CACHE_STUB, SimpleCacheBase), Exception("CACHE_STUB - must inherit from SimpleCacheBase")
 
-        # populate a fresh cache entry
-        CACHE[k] = (
-            int(time.time()),
-            _do_whois_query(
-                dl=dl,
-                ignore_returncode=ignore_returncode,
-                server=server,
-                verbose=verbose,
-                timeout=timeout,
-                parse_partial_response=parse_partial_response,
-                wh=wh,
-                simplistic=simplistic,
-            ),
-        )
+    keyString = ".".join(dList)
+
+    oldData: Optional[str] = CACHE_STUB.cacheGetData(keyString)
+
+    needFreshData: bool = False
+
+    if pc.force is True:
+        needFreshData = True
+
+    if oldData is None:
+        needFreshData = True
+
+    hasExpired: Optional[bool] = CACHE_STUB.cacheExpired(keyString)
+    if hasExpired is None:
+        needFreshData = True
+
+    if hasExpired is True:
+        needFreshData = True
+
+    if needFreshData is False:
+        return str(oldData)
+
+    newData: str = _execute_whois_query(
+        dList=dList,
+        pc=pc,
+    )
 
-        if cache_file:
-            _cache_save(cache_file)
+    # populate a fresh cache entry and save if needed
+    CACHE_STUB.cachePut(keyString, newData)
 
-    return CACHE[k][1]
+    return newData
```

### Comparing `whoisdomain-1.20230720.2/whoisdomain/_2_parse.py` & `whoisdomain-1.20230804.2/whoisdomain/doParse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,33 @@
+#! /usr/bin/env python3
+
 import re
 import sys
 
 from typing import (
     cast,
     Any,
     Dict,
     Optional,
     List,
     Tuple,
 )
 
-from ._0_init_tld import TLD_RE
-
-from ._3_adjust import (
-    Domain,
-)
-
 from .exceptions import (
     FailedParsingWhoisOutput,
     WhoisQuotaExceeded,
 )
 
+from ._0_init_tld import TLD_RE
+
+from .domain import Domain
+
+
+from .parameterContext import ParameterContext
+
 Verbose: bool = True
 
 NONESTRINGS: List[str] = [
     "the domain has not been registered",
     "no match found for",
     "no matching record",
     "no match",
@@ -40,228 +43,249 @@
     "nameserver not found",
     "malformed request",  # this means this domain is not in whois as it is on top of a registered domain
     "registration of this domain is restricted",
     "restricted",
     "this domain is currently available",
 ]
 
+
+def NoneStrings() -> List[str]:
+    return NONESTRINGS
+
+
+def NoneStringsAdd(aString: str) -> None:
+    if aString and isinstance(aString, str) and len(aString) > 0:
+        NONESTRINGS.append(aString)
+
+
 QUOTASTRINGS: List[str] = [
     "limit exceeded",
     "quota exceeded",
     "try again later",
     "please try again",
     "exceeded the maximum allowable number",
     "can temporarily not be answered",
     "please try again.",
     "queried interval is too short",
     "number of allowed queries exceeded",
 ]
 
 
+def QuotaStrings() -> List[str]:
+    return QUOTASTRINGS
+
+
+def QuotaStringsAdd(aString: str) -> None:
+    if aString and isinstance(aString, str) and len(aString) > 0:
+        NONESTRINGS.append(aString)
+
+
 def _handleShortResponse(
-    tld: str,
-    dl: List[str],
-    whois_str: str,
-    verbose: bool = False,
-    simplistic: bool = False,
-    include_raw_whois_text: bool = False,
+    tldString: str,
+    dList: List[str],
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> Optional[Domain]:
-    if verbose:
-        d = ".".join(dl)
-        print(f"line count < 5:: {tld} {d} {whois_str}", file=sys.stderr)
+    if pc.verbose:
+        d = ".".join(dList)
+        print(f"line count < 5:: {tldString} {d} {whoisStr}", file=sys.stderr)
 
     # TODO: some short responses are actually valid:
     # lookfor Domain: and Status but all other fields are missing so the regexec could fail
     # this domain is taken already or reserved
 
     # whois syswow.64-b.it
     # [Querying whois.nic.it]
     # [whois.nic.it]
     # Domain:             syswow.64-b.it
     # Status:             UNASSIGNABLE
 
-    s = whois_str.strip().lower()
+    s = whoisStr.strip().lower()
 
     # NOTE: from here s is lowercase only
     # ---------------------------------
     noneStrings = NoneStrings()
     for i in noneStrings:
         if i in s:
             return None
 
     # ---------------------------------
     # is there any error string in the result
     if s.count("error"):
-        if verbose:
+        if pc.verbose:
             print("i see 'error' in the result, return: None", file=sys.stderr)
         return None
 
     # ---------------------------------
     quotaStrings = QuotaStrings()
     for i in quotaStrings:
         if i in s:
-            if simplistic:
+            if pc.simplistic:
                 msg = "WhoisQuotaExceeded"
                 return Domain(
                     data={},
-                    whois_str=whois_str,
-                    verbose=verbose,
-                    include_raw_whois_text=include_raw_whois_text,
+                    pc=pc,
+                    whoisStr=whoisStr,
                     exeptionStr=msg,
                 )
-            raise WhoisQuotaExceeded(whois_str)
+            raise WhoisQuotaExceeded(whoisStr)
 
-    if simplistic:
+    if pc.simplistic:
         msg = "FailedParsingWhoisOutput"
         return Domain(
             data={},
-            whois_str=whois_str,
-            verbose=verbose,
-            include_raw_whois_text=include_raw_whois_text,
+            pc=pc,
+            whoisStr=whoisStr,
             exeptionStr=msg,
         )
 
-    raise FailedParsingWhoisOutput(whois_str)
+    raise FailedParsingWhoisOutput(whoisStr)
 
 
 def _doDnsSec(
-    whois_str: str,
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> bool:
-    whois_dnssec: Any = whois_str.split("DNSSEC:")
-    if len(whois_dnssec) >= 2:
-        whois_dnssec = whois_dnssec[1].split("\n")[0]
-        if whois_dnssec.strip() == "signedDelegation" or whois_dnssec.strip() == "yes":
+    whoisDnsSecList: List[str] = whoisStr.split("DNSSEC:")
+    if len(whoisDnsSecList) >= 2:
+        if pc.verbose:
+            msg = "i have seen dnssec: {whoisDnsSecStr}"
+            print(msg, file=sys.stderr)
+
+        whoisDnsSecStr: str = whoisDnsSecList[1].split("\n")[0]
+        if whoisDnsSecStr.strip() == "signedDelegation" or whoisDnsSecStr.strip() == "yes":
             return True
     return False
 
 
 def _doIfServerNameLookForDomainName(
-    whois_str: str,
-    verbose: bool = False,
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> str:
     # not often available anymore
-    if re.findall(r"Server Name:\s?(.+)", whois_str, re.IGNORECASE):
-        if verbose:
+    if re.findall(r"Server Name:\s?(.+)", whoisStr, re.IGNORECASE):
+        if pc.verbose:
             msg = "i have seen Server Name:, looking for Domain Name:"
             print(msg, file=sys.stderr)
-        whois_str = whois_str[whois_str.find("Domain Name:") :]
-    return whois_str
+        whoisStr = whoisStr[whoisStr.find("Domain Name:") :]
+    return whoisStr
 
 
 def _doExtractPattensIanaFromWhoisString(
-    tld: str,
+    tldString: str,
     r: Dict[str, Any],
-    whois_str: str,
-    verbose: bool = False,
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> Dict[str, Any]:
     # now handle the actual format if this whois response
     iana = {
         "domain_name": r"domain:\s?([^\n]+)",
         "registrar": r"organisation:\s?([^\n]+)",
         "creation_date": r"created:\s?([^\n]+)",
     }
     for k, v in iana.items():
-        zz = re.findall(v, whois_str)
+        zz = re.findall(v, whoisStr)
         if zz:
-            if verbose:
-                print(f"parsing iana data only for tld: {tld}, {zz}", file=sys.stderr)
+            if pc.verbose:
+                print(f"parsing iana data only for tld: {tldString}, {zz}", file=sys.stderr)
             r[k] = zz
     return r
 
 
 def _doExtractPattensFromWhoisString(
-    tld: str,
+    tldString: str,
     r: Dict[str, Any],
-    whois_str: str,
-    verbose: bool = False,
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> Dict[str, Any]:
-    for k, v in TLD_RE.get(tld, TLD_RE["com"]).items():  # use TLD_RE["com"] as default if a regex is missing
+    for k, v in TLD_RE.get(tldString, TLD_RE["com"]).items():  # use TLD_RE["com"] as default if a regex is missing
         if k.startswith("_"):  # skip meta element like: _server or _privateRegistry
             continue
 
         # Historical: here we use 'empty string' as default, not None
         if v is None:
             r[k] = [""]
         else:
-            r[k] = v.findall(whois_str) or [""]
+            r[k] = v.findall(whoisStr) or [""]
 
     return r
 
 
 def _doSourceIana(
-    tld: str,
+    tldString: str,
     r: Dict[str, Any],
-    whois_str: str,
-    verbose: bool = False,
+    whoisStr: str,
+    pc: ParameterContext,
 ) -> Tuple[str, Optional[Dict[str, Any]]]:
     # here we can handle the example.com and example.net permanent IANA domains
     k = "source:       IANA"
 
-    if verbose:
+    if pc.verbose:
         msg = f"i have seen {k}"
         print(msg, file=sys.stderr)
 
-    whois_splitted = whois_str.split(k)
+    whois_splitted = whoisStr.split(k)
     z = len(whois_splitted)
     if z > 2:
         return k.join(whois_splitted[1:]), None
 
     if z == 2 and whois_splitted[1].strip() != "":
         # if we see source: IANA and the part after is not only whitespace
-        if verbose:
+        if pc.verbose:
             msg = f"after: {k} we see not only whitespace: {whois_splitted[1]}"
             print(msg, file=sys.stderr)
 
         return whois_splitted[1], None
 
     # try to parse this as a IANA domain as after is only whitespace
     r = _doExtractPattensFromWhoisString(
-        tld,
+        tldString,
         r,
-        whois_str,
-        verbose,
+        whoisStr,
+        pc=pc,
     )  # set default values
 
     # now handle the actual format if this whois response
     r = _doExtractPattensIanaFromWhoisString(
-        tld,
+        tldString,
         r,
-        whois_str,
-        verbose,
+        whoisStr,
+        pc=pc,
     )
 
-    return whois_str, r
+    return whoisStr, r
 
 
 # PUBLIC
 
 
 def cleanupWhoisResponse(
-    whois_str: str,
+    whoisStr: str,
     verbose: bool = False,
     with_cleanup_results: bool = False,
     withRedacted: bool = False,
+    # pc: ParameterContext, # later as this func can be used from outside tha package
 ) -> str:
     tmp2: List[str] = []
 
     # note we cannot do yet rstrip() on the lines as many registrars use \r and even trailing whitespace after entries
     # as the resulting matches are all stripped of leading and trailing whitespace this currently is fixed there
     # and relaxes the regexes: you will often see a capture with (.*)
     # we would have to fix all regexes to allow stripping all trailing whitespace
     # it would make many matches easier though.
 
     skipFromHere = False
-    tmp: List[str] = whois_str.split("\n")
+    tmp: List[str] = whoisStr.split("\n")
     for line in tmp:
         if skipFromHere is True:
             continue
 
         # some servers respond with: % Quota exceeded in the comment section (lines starting with %)
         if "quota exceeded" in line.lower():
-            raise WhoisQuotaExceeded(whois_str)
+            raise WhoisQuotaExceeded(whoisStr)
 
         if with_cleanup_results is True and line.startswith("%"):  # only remove if requested
             continue
 
         if withRedacted is False:
             if "REDACTED FOR PRIVACY" in line:  # these lines contibute nothing so ignore
                 continue
@@ -281,70 +305,62 @@
             continue
 
         tmp2.append(line.strip("\r"))
 
     return "\n".join(tmp2)
 
 
-def NoneStrings() -> List[str]:
-    return NONESTRINGS
-
-
-def NoneStringsAdd(aString: str) -> None:
-    if aString and isinstance(aString, str) and len(aString) > 0:
-        NONESTRINGS.append(aString)
-
-
-def QuotaStrings() -> List[str]:
-    return QUOTASTRINGS
-
-
-def QuotaStringsAdd(aString: str) -> None:
-    if aString and isinstance(aString, str) and len(aString) > 0:
-        NONESTRINGS.append(aString)
-
-
 def do_parse(
-    whois_str: str,
-    tld: str,
-    dl: List[str],
-    verbose: bool = False,
-    with_cleanup_results: bool = False,
-    simplistic: bool = False,
-    include_raw_whois_text: bool = False,
-    withRedacted: bool = False,
+    whoisStr: str,
+    tldString: str,
+    dList: List[str],
+    pc: ParameterContext,
 ) -> Any:
 
-    whois_str = cleanupWhoisResponse(
-        whois_str=whois_str,
-        verbose=verbose,
-        with_cleanup_results=with_cleanup_results,
-        withRedacted=withRedacted,
+    whoisStr = cleanupWhoisResponse(
+        whoisStr=whoisStr,
+        verbose=pc.verbose,
+        with_cleanup_results=pc.with_cleanup_results,
+        withRedacted=pc.withRedacted,
     )
 
-    if whois_str.count("\n") < 5:
+    if whoisStr.count("\n") < 5:
         result = _handleShortResponse(  # may raise:    FailedParsingWhoisOutput,    WhoisQuotaExceeded,
-            tld=tld,
-            dl=dl,
-            whois_str=whois_str,
-            verbose=verbose,
-            simplistic=simplistic,
-            include_raw_whois_text=include_raw_whois_text,
+            tldString=tldString,
+            dList=dList,
+            whoisStr=whoisStr,
+            pc=pc,
         )
         return result
 
     # this is the beginning of the return data
     r: Dict[str, Any] = {
-        "tld": tld,
-        "DNSSEC": _doDnsSec(whois_str),
+        "tld": tldString,
+        "DNSSEC": _doDnsSec(whoisStr=whoisStr, pc=pc),
     }
 
-    if "source:       IANA" in whois_str:  # prepare for handling historical IANA domains
-        whois_str, ianaDomain = _doSourceIana(tld, r, whois_str, verbose)
+    if "source:       IANA" in whoisStr:  # prepare for handling historical IANA domains
+        whoisStr, ianaDomain = _doSourceIana(
+            tldString,
+            r=r,
+            whoisStr=whoisStr,
+            pc=pc,
+        )
         if ianaDomain is not None:
-            ianaDomain = cast(Optional[Dict[str, Any]], ianaDomain)
+            ianaDomain = cast(
+                Optional[Dict[str, Any]],
+                ianaDomain,
+            )
             return ianaDomain
 
-    if "Server Name" in whois_str:  # handle old type Server Name (not very common anymore)
-        whois_str = _doIfServerNameLookForDomainName(whois_str, verbose)
+    if "Server Name" in whoisStr:  # handle old type Server Name (not very common anymore)
+        whoisStr = _doIfServerNameLookForDomainName(
+            whoisStr,
+            pc.verbose,
+        )
 
-    return _doExtractPattensFromWhoisString(tld, r, whois_str, verbose)
+    return _doExtractPattensFromWhoisString(
+        tldString=tldString,
+        r=r,
+        whoisStr=whoisStr,
+        pc=pc,
+    )
```

### Comparing `whoisdomain-1.20230720.2/whoisdomain/exceptions.py` & `whoisdomain-1.20230804.2/whoisdomain/exceptions.py`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230720.2/whoisdomain/main.py` & `whoisdomain-1.20230804.2/whoisdomain/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 Verbose: bool = False
 PrintGetRawWhoisResult: bool = False
 Ruleset: bool = False
 
 Failures: Dict[str, Any] = {}
 IgnoreReturncode: bool = False
 TestAllTld: bool = False
+TestRunOnly: bool = False
 
 
 class ResponseCleaner:
     data: str
     rDict: Dict[str, Any] = {}
 
     def __init__(
@@ -206,26 +207,29 @@
     d: str,
     printgetRawWhoisResult: bool = False,
 ) -> None:
     global PrintGetRawWhoisResult
     global SIMPLISTIC
     global WithRedacted
     global TestAllTld
+    global TestRunOnly
 
     timeout = 30  # seconds
 
     w = whois.query(
         d,
         ignore_returncode=IgnoreReturncode,
         verbose=Verbose,
         internationalized=True,
         include_raw_whois_text=PrintGetRawWhoisResult,
         timeout=timeout,
         simplistic=SIMPLISTIC,
         withRedacted=WithRedacted,
+        # cache_file="/tmp/testCache.json",  # temp test
+        # cache_age=300,  # temp test
     )
 
     if w is None:
         print("None")
         print("\n", whois.get_last_raw_whois_data())
         return
 
@@ -343,38 +347,73 @@
         getTestFileOne(fPath, fileData)
 
 
 def getAllCurrentTld() -> List[str]:
     return whois.validTlds()
 
 
+def appendHintOrMeta(
+    rr: List[str],
+    allRegex: Optional[str],
+    tld: str,
+) -> None:
+    global TestAllTld
+    global TestRunOnly
+
+    if TestAllTld is True:
+        hint = whois.getTestHint(tld)
+        hint = hint if hint else f"meta.{tld}"
+        rr.append(f"{hint}")
+    else:
+        rr.append(f"meta.{tld}")
+
+
+def appendHint(
+    rr: List[str],
+    allRegex: Optional[str],
+    tld: str,
+) -> None:
+    global TestAllTld
+    global TestRunOnly
+
+    if TestAllTld is True:
+        hint = whois.getTestHint(tld)
+        if hint:
+            rr.append(f"{hint}")
+
+
 def makeMetaAllCurrentTld(
     allHaving: Optional[str] = None,
     allRegex: Optional[str] = None,
 ) -> List[str]:
-    global TestAllTld
 
-    def appendHint(
-        allRegex: Optional[str],
-        tld: str,
-    ) -> None:
-        if TestAllTld is True:
-            hint = whois.getTestHint(tld)
-            hint = hint if hint else f"meta.{tld}"
-            rr.append(f"{hint}")
-        else:
-            rr.append(f"meta.{tld}")
+    rr: List[str] = []
+    for tld in getAllCurrentTld():
+        if allRegex is None:
+            appendHintOrMeta(rr, allRegex, tld)
+            continue
+
+        if re.search(allRegex, tld):
+            appendHintOrMeta(rr, allRegex, tld)
+
+    return rr
+
+
+def makeTestAllCurrentTld(
+    allHaving: Optional[str] = None,
+    allRegex: Optional[str] = None,
+) -> List[str]:
 
     rr: List[str] = []
     for tld in getAllCurrentTld():
-        if allRegex:
-            if re.search(allRegex, tld):
-                appendHint(allRegex, tld)
-        else:
-            appendHint(allRegex, tld)
+        if allRegex is None:
+            appendHint(rr, allRegex, tld)
+            continue
+        if re.search(allRegex, tld):
+            appendHint(rr, allRegex, tld)
 
     return rr
 
 
 def showAllCurrentTld() -> None:
     print("Tld's currently supported")
     for tld in getAllCurrentTld():
@@ -489,26 +528,27 @@
     global Verbose
     global IgnoreReturncode
     global PrintGetRawWhoisResult
     global Ruleset
     global SIMPLISTIC
     global WithRedacted
     global TestAllTld
-
+    global TestRunOnly
     name: str = os.path.basename(sys.argv[0])
     if name == "test2.py":
         SIMPLISTIC = False
     else:
         SIMPLISTIC = True
 
     try:
         opts, args = getopt.getopt(
             sys.argv[1:],
-            "jRSpvVIhaf:d:D:r:H:C:",
+            "tjRSpvVIhaf:d:D:r:H:C:",
             [
+                "test",
                 "json",
                 "Ruleset",
                 "SupportedTld",
                 "print",
                 "verbose",
                 "Version",
                 "IgnoreReturncode",
@@ -575,14 +615,20 @@
 
         if opt in ("-p", "--print"):
             PrintGetRawWhoisResult = True
 
         if opt in ("-j", "--json"):
             PrintJson = True
 
+        if opt in ("-t", "--test"):
+            # collect all _test entries defined and only run those,
+            # o not run the default meta.tld
+            TestAllTld = True
+            TestRunOnly = True
+
         if opt in ("-R", "--Ruleset"):
             Ruleset = True
 
         if opt in ("-D", "--Directory"):
             directory = arg
             isDir = os.path.isdir(directory)
             if isDir is False:
@@ -622,16 +668,19 @@
 
     if Ruleset is True and len(domains):
         for domain in domains:
             ShowRuleset(domain)
         sys.exit(0)
 
     if TestAllTld:
-        allMetaTld = makeMetaAllCurrentTld(allHaving, allRegex)
-        testDomains(allMetaTld)
+        if TestRunOnly is False:
+            testDomains(makeMetaAllCurrentTld(allHaving, allRegex))
+        else:
+            testDomains(makeTestAllCurrentTld(allHaving, allRegex))
+
         showFailures()
         sys.exit(0)
 
     if len(dirs):
         fileData = {}
         for dName in dirs:
             getTestFilesAll(dName, fileData)
```

### Comparing `whoisdomain-1.20230720.2/whoisdomain/tld_regexpr.py` & `whoisdomain-1.20230804.2/whoisdomain/tld_regexpr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,29 +1,53 @@
 from typing import (
     Dict,
     Any,
 )
 
-ZZ: Dict[str, Any] = {}
 
-# elements starting with _
+# Interesting for future enhancements:
+# https://github.com/rfc1036/whois/blob/next/tld_serv_list
+# https://github.com/rfc1036/whois/blob/next/new_gtlds_list
+# seems the most up to date and maintained
+
+# =================================================================
+# Often we want to repeat regex patterns,
+#   ( typically with nameservers or status fields )
+#   that becomes unreadable very fast.
+# Allow for a simplification that expands on usage and
+#   allow forcing the first to be mandatory as default,
+#   but overridable when needed
+
+
+def xStr(what: str, times: int = 1, firstMandatory: bool = True) -> str:
+    if times < 1:
+        return ""
+
+    if firstMandatory and what[-1] == "?":
+        return what[:-1] + (what * (times - 1))
+    else:
+        return what * times
+
+
+# =================================================================
+# The database
+
+# Elements starting with _
 # are meta patterns and are not processed as domains
 # examples:  _donuts, _centralnic
 
-# elements ending in _
-# like id_ , is_, if_, in_, global_ are conflicting words in python without a trailing _
-# and auto replaced with a non conflicting word by adding a _ at the end
-
-# NOTE: many registrars use \r and some even have whitespace after the entry
 # Some items can be multiple: status, emails, name_servers
 # the remaining are always singular
 
-# when we finally apply the regexes we use IGNORE CASE allways on all matches
+# When we finally apply the regexes we use IGNORE CASE allways on all matches
+
+
+ZZ: Dict[str, Any] = {}
+
 
-# Commercial TLD - Original Big 7
 ZZ["com"] = {
     "extend": None,
     "domain_name": r"Domain Name\s*:\s*(.+)",
     "registrar": r"Registrar:\s?(.+)",
     "registrant": r"Registrant\s*Organi(?:s|z)ation:([^\n]*)",  # this seems to match Registrant Street: if Registrant Organization: is empty
     "registrant_country": r"Registrant Country:\s?(.+)",
     "creation_date": r"Creation Date:[ \t]*([^\n]*)",
@@ -50,21 +74,21 @@
     "name_servers": r"Servers:\s*(.+)\t\n\s*(.+)\t\n",
 }
 
 ZZ["co.uk"] = {
     "extend": "uk",
     "domain_name": r"Domain name:\s+(.+)",
     "registrar": r"Registrar:\s+(.+)",
-    "name_servers": r"Name servers:(?:\n\s+(\S+))?(?:\n\s+(\S+))?(?:\n\s+(\S+))?(?:\n\s+(\S+))?\n\n",  # capture up to 4
     "status": r"Registration status:\s*(.+)",
     "creation_date": r"Registered on:(.+)",
     "expiration_date": r"Expiry date:(.+)",
     "updated_date": r"Last updated:(.+)",
     "owner": r"Domain Owner:\s+(.+)",
     "registrant": r"Registrant:\n\s+(.+)",  # example meta.co.uk has a registrar google.co.uk has not
+    "_test": "livedns.co.uk",
 }
 
 ZZ["org.uk"] = {"extend": "co.uk"}
 ZZ["gov.uk"] = {"extend": "ac.uk"}
 
 # United Arab Emirates
 # ae = {    "extend": "ar"}
@@ -83,15 +107,16 @@
     "status": r"Status:\s(.+)",
     "registrar": r"Registrar:\s+(.+)",
     "registrant": r"Registrant:\s+(.+)",
     "registrant_country": r"Registrant:\n.+\n.+\n.+\n\s+(.+)",
     "creation_date": r"Registered:\s+(.+)",
     "expiration_date": r"Expires:\s+(.+)",
     "updated_date": r"Last modified:\s+(.+)",
-    "name_servers": r"DNS servers.*:\n(?:\s+(\S+)\n)(?:\s+(\S+)\n)?(?:\s+(\S+)\n)?(?:\s+(\S+)\n)\n?",
+    # "name_servers": r"DNS servers.*:\n(?:\s+(\S+)\n)(?:\s+(\S+)\n)?(?:\s+(\S+)\n)?(?:\s+(\S+)\n)\n?",
+    "name_servers": r"DNS servers.*:\n%s" % xStr(r"(?:\s+(\S+)\n)?", 4),
 }
 
 # Amsterdam
 ZZ["amsterdam"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s?(.+)",
     "registrar": r"Registrar:\s*(.+)",
@@ -150,15 +175,16 @@
     "status": r"status\.+:\s*(\S+)",
     "registrant": r"Holder\s+name\.+:\s*(.+)\r?\n",  # not always present see meta.ax and google.ax
     "registrant_country": r"country\.+:\s*(.+)\r?\n",  # not always present see meta.ax and google.ax
 }
 
 ZZ["aw"] = {
     "extend": "nl",
-    "name_servers": r"Domain nameservers:\s+(\S+)[ \t]*\r?\n(?:\s+(\S+))?",
+    # "name_servers": r"Domain nameservers:\s+(\S+)[ \t]*\r?\n(?:\s+(\S+))?",
+    "name_servers": r"Domain nameservers.*:\n%s" % xStr(r"(?:\s+(\S+)\n)?", 4),
 }
 
 # Banking TLD - ICANN
 ZZ["bank"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s?(.+)",
     "registrar": r"Registrar:\s*(.+)",
@@ -388,15 +414,16 @@
 
 ZZ["edu"] = {
     "extend": "com",
     "registrant": r"Registrant:\s*(.+)",
     "creation_date": r"Domain record activated:\s?(.+)",
     "updated_date": r"Domain record last updated:\s?(.+)",
     "expiration_date": r"Domain expires:\s?(.+)",
-    "name_servers": r"Name Servers:\s?(?:\t(.+)\n)(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?(?:\t(.+)\n)?",
+    "name_servers": r"Name Servers:\s?%s" % xStr(r"(?:\t(.+)\n)?", 10),
+    "_test": "rutgers.edu",
 }
 
 # estonian
 ZZ["ee"] = {
     "extend": "com",
     "domain_name": r"Domain:\nname:\s+(.+\.ee)\n",
     "registrar": r"Registrar:\nname:\s+(.+)\n",
@@ -748,42 +775,18 @@
 }
 
 ZZ["nl"] = {
     "extend": "com",
     "expiration_date": None,
     "registrant_country": None,
     "domain_name": r"Domain name:\s?(.+)",
-    "name_servers": (
-        r"""(?x:
-            Domain\ nameservers:\s+(\S+)\r?\n # the first
-            (?:\s+(\S+)\r?\n)?  # a optional 2th
-            (?:\s+(\S+)\r?\n)?  # a optional 3th
-            (?:\s+(\S+)\r?\n)?  # a optional 4th
-            (?:\s+(\S+)\r?\n)?  # a optional 5th
-            # there may be more, best use host -t ns <domain> to get the actual nameservers
-        )"""
-    ),
-    # the format with [A] or [AAAA] is no longer in use
-    #    "name_servers": (
-    #        r"""(?x:
-    #            Domain\ nameservers:[ \t]*\n
-    #            (?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n       # ns1.tld.nl [A?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns2.tld.nl [A?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns2.tld.nl [AAAA?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns3.tld.nl [A?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns3.tld.nl [AAAA?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns4.tld.nl [A?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns4.tld.nl [AAAA?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns5.tld.nl [A?]
-    #            (?:(?:[ \t]+) (\S+) (?:[ \t]+\S+)? \n)?  # opt-ns5.tld.nl [AAAA?]
-    #            # Don't check for final LF; there might be even more records..
-    #        )"""
-    #    ),
+    "name_servers": r"Domain nameservers.*:\n%s" % xStr(r"(?:\s+(\S+)\n)?", 10),
     "reseller": r"Reseller:\s?(.+)",
     "abuse_contact": r"Abuse Contact:\s?(.+)",
+    "_test": "google.nl",
 }
 
 # Norway
 ZZ["no"] = {
     "extend": None,
     "domain_name": r"Domain Name\.+:\s?(.+)",
     "registrar": r"Registrar Handle\.+:\s?(.+)",
@@ -853,16 +856,15 @@
 ZZ["pl"] = {
     # pl has lines ending in multiple line feeds \r and trailing whitespace
     "extend": "uk",
     "registrar": r"\nREGISTRAR:\s*(.+)\n",
     "creation_date": r"\ncreated:\s*(.+)\n",
     "updated_date": r"\nlast modified:\s*(.+)\n",
     "expiration_date": r"\noption expiration date:\s*(.+)\n",
-    # ns: match up to 4
-    "name_servers": r"nameservers:(?:\s+(\S+)[^\n]*\n)(?:\s+(\S+)[^\n]*\n)?(?:\s+(\S+)[^\n]*\n)?(?:\s+(\S+)[^\n]*\n)?",
+    "name_servers": r"nameservers:%s" % xStr(r"(?:\s+(\S+)[^\n]*\n)?", 4),
     "status": r"\nStatus:\n\s*(.+)",
 }
 
 ZZ["pro"] = {
     "extend": "com",
 }
 
@@ -877,15 +879,15 @@
     "extend": "com",
     "domain_name": r"Domain:\s?(.+)",
     "registrar": None,
     "creation_date": r"Creation Date:\s?(.+)",
     "expiration_date": r"Expiration Date:\s?(.+)",
     "updated_date": None,
     # nameservers have trailing info: Name Server: ns1.dnscpanel.com | IPv4:  and IPv6:
-    "name_servers": r"Name Server:(?:\s*(\S+)[^\n]*\n)(?:\s*(\S+)[^\n]*\n)?",
+    "name_servers": r"Name Server:%s" % xStr(r"(?:\s*(\S+)[^\n]*\n)?", 2),
     "status": r"Domain Status:\s?(.+)",
 }
 
 ZZ["pw"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s?(.+)",
     "registrar": r"Registrar:\s*(.+)",
@@ -1037,15 +1039,15 @@
     "domain_name": r"Domain name\.+:(.+)\s*",
     "registrar": r"Registrar\.+:(.+)\s*",
     "registrant": r"Owner Contact\n+Name\.+:\s?(.+)",
     "registrant_country": r"Owner Contact\n(?:.+\n)+Country\.+:\s(.+)",
     "creation_date": r"Creation date\.+:\s?(.+)",
     "expiration_date": None,
     "updated_date": None,
-    "name_servers": r"DNS servers\n(?:Name\.+:\s*(\S+)\n)(?:Name\.+:\s*(\S+)\n)?(?:Name\.+:\s*(\S+)\n)?(?:Name\.+:\s*(\S+)\n)?",
+    "name_servers": r"DNS servers\n%s" % xStr(r"(?:Name\.+:\s*(\S+)\n)?", 4),
     "status": r"Domain status\.+:(.+)",
     # "emails": r"[\w\.-]+@[\w\.-]+\.[\w]{2,4}",
 }
 
 ZZ["tokyo"] = {
     "extend": "com",
     "_server": "whois.nic.tokyo",
@@ -1105,29 +1107,29 @@
 
 ZZ["uk"] = {
     "extend": "com",
     "registrant": r"Registrant:\n\s*(.+)",
     "creation_date": r"Registered on:\s*(.+)",
     "expiration_date": r"Expiry date:\s*(.+)",
     "updated_date": r"Last updated:\s*(.+)",
-    "name_servers": r"Name Servers:\s*(\S+)\r?\n(?:\s+(\S+)\r?\n)?(?:\s+(\S+)\r?\n)?(?:\s+(\S+)\r?\n)?",
+    "name_servers": r"Name servers:%s\n\n" % xStr(r"(?:\n[ \t]+(\S+).*)?", 10),  # capture up to 10
     "status": r"Registration status:\n\s*(.+)",
 }
 
 ZZ["us"] = {"extend": "name"}
 
 ZZ["uz"] = {
     "extend": "com",
     "domain_name": r"Domain Name:\s?(.+)",
     "registrar": r"Registrar:\s*(.+)",
     "creation_date": r"Creation Date:\s?(.+)",
     "expiration_date": r"Expiration Date:\s?(.+)",
     "updated_date": r"Updated Date:\s?(.+)",
     "status": r"Status:\s?(.+)",
-    "name_servers": r"Domain servers in listed order:(?:\n\s+(\S+))(?:\n\s+(\S+))?(?:\n\s+(\S+))?(?:\n\s+(\S+))?\n\n",
+    "name_servers": r"Domain servers in listed order:%s\n\n" % xStr(r"(?:\n\s+(\S+))?", 4),
     # sometimes 'not.defined is returned as a nameserver (e.g. google.uz)
 }
 
 ZZ["vip"] = {
     "_server": "whois.nic.vip",
     "extend": "com",
     "updated_date": None,
@@ -1171,23 +1173,24 @@
 ZZ["net.za"] = {"extend": "za", "_server": "net-whois.registry.net.za"}
 ZZ["co.za"] = {"extend": "za", "_server": "coza-whois.registry.net.za"}
 
 ZZ["gy"] = {"extend": "com"}
 
 # Multiple initialization
 ZZ["ca"] = {"extend": "bank"}
+
 # Rwanda: https://en.wikipedia.org/wiki/.rw
 ZZ["rw"] = {"extend": "com", "_server": "whois.ricta.org.rw"}
-ZZ[".co.rw"] = {"extend": "rw"}
-ZZ[".org.rw"] = {"extend": "rw"}
-ZZ[".net.rw"] = {"extend": "rw"}
-ZZ[".ac.rw"] = {"extend": "rw"}
-ZZ[".gov.rw"] = {"extend": "rw"}
-ZZ[".mil.rw"] = {"extend": "rw"}
-ZZ[".coop.rw"] = {"extend": "rw"}
+ZZ["co.rw"] = {"extend": "rw"}
+ZZ["org.rw"] = {"extend": "rw"}
+ZZ["net.rw"] = {"extend": "rw"}
+ZZ["ac.rw"] = {"extend": "rw"}
+ZZ["gov.rw"] = {"extend": "rw"}
+ZZ["mil.rw"] = {"extend": "rw"}
+ZZ["coop.rw"] = {"extend": "rw"}
 # ZZ[".ltd.rw"] = {"extend": "rw"} # unclear, no longer in https://publicsuffix.org/list/public_suffix_list.dat 2023-06-27 mboot
 
 ZZ["mu"] = {"extend": "bank"}
 ZZ["mu"] = {"extend": "bank"}
 
 # Registry operator: donuts.domains
 # WHOIS server: whois.donuts.co
@@ -1564,15 +1567,16 @@
 }
 
 ZZ["bg"] = {
     "extend": None,
     "_server": "whois.register.bg",
     "domain_name": r"DOMAIN\s+NAME:\s+(.+)",
     "status": r"registration\s+status:\s(.+)",
-    "name_servers": r"NAME SERVER INFORMATION:\n(?:(.+)\n)(?:(.+)\n)?(?:(.+)\n)?(?:(.+)\n)?",
+    # "name_servers": r"NAME SERVER INFORMATION:\n(?:(.+)\n)(?:(.+)\n)?(?:(.+)\n)?(?:(.+)\n)?",
+    "name_servers": r"NAME SERVER INFORMATION:\n%s" % xStr(r"(?:(.+)\n)?", 4),
     "creation_date": None,
     "expiration_date": None,
     "updated_date": None,
     "registrar": None,
     "registrant_country": None,
 }
 
@@ -1740,16 +1744,17 @@
     "registrar": r"Registrar:\s+(.+)",
     "domain_name": r"\s+Domain name:\s+(.+)",
     "creation_date": r"\s+Creation Date:\s+(.+)",
     "expiration_date": r"\s+Expiration Date:\s+(.+)",
     "updated_date": r"\s+Modified Date:\s+(.+)",
     "status": r"\s+Domain Status:\s(.+)",
     "registrant_country": None,
-    "name_servers": r"Name Servers:(?:\n[ \t]+(\S+)[^\n]*)(?:\n[ \t]+(\S+)[^\n]*)?(?:\n[ \t]+(\S+)[^\n]*)?(?:\n[ \t]+(\S+)[^\n]*)?",
+    "name_servers": r"Name Servers:%s" % xStr(r"(?:\n[ \t]+(\S+)[^\n]*)?", 4),
     # make sure the dnssec is not matched
+    "_test": "google.sg",
 }
 
 ZZ["srl"] = {
     "_server": "whois.afilias-srs.net",
     "extend": "ac",
     "registrant_country": r"Registrant Country:\s+(.+)",
 }
@@ -1770,15 +1775,16 @@
     "domain_name": r"Domain Name:\s+(.+)",
     "creation_date": r"\s+Record created on\s+(.+)",
     "expiration_date": r"\s+Record expires on\s+(.+)",
     "status": r"\s+Domain Status:\s+(.+)",
     "registrar": r"Registration\s+Service\s+Provider:\s+(.+)",
     "updated_date": None,
     "registrant_country": None,
-    "name_servers": r"Domain servers in listed order:\s*(\S+)[ \t]*\r?\n(?:\s+(\S+)[ \t]*\r?\n)?(?:\s+(\S+)[ \t]*\r?\n)?(?:\s+(\S+)[ \t]*\r?\n)?",
+    "name_servers": r"Domain servers in listed order:%s" % xStr(r"(?:\s+(\S+)[ \t]*\r?\n)?", 4),
+    "_test": "google.tw",
 }
 
 ZZ["com.tw"] = {
     "extend": "tw",
 }
 
 ZZ["ug"] = {
@@ -2051,21 +2057,15 @@
 ZZ["cx"] = {"extend": "com"}
 ZZ["dz"] = {"extend": "_privateReg"}
 ZZ["gd"] = {"extend": "com"}
 ZZ["mn"] = {"extend": "com"}
 ZZ["tl"] = {"extend": "com"}
 ZZ["gay"] = {"extend": "com", "_server": "whois.nic.gay"}
 ZZ["tt"] = {"extend": "_privateReg"}
-ZZ["mo"] = {
-    "extend": "com",
-    "creation_date": r"created on\s+(.+)",
-    "expiration_date": r"expires on\s+(.+)",
-    "name_servers": r"Domain name servers:\s*\-+(?:\s*(\S+)\n)(?:\s*(\S+)\n)?(?:\s*(\S+)\n)?(?:\s*(\S+)\n)?",
-}
-ZZ["com.mo"] = {"extend": "mo"}
+
 ZZ["st"] = {
     # .ST domains can now be registered with many different competing registrars. and hence different formats
     # >>> line appears quite early, valid info after would have been suppressed with the ^>>> cleanup rule: switched off
     "extend": "com",
     "registrant_country": r"registrant-country:\s+(\S+)",
     "registrant": r"registrant-organi(?:s|z)ation:\s*(.+)\r?\n",
     "expiration_date": r"Expiration\s+Date:\s?(.+)",
@@ -2183,14 +2183,15 @@
 ZZ["mo"] = {
     "extend": "com",
     "_server": "whois.monic.mo",
     "name_servers": r"Domain name servers:\s+-+\s+(\S+)\n(?:(\S+)\n)?(?:(\S+)\n)?(?:(\S+)\n)?",
     "creation_date": r"Record created on (.+)",
     "expiration_date": r"Record expires on (.+)",
 }
+ZZ["com.mo"] = {"extend": "mo"}
 
 ZZ["ph"] = {"extend": "_privateReg"}
 
 ZZ["vc"] = {"extend": "com"}
 ZZ["cm"] = {"extend": "com"}
 
 # russian speaking community
@@ -3045,16 +3046,16 @@
 ZZ["xn--mgbbh1a"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--mgbbh1a71e"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--mgbgu82a"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--rvc1e0am3e"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--s9brj9c"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--xkc2dl3a5ee0h"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["xn--xhq521b"] = {"_server": "whois.ngtld.cn", "extend": "com"}
-ZZ["xn--kprw13d"] = {"extend": "tw"}
-ZZ["xn--kpry57d"] = {"extend": "tw"}
+ZZ["xn--kprw13d"] = {"extend": "tw", "_test": "google.xn--kprw13d"}
+ZZ["xn--kpry57d"] = {"extend": "tw", "_test": "google.xn--kpry57d"}
 ZZ["th"] = {"_server": "whois.thnic.co.th", "extend": "co.th"}
 # whois.thnic.co.th ['co.th']
 ZZ["xn--d1alf"] = {"_server": "whois.marnet.mk", "extend": "mk"}
 # whois.marnet.mk ['mk']
 ZZ["xn--mgb9awbf"] = {"_server": "whois.registry.om", "extend": "om"}
 # whois.registry.om ['om']
 ZZ["xn--mgbah1a3hjkrd"] = {"_server": "whois.nic.mr", "extend": "mr"}
@@ -3158,34 +3159,25 @@
 ZZ["測試"] = {"_privateRegistry": True}
 ZZ["ભરત"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["भरतम"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["भरत"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["भरत"] = {"_server": "whois.registry.in", "extend": "com"}
 ZZ["آزمایشی"] = {"_privateRegistry": True}
 ZZ["பரடச"] = {"_privateRegistry": True}
-ZZ["सगठन"] = {
-    "_server": "whois.nic.xn--i1b6b1a6a2e",
-    "extend": "xn--i1b6b1a6a2e",
-}  # whois.nic.xn--i1b6b1a6a2e ['xn--i1b6b1a6a2e']
+ZZ["सगठन"] = {"_server": "whois.nic.xn--i1b6b1a6a2e", "extend": "xn--i1b6b1a6a2e"}
 ZZ["网络"] = {"_server": "whois.ngtld.cn", "extend": "com"}
 ZZ["ком"] = {"_server": "whois.nic.xn--j1aef", "extend": "xn--j1aef"}  # whois.nic.xn--j1aef ['xn--j1aef']
 ZZ["香港"] = {"_server": "whois.hkirc.hk", "extend": "hk"}  # whois.hkirc.hk ['hk', 'xn--j6w193g']
-ZZ["亚马逊"] = {
-    "_server": "whois.nic.xn--jlq480n2rg",
-    "extend": "xn--jlq480n2rg",
-}  # whois.nic.xn--jlq480n2rg ['xn--jlq480n2rg']
+ZZ["亚马逊"] = {"_server": "whois.nic.xn--jlq480n2rg", "extend": "xn--jlq480n2rg"}
 ZZ["诺基亚"] = {"_privateRegistry": True}
 ZZ["δοκιμή"] = {"_privateRegistry": True}
-ZZ["飞利浦"] = {
-    "_server": "whois.nic.xn--kcrx77d1x4a",
-    "extend": "xn--kcrx77d1x4a",
-}  # whois.nic.xn--kcrx77d1x4a ['xn--kcrx77d1x4a']
+ZZ["飞利浦"] = {"_server": "whois.nic.xn--kcrx77d1x4a", "extend": "xn--kcrx77d1x4a"}
 ZZ["إختبار"] = {"_privateRegistry": True}
-ZZ["台湾"] = {"_server": "whois.twnic.net.tw", "extend": "tw"}
-ZZ["台灣"] = {"_server": "whois.twnic.net.tw", "extend": "tw"}
+ZZ["台湾"] = {"_server": "whois.twnic.net.tw", "extend": "tw", "_test": "google.台湾"}
+ZZ["台灣"] = {"_server": "whois.twnic.net.tw", "extend": "tw", "_test": "google.台灣"}
 ZZ["手表"] = {"_privateRegistry": True}
 ZZ["手机"] = {"_server": "whois.nic.xn--kput3i", "extend": "xn--kput3i"}  # whois.nic.xn--kput3i ['xn--kput3i']
 ZZ["عمان"] = {"_server": "whois.registry.om", "extend": "om"}  # whois.registry.om ['om', 'xn--mgb9awbf']
 ZZ["العليان"] = {
     "_server": "whois.nic.xn--mgba7c0bbn0a",
     "extend": "xn--mgba7c0bbn0a",
 }  # whois.nic.xn--mgba7c0bbn0a ['xn--mgba7c0bbn0a']
```

### Comparing `whoisdomain-1.20230720.2/.gitignore` & `whoisdomain-1.20230804.2/.gitignore`

 * *Files identical despite different names*

### Comparing `whoisdomain-1.20230720.2/README.md` & `whoisdomain-1.20230804.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -212,7 +212,16 @@
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
   * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
   * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
   * 1.20230718.3 fix typo in whois server hint for tld: ru
   * 1.20230720.1 add gov.tr; switch off status:available and status:free as None response, we should not interprete the result by default (we can add a option later)
   * 1.20230720.2 fix server hints for derived second level "xxx.tr", add processing "_test" hints during 'test2.py -a'
+  * add external caching framework that can be overridden for use of your own caching implementation
+  * renaming various vars to mak them more verbose
+  * preparing for capturing all parameters in one object and parring that object around instead of many arguments in methods/functions
+  * switch to json so we dont need a additional dependency in ParamContext
+  * finish rework args to ParameterContext, split of domain as file
+  * 1.20230803.1 frenzy refactor-release
+  * 1.20230804.1 testing
+  * 1.20230804.2 testing after remove of leading dot in rw second level domains
+
```

### Comparing `whoisdomain-1.20230720.2/pyproject.toml` & `whoisdomain-1.20230804.2/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,74 +1,75 @@
 [build-system]
-requires = ["hatchling"]
-build-backend = "hatchling.build"
-
-[tool.hatch.build]
-only-packages = true
-
-include = [
-    "whoisdomain/*.py",
-]
-
-exclude = [
-    "/Old/*",
-    "/lib/*",
-    "/etc/*",
-    "/bin/*",
-    "/testdata/*",
-    "Makefile",
-    ".gitignore",
-    "/.gitignore",
-]
+    requires = ["hatchling"]
+    build-backend = "hatchling.build"
 
 [project]
-name = "whoisdomain"
-dynamic = ['version']
+    name = "whoisdomain"
+    dynamic = ['version']
 
-authors = [
-  { name="DannyCork"},
-]
-
-maintainers = [
-  { name="Maarten Boot", email="130295084+mboot-github@users.noreply.github.com" },
-]
-
-description = "Python package for retrieving WHOIS information of domains."
-readme = "README.md"
-requires-python = ">=3.6"
-
-license = "MIT"
-
-classifiers = [
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: OS Independent",
-    "Intended Audience :: Developers",
-    "Environment :: Console",
-    "Programming Language :: Python :: 3",
-    "Topic :: Internet",
-    "Topic :: Software Development :: Libraries :: Python Modules",
-]
-
-keywords = [
-    "Python",
-    "whois",
-    "tld",
-    "domain",
-    "expiration",
-    "cctld",
-    "registrar",
-]
+    authors = [
+      { name="DannyCork"},
+    ]
+
+    maintainers = [
+      { name="Maarten Boot", email="130295084+mboot-github@users.noreply.github.com" },
+    ]
+
+    description = "Python package for retrieving WHOIS information of domains."
+    readme = "README.md"
+    requires-python = ">=3.6"
+
+    license = "MIT"
+
+    classifiers = [
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+        "Intended Audience :: Developers",
+        "Environment :: Console",
+        "Programming Language :: Python :: 3",
+        "Topic :: Internet",
+        "Topic :: Software Development :: Libraries :: Python Modules",
+    ]
+
+    keywords = [
+        "Python",
+        "whois",
+        "tld",
+        "domain",
+        "expiration",
+        "cctld",
+        "registrar",
+    ]
 
 [project.scripts]
-whoisdomain = 'whoisdomain.main:main'
+    whoisdomain = 'whoisdomain.main:main'
+
+[project.urls]
+    "Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
+    "Home Page" = "https://github.com/mboot-github/WhoisDomain/"
+    "Repository" = "https://github.com/mboot-github/WhoisDomain/"
 
 [tool.hatch.version]
-path = "whoisdomain/version.py"
+    path = "whoisdomain/version.py"
+
+[tool.hatch.build]
+    only-packages = true
+
+    include = [
+        "whoisdomain/*.py",
+    ]
+
+    exclude = [
+        "/Old/*",
+        "/lib/*",
+        "/etc/*",
+        "/bin/*",
+        "/testdata/*",
+        "Makefile",
+        ".gitignore",
+        "/.gitignore",
+    ]
 
 [tool.pylama]
-max_line_length = 160
-skip = "*/.pytest_cache/*, */.tox/*, */mypy_cache/*, ./dist, ./docs"
+    max_line_length = 160
+    skip = "*/.pytest_cache/*, */.tox/*, */mypy_cache/*, ./dist, ./docs"
 
-[project.urls]
-"Bug Tracker" = "https://github.com/mboot-github/WhoisDomain/issues"
-"Home Page" = "https://github.com/mboot-github/WhoisDomain/"
-"Repository" = "https://github.com/mboot-github/WhoisDomain/"
```

### Comparing `whoisdomain-1.20230720.2/PKG-INFO` & `whoisdomain-1.20230804.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: whoisdomain
-Version: 1.20230720.2
+Version: 1.20230804.2
 Summary: Python package for retrieving WHOIS information of domains.
 Project-URL: Bug Tracker, https://github.com/mboot-github/WhoisDomain/issues
 Project-URL: Home Page, https://github.com/mboot-github/WhoisDomain/
 Project-URL: Repository, https://github.com/mboot-github/WhoisDomain/
 Author: DannyCork
 Maintainer-email: Maarten Boot <130295084+mboot-github@users.noreply.github.com>
 License-Expression: MIT
@@ -233,7 +233,16 @@
   * 1.20230627.3 additional kenia second level domains
   * 1.20230712.2 tld .edu now can have up to 10 nameservers; remove action on pull request
   * 1.20230717.1 add tld: com.ru, msk.ru, spb.ru  (all have a test documented), also update the tld: ru, the newlines are not needed.
   * 1.20230717.2 add option to parse partial result after timout has occurred (parse_partial_response:bool default False); this will need `stdbuf` installed otherwise it will fail
   * 1.20230718.3 fix typo in whois server hint for tld: ru
   * 1.20230720.1 add gov.tr; switch off status:available and status:free as None response, we should not interprete the result by default (we can add a option later)
   * 1.20230720.2 fix server hints for derived second level "xxx.tr", add processing "_test" hints during 'test2.py -a'
+  * add external caching framework that can be overridden for use of your own caching implementation
+  * renaming various vars to mak them more verbose
+  * preparing for capturing all parameters in one object and parring that object around instead of many arguments in methods/functions
+  * switch to json so we dont need a additional dependency in ParamContext
+  * finish rework args to ParameterContext, split of domain as file
+  * 1.20230803.1 frenzy refactor-release
+  * 1.20230804.1 testing
+  * 1.20230804.2 testing after remove of leading dot in rw second level domains
+
```

