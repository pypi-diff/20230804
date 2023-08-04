# Comparing `tmp/temper_syntax-0.1.0.tar.gz` & `tmp/temper_syntax-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "temper_syntax-0.1.0.tar", max compression
+gzip compressed data, was "temper_syntax-0.1.1.tar", max compression
```

## Comparing `temper_syntax-0.1.0.tar` & `temper_syntax-0.1.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      803 2023-07-31 22:58:26.990693 temper_syntax-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-07-31 22:54:59.260105 temper_syntax-0.1.0/temper_syntax/__init__.py
--rw-r--r--   0        0        0      126 2023-07-31 22:54:59.278281 temper_syntax-0.1.0/temper_syntax/__init__.py.map
--rw-r--r--   0        0        0       99 2023-07-31 22:54:59.263051 temper_syntax-0.1.0/temper_syntax/config.py
--rw-r--r--   0        0        0      799 2023-07-31 22:54:59.275929 temper_syntax-0.1.0/temper_syntax/config.py.map
--rw-r--r--   0        0        0     5095 2023-07-31 22:54:59.275929 temper_syntax-0.1.0/temper_syntax/pygments.py
--rw-r--r--   0        0        0     9472 2023-07-31 22:54:59.278281 temper_syntax-0.1.0/temper_syntax/pygments.py.map
--rw-r--r--   0        0        0       44 2023-07-31 22:54:59.261902 temper_syntax-0.1.0/temper_syntax/pygments__preface.py
--rw-r--r--   0        0        0     3046 2023-07-31 22:54:59.263051 temper_syntax-0.1.0/temper_syntax/pygments__preface.py.map
--rw-r--r--   0        0        0     6411 2023-07-31 22:54:59.279281 temper_syntax-0.1.0/temper_syntax/temper_pygments.py
--rw-r--r--   0        0        0    12284 2023-07-31 22:54:59.282281 temper_syntax-0.1.0/temper_syntax/temper_pygments.py.map
--rw-r--r--   0        0        0       44 2023-07-31 22:54:59.261902 temper_syntax-0.1.0/temper_syntax/temper_pygments__preface.py
--rw-r--r--   0        0        0     4437 2023-07-31 22:54:59.264509 temper_syntax-0.1.0/temper_syntax/temper_pygments__preface.py.map
--rw-r--r--   0        0        0     4049 2023-07-31 22:54:59.273929 temper_syntax-0.1.0/temper_syntax/tempermd_pygments.py
--rw-r--r--   0        0        0     6291 2023-07-31 22:54:59.277272 temper_syntax-0.1.0/temper_syntax/tempermd_pygments.py.map
--rw-r--r--   0        0        0       44 2023-07-31 22:54:59.261902 temper_syntax-0.1.0/temper_syntax/tempermd_pygments__preface.py
--rw-r--r--   0        0        0     1771 2023-07-31 22:54:59.263051 temper_syntax-0.1.0/temper_syntax/tempermd_pygments__preface.py.map
--rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 temper_syntax-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      801 2023-08-04 17:21:36.942063 temper_syntax-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-08-04 17:21:36.937394 temper_syntax-0.1.1/temper_syntax/__init__.py
+-rw-r--r--   0        0        0      126 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/__init__.py.map
+-rw-r--r--   0        0        0       99 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/config.py
+-rw-r--r--   0        0        0      799 2023-08-04 17:21:36.957566 temper_syntax-0.1.1/temper_syntax/config.py.map
+-rw-r--r--   0        0        0     5095 2023-08-04 17:21:36.955569 temper_syntax-0.1.1/temper_syntax/pygments.py
+-rw-r--r--   0        0        0     9472 2023-08-04 17:21:36.956566 temper_syntax-0.1.1/temper_syntax/pygments.py.map
+-rw-r--r--   0        0        0       44 2023-08-04 17:21:36.939912 temper_syntax-0.1.1/temper_syntax/pygments__preface.py
+-rw-r--r--   0        0        0     3046 2023-08-04 17:21:36.956566 temper_syntax-0.1.1/temper_syntax/pygments__preface.py.map
+-rw-r--r--   0        0        0     6946 2023-08-04 17:21:36.958566 temper_syntax-0.1.1/temper_syntax/temper_pygments.py
+-rw-r--r--   0        0        0    13736 2023-08-04 17:21:36.961574 temper_syntax-0.1.1/temper_syntax/temper_pygments.py.map
+-rw-r--r--   0        0        0       44 2023-08-04 17:21:36.940911 temper_syntax-0.1.1/temper_syntax/temper_pygments__preface.py
+-rw-r--r--   0        0        0     5120 2023-08-04 17:21:36.942063 temper_syntax-0.1.1/temper_syntax/temper_pygments__preface.py.map
+-rw-r--r--   0        0        0     4049 2023-08-04 17:21:36.991575 temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py
+-rw-r--r--   0        0        0     6291 2023-08-04 17:21:36.992576 temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py.map
+-rw-r--r--   0        0        0       44 2023-08-04 17:21:36.952565 temper_syntax-0.1.1/temper_syntax/tempermd_pygments__preface.py
+-rw-r--r--   0        0        0     1771 2023-08-04 17:21:36.953566 temper_syntax-0.1.1/temper_syntax/tempermd_pygments__preface.py.map
+-rw-r--r--   0        0        0      382 1970-01-01 00:00:00.000000 temper_syntax-0.1.1/PKG-INFO
```

### Comparing `temper_syntax-0.1.0/pyproject.toml` & `temper_syntax-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "temper-syntax"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 readme = ""
 requires-python = "~=3.8"
 license = {text = ""}
 authors = [  ]
 
 maintainers = [ ]
