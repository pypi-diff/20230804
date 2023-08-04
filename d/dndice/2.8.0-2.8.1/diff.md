# Comparing `tmp/dndice-2.8.0.tar.gz` & `tmp/dndice-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dndice-2.8.0.tar", last modified: Sun Mar  8 19:04:17 2020, max compression
+gzip compressed data, was "dndice-2.8.1.tar", max compression
```

## Comparing `dndice-2.8.0.tar` & `dndice-2.8.1.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    35147 2020-02-18 03:57:45.408891 dndice-2.8.0/LICENSE
--rw-r--r--   0        0        0     6846 2020-02-28 06:15:06.421300 dndice-2.8.0/README.md
--rw-r--r--   0        0        0      662 2020-02-21 20:52:45.234095 dndice-2.8.0/dndice/__init__.py
--rw-r--r--   0        0        0     7413 2020-02-21 20:52:45.250095 dndice-2.8.0/dndice/core.py
--rw-r--r--   0        0        0        0 2020-02-18 05:09:12.780578 dndice-2.8.0/dndice/lib/__init__.py
--rw-r--r--   0        0        0    16928 2020-03-08 18:18:08.534343 dndice-2.8.0/dndice/lib/evaltree.py
--rw-r--r--   0        0        0     2104 2020-02-18 05:09:12.780578 dndice-2.8.0/dndice/lib/exceptions.py
--rw-r--r--   0        0        0     2442 2020-02-18 05:09:12.780578 dndice-2.8.0/dndice/lib/helpers.py
--rw-r--r--   0        0        0    24111 2020-02-28 04:09:11.354374 dndice-2.8.0/dndice/lib/operators.py
--rw-r--r--   0        0        0    18022 2020-02-18 05:09:12.780578 dndice-2.8.0/dndice/lib/tokenizer.py
--rwxr-xr-x   0        0        0     2496 2020-02-21 20:52:45.270095 dndice-2.8.0/dndice/roller.py
--rw-r--r--   0        0        0      513 2020-03-08 18:23:40.786487 dndice-2.8.0/pyproject.toml
--rw-r--r--   0        0        0     7531 1970-01-01 00:00:00.000000 dndice-2.8.0/setup.py
--rw-r--r--   0        0        0      504 1970-01-01 00:00:00.000000 dndice-2.8.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2023-07-29 17:10:02.781679 dndice-2.8.1/LICENSE
+-rw-r--r--   0        0        0     6846 2023-07-29 17:10:02.781679 dndice-2.8.1/README.md
+-rw-r--r--   0        0        0      662 2023-07-29 17:10:02.781679 dndice-2.8.1/dndice/__init__.py
+-rw-r--r--   0        0        0     5756 2023-08-04 04:32:09.813419 dndice-2.8.1/dndice/core.py
+-rw-r--r--   0        0        0        0 2023-07-29 17:10:02.781679 dndice-2.8.1/dndice/lib/__init__.py
+-rw-r--r--   0        0        0    18158 2023-08-04 04:32:09.813419 dndice-2.8.1/dndice/lib/evaltree.py
+-rw-r--r--   0        0        0     2104 2023-07-29 17:10:02.781679 dndice-2.8.1/dndice/lib/exceptions.py
+-rw-r--r--   0        0        0     2442 2023-07-29 17:10:02.781679 dndice-2.8.1/dndice/lib/helpers.py
+-rw-r--r--   0        0        0    24111 2023-07-29 17:10:02.781679 dndice-2.8.1/dndice/lib/operators.py
+-rw-r--r--   0        0        0    18043 2023-08-04 04:32:09.813419 dndice-2.8.1/dndice/lib/tokenizer.py
+-rwxr-xr-x   0        0        0     2496 2023-07-29 17:10:02.782678 dndice-2.8.1/dndice/roller.py
+-rw-r--r--   0        0        0      567 2023-08-04 05:39:38.065922 dndice-2.8.1/pyproject.toml
+-rw-r--r--   0        0        0     7604 1970-01-01 00:00:00.000000 dndice-2.8.1/PKG-INFO
```

### Comparing `dndice-2.8.0/LICENSE` & `dndice-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/README.md` & `dndice-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/dndice/__init__.py` & `dndice-2.8.1/dndice/__init__.py`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/dndice/core.py` & `dndice-2.8.1/dndice/core.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,14 @@
 import enum
 import typing
 
-if __name__ == '__main__':
-    # script version
-    from dndice.lib.exceptions import InputTypeError
-    from dndice.lib.operators import OPERATORS
-    from dndice.lib.tokenizer import Token
-    from dndice.lib.evaltree import EvalTree, EvalTreeNode
-else:
-    # module version
-    from .lib.exceptions import InputTypeError
-    from .lib.operators import OPERATORS
-    from .lib.tokenizer import tokens_lazy, Token
-    from .lib.evaltree import EvalTree, EvalTreeNode
+from .lib.evaltree import EvalTree, EvalTreeNode
+from .lib.exceptions import InputTypeError
+from .lib.operators import OPERATORS
+from .lib.tokenizer import Token, tokens_lazy
 
 
 class Mode(enum.Enum):
     """Change the way that a roll is performed.
 
     Average makes each die give back the average value, which ends up
     with halves for the normal even-sided dice. Critical causes a roll
@@ -162,62 +154,7 @@
     yield from tokens_lazy(expr)
     if modifiers != 0:
         yield ')'
         yield OPERATORS['+']
         yield modifiers
 
 
-if __name__ == '__main__':
-    testCases = [
-        "1d4+1",
-        "1d4-1",
-        "2d20h1",
-        "2d20l1",
-        "40d20r1h1",
-        "10d4r1",
-        "10d4R1",
-        "1d4d4d4",
-        "-5",
-        "+1d4",
-        "2*-1d4",
-        "-2^1d4",
-        "8d6/2",
-        "1+(1+4)d6",
-        "(1d6)!",
-        "1d6!",
-        "1d100<14",
-        "1d100<=18",
-        "8d6f2",
-        "1d20+5>10",
-        "5d20r<15",
-        "5d20R<15",
-        "(1d4-1)&(1d3-2>0)",
-        "(1d4-1)|(1d3-2>0)",
-        "1dc8+1dc4+3",
-        "1dm6+1d6",
-        "2d4c2",
-        "2da6",
-        "3da6",
-        "2d10%2",
-        "1d4=4|1d4=3",
-        "1d8>=6",
-        "10d8r>4",
-        "10d8R>4",
-        "10d[3,3,3,5]",
-        "10d[3, 3, 3, 5]",
-        "15d6t5",
-        "15d6T1",
-    ]
-    for expr in testCases:
-        tree = EvalTree(expr)
-        print('EVALUATING ' + expr)
-        print('EVALUATING USING TREE DIRECTLY')
-        print(tree.evaluate())
-        print('EVALUATING USING ROLL FUNCTION')
-        print(basic(expr))
-        print('EVALUATING USING ROLL FUNCTION IN VERBOSE MODE')
-        print(verbose(expr))
-        print('EVALUATING USING ROLL FUNCTION AND MODIFIER')
-        print(basic(expr, modifiers=3))
-        print('EVALUATING USING ROLL FUNCTION IN VERBOSE MODE AND MODIFIER')
-        print(verbose(expr, modifiers=3))
-        print()
```

