# Comparing `tmp/docleaf-0.8.2-cp39-none-win_amd64.whl.zip` & `tmp/docleaf-0.8.3-cp37-cp37m-macosx_10_7_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 1105906 bytes, number of entries: 11
--rw-r--r--  4.6 unx     6858 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/METADATA
--rw-r--r--  4.6 unx       96 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/WHEEL
--rw-r--r--  4.6 unx     3573 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/license_files/LICENSE.md
--rw-r--r--  4.6 unx   140320 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/license_files/LICENSES_THIRD_PARTY.md
--rw-r--r--  4.6 unx     5512 b- defN 23-Jul-13 15:02 docleaf/copied.py
--rw-r--r--  4.6 unx     3659 b- defN 23-Jul-13 15:02 docleaf/domains.py
--rw-r--r--  4.6 unx    17506 b- defN 23-Jul-13 15:02 docleaf/doxygen.py
--rw-r--r--  4.6 unx       99 b- defN 23-Jul-13 15:02 docleaf/errors.py
--rw-r--r--  4.6 unx        0 b- defN 23-Jul-13 15:02 docleaf/__init__.py
--rwxr-xr-x  4.6 unx  3031552 b- defN 23-Jul-13 15:02 docleaf/backend.cp39-win_amd64.pyd
--rw-r--r--  4.6 unx      895 b- defN 23-Jul-13 15:02 docleaf-0.8.2.dist-info/RECORD
-11 files, 3210070 bytes uncompressed, 1104402 bytes compressed:  65.6%
+Zip file size: 1344340 bytes, number of entries: 11
+-rw-r--r--  4.6 unx     6912 b- defN 23-Aug-04 19:33 docleaf-0.8.3.dist-info/METADATA
+-rw-r--r--  4.6 unx      106 b- defN 23-Aug-04 19:33 docleaf-0.8.3.dist-info/WHEEL
+-rw-r--r--  4.6 unx     3502 b- defN 23-Aug-04 19:33 docleaf-0.8.3.dist-info/license_files/LICENSE.md
+-rw-r--r--  4.6 unx   137320 b- defN 23-Aug-04 19:33 docleaf-0.8.3.dist-info/license_files/LICENSES_THIRD_PARTY.md
+-rw-r--r--  4.6 unx     3545 b- defN 23-Aug-04 19:33 docleaf/domains.py
+-rw-r--r--  4.6 unx        0 b- defN 23-Aug-04 19:33 docleaf/__init__.py
+-rw-r--r--  4.6 unx    17008 b- defN 23-Aug-04 19:33 docleaf/doxygen.py
+-rw-r--r--  4.6 unx     5379 b- defN 23-Aug-04 19:33 docleaf/copied.py
+-rw-r--r--  4.6 unx       93 b- defN 23-Aug-04 19:33 docleaf/errors.py
+-rwxr-xr-x  4.6 unx  3902112 b- defN 23-Aug-04 19:33 docleaf/backend.cpython-37m-darwin.so
+-rw-r--r--  4.6 unx      899 b- defN 23-Aug-04 19:33 docleaf-0.8.3.dist-info/RECORD
+11 files, 4076876 bytes uncompressed, 1342830 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
-Filename: docleaf-0.8.2.dist-info/METADATA
+Filename: docleaf-0.8.3.dist-info/METADATA
 Comment: 
 
-Filename: docleaf-0.8.2.dist-info/WHEEL
+Filename: docleaf-0.8.3.dist-info/WHEEL
 Comment: 
 
-Filename: docleaf-0.8.2.dist-info/license_files/LICENSE.md
+Filename: docleaf-0.8.3.dist-info/license_files/LICENSE.md
 Comment: 
 
-Filename: docleaf-0.8.2.dist-info/license_files/LICENSES_THIRD_PARTY.md
+Filename: docleaf-0.8.3.dist-info/license_files/LICENSES_THIRD_PARTY.md
 Comment: 
 
-Filename: docleaf/copied.py
+Filename: docleaf/domains.py
 Comment: 
 
-Filename: docleaf/domains.py
+Filename: docleaf/__init__.py
 Comment: 
 
 Filename: docleaf/doxygen.py
 Comment: 
 
-Filename: docleaf/errors.py
+Filename: docleaf/copied.py
 Comment: 
 
-Filename: docleaf/__init__.py
+Filename: docleaf/errors.py
 Comment: 
 
-Filename: docleaf/backend.cp39-win_amd64.pyd
+Filename: docleaf/backend.cpython-37m-darwin.so
 Comment: 
 
-Filename: docleaf-0.8.2.dist-info/RECORD
+Filename: docleaf-0.8.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## docleaf/copied.py

 * *Ordering differences only*

```diff
@@ -1,133 +1,133 @@
-# This code is taken from the Breathe project. The Breathe license is below.
-#
-# Copyright (c) 2009, Michael Jones
-# All rights reserved.
-#
-# Redistribution and use in source and binary forms, with or without modification,
-# are permitted provided that the following conditions are met:
-#
-#  * Redistributions of source code must retain the above copyright notice,
-#    this list of conditions and the following disclaimer.
-#  * Redistributions in binary form must reproduce the above copyright notice,
-#    this list of conditions and the following disclaimer in the documentation
-#    and/or other materials provided with the distribution.
-#  * The names of its contributors may not be used to endorse or promote
-#    products derived from this software without specific prior written
-#    permission.
-#
-# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
-# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
-# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
-# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
-# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
-# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
-# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
-# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-#
-
-from docutils.statemachine import UnexpectedIndentationError
-from docutils.parsers.rst.states import Text
-from docutils import nodes
-
-
-class NodeFinder(nodes.SparseNodeVisitor):
-    """Find the Docutils desc_signature declarator and desc_content nodes."""
-
-    def __init__(self, document):
-        super().__init__(document)
-        self.declarator = None
-        self.signature = None
-        self.content = None
-
-    def visit_desc_signature(self, node):
-        # Find the last signature node because it contains the actual declarator
-        # rather than "template <...>". In Sphinx 1.4.1 we'll be able to use sphinx_cpp_tagname:
-        # https://github.com/michaeljones/breathe/issues/242
-        self.declarator = node
-        self.signature = node
-
-    def visit_desc_signature_line(self, node):
-        # In sphinx 1.5, there is now a desc_signature_line node within the desc_signature
-        # This should be used instead
-        self.declarator = node
-
-    def visit_desc_content(self, node):
-        self.content = node
-        # The SparseNodeVisitor seems to not actually be universally Sparse,
-        # but only for nodes known to Docutils.
-        # So if there are extensions with new node types in the content,
-        # then the visitation will fail.
-        # We anyway don't need to visit the actual content, so skip it.
-        raise nodes.SkipChildren
-
-
-# Taken from the Breathe code base
-class InlineText(Text):
-    """
-    Add a custom docutils class to allow parsing inline text. This is to be
-    used inside a @verbatim/@endverbatim block but only the first line is
-    consumed and a inline element is generated as the parent, instead of the
-    paragraph used by Text.
-    """
-
-    patterns = {"inlinetext": r""}
-    initial_transitions = [("inlinetext",)]
-
-    def indent(self, match, context, next_state):
-        """
-        Avoid Text's indent from detecting space prefixed text and
-        doing "funny" stuff; always rely on inlinetext for parsing.
-        """
-        return self.inlinetext(match, context, next_state)
-
-    def eof(self, context):
-        """
-        Text.eof() inserts a paragraph, so override it to skip adding elements.
-        """
-        return []
-
-    def inlinetext(self, match, context, next_state):
-        """
-        Called by the StateMachine when an inline element is found (which is
-        any text when this class is added as the single transition.
-        """
-        startline = self.state_machine.abs_line_number() - 1
-        msg = None
-        try:
-            block = self.state_machine.get_text_block()
-        except UnexpectedIndentationError as err:
-            block, src, srcline = err.args
-            msg = self.reporter.error("Unexpected indentation.", source=src, line=srcline)
-        lines = context + list(block)
-        text, _ = self.inline_text(lines[0], startline)
-        self.parent += text
-        self.parent += msg
-        return [], next_state, []
-
-
-# Taken from the Breathe code base
-def nested_inline_parse_with_titles(state, content, node) -> str:
-    """
-    This code is basically a customized nested_parse_with_titles from
-    docutils, using the InlineText class on the statemachine.
-    """
-    surrounding_title_styles = state.memo.title_styles
-    surrounding_section_level = state.memo.section_level
-    state.memo.title_styles = []
-    state.memo.section_level = 0
-    try:
-        return state.nested_parse(
-            content,
-            0,
-            node,
-            match_titles=1,
-            state_machine_kwargs={
-                "state_classes": (InlineText,),
-                "initial_state": "InlineText",
-            },
-        )
-    finally:
-        state.memo.title_styles = surrounding_title_styles
-        state.memo.section_level = surrounding_section_level
+# This code is taken from the Breathe project. The Breathe license is below.
+#
+# Copyright (c) 2009, Michael Jones
+# All rights reserved.
+#
+# Redistribution and use in source and binary forms, with or without modification,
+# are permitted provided that the following conditions are met:
+#
+#  * Redistributions of source code must retain the above copyright notice,
+#    this list of conditions and the following disclaimer.
+#  * Redistributions in binary form must reproduce the above copyright notice,
+#    this list of conditions and the following disclaimer in the documentation
+#    and/or other materials provided with the distribution.
+#  * The names of its contributors may not be used to endorse or promote
+#    products derived from this software without specific prior written
+#    permission.
+#
+# THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND
+# ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+# WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE
+# DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR
+# ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES
+# (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+# LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON
+# ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT
+# (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+# SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+#
+
+from docutils.statemachine import UnexpectedIndentationError
+from docutils.parsers.rst.states import Text
+from docutils import nodes
+
+
+class NodeFinder(nodes.SparseNodeVisitor):
+    """Find the Docutils desc_signature declarator and desc_content nodes."""
+
+    def __init__(self, document):
+        super().__init__(document)
+        self.declarator = None
+        self.signature = None
+        self.content = None
+
+    def visit_desc_signature(self, node):
+        # Find the last signature node because it contains the actual declarator
+        # rather than "template <...>". In Sphinx 1.4.1 we'll be able to use sphinx_cpp_tagname:
+        # https://github.com/michaeljones/breathe/issues/242
+        self.declarator = node
+        self.signature = node
+
+    def visit_desc_signature_line(self, node):
+        # In sphinx 1.5, there is now a desc_signature_line node within the desc_signature
+        # This should be used instead
+        self.declarator = node
+
+    def visit_desc_content(self, node):
+        self.content = node
+        # The SparseNodeVisitor seems to not actually be universally Sparse,
+        # but only for nodes known to Docutils.
+        # So if there are extensions with new node types in the content,
+        # then the visitation will fail.
+        # We anyway don't need to visit the actual content, so skip it.
+        raise nodes.SkipChildren
+
+
+# Taken from the Breathe code base
+class InlineText(Text):
+    """
+    Add a custom docutils class to allow parsing inline text. This is to be
+    used inside a @verbatim/@endverbatim block but only the first line is
+    consumed and a inline element is generated as the parent, instead of the
+    paragraph used by Text.
+    """
+
+    patterns = {"inlinetext": r""}
+    initial_transitions = [("inlinetext",)]
+
+    def indent(self, match, context, next_state):
+        """
+        Avoid Text's indent from detecting space prefixed text and
+        doing "funny" stuff; always rely on inlinetext for parsing.
+        """
+        return self.inlinetext(match, context, next_state)
+
+    def eof(self, context):
+        """
+        Text.eof() inserts a paragraph, so override it to skip adding elements.
+        """
+        return []
+
+    def inlinetext(self, match, context, next_state):
+        """
+        Called by the StateMachine when an inline element is found (which is
+        any text when this class is added as the single transition.
+        """
+        startline = self.state_machine.abs_line_number() - 1
+        msg = None
+        try:
+            block = self.state_machine.get_text_block()
+        except UnexpectedIndentationError as err:
+            block, src, srcline = err.args
+            msg = self.reporter.error("Unexpected indentation.", source=src, line=srcline)
+        lines = context + list(block)
+        text, _ = self.inline_text(lines[0], startline)
+        self.parent += text
+        self.parent += msg
+        return [], next_state, []
+
+
+# Taken from the Breathe code base
+def nested_inline_parse_with_titles(state, content, node) -> str:
+    """
+    This code is basically a customized nested_parse_with_titles from
+    docutils, using the InlineText class on the statemachine.
+    """
+    surrounding_title_styles = state.memo.title_styles
+    surrounding_section_level = state.memo.section_level
+    state.memo.title_styles = []
+    state.memo.section_level = 0
+    try:
+        return state.nested_parse(
+            content,
+            0,
+            node,
+            match_titles=1,
+            state_machine_kwargs={
+                "state_classes": (InlineText,),
+                "initial_state": "InlineText",
+            },
+        )
+    finally:
+        state.memo.title_styles = surrounding_title_styles
+        state.memo.section_level = surrounding_section_level
```

## docleaf/domains.py

 * *Ordering differences only*

```diff
@@ -1,114 +1,114 @@
-from sphinx.domains import cpp, c
-
-from . import copied
-from .errors import DocleafError
-
-
-def null_handler(finder, location):
-    return
-
-
-def strip_desc_addname(finder, location):
-    # We pass qualified values to the domain directives but we don't always want Sphinx
-    # to show the qualified part in the output as normally it is shown but the nesting
-    # of the entities so we strip it out which involes removing the 'desc_addname' node
-    # in the output
-    finder.declarator.children = [node for node in finder.declarator.children if node.tagname != "desc_addname"]
-
-
-def add_location_via_names(finder, location):
-    if finder.signature and location:
-        finder.signature["names"] = f"{location['path']}:{location['line']}"
-
-
-def chain(*funcs):
-    def inner(finder, location):
-        for func in funcs:
-            func(finder, location)
-
-    return inner
-
-
-cpp_domain = {
-    "class": (cpp.CPPClassObject, "class", add_location_via_names),
-    "enum": (cpp.CPPEnumObject, "enum", add_location_via_names),
-    "enumerator": (
-        cpp.CPPEnumeratorObject,
-        "enumerator",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "function": (
-        cpp.CPPFunctionObject,
-        "function",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "member": (cpp.CPPMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
-    "struct": (cpp.CPPClassObject, "struct", add_location_via_names),
-}
-
-c_domain = {
-    "define": (c.CMacroObject, "macro", add_location_via_names),
-    "enum": (c.CEnumObject, "enum", add_location_via_names),
-    "enumerator": (
-        c.CEnumeratorObject,
-        "enumerator",
-        chain(strip_desc_addname, add_location_via_names),
-    ),
-    "function": (c.CFunctionObject, "function", add_location_via_names),
-    "member": (c.CMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
-    "struct": (c.CStructObject, "struct", add_location_via_names),
-    "typedef": (c.CTypeObject, "type", add_location_via_names),
-    "union": (c.CUnionObject, "union", chain(strip_desc_addname, add_location_via_names)),
-}
-
-domains = {"cpp": cpp_domain, "c": c_domain}
-
-
-def render_domain_entry(
-    domain_name: str,
-    type: str,
-    declaration: str,
-    location,
-    target,
-    directive_args: list,
-    content: list,
-):
-    # print("render_domain_entry", domain_name, type, declaration)
-    try:
-        domain = domains[domain_name]
-    except KeyError:
-        raise DocleafError(f"Unsupported domain: {domain_name}")
-
-    try:
-        (Directive, domain_specific_type, handler) = domain[type]
-    except KeyError:
-        raise DocleafError(f'Unsupported type "{type}" on domain "{domain_name}"')
-
-    directive_name = f"{domain_name}:{domain_specific_type}"
-
-    args = [directive_name, [declaration]] + directive_args[2:]
-    directive = Directive(*args)
-
-    nodes = directive.run()
-
-    rst_node = nodes[1]
-    finder = copied.NodeFinder(rst_node.document)
-    rst_node.walk(finder)
-
-    set_children(finder.content, content)
-    finder.declarator.children.insert(0, target)
-
-    handler(finder, location)
-
-    return nodes
-
-
-def set_children(node, children):
-    """
-    The children have to be informed of the parent and that happens in the parents
-    helper methods like 'append' and 'extend' so we can't just replace 'node.children'
-    with 'children'. Instead we empty the children list and then add the children so
-    they are set up properly.
-    """
-    node.children.clear()
-    node.extend(children)
+from sphinx.domains import cpp, c
+
+from . import copied
+from .errors import DocleafError
+
+
+def null_handler(finder, location):
+    return
+
+
+def strip_desc_addname(finder, location):
+    # We pass qualified values to the domain directives but we don't always want Sphinx
+    # to show the qualified part in the output as normally it is shown but the nesting
+    # of the entities so we strip it out which involes removing the 'desc_addname' node
+    # in the output
+    finder.declarator.children = [node for node in finder.declarator.children if node.tagname != "desc_addname"]
+
+
+def add_location_via_names(finder, location):
+    if finder.signature and location:
+        finder.signature["names"] = f"{location['path']}:{location['line']}"
+
+
+def chain(*funcs):
+    def inner(finder, location):
+        for func in funcs:
+            func(finder, location)
+
+    return inner
+
+
+cpp_domain = {
+    "class": (cpp.CPPClassObject, "class", add_location_via_names),
+    "enum": (cpp.CPPEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        cpp.CPPEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (
+        cpp.CPPFunctionObject,
+        "function",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "member": (cpp.CPPMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (cpp.CPPClassObject, "struct", add_location_via_names),
+}
+
+c_domain = {
+    "define": (c.CMacroObject, "macro", add_location_via_names),
+    "enum": (c.CEnumObject, "enum", add_location_via_names),
+    "enumerator": (
+        c.CEnumeratorObject,
+        "enumerator",
+        chain(strip_desc_addname, add_location_via_names),
+    ),
+    "function": (c.CFunctionObject, "function", add_location_via_names),
+    "member": (c.CMemberObject, "member", chain(strip_desc_addname, add_location_via_names)),
+    "struct": (c.CStructObject, "struct", add_location_via_names),
+    "typedef": (c.CTypeObject, "type", add_location_via_names),
+    "union": (c.CUnionObject, "union", chain(strip_desc_addname, add_location_via_names)),
+}
+
+domains = {"cpp": cpp_domain, "c": c_domain}
+
+
+def render_domain_entry(
+    domain_name: str,
+    type: str,
+    declaration: str,
+    location,
+    target,
+    directive_args: list,
+    content: list,
+):
+    # print("render_domain_entry", domain_name, type, declaration)
+    try:
+        domain = domains[domain_name]
+    except KeyError:
+        raise DocleafError(f"Unsupported domain: {domain_name}")
+
+    try:
+        (Directive, domain_specific_type, handler) = domain[type]
+    except KeyError:
+        raise DocleafError(f'Unsupported type "{type}" on domain "{domain_name}"')
+
+    directive_name = f"{domain_name}:{domain_specific_type}"
+
+    args = [directive_name, [declaration]] + directive_args[2:]
+    directive = Directive(*args)
+
+    nodes = directive.run()
+
+    rst_node = nodes[1]
+    finder = copied.NodeFinder(rst_node.document)
+    rst_node.walk(finder)
+
+    set_children(finder.content, content)
+    finder.declarator.children.insert(0, target)
+
+    handler(finder, location)
+
+    return nodes
+
+
+def set_children(node, children):
+    """
+    The children have to be informed of the parent and that happens in the parents
+    helper methods like 'append' and 'extend' so we can't just replace 'node.children'
+    with 'children'. Instead we empty the children list and then add the children so
+    they are set up properly.
+    """
+    node.children.clear()
+    node.extend(children)
```