@@ -20,15 +20,15 @@
 [project.gui-scripts]
 
 [project.entry-points]
 
 
 [tool.poetry]
 name = "temper-syntax"
-version = "0.1.0"
+version = "0.1.1"
 license = ""
 description = ""
 authors = [  ]
 
 packages = [{ include = "temper_syntax" }]
 include = ["temper_syntax/**/*", "./**/*.so"]
 
@@ -37,11 +37,11 @@
 temper-core = "0.0.5"
 
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
-python_functions = "test_[!_]*"
+python_functions = "test___*"
 python_files = "test_*.py"
 python_classes = "Test__*"
 testpaths = ["tests"]
```

### Comparing `temper_syntax-0.1.0/temper_syntax/config.py.map` & `temper_syntax-0.1.1/temper_syntax/config.py.map`

 * *Files 13% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourcesContent'": '[\'# Temper Syntax\\n\\n    export let name = "temper-syntax";\\n    export '*

 * *                     'let version = "0.1.1";\\n\\nThis temper library supports syntax highlighting '*

 * *                     'for multiple backends and\\nframeworks. The intent is that some shared '*

 * *                     'definitions can be used despite the\\nsubtle differences between '*

 * *                     'frameworks.\\n\\nIdeally, tree shaking / linking in backends can clean out '*

 * *                     'what\\ […]*

```diff
@@ -6,11 +6,11 @@
         "version",
         "return"
     ],
     "sources": [
         "-work/temper-syntax/config.temper.md"
     ],
     "sourcesContent": [
-        "# Temper Syntax\n\n    export let name = \"temper-syntax\";\n    export let version = \"0.1.0\";\n\nThis temper library supports syntax highlighting for multiple backends and\nframeworks. The intent is that some shared definitions can be used despite the\nsubtle differences between frameworks.\n\nIdeally, tree shaking / linking in backends can clean out what's unused.\n\n    import(\"./temper-pygments\");\n    import(\"./tempermd-pygments\");\n"
+        "# Temper Syntax\n\n    export let name = \"temper-syntax\";\n    export let version = \"0.1.1\";\n\nThis temper library supports syntax highlighting for multiple backends and\nframeworks. The intent is that some shared definitions can be used despite the\nsubtle differences between frameworks.\n\nIdeally, tree shaking / linking in backends can clean out what's unused.\n\n    import(\"./temper-pygments\");\n    import(\"./tempermd-pygments\");\n"
     ],
     "version": 3
 }
```

### Comparing `temper_syntax-0.1.0/temper_syntax/pygments.py` & `temper_syntax-0.1.1/temper_syntax/pygments.py`

 * *Files identical despite different names*

### Comparing `temper_syntax-0.1.0/temper_syntax/pygments.py.map` & `temper_syntax-0.1.1/temper_syntax/pygments.py.map`

 * *Files identical despite different names*

### Comparing `temper_syntax-0.1.0/temper_syntax/pygments__preface.py.map` & `temper_syntax-0.1.1/temper_syntax/pygments__preface.py.map`

 * *Files identical despite different names*

### Comparing `temper_syntax-0.1.0/temper_syntax/temper_pygments.py` & `temper_syntax-0.1.1/temper_syntax/temper_pygments.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,80 +10,92 @@
   __slots__ = ('name__34', 'aliases__35', 'filenames__36', 'tokens__37')
   def constructor__38(this__0, name: 'str' = ..., aliases: 'Tuple3[str, ...]' = ..., filenames: 'Tuple3[str, ...]' = ..., tokens: 'Map__16[str, (Tuple3[RuleOption__8, ...])]' = ...) -> Any1:
     name__39: 'str' = name
     aliases__40: 'Tuple3[str, ...]' = aliases
     filenames__41: 'Tuple3[str, ...]' = filenames
     tokens__42: 'Map__16[str, (Tuple3[RuleOption__8, ...])]' = tokens
     return__4: 'None'
-    t_190: 'Rule__9'
-    t_192: 'Rule__9'
-    t_193: 'Rule__9'
-    t_194: 'Map__16[str, (Tuple3[RuleOption__8, ...])]'
-    t_195: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
-    t_196: 'Rule__9'
-    t_197: 'Rule__9'
-    t_198: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
-    t_199: 'Include__10'
-    t_200: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
-    t_201: 'Rule__9'
-    t_202: 'Rule__9'
-    t_203: 'str'
-    t_204: 'str'
-    t_205: 'str'
-    t_206: 'str'
     t_207: 'Rule__9'
-    t_208: 'Rule__9'
     t_209: 'Rule__9'
     t_210: 'Rule__9'
     t_211: 'Rule__9'
