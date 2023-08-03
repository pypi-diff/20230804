# Comparing `tmp/rule-engine-4.0.1.tar.gz` & `tmp/rule-engine-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rule-engine-4.0.1.tar", last modified: Sun Jul 30 03:02:41 2023, max compression
+gzip compressed data, was "rule-engine-4.1.0.tar", last modified: Thu Aug  3 23:18:51 2023, max compression
```

## Comparing `rule-engine-4.0.1.tar` & `rule-engine-4.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.735775 rule-engine-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-07-30 03:02:01.000000 rule-engine-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-30 03:02:41.735775 rule-engine-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-07-30 03:02:01.000000 rule-engine-4.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.727774 rule-engine-4.0.1/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.731774 rule-engine-4.0.1/lib/rule_engine/
--rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    52714 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     8339 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/builtins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/debug_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/debug_repl.py
--rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/engine.py
--rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/suggestions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21819 2023-07-30 03:02:01.000000 rule-engine-4.0.1/lib/rule_engine/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-30 03:02:41.735775 rule-engine-4.0.1/lib/rule_engine.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-07-30 03:02:41.000000 rule-engine-4.0.1/lib/rule_engine.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-07-30 03:02:41.735775 rule-engine-4.0.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-07-30 03:02:01.000000 rule-engine-4.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:18:51.275212 rule-engine-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-08-03 23:18:14.000000 rule-engine-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-08-03 23:18:51.275212 rule-engine-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-08-03 23:18:14.000000 rule-engine-4.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:18:51.271212 rule-engine-4.1.0/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:18:51.275212 rule-engine-4.1.0/lib/rule_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)     1989 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52628 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8465 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/builtins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2512 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/debug_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/debug_repl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23588 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11982 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18616 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3654 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/suggestions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22572 2023-08-03 23:18:14.000000 rule-engine-4.1.0/lib/rule_engine/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-03 23:18:51.275212 rule-engine-4.1.0/lib/rule_engine.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5233 2023-08-03 23:18:51.000000 rule-engine-4.1.0/lib/rule_engine.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-08-03 23:18:51.000000 rule-engine-4.1.0/lib/rule_engine.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-03 23:18:51.000000 rule-engine-4.1.0/lib/rule_engine.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-08-03 23:18:51.000000 rule-engine-4.1.0/lib/rule_engine.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-03 23:18:51.000000 rule-engine-4.1.0/lib/rule_engine.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-03 23:18:51.275212 rule-engine-4.1.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3778 2023-08-03 23:18:14.000000 rule-engine-4.1.0/setup.py
```

### Comparing `rule-engine-4.0.1/LICENSE` & `rule-engine-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/PKG-INFO` & `rule-engine-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.0.1
+Version: 4.1.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.0.1/README.rst` & `rule-engine-4.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/__init__.py` & `rule-engine-4.1.0/lib/rule_engine/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 #  LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE,
 #  DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY
 #  THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
 #  (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
 #  OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 #
 
-__version__ = '4.0.1'
+__version__ = '4.1.0'
 
 from .engine import resolve_attribute
 from .engine import resolve_item
 from .engine import type_resolver_from_dict
 from .engine import Context
 from .engine import Rule
```

### Comparing `rule-engine-4.0.1/lib/rule_engine/_utils.py` & `rule-engine-4.1.0/lib/rule_engine/_utils.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/ast.py` & `rule-engine-4.1.0/lib/rule_engine/ast.py`

 * *Files 1% similar despite different names*

```diff
@@ -1077,17 +1077,15 @@
 		if function_type.argument_types is not DataType.UNDEFINED:
 			if len(arguments) > len(function_type.argument_types):
 				raise errors.FunctionCallError(
 					"expected at most {} positional arguments".format(len(function_type.argument_types)),
 					function_name=function_type.value_name
 				)
 			for pos, (arg1, arg2_type) in enumerate(zip(arguments, function_type.argument_types), 1):