## docleaf/doxygen.py

 * *Ordering differences only*

```diff
@@ -1,498 +1,498 @@
-from typing import List
-from pathlib import Path
-import itertools
-import textwrap
-import hashlib
-import time
-import sys
-import os
-
-from docutils.nodes import Node
-from docutils.parsers.rst import Directive, directives
-from docutils.statemachine import StringList
-from docutils import nodes
-
-from sphinx.application import Sphinx
-from sphinx.environment import BuildEnvironment
-from sphinx.util.nodes import nested_parse_with_titles
-from sphinx.util import logging
-import sphinx.addnodes
-
-from . import backend, domains, copied
-from .errors import DocleafError
-
-__version__ = "0.0.0"
-
-logger = logging.getLogger(__name__)
-
-
-class GitHubLinkResolver:
-    """
-    This works on the assumption that we can insert our own data into the 'names' field of desc_signature nodes in
-    domain entries. That assumption might fail or clash with other things so we try to be careful when extracting the
-    data from 'names' and fail early and quietly.
-    """
-
-    def __init__(self, *, root, user, repo, tag=None, branch=None, revision=None):
-        self.root = Path(root).resolve()
-        self.user = user
-        self.repo = repo
-        self.tag = tag
-        self.branch = branch
-        self.revision = revision
-
-    def __call__(self, domain, info):
-        if domain not in ["c", "cpp"]:
-            return None
-
-        names = info.get("names")
-        if not names:
-            return None
-
-        entries = names.rsplit(":", 1)
-        if len(entries) != 2:
-            return None
-
-        path = Path(entries[0]).resolve()
-        relative = path.relative_to(self.root)
-
-        try:
-            line = int(entries[1])
-        except ValueError:
-            # Unable to get line number - exit quietly
-            return None
-
-        reference = self.tag or self.branch or self.revision
-        if not reference:
-            return None
-
-        return f"https://github.com/{self.user}/{self.repo}/blob/{reference}/{relative}#L{line}"
-
-
-def as_list(node):
-    def wrapper(*children, **attributes):
-        return [node(*children, **attributes)]
-
-    return wrapper
-
-
-class NodeManager:
-    def __init__(self, state, directive_arguments):
-        self.state = state
-        self.directive_arguments = directive_arguments
-        self.lookup = {
-            "bullet_list": as_list(nodes.bullet_list),
-            "container": as_list(nodes.container),
-            "colspec": as_list(nodes.colspec),
-            "desc": as_list(sphinx.addnodes.desc),
-            "desc_content": as_list(sphinx.addnodes.desc_content),
-            "desc_name": as_list(sphinx.addnodes.desc_name),
-            "desc_parameter": as_list(sphinx.addnodes.desc_parameter),
-            "desc_parameterlist": as_list(sphinx.addnodes.desc_parameterlist),
-            "desc_sig_keyword": as_list(sphinx.addnodes.desc_sig_keyword),
-            "desc_sig_name": as_list(sphinx.addnodes.desc_sig_name),
-            "desc_sig_space": as_list(sphinx.addnodes.desc_sig_space),
-            "desc_signature": as_list(sphinx.addnodes.desc_signature),
-            "desc_signature_line": as_list(sphinx.addnodes.desc_signature_line),
-            "emphasis": as_list(nodes.emphasis),
-            "entry": as_list(nodes.entry),
-            "enumerated_list": as_list(nodes.enumerated_list),
-            "field_list": as_list(nodes.field_list),
-            "field": as_list(nodes.field),
-            "field_name": as_list(nodes.field_name),
-            "field_body": as_list(nodes.field_body),
-            "index": as_list(sphinx.addnodes.index),
-            "inline": as_list(nodes.inline),
-            "list_item": as_list(nodes.list_item),
-            "literal": as_list(nodes.literal),
-            "literal_block": as_list(nodes.literal_block),
-            "literal_strong": as_list(sphinx.addnodes.literal_strong),
-            "note": as_list(nodes.note),
-            "only": as_list(sphinx.addnodes.only),
-            "paragraph": as_list(nodes.paragraph),
-            "raw": as_list(nodes.raw),
-            "internal_reference": self.build_internal_reference,
-            "external_reference": as_list(nodes.reference),
-            "restructured_text_block": self.build_restructured_text_block,
-            "restructured_text_inline": self.build_restructured_text_inline,
-            "row": as_list(nodes.row),
-            "rubric": as_list(nodes.rubric),
-            "strong": as_list(nodes.strong),
-            "see_also": as_list(sphinx.addnodes.seealso),
-            "table": as_list(nodes.table),
-            "tbody": as_list(nodes.tbody),
-            "tgroup": as_list(nodes.tgroup),
-            "thead": as_list(nodes.thead),
-            "warning": as_list(nodes.warning),
-            # Special
-            "target": as_list(self.build_target),
-            "domain_entry": self.build_domain_entry,
-        }
-
-    def get_builder(self, node_type):
-        builder = self.lookup[node_type]
-        return builder
-
-    def build_target(self, *children, **attributes):
-        target = nodes.target(*children, **attributes)
-        self.state.document.note_explicit_target(target)
-        return target
-
-    def build_domain_entry(self, *children, **attributes):
-        return domains.render_domain_entry(
-            attributes["domain"],
-            attributes["type"],
-            attributes["declaration"],
-            attributes.get("location"),
-            self.build_target(**attributes["target"]),
-            self.directive_arguments,
-            children,
-        )
-
-    def build_internal_reference(self, *children, **attributes):
-        reference = sphinx.addnodes.pending_xref(
-            "",
-            *children,
-            reftype="ref",
-            refdomain="std",
-            refexplicit=True,
-            refid=attributes["refid"],
-            reftarget=attributes["refid"],
-        )
-        return [reference]
-
-    def build_restructured_text_block(self, *children, **attributes):
-        text = textwrap.dedent(children[0])
-
-        # Inspired by autodoc.py in Sphinx
-        rst = StringList()
-        for line in text.split("\n"):
-            rst.append(line, "<docleaf>")
-
-        # Parent node for the generated node subtree
-        rst_node = nodes.paragraph()
-        rst_node.document = self.state.document
-
-        nested_parse_with_titles(self.state, rst, rst_node)
-
-        # We render the block into a paragraph node but the rendred block will contain
-        # its own paragraph nodes at the top level so we don't need to return our
-        # paragraph node so we return its children (the top layer of rendered nodes) as
-        # the output
-        return rst_node.children
-
-    def build_restructured_text_inline(self, *children, **attributes):
-        text = children[0]
-
-        # Inspired by autodoc.py in Sphinx
-        rst = StringList()
-        for line in text.split("\n"):
-            rst.append(line, "<docleaf>")
-
-        rst_node = nodes.inline()
-        rst_node.document = self.state.document
-
-        copied.nested_inline_parse_with_titles(self.state, rst, rst_node)
-
-        return [rst_node]
-
-
-def render_node_list(node_list, node_manager):
-    # Use nested comprehension to flatten nodes lists coming back from render_node
-    return flatten(render_node(node, node_manager) for node in node_list)
-
-
-def flatten(list_of_lists):
-    return list(itertools.chain.from_iterable(list_of_lists))
-
-
-def render_node(node, node_manager):
-    if node.type == "text":
-        return [nodes.Text(node.text)]
-
-    node_builder = node_manager.get_builder(node.type)
-    children = render_node_list(node.children, node_manager)
-
-    if node.call_as == "text-element":
-        return node_builder("", "", *children, **node.attributes)
-    elif node.call_as == "element":
-        return node_builder("", *children, **node.attributes)
-    elif node.call_as == "function":
-        return node_builder(*children, **node.attributes)
-    else:
-        raise DocleafError("Call As not implemented: " + node.call_as)
-
-
-class Project:
-    def __init__(self, root, xml):
-        self._root = root
-        self._xml = xml
-
-    def root(self):
-        return self._root
-
-    def xml(self):
-        return self._xml
-
-    def get(projects, name: str):
-        # For each 'try' block we need to catch KeyError and TypeError (if project is a string) so we catch everything
-        # as there isn't much else that could go wrong
-
-        try:
-            data = projects[name]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find a project called '{name}' defined in the docleaf_projects config variable"
-            )
-
-        try:
-            root = data["root"]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find the 'root' entry in the data for '{name}' project defined in the docleaf_projects "
-                "config variable"
-            )
-
-        try:
-            xml = data["xml"]
-        except Exception:
-            raise DocleafError(
-                f"Unable to find the 'xml' entry in the data for '{name}' project defined in the docleaf_projects "
-                "config variable"
-            )
-
-        return Project(root, xml)
-
-
-class BaseDirective(Directive):
-    def get_directive_args(self) -> list:
-        # Must match order in docutils.parsers.rst.Directive.__init__
-        return [
-            self.name,
-            self.arguments,
-            self.options,
-            self.content,
-            self.lineno,
-            self.content_offset,
-            self.block_text,
-            self.state,
-            self.state_machine,
-        ]
-
-
-class BasicDoxygenDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "skip-xml-nodes": directives.unchanged,
-    }
-
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options["project"] or self.app.config.docleaf_default_project
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-        skip_settings = get_skip_settings(self.app, self.options)
-
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = self.render_function(name, project.xml(), context, tracked_cache)
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
-
-
-class ClassDirective(BasicDoxygenDirective):
-    render_function = backend.render_class
-
-
-class StructDirective(BasicDoxygenDirective):
-    render_function = backend.render_struct
-
-
-class EnumDirective(BasicDoxygenDirective):
-    render_function = backend.render_enum
-
-
-class FunctionDirective(BasicDoxygenDirective):
-    render_function = backend.render_function
-
-
-class GroupDirective(BaseDirective):
-    has_content = True
-    required_arguments = 1
-    optional_arguments = 0
-    final_argument_whitespace = True
-    option_spec = {
-        "project": directives.unchanged,
-        "content-only": directives.flag,  # TODO: Implement
-        "inner": directives.flag,  # TODO: Implement
-        "skip-xml-nodes": directives.unchanged,
-    }
-
-    def run(self) -> List[Node]:
-        name = self.arguments[0]
-        project_name = self.options.get("project", self.app.config.docleaf_default_project)
-        project = Project.get(self.app.config.docleaf_projects, project_name)
-
-        skip_settings = get_skip_settings(self.app, self.options)
-        content_only = "content-only" in self.options
-        inner_group = "inner" in self.options
-        context = backend.Context(
-            project.root(),
-            skip_settings,
-            self.app.config.docleaf_domain_by_extension,
-        )
-
-        tracked_cache = backend.TrackedCache(self.cache)
-        node_list = backend.render_group(
-            name,
-            project.xml(),
-            context,
-            content_only,
-            inner_group,
-            tracked_cache,
-        )
-        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
-
-        node_builder = NodeManager(self.state, self.get_directive_args())
-        return render_node_list(node_list, node_builder)
-
-
-def get_skip_settings(app, options):
-    """
-    Get the option for the directive and fallback to the app option if not defined on the directive
-    """
-    skip_settings = options.get("skip", None)
-    if skip_settings is None:
-        skip_settings = app.config.docleaf_doxygen_skip
-    else:
-        skip_settings = skip_settings.split(",")
-    return skip_settings
-
-
-class XmlFileInfo:
-    def __init__(self, hash, rst_files):
-        self.hash = hash
-        self.rst_files = rst_files
-
-
-def hash_file(path):
-    logger.debug(f"docleaf: hashing {path}")
-    if sys.version_info >= (3, 11):
-        with open(path, "rb") as f:
-            digest = hashlib.file_digest(f, "sha1")
-            return digest.hexdigest()
-    else:
-        contents = open(path, "rb").read()
-        hash = hashlib.sha1()
-        hash.update(contents)
-        return hash.hexdigest()
-
-
-def update_sphinx_env_file_data(env: BuildEnvironment, xml_paths: List[str], rst_file: str):
-    """
-    Update our file_data store to indicate which rst files are dependent on which xml files
-    """
-    if not hasattr(env, "docleaf_file_data"):
-        env.docleaf_file_data = {}
-
-    for path in xml_paths:
-        if path in env.docleaf_file_data:
-            env.docleaf_file_data[path].rst_files.add(rst_file)
-        else:
-            env.docleaf_file_data[path] = XmlFileInfo(hash_file(path), set([rst_file]))
-
-
-def calculate_files_to_refresh(app: Sphinx, env, added, changed, removed):
-    """
-    Sphinx tells us which rst files have changed on disk and we can tell it (by returning a list of doc names) which
-    documents need to be re-read and have their output re-generated.
-
-    We calculate which files to refresh by storing the last build time and comparing the modified time of each xml file
-    against the last build time and see if any are newer. From there we need to get from the xml files to the rst files
-    that they impact and return those rst files to be refreshed.
-    """
-    logger.debug("docleaf: calculate_files_to_refresh")
-
-    # Get the last build time before updating it
-    last_build_time = getattr(app.env, "docleaf_last_build_time", None)
-
-    # Store the current time as the build time
-    app.env.docleaf_last_build_time = time.time()
-
-    if not last_build_time:
-        return []
-
-    if not hasattr(app.env, "docleaf_file_data"):
-        return []
-
-    rst_files_to_refresh = set()
-
-    for xml_file_path, info in app.env.docleaf_file_data.items():
-        stat = os.stat(xml_file_path)
-        if stat.st_mtime > last_build_time:
-            hash = hash_file(xml_file_path)
-            logger.debug(f"docleaf: stored hash for {xml_file_path} = {hash}. Calculated hash: {info.hash}")
-            if hash != info.hash:
-                # Store the new hash
-                info.hash = hash
-                # Tell Sphinx to refresh all rst files associated with this file
-                rst_files_to_refresh.update(info.rst_files)
-
-    logger.verbose(f"docleaf: calculate_files_to_refresh - Rebuild: {rst_files_to_refresh}")
-    return rst_files_to_refresh
-
-
-def purge_file_data(app, env, docname):
-    """
-    Clear any file data associated with 'docname' in accordance with the Sphinx API
-    """
-    logger.debug("docleaf: purge_file_data - %s", docname)
-    if not hasattr(app.env, "docleaf_file_data"):
-        return
-
-    for xml_file_path, info in app.env.docleaf_file_data.items():
-        info.rst_files.discard(docname)
-
-
-class ExtensionContext:
-    def __init__(self, app: Sphinx, cache):
-        self.app = app
-        self.cache = cache
-
-
-def add_directive(context, name, Cls):
-    Cls.app = context.app
-    Cls.cache = context.cache
-    context.app.add_directive(name, Cls)
-
-
-def setup(app: Sphinx):
-    cache = backend.FileCache()
-
-    context = ExtensionContext(app, cache)
-
-    add_directive(context, "doxygenclass", ClassDirective)
-    add_directive(context, "doxygenenum", EnumDirective)
-    add_directive(context, "doxygenfunction", FunctionDirective)
-    add_directive(context, "doxygengroup", GroupDirective)
-    add_directive(context, "doxygenstruct", StructDirective)
-
-    app.add_config_value("docleaf_projects", {}, "env")
-    app.add_config_value("docleaf_default_project", None, "env")
-    app.add_config_value("docleaf_doxygen_skip", [], "env")
-    app.add_config_value("docleaf_domain_by_extension", {}, True)
-
-    app.connect("env-get-outdated", calculate_files_to_refresh)
-    app.connect("env-purge-doc", purge_file_data)
-
-    return {"version": __version__, "parallel_read_safe": True, "parallel_write_safe": True}
+from typing import List
+from pathlib import Path
+import itertools
+import textwrap
+import hashlib
+import time
+import sys
+import os
+
+from docutils.nodes import Node
+from docutils.parsers.rst import Directive, directives
+from docutils.statemachine import StringList
+from docutils import nodes
+
+from sphinx.application import Sphinx
+from sphinx.environment import BuildEnvironment
+from sphinx.util.nodes import nested_parse_with_titles
+from sphinx.util import logging
+import sphinx.addnodes
+
+from . import backend, domains, copied
+from .errors import DocleafError
+
+__version__ = "0.0.0"
+
+logger = logging.getLogger(__name__)
+
+
+class GitHubLinkResolver:
+    """
+    This works on the assumption that we can insert our own data into the 'names' field of desc_signature nodes in
+    domain entries. That assumption might fail or clash with other things so we try to be careful when extracting the
+    data from 'names' and fail early and quietly.
+    """
+
+    def __init__(self, *, root, user, repo, tag=None, branch=None, revision=None):
+        self.root = Path(root).resolve()
+        self.user = user
+        self.repo = repo
+        self.tag = tag
+        self.branch = branch
+        self.revision = revision
+
+    def __call__(self, domain, info):
+        if domain not in ["c", "cpp"]:
+            return None
+
+        names = info.get("names")
+        if not names:
+            return None
+
+        entries = names.rsplit(":", 1)
+        if len(entries) != 2:
+            return None
+
+        path = Path(entries[0]).resolve()
+        relative = path.relative_to(self.root)
+
+        try:
+            line = int(entries[1])
+        except ValueError:
+            # Unable to get line number - exit quietly
+            return None
+
+        reference = self.tag or self.branch or self.revision
+        if not reference:
+            return None
+
+        return f"https://github.com/{self.user}/{self.repo}/blob/{reference}/{relative}#L{line}"
+
+
+def as_list(node):
+    def wrapper(*children, **attributes):
+        return [node(*children, **attributes)]
+
+    return wrapper
+
+
+class NodeManager:
+    def __init__(self, state, directive_arguments):
+        self.state = state
+        self.directive_arguments = directive_arguments
+        self.lookup = {
+            "bullet_list": as_list(nodes.bullet_list),
+            "container": as_list(nodes.container),
+            "colspec": as_list(nodes.colspec),
+            "desc": as_list(sphinx.addnodes.desc),
+            "desc_content": as_list(sphinx.addnodes.desc_content),
+            "desc_name": as_list(sphinx.addnodes.desc_name),
+            "desc_parameter": as_list(sphinx.addnodes.desc_parameter),
+            "desc_parameterlist": as_list(sphinx.addnodes.desc_parameterlist),
+            "desc_sig_keyword": as_list(sphinx.addnodes.desc_sig_keyword),
+            "desc_sig_name": as_list(sphinx.addnodes.desc_sig_name),
+            "desc_sig_space": as_list(sphinx.addnodes.desc_sig_space),
+            "desc_signature": as_list(sphinx.addnodes.desc_signature),
+            "desc_signature_line": as_list(sphinx.addnodes.desc_signature_line),
+            "emphasis": as_list(nodes.emphasis),
+            "entry": as_list(nodes.entry),
+            "enumerated_list": as_list(nodes.enumerated_list),
+            "field_list": as_list(nodes.field_list),
+            "field": as_list(nodes.field),
+            "field_name": as_list(nodes.field_name),
+            "field_body": as_list(nodes.field_body),
+            "index": as_list(sphinx.addnodes.index),
+            "inline": as_list(nodes.inline),
+            "list_item": as_list(nodes.list_item),
+            "literal": as_list(nodes.literal),
+            "literal_block": as_list(nodes.literal_block),
+            "literal_strong": as_list(sphinx.addnodes.literal_strong),
+            "note": as_list(nodes.note),
+            "only": as_list(sphinx.addnodes.only),
+            "paragraph": as_list(nodes.paragraph),
+            "raw": as_list(nodes.raw),
+            "internal_reference": self.build_internal_reference,
+            "external_reference": as_list(nodes.reference),
+            "restructured_text_block": self.build_restructured_text_block,
+            "restructured_text_inline": self.build_restructured_text_inline,
+            "row": as_list(nodes.row),
+            "rubric": as_list(nodes.rubric),
+            "strong": as_list(nodes.strong),
+            "see_also": as_list(sphinx.addnodes.seealso),
+            "table": as_list(nodes.table),
+            "tbody": as_list(nodes.tbody),
+            "tgroup": as_list(nodes.tgroup),
+            "thead": as_list(nodes.thead),
+            "warning": as_list(nodes.warning),
+            # Special
+            "target": as_list(self.build_target),
+            "domain_entry": self.build_domain_entry,
+        }
+
+    def get_builder(self, node_type):
+        builder = self.lookup[node_type]
+        return builder
+
+    def build_target(self, *children, **attributes):
+        target = nodes.target(*children, **attributes)
+        self.state.document.note_explicit_target(target)
+        return target
+
+    def build_domain_entry(self, *children, **attributes):
+        return domains.render_domain_entry(
+            attributes["domain"],
+            attributes["type"],
+            attributes["declaration"],
+            attributes.get("location"),
+            self.build_target(**attributes["target"]),
+            self.directive_arguments,
+            children,
+        )
+
+    def build_internal_reference(self, *children, **attributes):
+        reference = sphinx.addnodes.pending_xref(
+            "",
+            *children,
+            reftype="ref",
+            refdomain="std",
+            refexplicit=True,
+            refid=attributes["refid"],
+            reftarget=attributes["refid"],
+        )
+        return [reference]
+
+    def build_restructured_text_block(self, *children, **attributes):
+        text = textwrap.dedent(children[0])
+
+        # Inspired by autodoc.py in Sphinx
+        rst = StringList()
+        for line in text.split("\n"):
+            rst.append(line, "<docleaf>")
+
+        # Parent node for the generated node subtree
+        rst_node = nodes.paragraph()
+        rst_node.document = self.state.document
+
+        nested_parse_with_titles(self.state, rst, rst_node)
+
+        # We render the block into a paragraph node but the rendred block will contain
+        # its own paragraph nodes at the top level so we don't need to return our
+        # paragraph node so we return its children (the top layer of rendered nodes) as
+        # the output
+        return rst_node.children
+
+    def build_restructured_text_inline(self, *children, **attributes):
+        text = children[0]
+
+        # Inspired by autodoc.py in Sphinx
+        rst = StringList()
+        for line in text.split("\n"):
+            rst.append(line, "<docleaf>")
+
+        rst_node = nodes.inline()
+        rst_node.document = self.state.document
+
+        copied.nested_inline_parse_with_titles(self.state, rst, rst_node)
+
+        return [rst_node]
+
+
+def render_node_list(node_list, node_manager):
+    # Use nested comprehension to flatten nodes lists coming back from render_node
+    return flatten(render_node(node, node_manager) for node in node_list)
+
+
+def flatten(list_of_lists):
+    return list(itertools.chain.from_iterable(list_of_lists))
+
+
+def render_node(node, node_manager):
+    if node.type == "text":
+        return [nodes.Text(node.text)]
+
+    node_builder = node_manager.get_builder(node.type)
+    children = render_node_list(node.children, node_manager)
+
+    if node.call_as == "text-element":
+        return node_builder("", "", *children, **node.attributes)
+    elif node.call_as == "element":
+        return node_builder("", *children, **node.attributes)
+    elif node.call_as == "function":
+        return node_builder(*children, **node.attributes)
+    else:
+        raise DocleafError("Call As not implemented: " + node.call_as)
+
+
+class Project:
+    def __init__(self, root, xml):
+        self._root = root
+        self._xml = xml
+
+    def root(self):
+        return self._root
+
+    def xml(self):
+        return self._xml
+
+    def get(projects, name: str):
+        # For each 'try' block we need to catch KeyError and TypeError (if project is a string) so we catch everything
+        # as there isn't much else that could go wrong
+
+        try:
+            data = projects[name]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find a project called '{name}' defined in the docleaf_projects config variable"
+            )
+
+        try:
+            root = data["root"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'root' entry in the data for '{name}' project defined in the docleaf_projects "
+                "config variable"
+            )
+
+        try:
+            xml = data["xml"]
+        except Exception:
+            raise DocleafError(
+                f"Unable to find the 'xml' entry in the data for '{name}' project defined in the docleaf_projects "
+                "config variable"
+            )
+
+        return Project(root, xml)
+
+
+class BaseDirective(Directive):
+    def get_directive_args(self) -> list:
+        # Must match order in docutils.parsers.rst.Directive.__init__
+        return [
+            self.name,
+            self.arguments,
+            self.options,
+            self.content,
+            self.lineno,
+            self.content_offset,
+            self.block_text,
+            self.state,
+            self.state_machine,
+        ]
+
+
+class BasicDoxygenDirective(BaseDirective):
+    has_content = True
+    required_arguments = 1
+    optional_arguments = 0
+    final_argument_whitespace = True
+    option_spec = {
+        "project": directives.unchanged,
+        "skip-xml-nodes": directives.unchanged,
+    }
+
+    def run(self) -> List[Node]:
+        name = self.arguments[0]
+        project_name = self.options["project"] or self.app.config.docleaf_default_project
+        project = Project.get(self.app.config.docleaf_projects, project_name)
+        skip_settings = get_skip_settings(self.app, self.options)
+
+        context = backend.Context(
+            project.root(),
+            skip_settings,
+            self.app.config.docleaf_domain_by_extension,
+        )
+
+        tracked_cache = backend.TrackedCache(self.cache)
+        node_list = self.render_function(name, project.xml(), context, tracked_cache)
+        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
+
+        node_builder = NodeManager(self.state, self.get_directive_args())
+        return render_node_list(node_list, node_builder)
+
+
+class ClassDirective(BasicDoxygenDirective):
+    render_function = backend.render_class
+
+
+class StructDirective(BasicDoxygenDirective):
+    render_function = backend.render_struct
+
+
+class EnumDirective(BasicDoxygenDirective):
+    render_function = backend.render_enum
+
+
+class FunctionDirective(BasicDoxygenDirective):
+    render_function = backend.render_function
+
+
+class GroupDirective(BaseDirective):
+    has_content = True
+    required_arguments = 1
+    optional_arguments = 0
+    final_argument_whitespace = True
+    option_spec = {
+        "project": directives.unchanged,
+        "content-only": directives.flag,  # TODO: Implement
+        "inner": directives.flag,  # TODO: Implement
+        "skip-xml-nodes": directives.unchanged,
+    }
+
+    def run(self) -> List[Node]:
+        name = self.arguments[0]
+        project_name = self.options.get("project", self.app.config.docleaf_default_project)
+        project = Project.get(self.app.config.docleaf_projects, project_name)
+
+        skip_settings = get_skip_settings(self.app, self.options)
+        content_only = "content-only" in self.options
+        inner_group = "inner" in self.options
+        context = backend.Context(
+            project.root(),
+            skip_settings,
+            self.app.config.docleaf_domain_by_extension,
+        )
+
+        tracked_cache = backend.TrackedCache(self.cache)
+        node_list = backend.render_group(
+            name,
+            project.xml(),
+            context,
+            content_only,
+            inner_group,
+            tracked_cache,
+        )
+        update_sphinx_env_file_data(self.app.env, tracked_cache.xml_paths(), self.app.env.docname)
+
+        node_builder = NodeManager(self.state, self.get_directive_args())
+        return render_node_list(node_list, node_builder)
+
+
+def get_skip_settings(app, options):
+    """
+    Get the option for the directive and fallback to the app option if not defined on the directive
+    """
+    skip_settings = options.get("skip", None)
+    if skip_settings is None:
+        skip_settings = app.config.docleaf_doxygen_skip
+    else:
+        skip_settings = skip_settings.split(",")
+    return skip_settings
+
+
+class XmlFileInfo:
+    def __init__(self, hash, rst_files):
+        self.hash = hash
+        self.rst_files = rst_files
+
+
+def hash_file(path):
+    logger.debug(f"docleaf: hashing {path}")
+    if sys.version_info >= (3, 11):
+        with open(path, "rb") as f:
+            digest = hashlib.file_digest(f, "sha1")
+            return digest.hexdigest()
+    else:
+        contents = open(path, "rb").read()
+        hash = hashlib.sha1()
+        hash.update(contents)
+        return hash.hexdigest()
+
+
+def update_sphinx_env_file_data(env: BuildEnvironment, xml_paths: List[str], rst_file: str):
+    """
+    Update our file_data store to indicate which rst files are dependent on which xml files
+    """
+    if not hasattr(env, "docleaf_file_data"):
+        env.docleaf_file_data = {}
+
+    for path in xml_paths:
+        if path in env.docleaf_file_data:
+            env.docleaf_file_data[path].rst_files.add(rst_file)
+        else:
+            env.docleaf_file_data[path] = XmlFileInfo(hash_file(path), set([rst_file]))
+
+
+def calculate_files_to_refresh(app: Sphinx, env, added, changed, removed):
+    """
+    Sphinx tells us which rst files have changed on disk and we can tell it (by returning a list of doc names) which
+    documents need to be re-read and have their output re-generated.
+
+    We calculate which files to refresh by storing the last build time and comparing the modified time of each xml file
+    against the last build time and see if any are newer. From there we need to get from the xml files to the rst files
+    that they impact and return those rst files to be refreshed.
+    """
+    logger.debug("docleaf: calculate_files_to_refresh")
+
+    # Get the last build time before updating it
+    last_build_time = getattr(app.env, "docleaf_last_build_time", None)
+
+    # Store the current time as the build time
+    app.env.docleaf_last_build_time = time.time()
+
+    if not last_build_time:
+        return []
+
+    if not hasattr(app.env, "docleaf_file_data"):
+        return []
+
+    rst_files_to_refresh = set()
+
+    for xml_file_path, info in app.env.docleaf_file_data.items():
+        stat = os.stat(xml_file_path)
+        if stat.st_mtime > last_build_time:
+            hash = hash_file(xml_file_path)
+            logger.debug(f"docleaf: stored hash for {xml_file_path} = {hash}. Calculated hash: {info.hash}")
+            if hash != info.hash:
+                # Store the new hash
+                info.hash = hash
+                # Tell Sphinx to refresh all rst files associated with this file
+                rst_files_to_refresh.update(info.rst_files)
+
+    logger.verbose(f"docleaf: calculate_files_to_refresh - Rebuild: {rst_files_to_refresh}")
+    return rst_files_to_refresh
+
+
+def purge_file_data(app, env, docname):
+    """
+    Clear any file data associated with 'docname' in accordance with the Sphinx API
+    """
+    logger.debug("docleaf: purge_file_data - %s", docname)
+    if not hasattr(app.env, "docleaf_file_data"):
+        return
+
+    for xml_file_path, info in app.env.docleaf_file_data.items():
+        info.rst_files.discard(docname)
+
+
+class ExtensionContext:
+    def __init__(self, app: Sphinx, cache):
+        self.app = app
+        self.cache = cache
+
+
+def add_directive(context, name, Cls):
+    Cls.app = context.app
+    Cls.cache = context.cache
+    context.app.add_directive(name, Cls)
+
+
+def setup(app: Sphinx):
+    cache = backend.FileCache()
+
+    context = ExtensionContext(app, cache)
+
+    add_directive(context, "doxygenclass", ClassDirective)
+    add_directive(context, "doxygenenum", EnumDirective)
+    add_directive(context, "doxygenfunction", FunctionDirective)
+    add_directive(context, "doxygengroup", GroupDirective)
+    add_directive(context, "doxygenstruct", StructDirective)
+
+    app.add_config_value("docleaf_projects", {}, "env")
+    app.add_config_value("docleaf_default_project", None, "env")
+    app.add_config_value("docleaf_doxygen_skip", [], "env")
+    app.add_config_value("docleaf_domain_by_extension", {}, True)
+
+    app.connect("env-get-outdated", calculate_files_to_refresh)
+    app.connect("env-purge-doc", purge_file_data)
+
+    return {"version": __version__, "parallel_read_safe": True, "parallel_write_safe": True}
```