### Comparing `dndice-2.8.0/dndice/lib/evaltree.py` & `dndice-2.8.1/dndice/lib/evaltree.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,14 +38,37 @@
             operand or expression to the right of this operator.
         """
         self.payload = payload  # type: Token
         self.left = left  # type: EvalTreeNode
         self.right = right  # type: EvalTreeNode
         self.value = None  # type: typing.Optional[Result]
 
+    def __repr__(self):
+        """Produce a string that could be used to reconstruct this node."""
+        def recursive(current: EvalTreeNode, depth: int) -> str:
+            if current is None:
+                return repr(current)
+            if current.is_leaf():
+                return 'EvalTreeNode({}, {}, {})'.format(current.payload,
+                                                         current.left,
+                                                         current.right)
+            return ('EvalTreeNode({payload},\n'
+                    '{indent}{left},\n'
+                    '{indent}{right}\n'
+                    '{short})').format(
+                payload=current.payload,
+                left=recursive(current.left, depth + 1),
+                right=recursive(current.right, depth + 1),
+                indent=' ' * len('EvalTreeNode(') * depth,
+                short=' ' * (len('EvalTreeNode(') * depth - 1),
+                align=' ' * len('EvalTreeNode(')
+            )
+
+        return recursive(self, 1)
+
     def evaluate(self) -> Result:
         """Recursively evaluate this subtree and return its computed value.
 
         As a side effect, it also annotates this node with the value. At
         the EvalTree level, this can be used to compose a more detailed
         report of the dice rolls.
 