-				if isinstance(arg1, LiteralExpressionBase):
-					arg1_type = arg1.result_type
-				elif isinstance(arg1, SymbolExpression):
+				if isinstance(arg1, ExpressionBase):
 					arg1_type = arg1.result_type
 				else:
 					arg1_type = DataType.from_value(arg1)
 				if not DataType.is_compatible(arg1_type, arg2_type):
 					raise errors.FunctionCallError(
 						"data type mismatch (argument #{})".format(pos),
 						function_name=function_type.value_name
```

### Comparing `rule-engine-4.0.1/lib/rule_engine/builtins.py` & `rule-engine-4.1.0/lib/rule_engine/builtins.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 		raise errors.FunctionCallError('argument #3 (maxsplit) must be a natural number')
 	return tuple(string.split(sep=sep, maxsplit=maxsplit))
 
 class BuiltinValueGenerator(object):
 	"""
 	A class used as a wrapper for builtin values to differentiate between a value that is a function and a value that
 	should be generated by calling a function. A value that is generated by calling a function is useful for determining
-	the value during evaluation for things like the curren time.
+	the value during evaluation for things like the current time.
 
 	.. versionadded:: 4.0.0
 	"""
 	__slots__ = ('callable',)
 	def __init__(self, callable):
 		self.callable = callable
 
@@ -149,14 +149,15 @@
 			# mathematical constants
 			'e': decimal.Decimal(repr(math.e)),
 			'pi': decimal.Decimal(repr(math.pi)),
 			# timestamps
 			'now': now,
 			'today': BuiltinValueGenerator(lambda builtins: now(builtins).replace(hour=0, minute=0, second=0, microsecond=0)),
 			# functions
+			'abs': abs,
 			'any': any,
 			'all': all,
 			'sum': sum,
 			'map': _builtin_map,
 			'max': max,
 			'min': min,
 			'filter': _builtin_filter,
@@ -171,14 +172,15 @@
 			# mathematical constants
 			'e': ast.DataType.FLOAT,
 			'pi': ast.DataType.FLOAT,
 			# timestamps
 			'now': ast.DataType.DATETIME,
 			'today': ast.DataType.DATETIME,
 			# functions
+			'abs': ast.DataType.FUNCTION('abs', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.FLOAT,)),
 			'all': ast.DataType.FUNCTION('all', return_type=ast.DataType.BOOLEAN, argument_types=(ast.DataType.ARRAY,)),
 			'any': ast.DataType.FUNCTION('any', return_type=ast.DataType.BOOLEAN, argument_types=(ast.DataType.ARRAY,)),
 			'sum': ast.DataType.FUNCTION('sum', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.ARRAY(ast.DataType.FLOAT),)),
 			'map': ast.DataType.FUNCTION('map', return_type=ast.DataType.ARRAY, argument_types=(ast.DataType.FUNCTION, ast.DataType.ARRAY)),
 			'max': ast.DataType.FUNCTION('max', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.ARRAY(ast.DataType.FLOAT),)),
 			'min': ast.DataType.FUNCTION('min', return_type=ast.DataType.FLOAT, argument_types=(ast.DataType.ARRAY(ast.DataType.FLOAT),)),
 			'filter': ast.DataType.FUNCTION('filter', return_type=ast.DataType.ARRAY, argument_types=(ast.DataType.FUNCTION, ast.DataType.ARRAY)),
```

### Comparing `rule-engine-4.0.1/lib/rule_engine/debug_ast.py` & `rule-engine-4.1.0/lib/rule_engine/debug_ast.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/debug_repl.py` & `rule-engine-4.1.0/lib/rule_engine/debug_repl.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/engine.py` & `rule-engine-4.1.0/lib/rule_engine/engine.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/errors.py` & `rule-engine-4.1.0/lib/rule_engine/errors.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/parser.py` & `rule-engine-4.1.0/lib/rule_engine/parser.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/suggestions.py` & `rule-engine-4.1.0/lib/rule_engine/suggestions.py`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/lib/rule_engine/types.py` & `rule-engine-4.1.0/lib/rule_engine/types.py`

 * *Files 8% similar despite different names*