## docleaf/errors.py

 * *Ordering differences only*

```diff
@@ -1,6 +1,6 @@
-class DocleafError(Exception):
-    """
-    Standard error type for docleaf
-    """
-
-    pass
+class DocleafError(Exception):
+    """
+    Standard error type for docleaf
+    """
+
+    pass
```

## Comparing `docleaf-0.8.2.dist-info/METADATA` & `docleaf-0.8.3.dist-info/METADATA`

 * *Files 24% similar despite different names*

```diff
@@ -1,206 +1,213 @@
 Metadata-Version: 2.1
 Name: docleaf
-Version: 0.8.2
+Version: 0.8.3
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Sphinx :: Extension
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Documentation
 Requires-Dist: docutils>=0.12
 Requires-Dist: Sphinx>=4.0,!=5.0.0
 License-File: LICENSE.md
 License-File: LICENSES_THIRD_PARTY.md
 Summary: Integrate your doxygen-generated technical documentation into Sphinx
 Keywords: sphinx,doxygen
 Author-email: Michael Jones <michael.jones@docleaf.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
-Project-URL: repository, https://github.com/docleaf-labs/docleaf
 Project-URL: homepage, https://docleaf.io
+Project-URL: repository, https://github.com/docleaf-labs/docleaf
 Project-URL: changelog, https://github.com/docleaf-labs/docleaf/blob/main/CHANGELOG.md
 
-<h1 align="center">
-  Docleaf
-</h1>
-
-<p align="center">
-   Your technical docs, beautifully integrated
-</p>
-
-Docleaf smoothly integrates your technical and long-form documentation. It is a Sphinx extension which reads Doxygen
-XML output and formats the information seamlessly with your user documentation.
-
-## License
-
-Docleaf is licensed under the [Parity Public License](./LICENSE.md). The Parity license allows permissive use of 
-Docleaf to help document open source projects. If you have a closed source project that you would like to document with
-Docleaf then you must purchase a commercial license.
-
-For further information please email: [support@docleaf.io](mailto:support@docleaf.io)
-
-## Features
-
-- Custom directives allowing you to target various parts of C and C++ code bases.
-- Integration with Sphinx C and C++ domains to support easily linking to your generated output.
-- Hash-based content checks, as well as timestamp checks, to minimize incremental build times after a Doxygen run.
-- Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
-  repository.
-
-## Installation
-
-Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
-
-```
-pip install docleaf
-```
-
-## Usage
-
-Include `docleaf.doxygen` as an extension in your Sphinx `conf.py` file:
-
-```python
-extensions = ["docleaf.doxygen"]
-```
-
-Configure the extension to know where your source code is stored and the Doxygen XML output has been generated for
-your project. Optionally set the default project:
-
-```python
-docleaf_projects = {
-  "my_project": {
-    "root": "../src",
-    "xml": "../doxygen/xml"
-  }
-
-}
-docleaf_default_project = "my_project"
-```
-
-The use the provided directives in your reStructuredText files:
-
-```rst
-.. doxygenstruct:: ExampleStruct
-```
-
-See below for available directives.
-
-### Directives
-
-Generate documentation for a C++ class.
-
-```rst
-.. doxygenclass:: ClassName
-```
-
-Generate documentation for a C or C++ struct.
-
-```rst
-.. doxygenstruct:: StructName
-```
-
-Generate documentation for a C or C++ function.
-
-```rst
-.. doxygenfunction:: function_name
-```
-
-Generate documentation for a C or C++ enum.
-
-```rst
-.. doxygenenum:: EnumName
-```
-
-Generate documentation for specific group as specified within your Doxygen set up and code comments.
-
-```rst
-.. doxygengroup:: group_name
-```
-
-All directives take a `:project:` option to specify the project to use from your `conf.py` if you don't want to use
-the default project.
-
-### Settings
-
-- `docleaf_projects` 
-
-  A Python dictionary mapping each project name to the folders where its source code and Doxygen XML output are stored.
-
-- `docleaf_default_project`
-
-  The default project to use when none is specified on the directive itself.
-  
-- `docleaf_domain_by_extension`
-
-  A Python dictionary mapping from file extension to Sphinx domain. Docleaf uses Doxygen's language classifications
-  where possible but for optimal control of how source files are classified it is useful to use this setting. For
-  example:
-
-  ```python
-  docleaf_domain_by_extension = {"hpp": "cpp", "h": "c"}
-  ```
-
-  Will make sure that all files that end in `.hpp` will be considered as C++ files and processed using the C++ Sphinx
-  domain whilst files that end in `.h` will be considered C files and processed with the C Sphinx domain.
-
-- `docleaf_doxygen_skip`
-
-  A list of instructions describing any parts of the Doxygen XML to skip when generating the output documentation.
-  Supported entries are:
-
-  - `members:all_caps` - Skips any function or variable members (as defined as a 'memberdef' by Doxygen) which have 
-    names which are all capital letters and underscores. This is to allow users to filter our unprocessed C/C++ macros
-    if desirable.
-  - `xml-nodes:<node name>` - Skips reading and process of the given XML node and its children in the Doxygen XML 
-    output. Support is limited to the `htmlonly` node.
-
-### Integration with `sphinx.ext.linkcode`
-
-Docleaf can integrate with the `sphinx.ext.linkcode` extension in order to add `[source]` links next to various
-supported entries in your documentation. Linking to GitHub based repositories is supported.
-
-In order to use it, add the `sphinx.ext.linkcode` extension to the `extensions` list in your Sphinx `conf.py` and use
-the `docleaf.doxygen.GitHubLinkResolver` with appropriate parameters for your repository.
-
-```python
-extensions = [
-  "docleaf.doxygen",
-  "sphinx.ext.linkcode",
-  ]
-
-linkcode_resolve = docleaf.doxygen.GitHubLinkResolver(
-    root="../../../", user="docleaf-labs", repo="docleaf", branch="main"
-)
-```
-
-Where:
-- `root` is the relative path to the root of your repository.
-- `user` is the user or organisation name for your GitHub repository.
-- `repo` is the name of your GitHub repository.
-- `tag` is the git tag that you would like the generated link URLs to target.
-- `branch` is the git branch that you would like the generated link URLs to target.
-- `commit` is the git commit SHA that you would like the generated link URLs to target.
-
-Only one of `tag`, `branch` and `commit` is necessary.
-
-
-## Performance
-
-When doing a clean build of the Zephyr RTOS documentation suite, Docleaf is 2.1x faster than Breathe.
-
-```
-Benchmark: docleaf
-  Time (mean ± σ):     180.383 s ±  3.213 s    [User: 448.242 s, System: 12.908 s]
-  Range (min … max):   175.695 s … 185.187 s    10 runs
-```
-
-```
-Benchmark: breathe
-  Time (mean ± σ):     389.658 s ±  5.271 s    [User: 1839.366 s, System: 24.895 s]
-  Range (min … max):   379.093 s … 394.315 s    10 runs
-```
-
-## History
-
-Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
-It was created to resolve some of the performance and memory consumption issues with Breathe by rewriting the code
-base to use Rust. The user experience is designed to match and improve on Breathe.
+<h1 align="center">
+  Docleaf
+</h1>
+
+<p align="center">
+   Your technical docs, beautifully integrated
+</p>
+
+Docleaf smoothly integrates your technical and long-form documentation. It is a Sphinx extension which reads Doxygen
+XML output and formats the information seamlessly with your user documentation.
+
+- [License](#license)
+- [Features](#features)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Performance](#performance)
+- [History](#history)
+
+## License
+
+Docleaf is licensed under the [Parity Public License](./LICENSE.md). The Parity license allows permissive use of 
+Docleaf to help document open source projects. If you have a closed source project that you would like to document with
+Docleaf then you must purchase a commercial license. Please see the [Docleaf Pricing](https://docleaf.io/pricing) page for more information.
+
+If you have any questions please email: [support@docleaf.io](mailto:support@docleaf.io)
+
+## Features
+
+- Custom directives allowing you to target various parts of C and C++ code bases.
+- Integration with Sphinx C and C++ domains to support easily linking to your generated output.
+- Hash-based content checks, as well as timestamp checks, to minimize incremental build times after a Doxygen run.
+- Integration with the `sphinx.ext.linkcode` extension to support links to source code locations in a GitHub
+  repository.
+
+## Installation
+
+Docleaf can be installed from [PyPI](https://pypi.org/project/docleaf/):
+
+```
+pip install docleaf
+```
+
+## Usage
+
+Include `docleaf.doxygen` as an extension in your Sphinx `conf.py` file:
+
+```python
+extensions = ["docleaf.doxygen"]
+```
+
+Configure the extension to know where your source code is stored and the Doxygen XML output has been generated for
+your project. Optionally set the default project:
+
+```python
+docleaf_projects = {
+  "my_project": {
+    "root": "../src",
+    "xml": "../doxygen/xml"
+  }
+
+}
+docleaf_default_project = "my_project"
+```
+
+The use the provided directives in your reStructuredText files:
+
+```rst
+.. doxygenstruct:: ExampleStruct
+```
+
+See below for available directives.
+
+### Directives
+
+Generate documentation for a C++ class.
+
+```rst
+.. doxygenclass:: ClassName
+```
+
+Generate documentation for a C or C++ struct.
+
+```rst
+.. doxygenstruct:: StructName
+```
+
+Generate documentation for a C or C++ function.
+
+```rst
+.. doxygenfunction:: function_name
+```
+
+Generate documentation for a C or C++ enum.
+
+```rst
+.. doxygenenum:: EnumName
+```
+
+Generate documentation for specific group as specified within your Doxygen set up and code comments.
+
+```rst
+.. doxygengroup:: group_name
+```
+
+All directives take a `:project:` option to specify the project to use from your `conf.py` if you don't want to use
+the default project.
+
+### Settings
+
+- `docleaf_projects` 
+
+  A Python dictionary mapping each project name to the folders where its source code and Doxygen XML output are stored.
+
+- `docleaf_default_project`
+
+  The default project to use when none is specified on the directive itself.
+  
+- `docleaf_domain_by_extension`
+
+  A Python dictionary mapping from file extension to Sphinx domain. Docleaf uses Doxygen's language classifications
+  where possible but for optimal control of how source files are classified it is useful to use this setting. For
+  example:
+
+  ```python
+  docleaf_domain_by_extension = {"hpp": "cpp", "h": "c"}
+  ```
+
+  Will make sure that all files that end in `.hpp` will be considered as C++ files and processed using the C++ Sphinx
+  domain whilst files that end in `.h` will be considered C files and processed with the C Sphinx domain.
+
+- `docleaf_doxygen_skip`
+
+  A list of instructions describing any parts of the Doxygen XML to skip when generating the output documentation.
+  Supported entries are:
+
+  - `members:all_caps` - Skips any function or variable members (as defined as a 'memberdef' by Doxygen) which have 
+    names which are all capital letters and underscores. This is to allow users to filter our unprocessed C/C++ macros
+    if desirable.
+  - `xml-nodes:<node name>` - Skips reading and process of the given XML node and its children in the Doxygen XML 
+    output. Support is limited to the `htmlonly` node.
+
+### Integration with `sphinx.ext.linkcode`
+
+Docleaf can integrate with the `sphinx.ext.linkcode` extension in order to add `[source]` links next to various
+supported entries in your documentation. Linking to GitHub based repositories is supported.
+
+In order to use it, add the `sphinx.ext.linkcode` extension to the `extensions` list in your Sphinx `conf.py` and use
+the `docleaf.doxygen.GitHubLinkResolver` with appropriate parameters for your repository.
+
+```python
+extensions = [
+  "docleaf.doxygen",
+  "sphinx.ext.linkcode",
+  ]
+
+linkcode_resolve = docleaf.doxygen.GitHubLinkResolver(
+    root="../../../", user="docleaf-labs", repo="docleaf", branch="main"
+)
+```
+
+Where:
+- `root` is the relative path to the root of your repository.
+- `user` is the user or organisation name for your GitHub repository.
+- `repo` is the name of your GitHub repository.
+- `tag` is the git tag that you would like the generated link URLs to target.
+- `branch` is the git branch that you would like the generated link URLs to target.
+- `commit` is the git commit SHA that you would like the generated link URLs to target.
+
+Only one of `tag`, `branch` and `commit` is necessary.
+
+
+## Performance
+
+When doing a clean build of the Zephyr RTOS documentation suite, Docleaf is 2.1x faster than Breathe.
+
+```
+Benchmark: docleaf
+  Time (mean ± σ):     180.383 s ±  3.213 s    [User: 448.242 s, System: 12.908 s]
+  Range (min … max):   175.695 s … 185.187 s    10 runs
+```
+
+```
+Benchmark: breathe
+  Time (mean ± σ):     389.658 s ±  5.271 s    [User: 1839.366 s, System: 24.895 s]
+  Range (min … max):   379.093 s … 394.315 s    10 runs
+```
+
+## History
+
+Docleaf is written and maintained by the creator of the [Breathe](https://github.com/breathe-doc/breathe) project.
+It was created to resolve some of the performance and memory consumption issues with Breathe by rewriting the code
+base to use Rust. The user experience is designed to match and improve on Breathe.
```