-    t_212: 'Rule__9'
-    t_213: 'Rule__9'
+    t_212: 'Map__16[str, (Tuple3[RuleOption__8, ...])]'
+    t_213: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
     t_214: 'Rule__9'
     t_215: 'Rule__9'
-    t_216: 'Rule__9'
-    t_127: 'Tuple3[RuleOption__8, ...]'
-    t_131: 'Tuple3[RuleOption__8, ...]'
-    t_136: 'Tuple3[RuleOption__8, ...]'
+    t_216: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
+    t_217: 'Include__10'
+    t_218: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
+    t_219: 'Rule__9'
+    t_220: 'Rule__9'
+    t_221: 'Rule__9'
+    t_222: 'Pair__22[str, (Tuple3[RuleOption__8, ...])]'
+    t_223: 'Rule__9'
+    t_224: 'Rule__9'
+    t_225: 'str'
+    t_226: 'str'
+    t_227: 'str'
+    t_228: 'str'
+    t_229: 'Rule__9'
+    t_230: 'Rule__9'
+    t_231: 'Rule__9'
+    t_232: 'Rule__9'
+    t_233: 'Rule__9'
+    t_234: 'Rule__9'
+    t_235: 'Rule__9'
+    t_236: 'Rule__9'
+    t_237: 'Rule__9'
+    t_238: 'Rule__9'
+    t_133: 'Tuple3[RuleOption__8, ...]'
+    t_139: 'Tuple3[RuleOption__8, ...]'
+    t_143: 'Tuple3[RuleOption__8, ...]'
+    t_148: 'Tuple3[RuleOption__8, ...]'
     if name__39 is ...:
       name__39 = 'Temper'
     if aliases__40 is ...:
       aliases__40 = ('temper',)
     if filenames__41 is ...:
       filenames__41 = ('*.temper',)
     if tokens__42 is ...:
-      t_190 = Rule__9('\\s+', Whitespace__33)
-      t_201 = Rule__9('//.*?$', CommentSingleline__21)
-      t_202 = Rule__9('(?s)/\\*.*\\*/', CommentMultiline__20)
-      t_203 = words__6('false', 'NaN', 'null', 'true', 'void')
-      t_216 = Rule__9(t_203, KeywordConstant__23)
-      t_204 = words__6('class', 'interface', 'let', 'private', 'public', 'sealed', 'var')
-      t_215 = Rule__9(t_204, KeywordDeclaration__24)
-      t_205 = words__6('do', 'else', 'export', 'extends', 'fn', 'if', 'import', 'is', 'match', 'new', 'orelse')
-      t_214 = Rule__9(t_205, Keyword__22)
-      t_206 = words__6('AnyValue', 'Boolean', 'Float64', 'Function', 'Int', 'List', 'ListBuilder', 'Listed', 'Map', 'MapBuilder', 'MapKey', 'Mapped', 'NoResult', 'Null', 'String', 'StringSlice', 'Void')
-      t_213 = Rule__9(t_206, NameBuiltin__26)
-      t_207 = Rule__9('"', StringKind__31, 'string')
-      t_208 = Rule__9('[-=+*&|<>]+|/=?', Operator__29)
-      t_209 = Rule__9('[{}();:.,]', Punctuation__30)
-      t_210 = Rule__9('\\d+\\.?\\d*|\\.\\d+', Number__28)
-      t_211 = Rule__9('@[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*', NameDecorator__27)
-      t_212 = Rule__9('[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*', Name__25)
-      t_127 = cast_by_type5((t_190, t_201, t_202, t_216, t_215, t_214, t_213, t_207, t_208, t_209, t_210, t_211, t_212), tuple4)
-      t_200 = Pair_255('root', t_127)
-      t_192 = Rule__9('}', StringInterpol__32, '#pop')
-      t_199 = include__11('root')
-      t_131 = cast_by_type5((t_192, t_199), tuple4)
-      t_198 = Pair_255('interpolation', t_131)
-      t_193 = Rule__9('"', StringKind__31, '#pop')
-      t_196 = Rule__9('\\$\\{', StringInterpol__32, 'interpolation')
-      t_197 = Rule__9('(?:[^"$]|\\$[^{])+', StringKind__31)
-      t_136 = cast_by_type5((t_193, t_196, t_197), tuple4)
-      t_195 = Pair_255('string', t_136)
-      t_194 = map_constructor_256((t_200, t_198, t_195))
-      tokens__42 = t_194
+      t_207 = Rule__9('\\s+', Whitespace__33)
+      t_223 = Rule__9('//.*?$', CommentSingleline__21)
+      t_224 = Rule__9('/\\*', CommentMultiline__20, 'nestedcomment')
+      t_225 = words__6('false', 'NaN', 'null', 'true', 'void')
+      t_238 = Rule__9(t_225, KeywordConstant__23)
+      t_226 = words__6('class', 'interface', 'let', 'private', 'public', 'sealed', 'var')
+      t_237 = Rule__9(t_226, KeywordDeclaration__24)
+      t_227 = words__6('do', 'else', 'export', 'extends', 'fn', 'if', 'import', 'is', 'match', 'new', 'orelse')
+      t_236 = Rule__9(t_227, Keyword__22)
+      t_228 = words__6('AnyValue', 'Boolean', 'Float64', 'Function', 'Int', 'List', 'ListBuilder', 'Listed', 'Map', 'MapBuilder', 'MapKey', 'Mapped', 'NoResult', 'Null', 'String', 'StringSlice', 'Void')
+      t_235 = Rule__9(t_228, NameBuiltin__26)
+      t_229 = Rule__9('"', StringKind__31, 'string')
+      t_230 = Rule__9('[-=+*&|<>]+|/=?', Operator__29)
+      t_231 = Rule__9('[{}();:.,]', Punctuation__30)
+      t_232 = Rule__9('\\d+\\.?\\d*|\\.\\d+', Number__28)
+      t_233 = Rule__9('@[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*', NameDecorator__27)
+      t_234 = Rule__9('[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*', Name__25)
+      t_133 = cast_by_type5((t_207, t_223, t_224, t_238, t_237, t_236, t_235, t_229, t_230, t_231, t_232, t_233, t_234), tuple4)
+      t_222 = Pair_255('root', t_133)
+      t_209 = Rule__9('[^*/]+', CommentMultiline__20)
+      t_219 = Rule__9('/\\*', CommentMultiline__20, '#push')
+      t_220 = Rule__9('\\*/', CommentMultiline__20, '#pop')
+      t_221 = Rule__9('[*/]', CommentMultiline__20)
+      t_139 = cast_by_type5((t_209, t_219, t_220, t_221), tuple4)
+      t_218 = Pair_255('nestedcomment', t_139)
+      t_210 = Rule__9('}', StringInterpol__32, '#pop')
+      t_217 = include__11('root')
+      t_143 = cast_by_type5((t_210, t_217), tuple4)
+      t_216 = Pair_255('interpolation', t_143)
+      t_211 = Rule__9('"', StringKind__31, '#pop')
+      t_214 = Rule__9('\\$\\{', StringInterpol__32, 'interpolation')
+      t_215 = Rule__9('(?:[^"$]|\\$[^{])+', StringKind__31)
+      t_148 = cast_by_type5((t_211, t_214, t_215), tuple4)
+      t_213 = Pair_255('string', t_148)
+      t_212 = map_constructor_256((t_222, t_218, t_216, t_213))
+      tokens__42 = t_212
     this__0.name__34 = name__39
     this__0.aliases__35 = aliases__40
     this__0.filenames__36 = filenames__41
     this__0.tokens__37 = tokens__42
     return__4 = None
     return return__4
   def __init__(this__0, name: 'str' = ..., aliases: 'Tuple3[str, ...]' = ..., filenames: 'Tuple3[str, ...]' = ..., tokens: 'Map__16[str, (Tuple3[RuleOption__8, ...])]' = ...) -> None:
@@ -111,18 +123,18 @@
   def tokens(this__60) -> 'Map__16[str, (Tuple3[RuleOption__8, ...])]':
     return__61: 'Map__16[str, (Tuple3[RuleOption__8, ...])]'
     return__61 = this__60.tokens__37
     return return__61
 def words__6(*names__43: 'str') -> 'str':
   global list_join_257, str_cat_258
   return__5: 'str'
-  def fn__218(x__45: 'str') -> 'str':
-    return__143: 'str'
-    return__143 = x__45
-    return return__143
-  t_220: 'Callable6[[str], str]' = fn__218
-  t_221: 'str' = list_join_257(names__43, '|', t_220)
-  return__5 = str_cat_258('\\b(?:', t_221, ')\\b')
+  def fn__240(x__45: 'str') -> 'str':
+    return__155: 'str'
+    return__155 = x__45
+    return return__155
+  t_242: 'Callable6[[str], str]' = fn__240
+  t_243: 'str' = list_join_257(names__43, '|', t_242)
+  return__5 = str_cat_258('\\b(?:', t_243, ')\\b')
   return return__5
 nameRegex__7: 'str' = '[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*'
-return__142: 'None' = None
-export = return__142
+return__154: 'None' = None
+export = return__154
```

### Comparing `temper_syntax-0.1.0/temper_syntax/temper_pygments.py.map` & `temper_syntax-0.1.1/temper_syntax/temper_pygments.py.map`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7961309523809524%*

 * *Differences: {"'mappings'": "'A,wB,Y,I,a,E,Y,I,a,E,I,I,Q,E,e,I,mB,E,S,I,a,E,O,I;A,mB,K,I,M,E,G,I,I,E,Q,I;A,qB,K,I;AAuBqB,IAA6B,8BAAA,AAA7B,CAAAc,UAA6B,GAAA,AAA7B,CAAAA,aAA6B,CAKxC,CAAAC,IAA8B,GAAA,AAA9B,CAAAA,OAA8B,CAqD9B,CAAAC,OAAe,GAAA,AAAf,CAAAA,WAAe,CA4BP,CAAAC,UAAA,IAAAA,cAAA,CAAA,AAAR,CAAAC,IAAG,GAAA,AAAH,CAAAA,QAAG,CAAK,CAAAC,kBAAA,IAAAA,qBAAA,EAAAC,iBAAA,IAAAA,oBAAA,EAAAC,gBAAA,IAAAA,mBAAA,EAAAC,mBAAA,IAAAA,sBAAA,EAAAC,OAAA,IAAAA,WAAA,EAAAC,YAAA,IAAAA,eAAA,EAAAC,WAAA,IAAAA,cAAA,EAAAC,QAAA,IAAAA,YAAA,EAAAC,WAAA,I […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "OUTPUT_ROOT/temper-syntax/py/temper_syntax/temper_pygments.py",
-    "mappings": "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",
+    "mappings": "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",
     "names": [
         "TemperObject",
         "cast_by_type",
         "Pair",
         "Pair#255",
         "map_constructor",
         "map_constructor#256",
@@ -46,52 +46,58 @@
         "name",
         "aliases",
         "filenames",
         "tokens",
         "constructor",
         "this",
         "return",
-        "t#190",
-        "t#192",
-        "t#193",
-        "t#194",
-        "t#195",
-        "t#196",
-        "t#197",
-        "t#198",
-        "t#199",
-        "t#200",
-        "t#201",
-        "t#202",
-        "t#203",
-        "t#204",
-        "t#205",
-        "t#206",
         "t#207",
-        "t#208",
         "t#209",
         "t#210",
         "t#211",
         "t#212",
         "t#213",
         "t#214",
         "t#215",
         "t#216",
-        "t#127",
-        "t#131",
-        "t#136",
+        "t#217",
+        "t#218",
+        "t#219",
+        "t#220",
+        "t#221",
+        "t#222",
+        "t#223",
+        "t#224",
+        "t#225",
+        "t#226",
+        "t#227",
+        "t#228",
+        "t#229",
+        "t#230",
+        "t#231",
+        "t#232",
+        "t#233",
+        "t#234",
+        "t#235",
+        "t#236",
+        "t#237",
+        "t#238",
+        "t#133",
+        "t#139",
+        "t#143",
+        "t#148",
         "words",
         "names",
         "fn",
         "x",
-        "t#220",
-        "t#221",
+        "t#242",
+        "t#243",
         "nameRegex"
     ],
     "sources": [
         "-work/temper-syntax/temper-pygments.temper.md"
     ],
     "sourcesContent": [
-        "# Temper Pygments Lexer\n\n## Lexer class\n\nWe can't easily access backend classes, so we can't subclass\n`pygments.lexer.RegexLexer`, but we can define a separate class that can then\nbe subclassed in Python or elsewhere.\n\nTODO Maybe define an independent Lexer type and just create an instance here?\n\n    export class TemperLexer {\n\nThese indicators seems somewhat redundant to me, but they follow the examples in\nthe [Pygments documentation][pygments-lexer-docs].\n\n      public name: String = \"Temper\";\n      public aliases: List<String> = [\"temper\"];\n      public filenames: List<String> = [\"*.temper\"];\n\n### Token rules\n\nMain thing, though, is the list of rules for definition tokens.\n\n      public tokens: Map<String, List<RuleOption>> = new Map([\n\n#### Root\n\n        new Pair(\"root\", [\n          new Rule(raw\"\\s+\", Whitespace),\n          new Rule(\"//.*?$\", CommentSingleline),\n\nMultiline comments in Temper don't nest at present, so this should be fine.\n\n          new Rule(raw\"(?s)/\\*.*\\*/\", CommentMultiline),\n          new Rule(\n            words(\"false\", \"NaN\", \"null\", \"true\", \"void\"),\n            KeywordConstant,\n          ),\n          new Rule(\n            words(\n              \"class\", \"interface\", \"let\", \"private\", \"public\", \"sealed\", \"var\",\n            ),\n            KeywordDeclaration,\n          ),\n          new Rule(\n            words(\n              \"do\", \"else\", \"export\", \"extends\", \"fn\", \"if\", \"import\", \"is\",\n              \"match\", \"new\", \"orelse\",\n            ),\n            Keyword,\n          ),\n          new Rule(\n            words(\n              \"AnyValue\", \"Boolean\", \"Float64\", \"Function\", \"Int\", \"List\",\n              \"ListBuilder\", \"Listed\", \"Map\", \"MapBuilder\", \"MapKey\", \"Mapped\",\n              \"NoResult\", \"Null\", \"String\", \"StringSlice\", \"Void\",\n            ),\n            NameBuiltin,\n          ),\n          new Rule(\"\\\"\", StringKind, \"string\"),\n          new Rule(\"[-=+*&|<>]+|/=?\", Operator),\n          new Rule(\"[{}();:.,]\", Punctuation),\n          new Rule(raw\"\\d+\\.?\\d*|\\.\\d+\", Number),\n          new Rule(\"@${nameRegex}\", NameDecorator),\n          new Rule(nameRegex, Name),\n        ].as<List<RuleOption>>()),\n\n#### Strings\n\n        new Pair(\"interpolation\", [\n          new Rule(\"}\", StringInterpol, \"#pop\"),\n          include(\"root\"),\n        ].as<List<RuleOption>>()),\n\nI'm not sure if order matters here. Seems simpler, but if I don't exclude `${`\nfrom core string chars, I don't get interp.\n\n        new Pair(\"string\", [\n          new Rule(\"\\\"\", StringKind, \"#pop\"),\n          new Rule(raw\"\\$\\{\", StringInterpol, \"interpolation\"),\n          new Rule(\"(?:[^\\\"$]|\\\\$[^{])+\", StringKind),\n        ].as<List<RuleOption>>()),\n\n      ]);\n\n    }\n\n## Helper functions and values\n\nBe sloppy with names for now. TODO More complete Unicode support.\n\n    let nameRegex = \"[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*\";\n\n    let words(...names: List<String>): String {\n      \"\\\\b(?:${names.join(\"|\") { (x);; x }})\\\\b\"\n    }\n\n## Imports and links\n\n    let { ... } = import(\"./pygments\");\n\n[issue1631]: https://github.com/temper-lang/temper/issues/1631\n[pygments-lexer-docs]: https://pygments.org/docs/lexerdevelopment/\n"
+        "# Temper Pygments Lexer\n\n## Lexer class\n\nWe can't easily access backend classes, so we can't subclass\n`pygments.lexer.RegexLexer`, but we can define a separate class that can then\nbe subclassed in Python or elsewhere.\n\nTODO Maybe define an independent Lexer type and just create an instance here?\n\n    export class TemperLexer {\n\nThese indicators seems somewhat redundant to me, but they follow the examples in\nthe [Pygments documentation][pygments-lexer-docs].\n\n      public name: String = \"Temper\";\n      public aliases: List<String> = [\"temper\"];\n      public filenames: List<String> = [\"*.temper\"];\n\n### Token rules\n\nMain thing, though, is the list of rules for definition tokens.\n\n      public tokens: Map<String, List<RuleOption>> = new Map([\n\n#### Root\n\n        new Pair(\"root\", [\n          new Rule(raw\"\\s+\", Whitespace),\n          new Rule(\"//.*?$\", CommentSingleline),\n          new Rule(raw\"/\\*\", CommentMultiline, \"nestedcomment\"),\n          new Rule(\n            words(\"false\", \"NaN\", \"null\", \"true\", \"void\"),\n            KeywordConstant,\n          ),\n          new Rule(\n            words(\n              \"class\", \"interface\", \"let\", \"private\", \"public\", \"sealed\", \"var\",\n            ),\n            KeywordDeclaration,\n          ),\n          new Rule(\n            words(\n              \"do\", \"else\", \"export\", \"extends\", \"fn\", \"if\", \"import\", \"is\",\n              \"match\", \"new\", \"orelse\",\n            ),\n            Keyword,\n          ),\n          new Rule(\n            words(\n              \"AnyValue\", \"Boolean\", \"Float64\", \"Function\", \"Int\", \"List\",\n              \"ListBuilder\", \"Listed\", \"Map\", \"MapBuilder\", \"MapKey\", \"Mapped\",\n              \"NoResult\", \"Null\", \"String\", \"StringSlice\", \"Void\",\n            ),\n            NameBuiltin,\n          ),\n          new Rule(\"\\\"\", StringKind, \"string\"),\n          new Rule(\"[-=+*&|<>]+|/=?\", Operator),\n          new Rule(\"[{}();:.,]\", Punctuation),\n          new Rule(raw\"\\d+\\.?\\d*|\\.\\d+\", Number),\n          new Rule(\"@${nameRegex}\", NameDecorator),\n          new Rule(nameRegex, Name),\n        ].as<List<RuleOption>>()),\n\n#### Multiline/Nested Comments\n\nWe plan to support nested comments soon, so just implement that already here.\nThe technique here is based on the `nestedcomment` for the [D Language lexer for\nPygments][dlang-nestedcomment].\n\n        new Pair(\"nestedcomment\", [\n          new Rule(raw\"[^*/]+\", CommentMultiline),\n          new Rule(raw\"/\\*\", CommentMultiline, \"#push\"),\n          new Rule(raw\"\\*/\", CommentMultiline, \"#pop\"),\n          new Rule(raw\"[*/]\", CommentMultiline),\n        ].as<List<RuleOption>>()),\n\n#### Strings\n\n        new Pair(\"interpolation\", [\n          new Rule(\"}\", StringInterpol, \"#pop\"),\n          include(\"root\"),\n        ].as<List<RuleOption>>()),\n\nI'm not sure if order matters here. Seems simpler, but if I don't exclude `${`\nfrom core string chars, I don't get interp.\n\n        new Pair(\"string\", [\n          new Rule(\"\\\"\", StringKind, \"#pop\"),\n          new Rule(raw\"\\$\\{\", StringInterpol, \"interpolation\"),\n          new Rule(\"(?:[^\\\"$]|\\\\$[^{])+\", StringKind),\n        ].as<List<RuleOption>>()),\n\n      ]);\n\n    }\n\n## Helper functions and values\n\nBe sloppy with names for now. TODO More complete Unicode support.\n\n    let nameRegex = \"[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*\";\n\n    let words(...names: List<String>): String {\n      \"\\\\b(?:${names.join(\"|\") { (x);; x }})\\\\b\"\n    }\n\n## Imports and links\n\n    let { ... } = import(\"./pygments\");\n\n[dlang-nestedcomment]: https://github.com/pygments/pygments/blob/d0acfff1121f9ee3696b01a9077ebe9990216634/pygments/lexers/d.py#L242\n[issue1631]: https://github.com/temper-lang/temper/issues/1631\n[pygments-lexer-docs]: https://pygments.org/docs/lexerdevelopment/\n"
     ],
     "version": 3
 }
```

### Comparing `temper_syntax-0.1.0/temper_syntax/temper_pygments__preface.py.map` & `temper_syntax-0.1.1/temper_syntax/temper_pygments__preface.py.map`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9166666666666666%*

 * *Differences: {"'sourcesContent'": "['# Temper Pygments Lexer\\n\\n## Lexer class\\n\\nWe can\\'t easily access "*

 * *                     "backend classes, so we can\\'t subclass\\n`pygments.lexer.RegexLexer`, but "*

 * *                     'we can define a separate class that can then\\nbe subclassed in Python or '*

 * *                     'elsewhere.\\n\\nTODO Maybe define an independent Lexer type and just create '*

 * *                     'an instance here?\\n\\n    export class TemperLexer {\\n\\nThese indicators '*

 * *                […]*

```diff
@@ -4,11 +4,11 @@
     "names": [
         "return"
     ],
     "sources": [
         "-work/temper-syntax/temper-pygments.temper.md"
     ],
     "sourcesContent": [
-        "# Temper Pygments Lexer\n\n## Lexer class\n\nWe can't easily access backend classes, so we can't subclass\n`pygments.lexer.RegexLexer`, but we can define a separate class that can then\nbe subclassed in Python or elsewhere.\n\nTODO Maybe define an independent Lexer type and just create an instance here?\n\n    export class TemperLexer {\n\nThese indicators seems somewhat redundant to me, but they follow the examples in\nthe [Pygments documentation][pygments-lexer-docs].\n\n      public name: String = \"Temper\";\n      public aliases: List<String> = [\"temper\"];\n      public filenames: List<String> = [\"*.temper\"];\n\n### Token rules\n\nMain thing, though, is the list of rules for definition tokens.\n\n      public tokens: Map<String, List<RuleOption>> = new Map([\n\n#### Root\n\n        new Pair(\"root\", [\n          new Rule(raw\"\\s+\", Whitespace),\n          new Rule(\"//.*?$\", CommentSingleline),\n\nMultiline comments in Temper don't nest at present, so this should be fine.\n\n          new Rule(raw\"(?s)/\\*.*\\*/\", CommentMultiline),\n          new Rule(\n            words(\"false\", \"NaN\", \"null\", \"true\", \"void\"),\n            KeywordConstant,\n          ),\n          new Rule(\n            words(\n              \"class\", \"interface\", \"let\", \"private\", \"public\", \"sealed\", \"var\",\n            ),\n            KeywordDeclaration,\n          ),\n          new Rule(\n            words(\n              \"do\", \"else\", \"export\", \"extends\", \"fn\", \"if\", \"import\", \"is\",\n              \"match\", \"new\", \"orelse\",\n            ),\n            Keyword,\n          ),\n          new Rule(\n            words(\n              \"AnyValue\", \"Boolean\", \"Float64\", \"Function\", \"Int\", \"List\",\n              \"ListBuilder\", \"Listed\", \"Map\", \"MapBuilder\", \"MapKey\", \"Mapped\",\n              \"NoResult\", \"Null\", \"String\", \"StringSlice\", \"Void\",\n            ),\n            NameBuiltin,\n          ),\n          new Rule(\"\\\"\", StringKind, \"string\"),\n          new Rule(\"[-=+*&|<>]+|/=?\", Operator),\n          new Rule(\"[{}();:.,]\", Punctuation),\n          new Rule(raw\"\\d+\\.?\\d*|\\.\\d+\", Number),\n          new Rule(\"@${nameRegex}\", NameDecorator),\n          new Rule(nameRegex, Name),\n        ].as<List<RuleOption>>()),\n\n#### Strings\n\n        new Pair(\"interpolation\", [\n          new Rule(\"}\", StringInterpol, \"#pop\"),\n          include(\"root\"),\n        ].as<List<RuleOption>>()),\n\nI'm not sure if order matters here. Seems simpler, but if I don't exclude `${`\nfrom core string chars, I don't get interp.\n\n        new Pair(\"string\", [\n          new Rule(\"\\\"\", StringKind, \"#pop\"),\n          new Rule(raw\"\\$\\{\", StringInterpol, \"interpolation\"),\n          new Rule(\"(?:[^\\\"$]|\\\\$[^{])+\", StringKind),\n        ].as<List<RuleOption>>()),\n\n      ]);\n\n    }\n\n## Helper functions and values\n\nBe sloppy with names for now. TODO More complete Unicode support.\n\n    let nameRegex = \"[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*\";\n\n    let words(...names: List<String>): String {\n      \"\\\\b(?:${names.join(\"|\") { (x);; x }})\\\\b\"\n    }\n\n## Imports and links\n\n    let { ... } = import(\"./pygments\");\n\n[issue1631]: https://github.com/temper-lang/temper/issues/1631\n[pygments-lexer-docs]: https://pygments.org/docs/lexerdevelopment/\n"
+        "# Temper Pygments Lexer\n\n## Lexer class\n\nWe can't easily access backend classes, so we can't subclass\n`pygments.lexer.RegexLexer`, but we can define a separate class that can then\nbe subclassed in Python or elsewhere.\n\nTODO Maybe define an independent Lexer type and just create an instance here?\n\n    export class TemperLexer {\n\nThese indicators seems somewhat redundant to me, but they follow the examples in\nthe [Pygments documentation][pygments-lexer-docs].\n\n      public name: String = \"Temper\";\n      public aliases: List<String> = [\"temper\"];\n      public filenames: List<String> = [\"*.temper\"];\n\n### Token rules\n\nMain thing, though, is the list of rules for definition tokens.\n\n      public tokens: Map<String, List<RuleOption>> = new Map([\n\n#### Root\n\n        new Pair(\"root\", [\n          new Rule(raw\"\\s+\", Whitespace),\n          new Rule(\"//.*?$\", CommentSingleline),\n          new Rule(raw\"/\\*\", CommentMultiline, \"nestedcomment\"),\n          new Rule(\n            words(\"false\", \"NaN\", \"null\", \"true\", \"void\"),\n            KeywordConstant,\n          ),\n          new Rule(\n            words(\n              \"class\", \"interface\", \"let\", \"private\", \"public\", \"sealed\", \"var\",\n            ),\n            KeywordDeclaration,\n          ),\n          new Rule(\n            words(\n              \"do\", \"else\", \"export\", \"extends\", \"fn\", \"if\", \"import\", \"is\",\n              \"match\", \"new\", \"orelse\",\n            ),\n            Keyword,\n          ),\n          new Rule(\n            words(\n              \"AnyValue\", \"Boolean\", \"Float64\", \"Function\", \"Int\", \"List\",\n              \"ListBuilder\", \"Listed\", \"Map\", \"MapBuilder\", \"MapKey\", \"Mapped\",\n              \"NoResult\", \"Null\", \"String\", \"StringSlice\", \"Void\",\n            ),\n            NameBuiltin,\n          ),\n          new Rule(\"\\\"\", StringKind, \"string\"),\n          new Rule(\"[-=+*&|<>]+|/=?\", Operator),\n          new Rule(\"[{}();:.,]\", Punctuation),\n          new Rule(raw\"\\d+\\.?\\d*|\\.\\d+\", Number),\n          new Rule(\"@${nameRegex}\", NameDecorator),\n          new Rule(nameRegex, Name),\n        ].as<List<RuleOption>>()),\n\n#### Multiline/Nested Comments\n\nWe plan to support nested comments soon, so just implement that already here.\nThe technique here is based on the `nestedcomment` for the [D Language lexer for\nPygments][dlang-nestedcomment].\n\n        new Pair(\"nestedcomment\", [\n          new Rule(raw\"[^*/]+\", CommentMultiline),\n          new Rule(raw\"/\\*\", CommentMultiline, \"#push\"),\n          new Rule(raw\"\\*/\", CommentMultiline, \"#pop\"),\n          new Rule(raw\"[*/]\", CommentMultiline),\n        ].as<List<RuleOption>>()),\n\n#### Strings\n\n        new Pair(\"interpolation\", [\n          new Rule(\"}\", StringInterpol, \"#pop\"),\n          include(\"root\"),\n        ].as<List<RuleOption>>()),\n\nI'm not sure if order matters here. Seems simpler, but if I don't exclude `${`\nfrom core string chars, I don't get interp.\n\n        new Pair(\"string\", [\n          new Rule(\"\\\"\", StringKind, \"#pop\"),\n          new Rule(raw\"\\$\\{\", StringInterpol, \"interpolation\"),\n          new Rule(\"(?:[^\\\"$]|\\\\$[^{])+\", StringKind),\n        ].as<List<RuleOption>>()),\n\n      ]);\n\n    }\n\n## Helper functions and values\n\nBe sloppy with names for now. TODO More complete Unicode support.\n\n    let nameRegex = \"[_<<Lu>><<Ll>>][_<<Lu>><<Ll>>0-9]*\";\n\n    let words(...names: List<String>): String {\n      \"\\\\b(?:${names.join(\"|\") { (x);; x }})\\\\b\"\n    }\n\n## Imports and links\n\n    let { ... } = import(\"./pygments\");\n\n[dlang-nestedcomment]: https://github.com/pygments/pygments/blob/d0acfff1121f9ee3696b01a9077ebe9990216634/pygments/lexers/d.py#L242\n[issue1631]: https://github.com/temper-lang/temper/issues/1631\n[pygments-lexer-docs]: https://pygments.org/docs/lexerdevelopment/\n"
     ],
     "version": 3
 }
```

### Comparing `temper_syntax-0.1.0/temper_syntax/tempermd_pygments.py` & `temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py`

 * *Files identical despite different names*

### Comparing `temper_syntax-0.1.0/temper_syntax/tempermd_pygments.py.map` & `temper_syntax-0.1.1/temper_syntax/tempermd_pygments.py.map`

 * *Files identical despite different names*

### Comparing `temper_syntax-0.1.0/temper_syntax/tempermd_pygments__preface.py.map` & `temper_syntax-0.1.1/temper_syntax/tempermd_pygments__preface.py.map`

 * *Files identical despite different names*