```diff
@@ -463,23 +463,26 @@
 		if not isinstance(dt, _DataTypeDef):
 			raise ValueError("can not map name {0!r} to a compatible data type".format(name))
 		return dt
 
 	@classmethod
 	def from_type(cls, python_type):
 		"""
-		Get the supported data type constant for the specified Python type. If the type can not be mapped to a supported
-		data type, then a :py:exc:`ValueError` exception will be raised. This function will not return
-		:py:attr:`.UNDEFINED`.
+		Get the supported data type constant for the specified Python type/type hint. If the type or typehint can not be
+		mapped to a supported data type, then a :py:exc:`ValueError` exception will be raised. This function will not
+		return :py:attr:`.UNDEFINED`.
 
-		:param type python_type: The native Python type to retrieve the corresponding type constant for.
+		:param type python_type: The native Python type or type hint to retrieve the corresponding type constant for.
 		:return: One of the constants.
+
+		.. versionchanged:: 4.1.0
+			Added support for typehints.
 		"""
-		if not isinstance(python_type, type):
-			raise TypeError('from_type argument 1 must be type, not ' + type(python_type).__name__)
+		if not (isinstance(python_type, type) or hasattr(python_type, '__origin__')):
+			raise TypeError('from_type argument 1 must be a type or a type hint, not ' + type(python_type).__name__)
 		if python_type in (list, range, tuple):
 			return cls.ARRAY
 		elif python_type is bool:
 			return cls.BOOLEAN
 		elif python_type is datetime.date or python_type is datetime.datetime:
 			return cls.DATETIME
 		elif python_type is datetime.timedelta:
@@ -492,14 +495,27 @@
 			return cls.NULL
 		elif python_type is set:
 			return cls.SET
 		elif python_type is str:
 			return cls.STRING
 		elif python_type is _PYTHON_FUNCTION_TYPE:
 			return cls.FUNCTION
+		elif hasattr(python_type, "__origin__"):
+			origin_python_type = python_type.__origin__
+			maintype = cls.from_type(origin_python_type)
+			if origin_python_type in (list, tuple, set):
+				if hasattr(python_type, "__args__") and origin_python_type is not tuple:
+					valuetype = cls.from_type(python_type.__args__[0])
+					return maintype(valuetype)
+			if origin_python_type is dict:
+				if hasattr(python_type, "__args__"):
+					key_type = cls.from_type(python_type.__args__[0])
+					value_type = cls.from_type(python_type.__args__[1])
+					return maintype(key_type, value_type)
+			return maintype
 		raise ValueError("can not map python type {0!r} to a compatible data type".format(python_type.__name__))
 
 	@classmethod
 	def from_value(cls, python_value):
 		"""
 		Get the supported data type constant for the specified Python value. If the value can not be mapped to a
 		supported data type, then a :py:exc:`TypeError` exception will be raised. This function will not return
```

### Comparing `rule-engine-4.0.1/lib/rule_engine.egg-info/PKG-INFO` & `rule-engine-4.1.0/lib/rule_engine.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rule-engine
-Version: 4.0.1
+Version: 4.1.0
 Summary: A lightweight, optionally typed expression language with a custom grammar for matching arbitrary Python objects.
 Home-page: https://github.com/zeroSteiner/rule-engine
 Author: Spencer McIntyre
 Author-email: zeroSteiner@gmail.com
 Maintainer: Spencer McIntyre
 Maintainer-email: zeroSteiner@gmail.com
 License: BSD
```

### Comparing `rule-engine-4.0.1/lib/rule_engine.egg-info/SOURCES.txt` & `rule-engine-4.1.0/lib/rule_engine.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rule-engine-4.0.1/setup.py` & `rule-engine-4.1.0/setup.py`

 * *Files identical despite different names*