## Comparing `docleaf-0.8.2.dist-info/license_files/LICENSE.md` & `docleaf-0.8.3.dist-info/license_files/LICENSE.md`

 * *Ordering differences only*

 * *Files 8% similar despite different names*

```diff
@@ -1,71 +1,71 @@
-# The Parity Public License 7.0.0
-
-Contributor: Michael Jones
-
-Source Code: https://github.com/docleaf-labs/docleaf
-
-## Purpose
-
-This license allows you to use and share this software for free, but you have to share software that builds on it alike.
-
-## Agreement
-
-In order to receive this license, you have to agree to its rules.  Those rules are both obligations under that agreement and conditions to your license.  Don't do anything with this software that triggers a rule you can't or won't follow.
-
-## Notices
-
-Make sure everyone who gets a copy of any part of this software from you, with or without changes, also gets the text of this license and the contributor and source code lines above.
-
-## Copyleft
-
-[Contribute](#contribute) software you develop, operate, or analyze with this software, including changes or additions to this software.  When in doubt, [contribute](#contribute).
-
-## Prototypes
-
-You don't have to [contribute](#contribute) any change, addition, or other software that meets all these criteria:
-
-1.  You don't use it for more than thirty days.
-
-2.  You don't share it outside the team developing it, other than for non-production user testing.
-
-3.  You don't develop, operate, or analyze other software with it for anyone outside the team developing it.
-
-## Reverse Engineering
-
-You may use this software to operate and analyze software you can't [contribute](#contribute) in order to develop alternatives you can and do [contribute](#contribute).
-
-## Contribute
-
-To [contribute](#contribute) software:
-
-1.  Publish all source code for the software in the preferred form for making changes through a freely accessible distribution system widely used for similar source code so the contributor and others can find and copy it.
-
-2.  Make sure every part of the source code is available under this license or another license that allows everything this license does, such as [the Blue Oak Model License 1.0.0](https://blueoakcouncil.org/license/1.0.0), [the Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html), [the MIT license](https://spdx.org/licenses/MIT.html), or [the two-clause BSD license](https://spdx.org/licenses/BSD-2-Clause.html).
-
-3.  Take these steps within thirty days.
-
-4.  Note that this license does _not_ allow you to change the license terms for this software.  You must follow [Notices](#notices).
-
-## Excuse
-
-You're excused for unknowingly breaking [Copyleft](#copyleft) if you [contribute](#contribute) as required, or stop doing anything requiring this license, within thirty days of learning you broke the rule.  You're excused for unknowingly breaking [Notices](#notices) if you take all practical steps to comply within thirty days of learning you broke the rule.
-
-## Defense
-
-Don't make any legal claim against anyone accusing this software, with or without changes, alone or with other technology, of infringing any patent.
-
-## Copyright
-
-The contributor licenses you to do everything with this software that would otherwise infringe their copyright in it.
-
-## Patent
-
-The contributor licenses you to do everything with this software that would otherwise infringe any patents they can license or become able to license.
-
-## Reliability
-
-The contributor can't revoke this license.
-
-## No Liability
-
-***As far as the law allows, this software comes as is, without any warranty or condition, and the contributor won't be liable to anyone for any damages related to this software or this license, under any kind of legal claim.***
+# The Parity Public License 7.0.0
+
+Contributor: Michael Jones
+
+Source Code: https://github.com/docleaf-labs/docleaf
+
+## Purpose
+
+This license allows you to use and share this software for free, but you have to share software that builds on it alike.
+
+## Agreement
+
+In order to receive this license, you have to agree to its rules.  Those rules are both obligations under that agreement and conditions to your license.  Don't do anything with this software that triggers a rule you can't or won't follow.
+
+## Notices
+
+Make sure everyone who gets a copy of any part of this software from you, with or without changes, also gets the text of this license and the contributor and source code lines above.
+
+## Copyleft
+
+[Contribute](#contribute) software you develop, operate, or analyze with this software, including changes or additions to this software.  When in doubt, [contribute](#contribute).
+
+## Prototypes
+
+You don't have to [contribute](#contribute) any change, addition, or other software that meets all these criteria:
+
+1.  You don't use it for more than thirty days.
+
+2.  You don't share it outside the team developing it, other than for non-production user testing.
+
+3.  You don't develop, operate, or analyze other software with it for anyone outside the team developing it.
+
+## Reverse Engineering
+
+You may use this software to operate and analyze software you can't [contribute](#contribute) in order to develop alternatives you can and do [contribute](#contribute).
+
+## Contribute
+
+To [contribute](#contribute) software:
+
+1.  Publish all source code for the software in the preferred form for making changes through a freely accessible distribution system widely used for similar source code so the contributor and others can find and copy it.
+
+2.  Make sure every part of the source code is available under this license or another license that allows everything this license does, such as [the Blue Oak Model License 1.0.0](https://blueoakcouncil.org/license/1.0.0), [the Apache License 2.0](https://www.apache.org/licenses/LICENSE-2.0.html), [the MIT license](https://spdx.org/licenses/MIT.html), or [the two-clause BSD license](https://spdx.org/licenses/BSD-2-Clause.html).
+
+3.  Take these steps within thirty days.
+
+4.  Note that this license does _not_ allow you to change the license terms for this software.  You must follow [Notices](#notices).
+
+## Excuse
+
+You're excused for unknowingly breaking [Copyleft](#copyleft) if you [contribute](#contribute) as required, or stop doing anything requiring this license, within thirty days of learning you broke the rule.  You're excused for unknowingly breaking [Notices](#notices) if you take all practical steps to comply within thirty days of learning you broke the rule.
+
+## Defense
+
+Don't make any legal claim against anyone accusing this software, with or without changes, alone or with other technology, of infringing any patent.
+
+## Copyright
+
+The contributor licenses you to do everything with this software that would otherwise infringe their copyright in it.
+
+## Patent
+
+The contributor licenses you to do everything with this software that would otherwise infringe any patents they can license or become able to license.
+
+## Reliability
+
+The contributor can't revoke this license.
+
+## No Liability
+
+***As far as the law allows, this software comes as is, without any warranty or condition, and the contributor won't be liable to anyone for any damages related to this software or this license, under any kind of legal claim.***
```

## Comparing `docleaf-0.8.2.dist-info/license_files/LICENSES_THIRD_PARTY.md` & `docleaf-0.8.3.dist-info/license_files/LICENSES_THIRD_PARTY.md`

 * *Ordering differences only*

 * *Files 10% similar despite different names*