@@ -167,14 +190,18 @@
         :param other: The EvalTree to join with this one.
         :raises NotImplementedError: If anything but an EvalTree is passed in.
         """
         if isinstance(other, EvalTree):
             return self.__in_place_concat(OPERATORS['-'], other)
         raise InputTypeError('Cannot subtract a {} from an EvalTree.'.format(type(other)))
 
+    def __repr__(self):
+        """Produce a string that can be used to reconstruct this tree."""
+        return 'EvalTree("{}")'.format(''.join(str(node.payload) for node in self.in_order()))
+
     def __concat(self, operation: Operator, other: 'EvalTree') -> 'EvalTree':
         new = self.copy()
         new.root = EvalTreeNode(operation, new.root, other.copy().root)
         return new
 
     def __in_place_concat(self, operation: Operator, other: 'EvalTree') -> 'EvalTree':
         self.root = EvalTreeNode(operation, self.root, other.root)
@@ -217,15 +244,15 @@
         final = self.root.evaluate()
         try:
             return sum(final)
         except TypeError:
             return final
 
     @wrap_exceptions_with(ParseError, 'Failed to construct an expression from the token list.')
-    def __from_tokens(self, tokens: typing.List[Token]) -> None:
+    def __from_tokens(self, tokens: typing.Sequence[Token]) -> None:
         """Construct the expression tree formed from the infix token list.
 
         This uses a `shunting-yard algorithm
         <https://en.wikipedia.org/wiki/Shunting-yard_algorithm>`_ to parse the infix token
         list into an expression tree. In relation to that algorithm, the "output" stack is
         populated with with subtrees that are progressively joined together using operators
         to create the final full tree.
```

### Comparing `dndice-2.8.0/dndice/lib/exceptions.py` & `dndice-2.8.1/dndice/lib/exceptions.py`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/dndice/lib/helpers.py` & `dndice-2.8.1/dndice/lib/helpers.py`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/dndice/lib/operators.py` & `dndice-2.8.1/dndice/lib/operators.py`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/dndice/lib/tokenizer.py` & `dndice-2.8.1/dndice/lib/tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         """Returns the correct unary operator.
 
         These are special cases to avoid ambiguity in the definitions.
         """
         token = agg[0]
         if token == '+':
             return OPERATORS['p']
-        if token == '-':
+        if token == '-':  # pragma: no branch
             return OPERATORS['m']
 
 
 class UnarySuffix(Operator):
     """A unary suffix operator.
 
     The only one that exists now is the factorial, !.
```

### Comparing `dndice-2.8.0/dndice/roller.py` & `dndice-2.8.1/dndice/roller.py`

 * *Files identical despite different names*

### Comparing `dndice-2.8.0/pyproject.toml` & `dndice-2.8.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 [tool.poetry]
 name = "dndice"
-version = "2.8.0"
+version = "2.8.1"
 description = "An engine to parse and evaluate D&D-inspired roll expressions"
 authors = ["Nick Thurmes <nthurmes@gmail.com>"]
 license = "GPL-2.0-or-later"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.5"
 
-[tool.poetry.dev-dependencies]
-nose2 = "^0.9.1"
+[tool.poetry.scripts]
+roll = "dndice:roller.main"
+
+[tool.poetry.group.dev.dependencies]
 sphinx = "^2.1"
 sphinx-rtd-theme = "^0.4.3"
 coveralls = "^1.11"
-
-[tool.poetry.scripts]
-roll = "dndice:roller.main"
+pylint = "^2.5"
+lz4 = "^3.1.3"
+coverage = "^5.5"
+pytest = "^6.0"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `dndice-2.8.0/setup.py` & `dndice-2.8.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,28 +1,86 @@
-# -*- coding: utf-8 -*-
-from distutils.core import setup
+Metadata-Version: 2.1
+Name: dndice
+Version: 2.8.1
+Summary: An engine to parse and evaluate D&D-inspired roll expressions
+License: GPL-2.0-or-later
+Author: Nick Thurmes
+Author-email: nthurmes@gmail.com
+Requires-Python: >=3.5,<4.0
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.5
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Description-Content-Type: text/markdown
+
+# DnDice
+
+[![PyPI version](https://badge.fury.io/py/dndice.svg)](https://badge.fury.io/py/dndice)
+[![Documentation Status](https://readthedocs.org/projects/rolling/badge/?version=latest)](https://rolling.readthedocs.io/en/latest/?badge=latest)
+[![Coverage Status](https://coveralls.io/repos/github/the-nick-of-time/dndice/badge.svg?branch=master)](https://coveralls.io/github/the-nick-of-time/dndice?branch=master)
+[![Build Status](https://travis-ci.org/the-nick-of-time/dndice.svg?branch=master)](https://travis-ci.org/the-nick-of-time/dndice)
+
+This package deals with roll expressions, which are inspired by the syntax D&D uses.
+At the most basic, there are expressions like `1d20` which means "roll one 20-sided die".
+D&D stops around when modifiers are added, like `1d6+2`.
+This package runs with it and introduces these dice expressions to an entire arithmetic framework.
+You can add, subtract, multiply, even exponentiate rolls together, not to mention all of the roll-specific operations like taking the highest or lowest rolls or rerolling given a condition.
+As these are mathematical expressions just like normal ones, note that they can get arbitrarily complicated.
+The only limit is how much resources Python can bring to bear calculating your `(9^9^9^9^9)d10000` or similar ridiculous expression.  
+
+The full specification of what operators are supported and what they do is below.
+
+| Operator | Format          | Meaning
+| :------- | :-------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------
+| !        | *x*__!__        | Calculate the factorial of _x_.
+| d        | *x*__d__*y*     | Take a _y_-sided die and roll _x_ of them. _y_ can be an integer, and works just as you would expect. It can also be a list of arbitrary numbers (delineated by `[]` and separated with commas), in which case it works as a die with one side labeled with each number in the list.
+| da       | *x*__da__*y*    | Take a _y_-sided die and return the average as if _x_ of them had been rolled. This returns an unrounded number.
+| dc       | *x*__dc__*y*    | Roll a critical hit, where the number of dice rolled is doubled.
+| dm       | *x*__dm__*y*    | Roll the maximum on every die rolled.
+| h        | *ROLL*__h__*n*  | After making a roll, discard all but the highest _n_ of the rolls. Hint: 2d20h1 is advantage.
+| l        | *ROLL*__l__*n*  | After making a roll, discard all but the lowest _n_ of the rolls. Hint: 2d20l1 is disadvantage.
+| f        | *ROLL*__f__*n*  | After making a roll, treat any value that is less than _n_ as _n_.
+| c        | *ROLL*__c__*n*  | After making a roll, treat any value that is greater than _n_ as _n_.
+| r or ro  | *ROLL*__ro__*n* | After making a roll, look at all of them and reroll any that are equal to _n_, reroll those, and take the result.
+| R or Ro  | *ROLL*__Ro__*n* | After making a roll, look at all of them and reroll any that are equal to _n_ and reroll those. If that number comes up again, continue rerolling until you get something different.
+| r> or rh | *ROLL*__rh__*n* | After making a roll, look at all of them and reroll any that are strictly greater than _n_, reroll those, and take the result.
+| R> or Rh | *ROLL*__Rh__*n* | After making a roll, look at all of them and reroll any that are greater than _n_ and reroll those. If a number greater than _n_ comes up again, continue rerolling until you get something different.
+| r< or rl | *ROLL*__rl__*n* | After making a roll, look at all of them and reroll any that are strictly less than _n_, reroll those, and take the result.
+| R< or Rl | *ROLL*__Rl__*n* | After making a roll, look at all of them and reroll any that are less than _n_ and reroll those. If a number less than _n_ comes up again, continue rerolling until you get something different.
+| t        | *ROLL*__t__*n*  | After making the roll, count the number of rolls that were at least _n_.
+| T        | *ROLL*__T__*n*  | After making the roll, count the number of rolls that were at most _n_.
+| ^        | *x*__^__*y*     | Raise _x_ to the _y_ power. This operation is right-associative, meaning that the right side of the expression is evaluated before the left. This really only comes up when chained, for example in `2^3^2`. This would not be `(2^3)^2=8^2=64`, but rather `2^(3^2)=2^9=512`.
+| *        | *x*__*__*y*     | _x_ times _y_.
+| /        | *x*__/__*y*     | _x_ divided by _y_. This returns an unrounded number.
+| %        | *x*__%__*y*     | _x_ modulo _y_. That is, the remainder after _x_ is divided by _y_.
+| +        | *x*__+__*y*     | _x_ plus _y_.
+| -        | *x*__-__*y*     | _x_ minus _y_.
+| > or gt  | *x*__>__*y*     | Check if _x_ is greater than _y_. Returns a 1 for yes and 0 for no.
+| >= or ge | *x*__>=__*y*    | Check if _x_ is greater than or equal to _y_. Returns a 1 for yes and 0 for no.
+| < or lt  | *x*__<__*y*     | Check if _x_ is less than _y_. Returns a 1 for yes and 0 for no.
+| <= or le | *x*__<=__*y*    | Check if _x_ is less than or equal to _y_. Returns a 1 for yes and 0 for no.
+| =        | *x*__=__*y*     | Check if _x_ is equal to _y_. Returns a 1 for yes and 0 for no.
+| &        | *x*__&__*y*     | Check if _x_ and _y_ are both nonzero.
+| \|       | *x*__\|__*y*    | Check if at least one of _x_ or _y_ is nonzero.
+
+
+
+## Using this package
+
+### As a user or player
+
+Installing this package from PyPI will also install the script `roll` to your path. This is a simple command-line script that allows you to exercise all the powers of this package.
+For a GUI that does the same, check out my repository [DnD](https://github.com/the-nick-of-time/DnD) which is a larger project focused around D&D 5e, allowing you to track your characters and monsters.
 
-packages = \
-['dndice', 'dndice.lib']
 
-package_data = \
-{'': ['*']}
+### As a developer
 
-entry_points = \
-{'console_scripts': ['roll = dndice:roller.main']}
-
-setup_kwargs = {
-    'name': 'dndice',
-    'version': '2.8.0',
-    'description': 'An engine to parse and evaluate D&D-inspired roll expressions',
-    'long_description': '# DnDice\n\n[![PyPI version](https://badge.fury.io/py/dndice.svg)](https://badge.fury.io/py/dndice)\n[![Documentation Status](https://readthedocs.org/projects/rolling/badge/?version=latest)](https://rolling.readthedocs.io/en/latest/?badge=latest)\n[![Coverage Status](https://coveralls.io/repos/github/the-nick-of-time/dndice/badge.svg?branch=master)](https://coveralls.io/github/the-nick-of-time/dndice?branch=master)\n[![Build Status](https://travis-ci.org/the-nick-of-time/dndice.svg?branch=master)](https://travis-ci.org/the-nick-of-time/dndice)\n\nThis package deals with roll expressions, which are inspired by the syntax D&D uses.\nAt the most basic, there are expressions like `1d20` which means "roll one 20-sided die".\nD&D stops around when modifiers are added, like `1d6+2`.\nThis package runs with it and introduces these dice expressions to an entire arithmetic framework.\nYou can add, subtract, multiply, even exponentiate rolls together, not to mention all of the roll-specific operations like taking the highest or lowest rolls or rerolling given a condition.\nAs these are mathematical expressions just like normal ones, note that they can get arbitrarily complicated.\nThe only limit is how much resources Python can bring to bear calculating your `(9^9^9^9^9)d10000` or similar ridiculous expression.  \n\nThe full specification of what operators are supported and what they do is below.\n\n| Operator | Format          | Meaning\n| :------- | :-------------- | :------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------\n| !        | *x*__!__        | Calculate the factorial of _x_.\n| d        | *x*__d__*y*     | Take a _y_-sided die and roll _x_ of them. _y_ can be an integer, and works just as you would expect. It can also be a list of arbitrary numbers (delineated by `[]` and separated with commas), in which case it works as a die with one side labeled with each number in the list.\n| da       | *x*__da__*y*    | Take a _y_-sided die and return the average as if _x_ of them had been rolled. This returns an unrounded number.\n| dc       | *x*__dc__*y*    | Roll a critical hit, where the number of dice rolled is doubled.\n| dm       | *x*__dm__*y*    | Roll the maximum on every die rolled.\n| h        | *ROLL*__h__*n*  | After making a roll, discard all but the highest _n_ of the rolls. Hint: 2d20h1 is advantage.\n| l        | *ROLL*__l__*n*  | After making a roll, discard all but the lowest _n_ of the rolls. Hint: 2d20l1 is disadvantage.\n| f        | *ROLL*__f__*n*  | After making a roll, treat any value that is less than _n_ as _n_.\n| c        | *ROLL*__c__*n*  | After making a roll, treat any value that is greater than _n_ as _n_.\n| r or ro  | *ROLL*__ro__*n* | After making a roll, look at all of them and reroll any that are equal to _n_, reroll those, and take the result.\n| R or Ro  | *ROLL*__Ro__*n* | After making a roll, look at all of them and reroll any that are equal to _n_ and reroll those. If that number comes up again, continue rerolling until you get something different.\n| r> or rh | *ROLL*__rh__*n* | After making a roll, look at all of them and reroll any that are strictly greater than _n_, reroll those, and take the result.\n| R> or Rh | *ROLL*__Rh__*n* | After making a roll, look at all of them and reroll any that are greater than _n_ and reroll those. If a number greater than _n_ comes up again, continue rerolling until you get something different.\n| r< or rl | *ROLL*__rl__*n* | After making a roll, look at all of them and reroll any that are strictly less than _n_, reroll those, and take the result.\n| R< or Rl | *ROLL*__Rl__*n* | After making a roll, look at all of them and reroll any that are less than _n_ and reroll those. If a number less than _n_ comes up again, continue rerolling until you get something different.\n| t        | *ROLL*__t__*n*  | After making the roll, count the number of rolls that were at least _n_.\n| T        | *ROLL*__T__*n*  | After making the roll, count the number of rolls that were at most _n_.\n| ^        | *x*__^__*y*     | Raise _x_ to the _y_ power. This operation is right-associative, meaning that the right side of the expression is evaluated before the left. This really only comes up when chained, for example in `2^3^2`. This would not be `(2^3)^2=8^2=64`, but rather `2^(3^2)=2^9=512`.\n| *        | *x*__*__*y*     | _x_ times _y_.\n| /        | *x*__/__*y*     | _x_ divided by _y_. This returns an unrounded number.\n| %        | *x*__%__*y*     | _x_ modulo _y_. That is, the remainder after _x_ is divided by _y_.\n| +        | *x*__+__*y*     | _x_ plus _y_.\n| -        | *x*__-__*y*     | _x_ minus _y_.\n| > or gt  | *x*__>__*y*     | Check if _x_ is greater than _y_. Returns a 1 for yes and 0 for no.\n| >= or ge | *x*__>=__*y*    | Check if _x_ is greater than or equal to _y_. Returns a 1 for yes and 0 for no.\n| < or lt  | *x*__<__*y*     | Check if _x_ is less than _y_. Returns a 1 for yes and 0 for no.\n| <= or le | *x*__<=__*y*    | Check if _x_ is less than or equal to _y_. Returns a 1 for yes and 0 for no.\n| =        | *x*__=__*y*     | Check if _x_ is equal to _y_. Returns a 1 for yes and 0 for no.\n| &        | *x*__&__*y*     | Check if _x_ and _y_ are both nonzero.\n| \\|       | *x*__\\|__*y*    | Check if at least one of _x_ or _y_ is nonzero.\n\n\n\n## Using this package\n\n### As a user or player\n\nInstalling this package from PyPI will also install the script `roll` to your path. This is a simple command-line script that allows you to exercise all the powers of this package.\nFor a GUI that does the same, check out my repository [DnD](https://github.com/the-nick-of-time/DnD) which is a larger project focused around D&D 5e, allowing you to track your characters and monsters.\n\n\n### As a developer\n\nIf you just want to use this in an application, install it through PyPI and import it as `dndice`. The main function you want is `basic`, which will simply evaluate an expression and return the final number. `verbose` is useful for giving a more detailed look at what was actually rolled, targeted at direct display to a user. `compile` can be used to precompile expressions for quick evaluation of the same expression many times. For a complete view, see [the docs](https://rolling.readthedocs.io/en/latest/).\n\nTo modify this package, first install [poetry](https://github.com/sdispater/poetry) for dependency management. There are no runtime dependencies, and the only development dependencies are [sphinx](http://www.sphinx-doc.org/en/master/) for documentation and [nose2](https://nose2.readthedocs.io/en/latest/index.html) for testing.\nYou probably also want GNU make because I have a number of tasks scripted in the Makefile at the project root.\n',
-    'author': 'Nick Thurmes',
-    'author_email': 'nthurmes@gmail.com',
-    'url': None,
-    'packages': packages,
-    'package_data': package_data,
-    'entry_points': entry_points,
-    'python_requires': '>=3.5,<4.0',
-}
+If you just want to use this in an application, install it through PyPI and import it as `dndice`. The main function you want is `basic`, which will simply evaluate an expression and return the final number. `verbose` is useful for giving a more detailed look at what was actually rolled, targeted at direct display to a user. `compile` can be used to precompile expressions for quick evaluation of the same expression many times. For a complete view, see [the docs](https://rolling.readthedocs.io/en/latest/).
 
+To modify this package, first install [poetry](https://github.com/sdispater/poetry) for dependency management. There are no runtime dependencies, and the only development dependencies are [sphinx](http://www.sphinx-doc.org/en/master/) for documentation and [nose2](https://nose2.readthedocs.io/en/latest/index.html) for testing.
+You probably also want GNU make because I have a number of tasks scripted in the Makefile at the project root.
 
-setup(**setup_kwargs)
```