```diff
@@ -1,3000 +1,3000 @@
-Third Party Licenses
-====================
-
-This file contains all the open source licenses for the Rust crates that
-Docleaf depends on. It has been created so that it is bundled into the 
-wheel so that the licenses are appropriately distributed with the compiled
-code.
-
-This file is generated by 'rust/script/licenses.py' and placed here so that
-it is picked up and package by maturin. See: 
-
-    https://github.com/PyO3/maturin/pull/862
-
-
-aho-corasick (0.7.19)
-=====================
-
-The MIT License (MIT)
-
-Copyright (c) 2015 Andrew Gallant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-anyhow (1.0.65)
-===============
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-atty (0.2.14)
-=============
-
-Copyright (c) 2015-2019 Doug Tangren
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-bitflags (1.3.2)
-================
-
-Copyright (c) 2014 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-cfg-if (1.0.0)
-==============
-
-Copyright (c) 2014 Alex Crichton
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-either (1.8.1)
-==============
-
-Copyright (c) 2015
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-env_logger (0.9.0)
-==================
-
-Copyright (c) 2014 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-heck (0.4.1)
-============
-
-Copyright (c) 2015 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-hermit-abi (0.1.19)
-===================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-html-escape (0.2.13)
-====================
-
-MIT License
-
-Copyright (c) 2020 magiclen.org (Ron Li)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-humantime (2.1.0)
-=================
-
-Copyright (c) 2016 The humantime Developers
-
-Includes parts of http date with the following copyright:
-Copyright (c) 2016 Pyfisch
-
-Includes portions of musl libc with the following copyright:
-Copyright © 2005-2013 Rich Felker
-
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-indoc (1.0.7)
-=============
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-itertools (0.10.5)
-==================
-
-Copyright (c) 2015
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-lazy_static (1.4.0)
-===================
-
-Copyright (c) 2010 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-libc (0.2.132)
-==============
-
-Copyright (c) 2014-2020 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-lock_api (0.4.8)
-================
-
-Copyright (c) 2016 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-log (0.4.17)
-============
-
-Copyright (c) 2014 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-matchers (0.1.0)
-================
-
-Copyright (c) 2019 Eliza Weisman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-memchr (2.5.0)
-==============
-
-The MIT License (MIT)
-
-Copyright (c) 2015 Andrew Gallant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-nu-ansi-term (0.46.0)
-=====================
-
-The MIT License (MIT)
-
-Copyright (c) 2014 Benjamin Sago
-Copyright (c) 2021-2022 The Nushell Project Developers
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-once_cell (1.14.0)
-==================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-overload (0.1.1)
-================
-
-MIT License
-
-Copyright (c) 2019 Daniel Augusto Rizzi Salvadori
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-parking_lot (0.12.1)
-====================
-
-Copyright (c) 2016 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-parking_lot_core (0.9.3)
-========================
-
-Copyright (c) 2016 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-pin-project-lite (0.2.9)
-========================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-proc-macro2 (1.0.58)
-====================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-pyo3 (0.16.6)
-=============
-
-Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-
-pyo3-ffi (0.16.6)
-=================
-
-A. HISTORY OF THE SOFTWARE
-==========================
-
-Python was created in the early 1990s by Guido van Rossum at Stichting
-Mathematisch Centrum (CWI, see http://www.cwi.nl) in the Netherlands
-as a successor of a language called ABC.  Guido remains Python's
-principal author, although it includes many contributions from others.
-
-In 1995, Guido continued his work on Python at the Corporation for
-National Research Initiatives (CNRI, see http://www.cnri.reston.va.us)
-in Reston, Virginia where he released several versions of the
-software.
-
-In May 2000, Guido and the Python core development team moved to
-BeOpen.com to form the BeOpen PythonLabs team.  In October of the same
-year, the PythonLabs team moved to Digital Creations (now Zope
-Corporation, see http://www.zope.com).  In 2001, the Python Software
-Foundation (PSF, see http://www.python.org/psf/) was formed, a
-non-profit organization created specifically to own Python-related
-Intellectual Property.  Zope Corporation is a sponsoring member of
-the PSF.
-
-All Python releases are Open Source (see http://www.opensource.org for
-the Open Source Definition).  Historically, most, but not all, Python
-releases have also been GPL-compatible; the table below summarizes
-the various releases.
-
-    Release         Derived     Year        Owner       GPL-
-                    from                                compatible? (1)
-
-    0.9.0 thru 1.2              1991-1995   CWI         yes
-    1.3 thru 1.5.2  1.2         1995-1999   CNRI        yes
-    1.6             1.5.2       2000        CNRI        no
-    2.0             1.6         2000        BeOpen.com  no
-    1.6.1           1.6         2001        CNRI        yes (2)
-    2.1             2.0+1.6.1   2001        PSF         no
-    2.0.1           2.0+1.6.1   2001        PSF         yes
-    2.1.1           2.1+2.0.1   2001        PSF         yes
-    2.1.2           2.1.1       2002        PSF         yes
-    2.1.3           2.1.2       2002        PSF         yes
-    2.2 and above   2.1.1       2001-now    PSF         yes
-
-Footnotes:
-
-(1) GPL-compatible doesn't mean that we're distributing Python under
-    the GPL.  All Python licenses, unlike the GPL, let you distribute
-    a modified version without making your changes open source.  The
-    GPL-compatible licenses make it possible to combine Python with
-    other software that is released under the GPL; the others don't.
-
-(2) According to Richard Stallman, 1.6.1 is not GPL-compatible,
-    because its license has a choice of law clause.  According to
-    CNRI, however, Stallman's lawyer has told CNRI's lawyer that 1.6.1
-    is "not incompatible" with the GPL.
-
-Thanks to the many outside volunteers who have worked under Guido's
-direction to make these releases possible.
-
-
-B. TERMS AND CONDITIONS FOR ACCESSING OR OTHERWISE USING PYTHON
-===============================================================
-
-PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
---------------------------------------------
-
-1. This LICENSE AGREEMENT is between the Python Software Foundation
-("PSF"), and the Individual or Organization ("Licensee") accessing and
-otherwise using this software ("Python") in source or binary form and
-its associated documentation.
-
-2. Subject to the terms and conditions of this License Agreement, PSF hereby
-grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce,
-analyze, test, perform and/or display publicly, prepare derivative works,
-distribute, and otherwise use Python alone or in any derivative version,
-provided, however, that PSF's License Agreement and PSF's notice of copyright,
-i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
-2011, 2012, 2013, 2014, 2015 Python Software Foundation; All Rights Reserved"
-are retained in Python alone or in any derivative version prepared by Licensee.
-
-3. In the event Licensee prepares a derivative work that is based on
-or incorporates Python or any part thereof, and wants to make
-the derivative work available to others as provided herein, then
-Licensee hereby agrees to include in any such work a brief summary of
-the changes made to Python.
-
-4. PSF is making Python available to Licensee on an "AS IS"
-basis.  PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
-IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND
-DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
-FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON WILL NOT
-INFRINGE ANY THIRD PARTY RIGHTS.
-
-5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
-FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
-A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON,
-OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-6. This License Agreement will automatically terminate upon a material
-breach of its terms and conditions.
-
-7. Nothing in this License Agreement shall be deemed to create any
-relationship of agency, partnership, or joint venture between PSF and
-Licensee.  This License Agreement does not grant permission to use PSF
-trademarks or trade name in a trademark sense to endorse or promote
-products or services of Licensee, or any third party.
-
-8. By copying, installing or otherwise using Python, Licensee
-agrees to be bound by the terms and conditions of this License
-Agreement.
-
-
-BEOPEN.COM LICENSE AGREEMENT FOR PYTHON 2.0
--------------------------------------------
-
-BEOPEN PYTHON OPEN SOURCE LICENSE AGREEMENT VERSION 1
-
-1. This LICENSE AGREEMENT is between BeOpen.com ("BeOpen"), having an
-office at 160 Saratoga Avenue, Santa Clara, CA 95051, and the
-Individual or Organization ("Licensee") accessing and otherwise using
-this software in source or binary form and its associated
-documentation ("the Software").
-
-2. Subject to the terms and conditions of this BeOpen Python License
-Agreement, BeOpen hereby grants Licensee a non-exclusive,
-royalty-free, world-wide license to reproduce, analyze, test, perform
-and/or display publicly, prepare derivative works, distribute, and
-otherwise use the Software alone or in any derivative version,
-provided, however, that the BeOpen Python License is retained in the
-Software, alone or in any derivative version prepared by Licensee.
-
-3. BeOpen is making the Software available to Licensee on an "AS IS"
-basis.  BEOPEN MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
-IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, BEOPEN MAKES NO AND
-DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
-FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF THE SOFTWARE WILL NOT
-INFRINGE ANY THIRD PARTY RIGHTS.
-
-4. BEOPEN SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF THE
-SOFTWARE FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS
-AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THE SOFTWARE, OR ANY
-DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-5. This License Agreement will automatically terminate upon a material
-breach of its terms and conditions.
-
-6. This License Agreement shall be governed by and interpreted in all
-respects by the law of the State of California, excluding conflict of
-law provisions.  Nothing in this License Agreement shall be deemed to
-create any relationship of agency, partnership, or joint venture
-between BeOpen and Licensee.  This License Agreement does not grant
-permission to use BeOpen trademarks or trade names in a trademark
-sense to endorse or promote products or services of Licensee, or any
-third party.  As an exception, the "BeOpen Python" logos available at
-http://www.pythonlabs.com/logos.html may be used according to the
-permissions granted on that web page.
-
-7. By copying, installing or otherwise using the software, Licensee
-agrees to be bound by the terms and conditions of this License
-Agreement.
-
-
-CNRI LICENSE AGREEMENT FOR PYTHON 1.6.1
----------------------------------------
-
-1. This LICENSE AGREEMENT is between the Corporation for National
-Research Initiatives, having an office at 1895 Preston White Drive,
-Reston, VA 20191 ("CNRI"), and the Individual or Organization
-("Licensee") accessing and otherwise using Python 1.6.1 software in
-source or binary form and its associated documentation.
-
-2. Subject to the terms and conditions of this License Agreement, CNRI
-hereby grants Licensee a nonexclusive, royalty-free, world-wide
-license to reproduce, analyze, test, perform and/or display publicly,
-prepare derivative works, distribute, and otherwise use Python 1.6.1
-alone or in any derivative version, provided, however, that CNRI's
-License Agreement and CNRI's notice of copyright, i.e., "Copyright (c)
-1995-2001 Corporation for National Research Initiatives; All Rights
-Reserved" are retained in Python 1.6.1 alone or in any derivative
-version prepared by Licensee.  Alternately, in lieu of CNRI's License
-Agreement, Licensee may substitute the following text (omitting the
-quotes): "Python 1.6.1 is made available subject to the terms and
-conditions in CNRI's License Agreement.  This Agreement together with
-Python 1.6.1 may be located on the Internet using the following
-unique, persistent identifier (known as a handle): 1895.22/1013.  This
-Agreement may also be obtained from a proxy server on the Internet
-using the following URL: http://hdl.handle.net/1895.22/1013".
-
-3. In the event Licensee prepares a derivative work that is based on
-or incorporates Python 1.6.1 or any part thereof, and wants to make
-the derivative work available to others as provided herein, then
-Licensee hereby agrees to include in any such work a brief summary of
-the changes made to Python 1.6.1.
-
-4. CNRI is making Python 1.6.1 available to Licensee on an "AS IS"
-basis.  CNRI MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
-IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, CNRI MAKES NO AND
-DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
-FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON 1.6.1 WILL NOT
-INFRINGE ANY THIRD PARTY RIGHTS.
-
-5. CNRI SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
-1.6.1 FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
-A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON 1.6.1,
-OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
-
-6. This License Agreement will automatically terminate upon a material
-breach of its terms and conditions.
-
-7. This License Agreement shall be governed by the federal
-intellectual property law of the United States, including without
-limitation the federal copyright law, and, to the extent such
-U.S. federal law does not apply, by the law of the Commonwealth of
-Virginia, excluding Virginia's conflict of law provisions.
-Notwithstanding the foregoing, with regard to derivative works based
-on Python 1.6.1 that incorporate non-separable material that was
-previously distributed under the GNU General Public License (GPL), the
-law of the Commonwealth of Virginia shall govern this License
-Agreement only as to issues arising under or with respect to
-Paragraphs 4, 5, and 7 of this License Agreement.  Nothing in this
-License Agreement shall be deemed to create any relationship of
-agency, partnership, or joint venture between CNRI and Licensee.  This
-License Agreement does not grant permission to use CNRI trademarks or
-trade name in a trademark sense to endorse or promote products or
-services of Licensee, or any third party.
-
-8. By clicking on the "ACCEPT" button where indicated, or by copying,
-installing or otherwise using Python 1.6.1, Licensee agrees to be
-bound by the terms and conditions of this License Agreement.
-
-        ACCEPT
-
-
-CWI LICENSE AGREEMENT FOR PYTHON 0.9.0 THROUGH 1.2
---------------------------------------------------
-
-Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam,
-The Netherlands.  All rights reserved.
-
-Permission to use, copy, modify, and distribute this software and its
-documentation for any purpose and without fee is hereby granted,
-provided that the above copyright notice appear in all copies and that
-both that copyright notice and this permission notice appear in
-supporting documentation, and that the name of Stichting Mathematisch
-Centrum or CWI not be used in advertising or publicity pertaining to
-distribution of the software without specific, written prior
-permission.
-
-STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO
-THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
-FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE
-FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
-WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
-ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
-OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
-
-
-Additional Conditions for this Windows binary build
----------------------------------------------------
-
-This program is linked with and uses Microsoft Distributable Code,
-copyrighted by Microsoft Corporation. The Microsoft Distributable Code
-includes the following files:
-
-msvcr90.dll
-msvcp90.dll
-msvcm90.dll
-
-If you further distribute programs that include the Microsoft
-Distributable Code, you must comply with the restrictions on
-distribution specified by Microsoft. In particular, you must require
-distributors and external end users to agree to terms that protect the
-Microsoft Distributable Code at least as much as Microsoft's own
-requirements for the Distributable Code. See Microsoft's documentation
-(included in its developer tools and on its website at microsoft.com)
-for specific details.
-
-Redistribution of the Windows binary build of the Python interpreter
-complies with this agreement, provided that you do not:
-
-- alter any copyright, trademark or patent notice in Microsoft's
-Distributable Code;
-
-- use Microsoft's trademarks in your programs' names or in a way that
-suggests your programs come from or are endorsed by Microsoft;
-
-- distribute Microsoft's Distributable Code to run on a platform other
-than Microsoft operating systems, run-time technologies or application
-platforms; or
-
-- include Microsoft Distributable Code in malicious, deceptive or
-unlawful programs.
-
-These restrictions apply only to the Microsoft Distributable Code as
-defined above, not to Python itself or any programs running on the
-Python interpreter. The redistribution of the Python interpreter and
-libraries is governed by the Python Software License included with this
-file, or by other licenses as marked.
-
-
-This copy of Python includes a copy of bzip2, which is licensed under the following terms:
-
-
---------------------------------------------------------------------------
-
-This program, "bzip2", the associated library "libbzip2", and all
-documentation, are copyright (C) 1996-2010 Julian R Seward.  All
-rights reserved.
-
-Redistribution and use in source and binary forms, with or without
-modification, are permitted provided that the following conditions
-are met:
-
-1. Redistributions of source code must retain the above copyright
-   notice, this list of conditions and the following disclaimer.
-
-2. The origin of this software must not be misrepresented; you must 
-   not claim that you wrote the original software.  If you use this 
-   software in a product, an acknowledgment in the product 
-   documentation would be appreciated but is not required.
-
-3. Altered source versions must be plainly marked as such, and must
-   not be misrepresented as being the original software.
-
-4. The name of the author may not be used to endorse or promote 
-   products derived from this software without specific prior written 
-   permission.
-
-THIS SOFTWARE IS PROVIDED BY THE AUTHOR ``AS IS'' AND ANY EXPRESS
-OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
-WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
-ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY
-DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
-DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
-GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
-INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
-WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
-NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
-SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
-
-Julian Seward, jseward@bzip.org
-bzip2/libbzip2 version 1.0.6 of 6 September 2010
-
---------------------------------------------------------------------------
-
-This copy of Python includes a copy of openssl, which is licensed under the following terms:
-
-
-  LICENSE ISSUES
-  ==============
-
-  The OpenSSL toolkit stays under a dual license, i.e. both the conditions of
-  the OpenSSL License and the original SSLeay license apply to the toolkit.
-  See below for the actual license texts. Actually both licenses are BSD-style
-  Open Source licenses. In case of any license issues related to OpenSSL
-  please contact openssl-core@openssl.org.
-
-  OpenSSL License
-  ---------------
-
-/* ====================================================================
- * Copyright (c) 1998-2011 The OpenSSL Project.  All rights reserved.
- *
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions
- * are met:
- *
- * 1. Redistributions of source code must retain the above copyright
- *    notice, this list of conditions and the following disclaimer. 
- *
- * 2. Redistributions in binary form must reproduce the above copyright
- *    notice, this list of conditions and the following disclaimer in
- *    the documentation and/or other materials provided with the
- *    distribution.
- *
- * 3. All advertising materials mentioning features or use of this
- *    software must display the following acknowledgment:
- *    "This product includes software developed by the OpenSSL Project
- *    for use in the OpenSSL Toolkit. (http://www.openssl.org/)"
- *
- * 4. The names "OpenSSL Toolkit" and "OpenSSL Project" must not be used to
- *    endorse or promote products derived from this software without
- *    prior written permission. For written permission, please contact
- *    openssl-core@openssl.org.
- *
- * 5. Products derived from this software may not be called "OpenSSL"
- *    nor may "OpenSSL" appear in their names without prior written
- *    permission of the OpenSSL Project.
- *
- * 6. Redistributions of any form whatsoever must retain the following
- *    acknowledgment:
- *    "This product includes software developed by the OpenSSL Project
- *    for use in the OpenSSL Toolkit (http://www.openssl.org/)"
- *
- * THIS SOFTWARE IS PROVIDED BY THE OpenSSL PROJECT ``AS IS'' AND ANY
- * EXPRESSED OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
- * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
- * PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE OpenSSL PROJECT OR
- * ITS CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
- * SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
- * NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
- * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
- * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
- * STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
- * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
- * OF THE POSSIBILITY OF SUCH DAMAGE.
- * ====================================================================
- *
- * This product includes cryptographic software written by Eric Young
- * (eay@cryptsoft.com).  This product includes software written by Tim
- * Hudson (tjh@cryptsoft.com).
- *
- */
-
- Original SSLeay License
- -----------------------
-
-/* Copyright (C) 1995-1998 Eric Young (eay@cryptsoft.com)
- * All rights reserved.
- *
- * This package is an SSL implementation written
- * by Eric Young (eay@cryptsoft.com).
- * The implementation was written so as to conform with Netscapes SSL.
- * 
- * This library is free for commercial and non-commercial use as long as
- * the following conditions are aheared to.  The following conditions
- * apply to all code found in this distribution, be it the RC4, RSA,
- * lhash, DES, etc., code; not just the SSL code.  The SSL documentation
- * included with this distribution is covered by the same copyright terms
- * except that the holder is Tim Hudson (tjh@cryptsoft.com).
- * 
- * Copyright remains Eric Young's, and as such any Copyright notices in
- * the code are not to be removed.
- * If this package is used in a product, Eric Young should be given attribution
- * as the author of the parts of the library used.
- * This can be in the form of a textual message at program startup or
- * in documentation (online or textual) provided with the package.
- * 
- * Redistribution and use in source and binary forms, with or without
- * modification, are permitted provided that the following conditions
- * are met:
- * 1. Redistributions of source code must retain the copyright
- *    notice, this list of conditions and the following disclaimer.
- * 2. Redistributions in binary form must reproduce the above copyright
- *    notice, this list of conditions and the following disclaimer in the
- *    documentation and/or other materials provided with the distribution.
- * 3. All advertising materials mentioning features or use of this software
- *    must display the following acknowledgement:
- *    "This product includes cryptographic software written by
- *     Eric Young (eay@cryptsoft.com)"
- *    The word 'cryptographic' can be left out if the rouines from the library
- *    being used are not cryptographic related :-).
- * 4. If you include any Windows specific code (or a derivative thereof) from 
- *    the apps directory (application code) you must include an acknowledgement:
- *    "This product includes software written by Tim Hudson (tjh@cryptsoft.com)"
- * 
- * THIS SOFTWARE IS PROVIDED BY ERIC YOUNG ``AS IS'' AND
- * ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
- * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
- * ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
- * FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
- * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
- * OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
- * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
- * LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
- * OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
- * SUCH DAMAGE.
- * 
- * The licence and distribution terms for any publically available version or
- * derivative of this code cannot be changed.  i.e. this code cannot simply be
- * copied and put under another distribution licence
- * [including the GNU Public Licence.]
- */
-
-
-This copy of Python includes a copy of Tcl, which is licensed under the following terms:
-
-This software is copyrighted by the Regents of the University of
-California, Sun Microsystems, Inc., Scriptics Corporation, ActiveState
-Corporation and other parties.  The following terms apply to all files
-associated with the software unless explicitly disclaimed in
-individual files.
-
-The authors hereby grant permission to use, copy, modify, distribute,
-and license this software and its documentation for any purpose, provided
-that existing copyright notices are retained in all copies and that this
-notice is included verbatim in any distributions. No written agreement,
-license, or royalty fee is required for any of the authorized uses.
-Modifications to this software may be copyrighted by their authors
-and need not follow the licensing terms described here, provided that
-the new terms are clearly indicated on the first page of each file where
-they apply.
-
-IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
-FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
-DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-
-THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
-IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
-NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
-MODIFICATIONS.
-
-GOVERNMENT USE: If you are acquiring this software on behalf of the
-U.S. government, the Government shall have only "Restricted Rights"
-in the software and related documentation as defined in the Federal 
-Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
-are acquiring the software on behalf of the Department of Defense, the
-software shall be classified as "Commercial Computer Software" and the
-Government shall have only "Restricted Rights" as defined in Clause
-252.227-7014 (b) (3) of DFARs.  Notwithstanding the foregoing, the
-authors grant the U.S. Government and others acting in its behalf
-permission to use and distribute the software in accordance with the
-terms specified in this license. 
-
-This copy of Python includes a copy of Tk, which is licensed under the following terms:
-
-This software is copyrighted by the Regents of the University of
-California, Sun Microsystems, Inc., Scriptics Corporation, ActiveState
-Corporation, Apple Inc. and other parties.  The following terms apply to
-all files associated with the software unless explicitly disclaimed in
-individual files.
-
-The authors hereby grant permission to use, copy, modify, distribute,
-and license this software and its documentation for any purpose, provided
-that existing copyright notices are retained in all copies and that this
-notice is included verbatim in any distributions. No written agreement,
-license, or royalty fee is required for any of the authorized uses.
-Modifications to this software may be copyrighted by their authors
-and need not follow the licensing terms described here, provided that
-the new terms are clearly indicated on the first page of each file where
-they apply.
-
-IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
-FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
-DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-
-THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
-IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
-NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
-MODIFICATIONS.
-
-GOVERNMENT USE: If you are acquiring this software on behalf of the
-U.S. government, the Government shall have only "Restricted Rights"
-in the software and related documentation as defined in the Federal
-Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
-are acquiring the software on behalf of the Department of Defense, the
-software shall be classified as "Commercial Computer Software" and the
-Government shall have only "Restricted Rights" as defined in Clause
-252.227-7013 (b) (3) of DFARs.  Notwithstanding the foregoing, the
-authors grant the U.S. Government and others acting in its behalf
-permission to use and distribute the software in accordance with the
-terms specified in this license.
-
-This copy of Python includes a copy of Tix, which is licensed under the following terms:
-
-Copyright (c) 1993-1999 Ioi Kim Lam.
-Copyright (c) 2000-2001 Tix Project Group.
-Copyright (c) 2004 ActiveState
-
-This software is copyrighted by the above entities
-and other parties.  The following terms apply to all files associated
-with the software unless explicitly disclaimed in individual files.
-
-The authors hereby grant permission to use, copy, modify, distribute,
-and license this software and its documentation for any purpose, provided
-that existing copyright notices are retained in all copies and that this
-notice is included verbatim in any distributions. No written agreement,
-license, or royalty fee is required for any of the authorized uses.
-Modifications to this software may be copyrighted by their authors
-and need not follow the licensing terms described here, provided that
-the new terms are clearly indicated on the first page of each file where
-they apply.
-
-IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
-FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
-ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
-DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
-POSSIBILITY OF SUCH DAMAGE.
-
-THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
-INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
-IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
-NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
-MODIFICATIONS.
-
-GOVERNMENT USE: If you are acquiring this software on behalf of the
-U.S. government, the Government shall have only "Restricted Rights"
-in the software and related documentation as defined in the Federal 
-Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
-are acquiring the software on behalf of the Department of Defense, the
-software shall be classified as "Commercial Computer Software" and the
-Government shall have only "Restricted Rights" as defined in Clause
-252.227-7013 (c) (1) of DFARs.  Notwithstanding the foregoing, the
-authors grant the U.S. Government and others acting in its behalf
-permission to use and distribute the software in accordance with the
-terms specified in this license. 
-
-----------------------------------------------------------------------
-
-Parts of this software are based on the Tcl/Tk software copyrighted by
-the Regents of the University of California, Sun Microsystems, Inc.,
-and other parties. The original license terms of the Tcl/Tk software
-distribution is included in the file docs/license.tcltk.
-
-Parts of this software are based on the HTML Library software
-copyrighted by Sun Microsystems, Inc. The original license terms of
-the HTML Library software distribution is included in the file
-docs/license.html_lib.
-
-
-pyo3-macros (0.16.6)
-====================
-
-Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-
-pyo3-macros-backend (0.16.6)
-============================
-
-Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
-
-
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-
-quick-xml (0.27.1)
-==================
-
-The MIT License (MIT)
-
-Copyright (c) 2016 Johann Tuffe
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-quote (1.0.27)
-==============
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-redox_syscall (0.2.16)
-======================
-
-Copyright (c) 2017 Redox OS Developers
-
-MIT License
-
-Permission is hereby granted, free of charge, to any person obtaining
-a copy of this software and associated documentation files (the
-"Software"), to deal in the Software without restriction, including
-without limitation the rights to use, copy, modify, merge, publish,
-distribute, sublicense, and/or sell copies of the Software, and to
-permit persons to whom the Software is furnished to do so, subject to
-the following conditions:
-
-The above copyright notice and this permission notice shall be
-included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
-EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
-MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
-NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
-LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
-WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-regex (1.6.0)
-=============
-
-Copyright (c) 2014 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-regex-automata (0.1.10)
-=======================
-
-The MIT License (MIT)
-
-Copyright (c) 2015 Andrew Gallant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-regex-syntax (0.6.27)
-=====================
-
-Copyright (c) 2014 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-roxmltree (0.18.0)
-==================
-
-The MIT License (MIT)
-
-Copyright (c) 2018 Yevhenii Reizner
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-rustversion (1.0.11)
-====================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-scopeguard (1.1.0)
-==================
-
-Copyright (c) 2016-2019 Ulrik Sverdrup "bluss" and scopeguard developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-serde (1.0.144)
-===============
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-serde_derive (1.0.144)
-======================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-sharded-slab (0.1.4)
-====================
-
-Copyright (c) 2019 Eliza Weisman
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-smallvec (1.9.0)
-================
-
-Copyright (c) 2018 The Servo Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-strum (0.24.1)
-==============
-
-MIT License
-
-Copyright (c) 2019 Peter Glotfelty
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-strum_macros (0.24.3)
-=====================
-
-MIT License
-
-Copyright (c) 2019 Peter Glotfelty
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-syn (2.0.16)
-============
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-termcolor (1.1.3)
-=================
-
-The MIT License (MIT)
-
-Copyright (c) 2015 Andrew Gallant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-thiserror (1.0.40)
-==================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-thiserror-impl (1.0.40)
-=======================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-thread_local (1.1.7)
-====================
-
-Copyright (c) 2016 The Rust Project Developers
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-tracing (0.1.37)
-================
-
-Copyright (c) 2019 Tokio Contributors
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-tracing-attributes (0.1.23)
-===========================
-
-Copyright (c) 2019 Tokio Contributors
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-tracing-core (0.1.30)
-=====================
-
-Copyright (c) 2019 Tokio Contributors
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-tracing-log (0.1.3)
-===================
-
-Copyright (c) 2019 Tokio Contributors
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-tracing-subscriber (0.3.16)
-===========================
-
-Copyright (c) 2019 Tokio Contributors
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-unicode-ident (1.0.3)
-=====================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-unindent (0.1.10)
-=================
-
-Permission is hereby granted, free of charge, to any
-person obtaining a copy of this software and associated
-documentation files (the "Software"), to deal in the
-Software without restriction, including without
-limitation the rights to use, copy, modify, merge,
-publish, distribute, sublicense, and/or sell copies of
-the Software, and to permit persons to whom the Software
-is furnished to do so, subject to the following
-conditions:
-
-The above copyright notice and this permission notice
-shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
-ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
-PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
-SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
-CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
-OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
-IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-utf8-width (0.1.6)
-==================
-
-MIT License
-
-Copyright (c) 2020 magiclen.org (Ron Li)
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-valuable (0.1.0)
-================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-vec1 (1.10.1)
-=============
-
-Copyright 2021 Philipp Korber
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
-
-
-winapi (0.3.9)
-==============
-
-Copyright (c) 2015-2018 The winapi-rs Developers
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
-
-winapi-i686-pc-windows-gnu (0.4.0)
-==================================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-winapi-util (0.1.5)
-===================
-
-The MIT License (MIT)
-
-Copyright (c) 2017 Andrew Gallant
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in
-all copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
-THE SOFTWARE.
-
-
-winapi-x86_64-pc-windows-gnu (0.4.0)
-====================================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-windows-sys (0.36.1)
-====================
-
-MIT License
-
-    Copyright (c) Microsoft Corporation.
-
-    Permission is hereby granted, free of charge, to any person obtaining a copy
-    of this software and associated documentation files (the "Software"), to deal
-    in the Software without restriction, including without limitation the rights
-    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-    copies of the Software, and to permit persons to whom the Software is
-    furnished to do so, subject to the following conditions:
-
-    The above copyright notice and this permission notice shall be included in all
-    copies or substantial portions of the Software.
-
-    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-    SOFTWARE
-
-
-windows_aarch64_msvc (0.36.1)
-=============================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-windows_i686_gnu (0.36.1)
-=========================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-windows_i686_msvc (0.36.1)
-==========================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-windows_x86_64_gnu (0.36.1)
-===========================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-windows_x86_64_msvc (0.36.1)
-============================
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
-documentation files (the “Software”), to deal in the Software without restriction, including without limitation
-the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
-and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions
-of the Software.
-
-THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
-TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
-THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
-CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
-DEALINGS IN THE SOFTWARE.
-
-
-xmlparser (0.13.5)
-==================
-
-The MIT License (MIT)
-
-Copyright (c) 2018 Reizner Evgeniy
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
-
+Third Party Licenses
+====================
+
+This file contains all the open source licenses for the Rust crates that
+Docleaf depends on. It has been created so that it is bundled into the 
+wheel so that the licenses are appropriately distributed with the compiled
+code.
+
+This file is generated by 'rust/script/licenses.py' and placed here so that
+it is picked up and package by maturin. See: 
+
+    https://github.com/PyO3/maturin/pull/862
+
+
+aho-corasick (0.7.19)
+=====================
+
+The MIT License (MIT)
+
+Copyright (c) 2015 Andrew Gallant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+anyhow (1.0.65)
+===============
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+atty (0.2.14)
+=============
+
+Copyright (c) 2015-2019 Doug Tangren
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+bitflags (1.3.2)
+================
+
+Copyright (c) 2014 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+cfg-if (1.0.0)
+==============
+
+Copyright (c) 2014 Alex Crichton
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+either (1.8.1)
+==============
+
+Copyright (c) 2015
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+env_logger (0.9.0)
+==================
+
+Copyright (c) 2014 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+heck (0.4.1)
+============
+
+Copyright (c) 2015 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+hermit-abi (0.1.19)
+===================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+html-escape (0.2.13)
+====================
+
+MIT License
+
+Copyright (c) 2020 magiclen.org (Ron Li)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+humantime (2.1.0)
+=================
+
+Copyright (c) 2016 The humantime Developers
+
+Includes parts of http date with the following copyright:
+Copyright (c) 2016 Pyfisch
+
+Includes portions of musl libc with the following copyright:
+Copyright © 2005-2013 Rich Felker
+
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+indoc (1.0.7)
+=============
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+itertools (0.10.5)
+==================
+
+Copyright (c) 2015
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+lazy_static (1.4.0)
+===================
+
+Copyright (c) 2010 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+libc (0.2.132)
+==============
+
+Copyright (c) 2014-2020 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+lock_api (0.4.8)
+================
+
+Copyright (c) 2016 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+log (0.4.17)
+============
+
+Copyright (c) 2014 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+matchers (0.1.0)
+================
+
+Copyright (c) 2019 Eliza Weisman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+memchr (2.5.0)
+==============
+
+The MIT License (MIT)
+
+Copyright (c) 2015 Andrew Gallant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+nu-ansi-term (0.46.0)
+=====================
+
+The MIT License (MIT)
+
+Copyright (c) 2014 Benjamin Sago
+Copyright (c) 2021-2022 The Nushell Project Developers
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+once_cell (1.14.0)
+==================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+overload (0.1.1)
+================
+
+MIT License
+
+Copyright (c) 2019 Daniel Augusto Rizzi Salvadori
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+parking_lot (0.12.1)
+====================
+
+Copyright (c) 2016 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+parking_lot_core (0.9.3)
+========================
+
+Copyright (c) 2016 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+pin-project-lite (0.2.9)
+========================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+proc-macro2 (1.0.58)
+====================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+pyo3 (0.16.6)
+=============
+
+Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+
+pyo3-ffi (0.16.6)
+=================
+
+A. HISTORY OF THE SOFTWARE
+==========================
+
+Python was created in the early 1990s by Guido van Rossum at Stichting
+Mathematisch Centrum (CWI, see http://www.cwi.nl) in the Netherlands
+as a successor of a language called ABC.  Guido remains Python's
+principal author, although it includes many contributions from others.
+
+In 1995, Guido continued his work on Python at the Corporation for
+National Research Initiatives (CNRI, see http://www.cnri.reston.va.us)
+in Reston, Virginia where he released several versions of the
+software.
+
+In May 2000, Guido and the Python core development team moved to
+BeOpen.com to form the BeOpen PythonLabs team.  In October of the same
+year, the PythonLabs team moved to Digital Creations (now Zope
+Corporation, see http://www.zope.com).  In 2001, the Python Software
+Foundation (PSF, see http://www.python.org/psf/) was formed, a
+non-profit organization created specifically to own Python-related
+Intellectual Property.  Zope Corporation is a sponsoring member of
+the PSF.
+
+All Python releases are Open Source (see http://www.opensource.org for
+the Open Source Definition).  Historically, most, but not all, Python
+releases have also been GPL-compatible; the table below summarizes
+the various releases.
+
+    Release         Derived     Year        Owner       GPL-
+                    from                                compatible? (1)
+
+    0.9.0 thru 1.2              1991-1995   CWI         yes
+    1.3 thru 1.5.2  1.2         1995-1999   CNRI        yes
+    1.6             1.5.2       2000        CNRI        no
+    2.0             1.6         2000        BeOpen.com  no
+    1.6.1           1.6         2001        CNRI        yes (2)
+    2.1             2.0+1.6.1   2001        PSF         no
+    2.0.1           2.0+1.6.1   2001        PSF         yes
+    2.1.1           2.1+2.0.1   2001        PSF         yes
+    2.1.2           2.1.1       2002        PSF         yes
+    2.1.3           2.1.2       2002        PSF         yes
+    2.2 and above   2.1.1       2001-now    PSF         yes
+
+Footnotes:
+
+(1) GPL-compatible doesn't mean that we're distributing Python under
+    the GPL.  All Python licenses, unlike the GPL, let you distribute
+    a modified version without making your changes open source.  The
+    GPL-compatible licenses make it possible to combine Python with
+    other software that is released under the GPL; the others don't.
+
+(2) According to Richard Stallman, 1.6.1 is not GPL-compatible,
+    because its license has a choice of law clause.  According to
+    CNRI, however, Stallman's lawyer has told CNRI's lawyer that 1.6.1
+    is "not incompatible" with the GPL.
+
+Thanks to the many outside volunteers who have worked under Guido's
+direction to make these releases possible.
+
+
+B. TERMS AND CONDITIONS FOR ACCESSING OR OTHERWISE USING PYTHON
+===============================================================
+
+PYTHON SOFTWARE FOUNDATION LICENSE VERSION 2
+--------------------------------------------
+
+1. This LICENSE AGREEMENT is between the Python Software Foundation
+("PSF"), and the Individual or Organization ("Licensee") accessing and
+otherwise using this software ("Python") in source or binary form and
+its associated documentation.
+
+2. Subject to the terms and conditions of this License Agreement, PSF hereby
+grants Licensee a nonexclusive, royalty-free, world-wide license to reproduce,
+analyze, test, perform and/or display publicly, prepare derivative works,
+distribute, and otherwise use Python alone or in any derivative version,
+provided, however, that PSF's License Agreement and PSF's notice of copyright,
+i.e., "Copyright (c) 2001, 2002, 2003, 2004, 2005, 2006, 2007, 2008, 2009, 2010,
+2011, 2012, 2013, 2014, 2015 Python Software Foundation; All Rights Reserved"
+are retained in Python alone or in any derivative version prepared by Licensee.
+
+3. In the event Licensee prepares a derivative work that is based on
+or incorporates Python or any part thereof, and wants to make
+the derivative work available to others as provided herein, then
+Licensee hereby agrees to include in any such work a brief summary of
+the changes made to Python.
+
+4. PSF is making Python available to Licensee on an "AS IS"
+basis.  PSF MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, PSF MAKES NO AND
+DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON WILL NOT
+INFRINGE ANY THIRD PARTY RIGHTS.
+
+5. PSF SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
+FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
+A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON,
+OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
+
+6. This License Agreement will automatically terminate upon a material
+breach of its terms and conditions.
+
+7. Nothing in this License Agreement shall be deemed to create any
+relationship of agency, partnership, or joint venture between PSF and
+Licensee.  This License Agreement does not grant permission to use PSF
+trademarks or trade name in a trademark sense to endorse or promote
+products or services of Licensee, or any third party.
+
+8. By copying, installing or otherwise using Python, Licensee
+agrees to be bound by the terms and conditions of this License
+Agreement.
+
+
+BEOPEN.COM LICENSE AGREEMENT FOR PYTHON 2.0
+-------------------------------------------
+
+BEOPEN PYTHON OPEN SOURCE LICENSE AGREEMENT VERSION 1
+
+1. This LICENSE AGREEMENT is between BeOpen.com ("BeOpen"), having an
+office at 160 Saratoga Avenue, Santa Clara, CA 95051, and the
+Individual or Organization ("Licensee") accessing and otherwise using
+this software in source or binary form and its associated
+documentation ("the Software").
+
+2. Subject to the terms and conditions of this BeOpen Python License
+Agreement, BeOpen hereby grants Licensee a non-exclusive,
+royalty-free, world-wide license to reproduce, analyze, test, perform
+and/or display publicly, prepare derivative works, distribute, and
+otherwise use the Software alone or in any derivative version,
+provided, however, that the BeOpen Python License is retained in the
+Software, alone or in any derivative version prepared by Licensee.
+
+3. BeOpen is making the Software available to Licensee on an "AS IS"
+basis.  BEOPEN MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, BEOPEN MAKES NO AND
+DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF THE SOFTWARE WILL NOT
+INFRINGE ANY THIRD PARTY RIGHTS.
+
+4. BEOPEN SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF THE
+SOFTWARE FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS
+AS A RESULT OF USING, MODIFYING OR DISTRIBUTING THE SOFTWARE, OR ANY
+DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
+
+5. This License Agreement will automatically terminate upon a material
+breach of its terms and conditions.
+
+6. This License Agreement shall be governed by and interpreted in all
+respects by the law of the State of California, excluding conflict of
+law provisions.  Nothing in this License Agreement shall be deemed to
+create any relationship of agency, partnership, or joint venture
+between BeOpen and Licensee.  This License Agreement does not grant
+permission to use BeOpen trademarks or trade names in a trademark
+sense to endorse or promote products or services of Licensee, or any
+third party.  As an exception, the "BeOpen Python" logos available at
+http://www.pythonlabs.com/logos.html may be used according to the
+permissions granted on that web page.
+
+7. By copying, installing or otherwise using the software, Licensee
+agrees to be bound by the terms and conditions of this License
+Agreement.
+
+
+CNRI LICENSE AGREEMENT FOR PYTHON 1.6.1
+---------------------------------------
+
+1. This LICENSE AGREEMENT is between the Corporation for National
+Research Initiatives, having an office at 1895 Preston White Drive,
+Reston, VA 20191 ("CNRI"), and the Individual or Organization
+("Licensee") accessing and otherwise using Python 1.6.1 software in
+source or binary form and its associated documentation.
+
+2. Subject to the terms and conditions of this License Agreement, CNRI
+hereby grants Licensee a nonexclusive, royalty-free, world-wide
+license to reproduce, analyze, test, perform and/or display publicly,
+prepare derivative works, distribute, and otherwise use Python 1.6.1
+alone or in any derivative version, provided, however, that CNRI's
+License Agreement and CNRI's notice of copyright, i.e., "Copyright (c)
+1995-2001 Corporation for National Research Initiatives; All Rights
+Reserved" are retained in Python 1.6.1 alone or in any derivative
+version prepared by Licensee.  Alternately, in lieu of CNRI's License
+Agreement, Licensee may substitute the following text (omitting the
+quotes): "Python 1.6.1 is made available subject to the terms and
+conditions in CNRI's License Agreement.  This Agreement together with
+Python 1.6.1 may be located on the Internet using the following
+unique, persistent identifier (known as a handle): 1895.22/1013.  This
+Agreement may also be obtained from a proxy server on the Internet
+using the following URL: http://hdl.handle.net/1895.22/1013".
+
+3. In the event Licensee prepares a derivative work that is based on
+or incorporates Python 1.6.1 or any part thereof, and wants to make
+the derivative work available to others as provided herein, then
+Licensee hereby agrees to include in any such work a brief summary of
+the changes made to Python 1.6.1.
+
+4. CNRI is making Python 1.6.1 available to Licensee on an "AS IS"
+basis.  CNRI MAKES NO REPRESENTATIONS OR WARRANTIES, EXPRESS OR
+IMPLIED.  BY WAY OF EXAMPLE, BUT NOT LIMITATION, CNRI MAKES NO AND
+DISCLAIMS ANY REPRESENTATION OR WARRANTY OF MERCHANTABILITY OR FITNESS
+FOR ANY PARTICULAR PURPOSE OR THAT THE USE OF PYTHON 1.6.1 WILL NOT
+INFRINGE ANY THIRD PARTY RIGHTS.
+
+5. CNRI SHALL NOT BE LIABLE TO LICENSEE OR ANY OTHER USERS OF PYTHON
+1.6.1 FOR ANY INCIDENTAL, SPECIAL, OR CONSEQUENTIAL DAMAGES OR LOSS AS
+A RESULT OF MODIFYING, DISTRIBUTING, OR OTHERWISE USING PYTHON 1.6.1,
+OR ANY DERIVATIVE THEREOF, EVEN IF ADVISED OF THE POSSIBILITY THEREOF.
+
+6. This License Agreement will automatically terminate upon a material
+breach of its terms and conditions.
+
+7. This License Agreement shall be governed by the federal
+intellectual property law of the United States, including without
+limitation the federal copyright law, and, to the extent such
+U.S. federal law does not apply, by the law of the Commonwealth of
+Virginia, excluding Virginia's conflict of law provisions.
+Notwithstanding the foregoing, with regard to derivative works based
+on Python 1.6.1 that incorporate non-separable material that was
+previously distributed under the GNU General Public License (GPL), the
+law of the Commonwealth of Virginia shall govern this License
+Agreement only as to issues arising under or with respect to
+Paragraphs 4, 5, and 7 of this License Agreement.  Nothing in this
+License Agreement shall be deemed to create any relationship of
+agency, partnership, or joint venture between CNRI and Licensee.  This
+License Agreement does not grant permission to use CNRI trademarks or
+trade name in a trademark sense to endorse or promote products or
+services of Licensee, or any third party.
+
+8. By clicking on the "ACCEPT" button where indicated, or by copying,
+installing or otherwise using Python 1.6.1, Licensee agrees to be
+bound by the terms and conditions of this License Agreement.
+
+        ACCEPT
+
+
+CWI LICENSE AGREEMENT FOR PYTHON 0.9.0 THROUGH 1.2
+--------------------------------------------------
+
+Copyright (c) 1991 - 1995, Stichting Mathematisch Centrum Amsterdam,
+The Netherlands.  All rights reserved.
+
+Permission to use, copy, modify, and distribute this software and its
+documentation for any purpose and without fee is hereby granted,
+provided that the above copyright notice appear in all copies and that
+both that copyright notice and this permission notice appear in
+supporting documentation, and that the name of Stichting Mathematisch
+Centrum or CWI not be used in advertising or publicity pertaining to
+distribution of the software without specific, written prior
+permission.
+
+STICHTING MATHEMATISCH CENTRUM DISCLAIMS ALL WARRANTIES WITH REGARD TO
+THIS SOFTWARE, INCLUDING ALL IMPLIED WARRANTIES OF MERCHANTABILITY AND
+FITNESS, IN NO EVENT SHALL STICHTING MATHEMATISCH CENTRUM BE LIABLE
+FOR ANY SPECIAL, INDIRECT OR CONSEQUENTIAL DAMAGES OR ANY DAMAGES
+WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
+ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT
+OF OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
+
+
+Additional Conditions for this Windows binary build
+---------------------------------------------------
+
+This program is linked with and uses Microsoft Distributable Code,
+copyrighted by Microsoft Corporation. The Microsoft Distributable Code
+includes the following files:
+
+msvcr90.dll
+msvcp90.dll
+msvcm90.dll
+
+If you further distribute programs that include the Microsoft
+Distributable Code, you must comply with the restrictions on
+distribution specified by Microsoft. In particular, you must require
+distributors and external end users to agree to terms that protect the
+Microsoft Distributable Code at least as much as Microsoft's own
+requirements for the Distributable Code. See Microsoft's documentation
+(included in its developer tools and on its website at microsoft.com)
+for specific details.
+
+Redistribution of the Windows binary build of the Python interpreter
+complies with this agreement, provided that you do not:
+
+- alter any copyright, trademark or patent notice in Microsoft's
+Distributable Code;
+
+- use Microsoft's trademarks in your programs' names or in a way that
+suggests your programs come from or are endorsed by Microsoft;
+
+- distribute Microsoft's Distributable Code to run on a platform other
+than Microsoft operating systems, run-time technologies or application
+platforms; or
+
+- include Microsoft Distributable Code in malicious, deceptive or
+unlawful programs.
+
+These restrictions apply only to the Microsoft Distributable Code as
+defined above, not to Python itself or any programs running on the
+Python interpreter. The redistribution of the Python interpreter and
+libraries is governed by the Python Software License included with this
+file, or by other licenses as marked.
+
+
+This copy of Python includes a copy of bzip2, which is licensed under the following terms:
+
+
+--------------------------------------------------------------------------
+
+This program, "bzip2", the associated library "libbzip2", and all
+documentation, are copyright (C) 1996-2010 Julian R Seward.  All
+rights reserved.
+
+Redistribution and use in source and binary forms, with or without
+modification, are permitted provided that the following conditions
+are met:
+
+1. Redistributions of source code must retain the above copyright
+   notice, this list of conditions and the following disclaimer.
+
+2. The origin of this software must not be misrepresented; you must 
+   not claim that you wrote the original software.  If you use this 
+   software in a product, an acknowledgment in the product 
+   documentation would be appreciated but is not required.
+
+3. Altered source versions must be plainly marked as such, and must
+   not be misrepresented as being the original software.
+
+4. The name of the author may not be used to endorse or promote 
+   products derived from this software without specific prior written 
+   permission.
+
+THIS SOFTWARE IS PROVIDED BY THE AUTHOR ``AS IS'' AND ANY EXPRESS
+OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED
+WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR BE LIABLE FOR ANY
+DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE
+GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS
+INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY,
+WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
+NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
+SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+
+Julian Seward, jseward@bzip.org
+bzip2/libbzip2 version 1.0.6 of 6 September 2010
+
+--------------------------------------------------------------------------
+
+This copy of Python includes a copy of openssl, which is licensed under the following terms:
+
+
+  LICENSE ISSUES
+  ==============
+
+  The OpenSSL toolkit stays under a dual license, i.e. both the conditions of
+  the OpenSSL License and the original SSLeay license apply to the toolkit.
+  See below for the actual license texts. Actually both licenses are BSD-style
+  Open Source licenses. In case of any license issues related to OpenSSL
+  please contact openssl-core@openssl.org.
+
+  OpenSSL License
+  ---------------
+
+/* ====================================================================
+ * Copyright (c) 1998-2011 The OpenSSL Project.  All rights reserved.
+ *
+ * Redistribution and use in source and binary forms, with or without
+ * modification, are permitted provided that the following conditions
+ * are met:
+ *
+ * 1. Redistributions of source code must retain the above copyright
+ *    notice, this list of conditions and the following disclaimer. 
+ *
+ * 2. Redistributions in binary form must reproduce the above copyright
+ *    notice, this list of conditions and the following disclaimer in
+ *    the documentation and/or other materials provided with the
+ *    distribution.
+ *
+ * 3. All advertising materials mentioning features or use of this
+ *    software must display the following acknowledgment:
+ *    "This product includes software developed by the OpenSSL Project
+ *    for use in the OpenSSL Toolkit. (http://www.openssl.org/)"
+ *
+ * 4. The names "OpenSSL Toolkit" and "OpenSSL Project" must not be used to
+ *    endorse or promote products derived from this software without
+ *    prior written permission. For written permission, please contact
+ *    openssl-core@openssl.org.
+ *
+ * 5. Products derived from this software may not be called "OpenSSL"
+ *    nor may "OpenSSL" appear in their names without prior written
+ *    permission of the OpenSSL Project.
+ *
+ * 6. Redistributions of any form whatsoever must retain the following
+ *    acknowledgment:
+ *    "This product includes software developed by the OpenSSL Project
+ *    for use in the OpenSSL Toolkit (http://www.openssl.org/)"
+ *
+ * THIS SOFTWARE IS PROVIDED BY THE OpenSSL PROJECT ``AS IS'' AND ANY
+ * EXPRESSED OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR
+ * PURPOSE ARE DISCLAIMED.  IN NO EVENT SHALL THE OpenSSL PROJECT OR
+ * ITS CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL,
+ * SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT
+ * NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES;
+ * LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+ * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT,
+ * STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE)
+ * ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED
+ * OF THE POSSIBILITY OF SUCH DAMAGE.
+ * ====================================================================
+ *
+ * This product includes cryptographic software written by Eric Young
+ * (eay@cryptsoft.com).  This product includes software written by Tim
+ * Hudson (tjh@cryptsoft.com).
+ *
+ */
+
+ Original SSLeay License
+ -----------------------
+
+/* Copyright (C) 1995-1998 Eric Young (eay@cryptsoft.com)
+ * All rights reserved.
+ *
+ * This package is an SSL implementation written
+ * by Eric Young (eay@cryptsoft.com).
+ * The implementation was written so as to conform with Netscapes SSL.
+ * 
+ * This library is free for commercial and non-commercial use as long as
+ * the following conditions are aheared to.  The following conditions
+ * apply to all code found in this distribution, be it the RC4, RSA,
+ * lhash, DES, etc., code; not just the SSL code.  The SSL documentation
+ * included with this distribution is covered by the same copyright terms
+ * except that the holder is Tim Hudson (tjh@cryptsoft.com).
+ * 
+ * Copyright remains Eric Young's, and as such any Copyright notices in
+ * the code are not to be removed.
+ * If this package is used in a product, Eric Young should be given attribution
+ * as the author of the parts of the library used.
+ * This can be in the form of a textual message at program startup or
+ * in documentation (online or textual) provided with the package.
+ * 
+ * Redistribution and use in source and binary forms, with or without
+ * modification, are permitted provided that the following conditions
+ * are met:
+ * 1. Redistributions of source code must retain the copyright
+ *    notice, this list of conditions and the following disclaimer.
+ * 2. Redistributions in binary form must reproduce the above copyright
+ *    notice, this list of conditions and the following disclaimer in the
+ *    documentation and/or other materials provided with the distribution.
+ * 3. All advertising materials mentioning features or use of this software
+ *    must display the following acknowledgement:
+ *    "This product includes cryptographic software written by
+ *     Eric Young (eay@cryptsoft.com)"
+ *    The word 'cryptographic' can be left out if the rouines from the library
+ *    being used are not cryptographic related :-).
+ * 4. If you include any Windows specific code (or a derivative thereof) from 
+ *    the apps directory (application code) you must include an acknowledgement:
+ *    "This product includes software written by Tim Hudson (tjh@cryptsoft.com)"
+ * 
+ * THIS SOFTWARE IS PROVIDED BY ERIC YOUNG ``AS IS'' AND
+ * ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE
+ * IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE
+ * ARE DISCLAIMED.  IN NO EVENT SHALL THE AUTHOR OR CONTRIBUTORS BE LIABLE
+ * FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL
+ * DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS
+ * OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION)
+ * HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT
+ * LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY
+ * OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF
+ * SUCH DAMAGE.
+ * 
+ * The licence and distribution terms for any publically available version or
+ * derivative of this code cannot be changed.  i.e. this code cannot simply be
+ * copied and put under another distribution licence
+ * [including the GNU Public Licence.]
+ */
+
+
+This copy of Python includes a copy of Tcl, which is licensed under the following terms:
+
+This software is copyrighted by the Regents of the University of
+California, Sun Microsystems, Inc., Scriptics Corporation, ActiveState
+Corporation and other parties.  The following terms apply to all files
+associated with the software unless explicitly disclaimed in
+individual files.
+
+The authors hereby grant permission to use, copy, modify, distribute,
+and license this software and its documentation for any purpose, provided
+that existing copyright notices are retained in all copies and that this
+notice is included verbatim in any distributions. No written agreement,
+license, or royalty fee is required for any of the authorized uses.
+Modifications to this software may be copyrighted by their authors
+and need not follow the licensing terms described here, provided that
+the new terms are clearly indicated on the first page of each file where
+they apply.
+
+IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
+FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
+DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
+
+THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
+IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
+NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
+MODIFICATIONS.
+
+GOVERNMENT USE: If you are acquiring this software on behalf of the
+U.S. government, the Government shall have only "Restricted Rights"
+in the software and related documentation as defined in the Federal 
+Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
+are acquiring the software on behalf of the Department of Defense, the
+software shall be classified as "Commercial Computer Software" and the
+Government shall have only "Restricted Rights" as defined in Clause
+252.227-7014 (b) (3) of DFARs.  Notwithstanding the foregoing, the
+authors grant the U.S. Government and others acting in its behalf
+permission to use and distribute the software in accordance with the
+terms specified in this license. 
+
+This copy of Python includes a copy of Tk, which is licensed under the following terms:
+
+This software is copyrighted by the Regents of the University of
+California, Sun Microsystems, Inc., Scriptics Corporation, ActiveState
+Corporation, Apple Inc. and other parties.  The following terms apply to
+all files associated with the software unless explicitly disclaimed in
+individual files.
+
+The authors hereby grant permission to use, copy, modify, distribute,
+and license this software and its documentation for any purpose, provided
+that existing copyright notices are retained in all copies and that this
+notice is included verbatim in any distributions. No written agreement,
+license, or royalty fee is required for any of the authorized uses.
+Modifications to this software may be copyrighted by their authors
+and need not follow the licensing terms described here, provided that
+the new terms are clearly indicated on the first page of each file where
+they apply.
+
+IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
+FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
+DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
+
+THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
+IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
+NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
+MODIFICATIONS.
+
+GOVERNMENT USE: If you are acquiring this software on behalf of the
+U.S. government, the Government shall have only "Restricted Rights"
+in the software and related documentation as defined in the Federal
+Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
+are acquiring the software on behalf of the Department of Defense, the
+software shall be classified as "Commercial Computer Software" and the
+Government shall have only "Restricted Rights" as defined in Clause
+252.227-7013 (b) (3) of DFARs.  Notwithstanding the foregoing, the
+authors grant the U.S. Government and others acting in its behalf
+permission to use and distribute the software in accordance with the
+terms specified in this license.
+
+This copy of Python includes a copy of Tix, which is licensed under the following terms:
+
+Copyright (c) 1993-1999 Ioi Kim Lam.
+Copyright (c) 2000-2001 Tix Project Group.
+Copyright (c) 2004 ActiveState
+
+This software is copyrighted by the above entities
+and other parties.  The following terms apply to all files associated
+with the software unless explicitly disclaimed in individual files.
+
+The authors hereby grant permission to use, copy, modify, distribute,
+and license this software and its documentation for any purpose, provided
+that existing copyright notices are retained in all copies and that this
+notice is included verbatim in any distributions. No written agreement,
+license, or royalty fee is required for any of the authorized uses.
+Modifications to this software may be copyrighted by their authors
+and need not follow the licensing terms described here, provided that
+the new terms are clearly indicated on the first page of each file where
+they apply.
+
+IN NO EVENT SHALL THE AUTHORS OR DISTRIBUTORS BE LIABLE TO ANY PARTY
+FOR DIRECT, INDIRECT, SPECIAL, INCIDENTAL, OR CONSEQUENTIAL DAMAGES
+ARISING OUT OF THE USE OF THIS SOFTWARE, ITS DOCUMENTATION, OR ANY
+DERIVATIVES THEREOF, EVEN IF THE AUTHORS HAVE BEEN ADVISED OF THE
+POSSIBILITY OF SUCH DAMAGE.
+
+THE AUTHORS AND DISTRIBUTORS SPECIFICALLY DISCLAIM ANY WARRANTIES,
+INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE, AND NON-INFRINGEMENT.  THIS SOFTWARE
+IS PROVIDED ON AN "AS IS" BASIS, AND THE AUTHORS AND DISTRIBUTORS HAVE
+NO OBLIGATION TO PROVIDE MAINTENANCE, SUPPORT, UPDATES, ENHANCEMENTS, OR
+MODIFICATIONS.
+
+GOVERNMENT USE: If you are acquiring this software on behalf of the
+U.S. government, the Government shall have only "Restricted Rights"
+in the software and related documentation as defined in the Federal 
+Acquisition Regulations (FARs) in Clause 52.227.19 (c) (2).  If you
+are acquiring the software on behalf of the Department of Defense, the
+software shall be classified as "Commercial Computer Software" and the
+Government shall have only "Restricted Rights" as defined in Clause
+252.227-7013 (c) (1) of DFARs.  Notwithstanding the foregoing, the
+authors grant the U.S. Government and others acting in its behalf
+permission to use and distribute the software in accordance with the
+terms specified in this license. 
+
+----------------------------------------------------------------------
+
+Parts of this software are based on the Tcl/Tk software copyrighted by
+the Regents of the University of California, Sun Microsystems, Inc.,
+and other parties. The original license terms of the Tcl/Tk software
+distribution is included in the file docs/license.tcltk.
+
+Parts of this software are based on the HTML Library software
+copyrighted by Sun Microsystems, Inc. The original license terms of
+the HTML Library software distribution is included in the file
+docs/license.html_lib.
+
+
+pyo3-macros (0.16.6)
+====================
+
+Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+
+pyo3-macros-backend (0.16.6)
+============================
+
+Copyright (c) 2017-present PyO3 Project and Contributors.  https://github.com/PyO3
+
+   Licensed under the Apache License, Version 2.0 (the "License");
+   you may not use this file except in compliance with the License.
+   You may obtain a copy of the License at
+
+       http://www.apache.org/licenses/LICENSE-2.0
+
+   Unless required by applicable law or agreed to in writing, software
+   distributed under the License is distributed on an "AS IS" BASIS,
+   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+   See the License for the specific language governing permissions and
+   limitations under the License.
+
+
+                                 Apache License
+                           Version 2.0, January 2004
+                        http://www.apache.org/licenses/
+
+   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+   1. Definitions.
+
+      "License" shall mean the terms and conditions for use, reproduction,
+      and distribution as defined by Sections 1 through 9 of this document.
+
+      "Licensor" shall mean the copyright owner or entity authorized by
+      the copyright owner that is granting the License.
+
+      "Legal Entity" shall mean the union of the acting entity and all
+      other entities that control, are controlled by, or are under common
+      control with that entity. For the purposes of this definition,
+      "control" means (i) the power, direct or indirect, to cause the
+      direction or management of such entity, whether by contract or
+      otherwise, or (ii) ownership of fifty percent (50%) or more of the
+      outstanding shares, or (iii) beneficial ownership of such entity.
+
+      "You" (or "Your") shall mean an individual or Legal Entity
+      exercising permissions granted by this License.
+
+      "Source" form shall mean the preferred form for making modifications,
+      including but not limited to software source code, documentation
+      source, and configuration files.
+
+      "Object" form shall mean any form resulting from mechanical
+      transformation or translation of a Source form, including but
+      not limited to compiled object code, generated documentation,
+      and conversions to other media types.
+
+      "Work" shall mean the work of authorship, whether in Source or
+      Object form, made available under the License, as indicated by a
+      copyright notice that is included in or attached to the work
+      (an example is provided in the Appendix below).
+
+      "Derivative Works" shall mean any work, whether in Source or Object
+      form, that is based on (or derived from) the Work and for which the
+      editorial revisions, annotations, elaborations, or other modifications
+      represent, as a whole, an original work of authorship. For the purposes
+      of this License, Derivative Works shall not include works that remain
+      separable from, or merely link (or bind by name) to the interfaces of,
+      the Work and Derivative Works thereof.
+
+      "Contribution" shall mean any work of authorship, including
+      the original version of the Work and any modifications or additions
+      to that Work or Derivative Works thereof, that is intentionally
+      submitted to Licensor for inclusion in the Work by the copyright owner
+      or by an individual or Legal Entity authorized to submit on behalf of
+      the copyright owner. For the purposes of this definition, "submitted"
+      means any form of electronic, verbal, or written communication sent
+      to the Licensor or its representatives, including but not limited to
+      communication on electronic mailing lists, source code control systems,
+      and issue tracking systems that are managed by, or on behalf of, the
+      Licensor for the purpose of discussing and improving the Work, but
+      excluding communication that is conspicuously marked or otherwise
+      designated in writing by the copyright owner as "Not a Contribution."
+
+      "Contributor" shall mean Licensor and any individual or Legal Entity
+      on behalf of whom a Contribution has been received by Licensor and
+      subsequently incorporated within the Work.
+
+   2. Grant of Copyright License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      copyright license to reproduce, prepare Derivative Works of,
+      publicly display, publicly perform, sublicense, and distribute the
+      Work and such Derivative Works in Source or Object form.
+
+   3. Grant of Patent License. Subject to the terms and conditions of
+      this License, each Contributor hereby grants to You a perpetual,
+      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+      (except as stated in this section) patent license to make, have made,
+      use, offer to sell, sell, import, and otherwise transfer the Work,
+      where such license applies only to those patent claims licensable
+      by such Contributor that are necessarily infringed by their
+      Contribution(s) alone or by combination of their Contribution(s)
+      with the Work to which such Contribution(s) was submitted. If You
+      institute patent litigation against any entity (including a
+      cross-claim or counterclaim in a lawsuit) alleging that the Work
+      or a Contribution incorporated within the Work constitutes direct
+      or contributory patent infringement, then any patent licenses
+      granted to You under this License for that Work shall terminate
+      as of the date such litigation is filed.
+
+   4. Redistribution. You may reproduce and distribute copies of the
+      Work or Derivative Works thereof in any medium, with or without
+      modifications, and in Source or Object form, provided that You
+      meet the following conditions:
+
+      (a) You must give any other recipients of the Work or
+          Derivative Works a copy of this License; and
+
+      (b) You must cause any modified files to carry prominent notices
+          stating that You changed the files; and
+
+      (c) You must retain, in the Source form of any Derivative Works
+          that You distribute, all copyright, patent, trademark, and
+          attribution notices from the Source form of the Work,
+          excluding those notices that do not pertain to any part of
+          the Derivative Works; and
+
+      (d) If the Work includes a "NOTICE" text file as part of its
+          distribution, then any Derivative Works that You distribute must
+          include a readable copy of the attribution notices contained
+          within such NOTICE file, excluding those notices that do not
+          pertain to any part of the Derivative Works, in at least one
+          of the following places: within a NOTICE text file distributed
+          as part of the Derivative Works; within the Source form or
+          documentation, if provided along with the Derivative Works; or,
+          within a display generated by the Derivative Works, if and
+          wherever such third-party notices normally appear. The contents
+          of the NOTICE file are for informational purposes only and
+          do not modify the License. You may add Your own attribution
+          notices within Derivative Works that You distribute, alongside
+          or as an addendum to the NOTICE text from the Work, provided
+          that such additional attribution notices cannot be construed
+          as modifying the License.
+
+      You may add Your own copyright statement to Your modifications and
+      may provide additional or different license terms and conditions
+      for use, reproduction, or distribution of Your modifications, or
+      for any such Derivative Works as a whole, provided Your use,
+      reproduction, and distribution of the Work otherwise complies with
+      the conditions stated in this License.
+
+   5. Submission of Contributions. Unless You explicitly state otherwise,
+      any Contribution intentionally submitted for inclusion in the Work
+      by You to the Licensor shall be under the terms and conditions of
+      this License, without any additional terms or conditions.
+      Notwithstanding the above, nothing herein shall supersede or modify
+      the terms of any separate license agreement you may have executed
+      with Licensor regarding such Contributions.
+
+   6. Trademarks. This License does not grant permission to use the trade
+      names, trademarks, service marks, or product names of the Licensor,
+      except as required for reasonable and customary use in describing the
+      origin of the Work and reproducing the content of the NOTICE file.
+
+   7. Disclaimer of Warranty. Unless required by applicable law or
+      agreed to in writing, Licensor provides the Work (and each
+      Contributor provides its Contributions) on an "AS IS" BASIS,
+      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+      implied, including, without limitation, any warranties or conditions
+      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+      PARTICULAR PURPOSE. You are solely responsible for determining the
+      appropriateness of using or redistributing the Work and assume any
+      risks associated with Your exercise of permissions under this License.
+
+   8. Limitation of Liability. In no event and under no legal theory,
+      whether in tort (including negligence), contract, or otherwise,
+      unless required by applicable law (such as deliberate and grossly
+      negligent acts) or agreed to in writing, shall any Contributor be
+      liable to You for damages, including any direct, indirect, special,
+      incidental, or consequential damages of any character arising as a
+      result of this License or out of the use or inability to use the
+      Work (including but not limited to damages for loss of goodwill,
+      work stoppage, computer failure or malfunction, or any and all
+      other commercial damages or losses), even if such Contributor
+      has been advised of the possibility of such damages.
+
+   9. Accepting Warranty or Additional Liability. While redistributing
+      the Work or Derivative Works thereof, You may choose to offer,
+      and charge a fee for, acceptance of support, warranty, indemnity,
+      or other liability obligations and/or rights consistent with this
+      License. However, in accepting such obligations, You may act only
+      on Your own behalf and on Your sole responsibility, not on behalf
+      of any other Contributor, and only if You agree to indemnify,
+      defend, and hold each Contributor harmless for any liability
+      incurred by, or claims asserted against, such Contributor by reason
+      of your accepting any such warranty or additional liability.
+
+
+quick-xml (0.27.1)
+==================
+
+The MIT License (MIT)
+
+Copyright (c) 2016 Johann Tuffe
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.  IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+quote (1.0.27)
+==============
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+redox_syscall (0.2.16)
+======================
+
+Copyright (c) 2017 Redox OS Developers
+
+MIT License
+
+Permission is hereby granted, free of charge, to any person obtaining
+a copy of this software and associated documentation files (the
+"Software"), to deal in the Software without restriction, including
+without limitation the rights to use, copy, modify, merge, publish,
+distribute, sublicense, and/or sell copies of the Software, and to
+permit persons to whom the Software is furnished to do so, subject to
+the following conditions:
+
+The above copyright notice and this permission notice shall be
+included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
+EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
+MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
+NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
+LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
+WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+regex (1.6.0)
+=============
+
+Copyright (c) 2014 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+regex-automata (0.1.10)
+=======================
+
+The MIT License (MIT)
+
+Copyright (c) 2015 Andrew Gallant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+regex-syntax (0.6.27)
+=====================
+
+Copyright (c) 2014 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+roxmltree (0.18.0)
+==================
+
+The MIT License (MIT)
+
+Copyright (c) 2018 Yevhenii Reizner
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+rustversion (1.0.11)
+====================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+scopeguard (1.1.0)
+==================
+
+Copyright (c) 2016-2019 Ulrik Sverdrup "bluss" and scopeguard developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+serde (1.0.144)
+===============
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+serde_derive (1.0.144)
+======================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+sharded-slab (0.1.4)
+====================
+
+Copyright (c) 2019 Eliza Weisman
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+smallvec (1.9.0)
+================
+
+Copyright (c) 2018 The Servo Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+strum (0.24.1)
+==============
+
+MIT License
+
+Copyright (c) 2019 Peter Glotfelty
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+strum_macros (0.24.3)
+=====================
+
+MIT License
+
+Copyright (c) 2019 Peter Glotfelty
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+syn (2.0.16)
+============
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+termcolor (1.1.3)
+=================
+
+The MIT License (MIT)
+
+Copyright (c) 2015 Andrew Gallant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+thiserror (1.0.40)
+==================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+thiserror-impl (1.0.40)
+=======================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+thread_local (1.1.7)
+====================
+
+Copyright (c) 2016 The Rust Project Developers
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+tracing (0.1.37)
+================
+
+Copyright (c) 2019 Tokio Contributors
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+tracing-attributes (0.1.23)
+===========================
+
+Copyright (c) 2019 Tokio Contributors
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+tracing-core (0.1.30)
+=====================
+
+Copyright (c) 2019 Tokio Contributors
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+tracing-log (0.1.3)
+===================
+
+Copyright (c) 2019 Tokio Contributors
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+tracing-subscriber (0.3.16)
+===========================
+
+Copyright (c) 2019 Tokio Contributors
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+unicode-ident (1.0.3)
+=====================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+unindent (0.1.10)
+=================
+
+Permission is hereby granted, free of charge, to any
+person obtaining a copy of this software and associated
+documentation files (the "Software"), to deal in the
+Software without restriction, including without
+limitation the rights to use, copy, modify, merge,
+publish, distribute, sublicense, and/or sell copies of
+the Software, and to permit persons to whom the Software
+is furnished to do so, subject to the following
+conditions:
+
+The above copyright notice and this permission notice
+shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF
+ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A
+PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT
+SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY
+CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
+OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR
+IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+utf8-width (0.1.6)
+==================
+
+MIT License
+
+Copyright (c) 2020 magiclen.org (Ron Li)
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+valuable (0.1.0)
+================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+vec1 (1.10.1)
+=============
+
+Copyright 2021 Philipp Korber
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
+
+
+winapi (0.3.9)
+==============
+
+Copyright (c) 2015-2018 The winapi-rs Developers
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
+
+winapi-i686-pc-windows-gnu (0.4.0)
+==================================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+winapi-util (0.1.5)
+===================
+
+The MIT License (MIT)
+
+Copyright (c) 2017 Andrew Gallant
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in
+all copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
+THE SOFTWARE.
+
+
+winapi-x86_64-pc-windows-gnu (0.4.0)
+====================================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+windows-sys (0.36.1)
+====================
+
+MIT License
+
+    Copyright (c) Microsoft Corporation.
+
+    Permission is hereby granted, free of charge, to any person obtaining a copy
+    of this software and associated documentation files (the "Software"), to deal
+    in the Software without restriction, including without limitation the rights
+    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+    copies of the Software, and to permit persons to whom the Software is
+    furnished to do so, subject to the following conditions:
+
+    The above copyright notice and this permission notice shall be included in all
+    copies or substantial portions of the Software.
+
+    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+    SOFTWARE
+
+
+windows_aarch64_msvc (0.36.1)
+=============================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+windows_i686_gnu (0.36.1)
+=========================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+windows_i686_msvc (0.36.1)
+==========================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+windows_x86_64_gnu (0.36.1)
+===========================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+windows_x86_64_msvc (0.36.1)
+============================
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated
+documentation files (the “Software”), to deal in the Software without restriction, including without limitation
+the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software,
+and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions
+of the Software.
+
+THE SOFTWARE IS PROVIDED “AS IS”, WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED
+TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
+THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF
+CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER
+DEALINGS IN THE SOFTWARE.
+
+
+xmlparser (0.13.5)
+==================
+
+The MIT License (MIT)
+
+Copyright (c) 2018 Reizner Evgeniy
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
+
```

