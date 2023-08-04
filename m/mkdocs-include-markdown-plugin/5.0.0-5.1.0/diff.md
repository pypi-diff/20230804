# Comparing `tmp/mkdocs_include_markdown_plugin-5.0.0.tar.gz` & `tmp/mkdocs_include_markdown_plugin-5.1.0.tar.gz`

## Comparing `mkdocs_include_markdown_plugin-5.0.0.tar` & `mkdocs_include_markdown_plugin-5.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/__init__.py
--rw-r--r--   0        0        0     2710 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/cache.py
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/config.py
--rw-r--r--   0        0        0    27227 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/event.py
--rw-r--r--   0        0        0      267 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/files_watcher.py
--rw-r--r--   0        0        0     3749 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/plugin.py
--rw-r--r--   0        0        0    13050 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/process.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/py.typed
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/regexes.py
--rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/.gitignore
--rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/LICENSE
--rw-r--r--   0        0        0     8775 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/README.md
--rw-r--r--   0        0        0     5850 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/pyproject.toml
--rw-r--r--   0        0        0    10324 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.0.0/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/__init__.py
+-rw-r--r--   0        0        0     2771 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/cache.py
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/config.py
+-rw-r--r--   0        0        0     4842 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/directive.py
+-rw-r--r--   0        0        0    24183 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/event.py
+-rw-r--r--   0        0        0      287 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/files_watcher.py
+-rw-r--r--   0        0        0     3716 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/plugin.py
+-rw-r--r--   0        0        0    14066 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/process.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/py.typed
+-rw-r--r--   0        0        0      175 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/.gitignore
+-rw-r--r--   0        0        0    11365 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/LICENSE
+-rw-r--r--   0        0        0     8907 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/README.md
+-rw-r--r--   0        0        0     5844 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/pyproject.toml
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 mkdocs_include_markdown_plugin-5.1.0/PKG-INFO
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/cache.py` & `mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/cache.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,43 +4,51 @@
 
 import base64
 import hashlib
 import os
 import time
 
 
+try:
+    from platformdirs import user_data_dir
+except ImportError:
+    CACHE_AVAILABLE = False
+else:
+    CACHE_AVAILABLE = True
+
+
 class Cache:
     """Cache for arbitrary content, one file per entry."""
 
     def __init__(self, cache_dir: str, expiration_seconds: int = 0):
         self.cache_dir = cache_dir
         self.expiration_seconds = expiration_seconds
 
     def get_creation_time_from_fpath(self, fpath: str) -> int:
         """Get creation time of an entry in the cache given its path."""
         with open(fpath, encoding='utf-8') as f:
-            return int(f.readline().strip())
+            return int(f.readline())
 
     @classmethod
     def generate_unique_key_from_url(cls, url: str) -> str:
         """Generate a unique key from an URL."""
         return base64.urlsafe_b64encode(
             hashlib.sha3_512(url.encode()).digest(),
         ).decode('utf-8')
 
     def read_file(self, fpath: str) -> str:  # noqa: D102
         with open(fpath, encoding='utf-8') as f:
-            return '\n'.join(f.read().split('\n')[1:])
+            return f.read().split('\n', 1)[1]
 
     def get_(self, url: str) -> str | None:  # noqa: D102
         key = self.generate_unique_key_from_url(url)
         fpath = os.path.join(self.cache_dir, key)
         if os.path.isfile(fpath):
             creation_time = self.get_creation_time_from_fpath(fpath)
-            if time.time() > creation_time + self.expiration_seconds:
+            if time.time() < creation_time + self.expiration_seconds:
                 return self.read_file(fpath)
             else:
                 os.remove(fpath)
                 return None
         else:
             return None
 
@@ -58,26 +66,23 @@
             creation_time = self.get_creation_time_from_fpath(fpath)
             if time.time() > creation_time + self.expiration_seconds:
                 os.remove(fpath)
 
 
 def get_cache_directory() -> str | None:
     """Get the cache directory."""
-    try:
-        from platformdirs import user_data_dir
-    except ImportError:
+    if not CACHE_AVAILABLE:
         return None
 
     cache_dir = user_data_dir('mkdocs-include-markdown-plugin')
     if not os.path.isdir(cache_dir):
         os.makedirs(cache_dir)
 
     return cache_dir
 
 
 def initialize_cache(expiration_seconds: int) -> Cache | None:
     """Initialize a cache instance."""
     cache_dir = get_cache_directory()
-    if cache_dir is None:
-        return None
-
-    return Cache(cache_dir, expiration_seconds)
+    return None if cache_dir is None else Cache(
+        cache_dir, expiration_seconds,
+    )
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/event.py` & `mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/event.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,173 +4,70 @@
 
 import glob
 import html
 import logging
 import os
 import re
 import textwrap
-import urllib.request
 from collections.abc import MutableMapping
 from typing import TYPE_CHECKING, Any
-from urllib.parse import urlparse
 
 from mkdocs.exceptions import BuildError
 
 from mkdocs_include_markdown_plugin import process
 from mkdocs_include_markdown_plugin.cache import Cache
-from mkdocs_include_markdown_plugin.config import (
-    CONFIG_DEFAULTS,
-    DEFAULT_CLOSING_TAG,
-    DEFAULT_COMMENTS,
-    DEFAULT_OPENING_TAG,
+from mkdocs_include_markdown_plugin.config import CONFIG_DEFAULTS
+from mkdocs_include_markdown_plugin.directive import (
+    ARGUMENT_REGEXES,
     create_include_tag,
+    parse_bool_options,
+    parse_filename_argument,
+    parse_string_argument,
 )
 from mkdocs_include_markdown_plugin.files_watcher import FilesWatcher
-from mkdocs_include_markdown_plugin.regexes import (
-    DOUBLE_QUOTED_STR_RE,
-    SINGLE_QUOTED_STR_RE,
-)
 
 
 if TYPE_CHECKING:  # remove this for mypyc compiling
     from typing import TypedDict
 
     from mkdocs.structure.pages import Page
 
-    class DirectiveBoolArgument(TypedDict):  # noqa: D101
-        value: bool
-        regex: re.Pattern[str]
-
+    from mkdocs_include_markdown_plugin.directive import DefaultValues
 
-logger = logging.getLogger('mkdocs.plugins.mkdocs_include_markdown_plugin')
-
-TRUE_FALSE_STR_BOOL = {
-    'true': True,
-    'false': False,
-}
-
-TRUE_FALSE_BOOL_STR = {
-    True: 'true',
-    False: 'false',
-}
-
-
-def is_url(string: str) -> bool:
-    """Determines if a string is a URL."""
-    try:
-        result = urlparse(string)
-        return all([result.scheme, result.netloc])
-    except ValueError:
-        return False
-
-
-def bool_arg(arg: str) -> re.Pattern[str]:
-    """Return a compiled regexp to match a boolean argument."""
-    return re.compile(rf'{arg}=(\w+)')
-
-
-def str_arg(arg: str) -> re.Pattern[str]:
-    """Return a compiled regexp to match a string argument."""
-    return re.compile(
-        rf'{arg}=(?:"({DOUBLE_QUOTED_STR_RE})")?'
-        rf"(?:'({SINGLE_QUOTED_STR_RE})')?",
+    IncludeTags = TypedDict(
+        'IncludeTags', {
+            'include': re.Pattern[str],
+            'include-markdown': re.Pattern[str],
+        },
     )
 
 
-ARGUMENT_REGEXES = {
-    'start': str_arg('start'),
-    'end': str_arg('end'),
-    'exclude': str_arg('exclude'),
-    'encoding': str_arg('encoding'),
-
-    # bool
-    'comments': bool_arg('comments'),
-    'preserve-includer-indent': bool_arg('preserve-includer-indent'),
-    'dedent': bool_arg('dedent'),
-    'trailing-newlines': bool_arg('trailing-newlines'),
-    'rewrite-relative-urls': bool_arg('rewrite-relative-urls'),
-
-    # int
-    'heading-offset': re.compile(r'heading-offset=(-?\d+)'),
-}
-
-
-def parse_filename_argument(
-        match: re.Match[str],
-) -> tuple[str | None, str | None]:
-    """Return the filename argument matched by ``match``."""
-    raw_filename = match.group('double_quoted_filename')
-    if raw_filename is None:
-        raw_filename = match.group('single_quoted_filename')
-        if raw_filename is None:
-            filename = None
-        else:
-            filename = raw_filename.replace("\\'", "'")
-    else:
-        filename = raw_filename.replace('\\"', '"')
-    return filename, raw_filename
-
-
-def parse_string_argument(match: re.Match[str]) -> str | None:
-    """Return the string argument matched by ``match``."""
-    value = match.group(1)
-    if value is None:
-        value = match.group(3)
-        if value is not None:
-            value = value.replace("\\'", "'")
-    else:
-        value = value.replace('\\"', '"')
-    return value
+logger = logging.getLogger('mkdocs.plugins.mkdocs_include_markdown_plugin')
 
 
 def lineno_from_content_start(content: str, start: int) -> int:
     """Return the line number of the first line of ``start`` in ``content``."""
     return content[:start].count('\n') + 1
 
 
-def read_file(file_path: str, encoding: str) -> str:
-    """Read a file and return its content."""
-    with open(file_path, encoding=encoding) as f:
-        return f.read()
-
-
-def read_http(target_url: str, http_cache: Cache | None) -> Any:  # noqa: U100
-    """Read an http location and return its content."""
-    if http_cache is not None:
-        cached_content = http_cache.get_(target_url)
-        if cached_content is not None:
-            return cached_content
-    req = urllib.request.Request(target_url)
-    with urllib.request.urlopen(req) as response:
-        content = response.read().decode('UTF-8')
-    if http_cache is not None:
-        http_cache.set_(target_url, content)
-    return content
-
-
 def get_file_content(
-    markdown: str,
-    page_src_path: str,
-    docs_dir: str,
-    include_tag_regex: re.Pattern[str],
-    include_markdown_tag_regex: re.Pattern[str],
-    default_encoding: str,
-    default_preserve_includer_indent: bool,
-    default_dedent: bool,
-    default_trailing_newlines: bool,
-    default_comments: bool = DEFAULT_COMMENTS,
-    cumulative_heading_offset: int = 0,
-    files_watcher: FilesWatcher | None = None,
-    http_cache: Cache | None = None,
+        markdown: str,
+        page_src_path: str,
+        docs_dir: str,
+        tags: IncludeTags,
+        defaults: DefaultValues,
+        cumulative_heading_offset: int = 0,
+        files_watcher: FilesWatcher | None = None,
+        http_cache: Cache | None = None,
 ) -> str:
     """Return the content of the file to include."""
     def found_include_tag(match: re.Match[str]) -> str:
         directive_match_start = match.start()
 
-        _includer_indent = match.group('_includer_indent')
+        includer_indent = match.group('_includer_indent')
 
         filename, raw_filename = parse_filename_argument(match)
         if filename is None:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
@@ -178,137 +75,119 @@
                 "Found no path passed including with 'include'"
                 f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
 
         arguments_string = match.group('arguments')
 
-        if os.path.isabs(filename):
-            file_path_glob = filename
-        elif is_url(filename):
+        if os.path.isabs(filename) or process.is_url(filename):
             file_path_glob = filename
         else:
             file_path_glob = os.path.join(
                 os.path.abspath(os.path.dirname(page_src_path)),
                 filename,
             )
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
         if exclude_match is None:
-            ignore_paths: list[str] = []
+            if defaults['exclude'] is None:  # pragma: no branch
+                ignore_paths: list[str] = []
+            else:  # pragma: no cover
+                ignore_paths = glob.glob(defaults['exclude'])
         else:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise BuildError(
                     "Invalid empty 'exclude' argument in 'include' directive"
                     f' at {os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
             else:
-
                 if os.path.isabs(exclude_string):
                     exclude_globstr = exclude_string
                 else:
                     exclude_globstr = os.path.realpath(
                         os.path.join(
                             os.path.abspath(os.path.dirname(page_src_path)),
                             exclude_string,
                         ),
                     )
                 ignore_paths = glob.glob(exclude_globstr)
 
-        file_paths_to_include = process.filter_paths(
-            glob.iglob(file_path_glob, recursive=True),
-            ignore_paths=ignore_paths,
-        )
-        if is_url(filename):
+        if process.is_url(filename):
             file_paths_to_include = [file_path_glob]
+        else:
+            file_paths_to_include = process.filter_paths(
+                glob.iglob(file_path_glob, recursive=True),
+                ignore_paths,
+            )
 
         if not file_paths_to_include:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
             raise BuildError(
                 f"No files found including '{raw_filename}'"
                 f' at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
         elif files_watcher is not None:
-            if not is_url(file_path_glob):
+            if not process.is_url(file_path_glob):
                 files_watcher.included_files.extend(file_paths_to_include)
 
-        bool_options: dict[str, DirectiveBoolArgument] = {
-            'preserve-includer-indent': {
-                'value': default_preserve_includer_indent,
-                'regex': ARGUMENT_REGEXES['preserve-includer-indent'],
-            },
-            'dedent': {
-                'value': default_dedent,
-                'regex': ARGUMENT_REGEXES['dedent'],
-            },
-            'trailing-newlines': {
-                'value': default_trailing_newlines,
-                'regex': ARGUMENT_REGEXES['trailing-newlines'],
-            },
-        }
-
-        for arg_name, arg in bool_options.items():
-            bool_arg_match = arg['regex'].search(arguments_string)
-            if bool_arg_match is None:
-                continue
-            try:
-                bool_options[arg_name]['value'] = TRUE_FALSE_STR_BOOL[
-                    bool_arg_match.group(
-                        1,
-                    ) or TRUE_FALSE_BOOL_STR[arg['value']]
-                ]
-            except KeyError:
-                lineno = lineno_from_content_start(
-                    markdown,
-                    directive_match_start,
-                )
-                raise BuildError(
-                    f"Invalid value for '{arg_name}' argument of 'include'"
-                    f' directive at {os.path.relpath(page_src_path, docs_dir)}'
-                    f':{lineno}. Possible values are true or false.',
-                )
+        bool_options, invalid_bool_args = parse_bool_options(
+            ['preserve-includer-indent', 'dedent', 'trailing-newlines'],
+            defaults,
+            arguments_string,
+        )
+        if invalid_bool_args:
+            lineno = lineno_from_content_start(
+                markdown,
+                directive_match_start,
+            )
+            raise BuildError(
+                f"Invalid value for '{invalid_bool_args[0]}' argument of"
+                " 'include' directive at"
+                f' {os.path.relpath(page_src_path, docs_dir)}'
+                f':{lineno}. Possible values are true or false.',
+            )
 
         start_match = ARGUMENT_REGEXES['start'].search(arguments_string)
         if start_match:
             start = parse_string_argument(start_match)
             if start is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise BuildError(
                     "Invalid empty 'start' argument in 'include' directive at "
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
         else:
-            start = None
+            start = defaults['start']
 
         end_match = ARGUMENT_REGEXES['end'].search(arguments_string)
         if end_match:
             end = parse_string_argument(end_match)
             if end is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise BuildError(
                     "Invalid empty 'end' argument in 'include' directive at "
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
         else:
-            end = None
+            end = defaults['end']
 
         encoding_match = ARGUMENT_REGEXES['encoding'].search(arguments_string)
         if encoding_match:
             encoding = parse_string_argument(encoding_match)
             if encoding is None:
                 lineno = lineno_from_content_start(
                     markdown,
@@ -316,25 +195,25 @@
                 )
                 raise BuildError(
                     "Invalid empty 'encoding' argument in 'include'"
                     ' directive at '
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
         else:
-            encoding = default_encoding
+            encoding = defaults['encoding']
 
         text_to_include = ''
         expected_but_any_found = [start is not None, end is not None]
         for file_path in file_paths_to_include:
-            if is_url(filename):
-                new_text_to_include = read_http(file_path, http_cache)
+            if process.is_url(filename):
+                new_text_to_include = process.read_url(file_path, http_cache)
             else:
-                new_text_to_include = read_file(file_path, encoding)
+                new_text_to_include = process.read_file(file_path, encoding)
 
-            if start is not None or end is not None:
+            if start or end:
                 new_text_to_include, *expected_not_found = (
                     process.filter_inclusions(
                         start,
                         end,
                         new_text_to_include,
                     )
                 )
@@ -343,20 +222,16 @@
                         expected_but_any_found[i] = False
 
             # nested includes
             new_text_to_include = get_file_content(
                 new_text_to_include,
                 file_path,
                 docs_dir,
-                include_tag_regex,
-                include_markdown_tag_regex,
-                default_encoding,
-                default_preserve_includer_indent,
-                default_dedent,
-                default_trailing_newlines,
+                tags,
+                defaults,
                 files_watcher=files_watcher,
                 http_cache=http_cache,
             )
 
             # trailing newlines right stripping
             if not bool_options['trailing-newlines']['value']:
                 new_text_to_include = process.rstrip_trailing_newlines(
@@ -365,22 +240,22 @@
 
             if bool_options['dedent']['value']:
                 new_text_to_include = textwrap.dedent(new_text_to_include)
 
             # includer indentation preservation
             if bool_options['preserve-includer-indent']['value']:
                 new_text_to_include = ''.join(
-                    _includer_indent + line
+                    includer_indent + line
                     for line in (
                         new_text_to_include.splitlines(keepends=True)
                         or ['']
                     )
                 )
             else:
-                new_text_to_include = _includer_indent + new_text_to_include
+                new_text_to_include = includer_indent + new_text_to_include
 
             text_to_include += new_text_to_include
 
         # warn if expected start or ends haven't been found in included content
         for i, argname in enumerate(['start', 'end']):
             if expected_but_any_found[i]:
                 value = locals()[argname]
@@ -401,16 +276,16 @@
                 )
 
         return text_to_include
 
     def found_include_markdown_tag(match: re.Match[str]) -> str:
         directive_match_start = match.start()
 
-        _includer_indent = match.group('_includer_indent')
-        _empty_includer_indent = ' ' * len(_includer_indent)
+        includer_indent = match.group('_includer_indent')
+        empty_includer_indent = ' ' * len(includer_indent)
 
         filename, raw_filename = parse_filename_argument(match)
         if filename is None:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
@@ -418,27 +293,28 @@
                 "Found no path passed including with 'include-markdown'"
                 f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
 
         arguments_string = match.group('arguments')
 
-        if os.path.isabs(filename):
-            file_path_glob = filename
-        elif is_url(filename):
+        if os.path.isabs(filename) or process.is_url(filename):
             file_path_glob = filename
         else:
             file_path_glob = os.path.join(
                 os.path.abspath(os.path.dirname(page_src_path)),
                 filename,
             )
 
         exclude_match = ARGUMENT_REGEXES['exclude'].search(arguments_string)
         if exclude_match is None:
-            ignore_paths: list[str] = []
+            if defaults['exclude'] is None:  # pragma: no branch
+                ignore_paths: list[str] = []
+            else:  # pragma: no cover
+                ignore_paths = glob.glob(defaults['exclude'])
         else:
             exclude_string = parse_string_argument(exclude_match)
             if exclude_string is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
@@ -455,80 +331,56 @@
                         os.path.join(
                             os.path.abspath(os.path.dirname(page_src_path)),
                             exclude_string,
                         ),
                     )
                 ignore_paths = glob.glob(exclude_globstr)
 
-        file_paths_to_include = process.filter_paths(
-            glob.iglob(file_path_glob, recursive=True),
-            ignore_paths=ignore_paths,
-        )
-
-        if is_url(filename):
+        if process.is_url(filename):
             file_paths_to_include = [file_path_glob]
+        else:
+            file_paths_to_include = process.filter_paths(
+                glob.iglob(file_path_glob, recursive=True),
+                ignore_paths,
+            )
 
         if not file_paths_to_include:
             lineno = lineno_from_content_start(
                 markdown,
                 directive_match_start,
             )
             raise BuildError(
                 f"No files found including '{raw_filename}' at"
                 f' {os.path.relpath(page_src_path, docs_dir)}'
                 f':{lineno}',
             )
         elif files_watcher is not None:
-            if not is_url(file_path_glob):
+            if not process.is_url(file_path_glob):
                 files_watcher.included_files.extend(file_paths_to_include)
 
-        bool_options: dict[str, DirectiveBoolArgument] = {
-            'rewrite-relative-urls': {
-                'value': True,
-                'regex': ARGUMENT_REGEXES['rewrite-relative-urls'],
-            },
-            'comments': {
-                'value': default_comments,
-                'regex': ARGUMENT_REGEXES['comments'],
-            },
-            'preserve-includer-indent': {
-                'value': default_preserve_includer_indent,
-                'regex': ARGUMENT_REGEXES['preserve-includer-indent'],
-            },
-            'dedent': {
-                'value': default_dedent,
-                'regex': ARGUMENT_REGEXES['dedent'],
-            },
-            'trailing-newlines': {
-                'value': default_trailing_newlines,
-                'regex': ARGUMENT_REGEXES['trailing-newlines'],
-            },
-        }
-
-        for arg_name, arg in bool_options.items():
-            bool_arg_match = arg['regex'].search(arguments_string)
-            if bool_arg_match is None:
-                continue
-            try:
-                bool_options[arg_name]['value'] = TRUE_FALSE_STR_BOOL[
-                    bool_arg_match.group(
-                        1,
-                    ) or TRUE_FALSE_BOOL_STR[arg['value']]
-                ]
-            except KeyError:
-                lineno = lineno_from_content_start(
-                    markdown,
-                    directive_match_start,
-                )
-                raise BuildError(
-                    f"Invalid value for '{arg_name}' argument of"
-                    " 'include-markdown' directive at"
-                    f' {os.path.relpath(page_src_path, docs_dir)}'
-                    f':{lineno}. Possible values are true or false.',
-                )
+        bool_options, invalid_bool_args = parse_bool_options(
+            [
+                'rewrite-relative-urls', 'comments',
+                'preserve-includer-indent', 'dedent',
+                'trailing-newlines',
+            ],
+            defaults,
+            arguments_string,
+        )
+        if invalid_bool_args:
+            lineno = lineno_from_content_start(
+                markdown,
+                directive_match_start,
+            )
+            raise BuildError(
+                f"Invalid value for '{invalid_bool_args[0]}' argument of"
+                " 'include-markdown' directive at"
+                f' {os.path.relpath(page_src_path, docs_dir)}'
+                f':{lineno}. Possible values are true or false.',
+            )
 
         # start and end arguments
         start_match = ARGUMENT_REGEXES['start'].search(arguments_string)
         if start_match:
             start = parse_string_argument(start_match)
             if start is None:
                 lineno = lineno_from_content_start(
@@ -537,15 +389,15 @@
                 )
                 raise BuildError(
                     "Invalid empty 'start' argument in 'include-markdown'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}',
                 )
         else:
-            start = None
+            start = defaults['start']
 
         end_match = ARGUMENT_REGEXES['end'].search(arguments_string)
         if end_match:
             end = parse_string_argument(end_match)
             if end is None:
                 lineno = lineno_from_content_start(
                     markdown,
@@ -553,40 +405,62 @@
                 )
                 raise BuildError(
                     "Invalid empty 'end' argument in 'include-markdown'"
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno}',
                 )
         else:
-            end = None
+            end = defaults['end']
 
         encoding_match = ARGUMENT_REGEXES['encoding'].search(arguments_string)
         if encoding_match:
             encoding = parse_string_argument(encoding_match)
             if encoding is None:
                 lineno = lineno_from_content_start(
                     markdown,
                     directive_match_start,
                 )
                 raise BuildError(
                     "Invalid empty 'encoding' argument in 'include-markdown'"
                     ' directive at '
                     f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
                 )
-                encoding = 'utf-8'
         else:
-            encoding = default_encoding
+            encoding = defaults['encoding']
 
         # heading offset
-        offset = 0
         offset_match = ARGUMENT_REGEXES['heading-offset'].search(
             arguments_string,
         )
         if offset_match:
-            offset += int(offset_match.group(1))
+            offset = offset_match.group(1)
+            if offset == '':
+                lineno = lineno_from_content_start(
+                    markdown,
+                    directive_match_start,
+                )
+                raise BuildError(
+                    "Invalid empty 'heading-offset' argument in"
+                    " 'include-markdown' directive at"
+                    f' {os.path.relpath(page_src_path, docs_dir)}:{lineno}',
+                )
+            try:
+                offset = int(offset)
+            except ValueError:
+                lineno = lineno_from_content_start(
+                    markdown,
+                    directive_match_start,
+                )
+                raise BuildError(
+                    f"Invalid 'heading-offset' argument \"{offset}\" in"
+                    " 'include-markdown' directive at "
+                    f'{os.path.relpath(page_src_path, docs_dir)}:{lineno}',
+                )
+        else:
+            offset = defaults['heading-offset']
 
         separator = '\n' if bool_options['trailing-newlines']['value'] else ''
         if not start and not end:
             start_end_part = ''
         else:
             start_end_part = f"'{html.escape(start)}' " if start else "'' "
             start_end_part += f"'{html.escape(end)}' " if end else "'' "
@@ -596,20 +470,20 @@
         #
         # `True` means that no start/end strings have been found in content
         # but they have been specified, so the warning(s) must be raised
         expected_but_any_found = [start is not None, end is not None]
 
         text_to_include = ''
         for file_path in file_paths_to_include:
-            if is_url(filename):
-                new_text_to_include = read_http(file_path, http_cache)
+            if process.is_url(filename):
+                new_text_to_include = process.read_url(file_path, http_cache)
             else:
-                new_text_to_include = read_file(file_path, encoding)
+                new_text_to_include = process.read_file(file_path, encoding)
 
-            if start is not None or end is not None:
+            if start or end:
                 new_text_to_include, *expected_not_found = (
                     process.filter_inclusions(
                         start,
                         end,
                         new_text_to_include,
                     )
                 )
@@ -618,21 +492,16 @@
                         expected_but_any_found[i] = False
 
             # nested includes
             new_text_to_include = get_file_content(
                 new_text_to_include,
                 file_path,
                 docs_dir,
-                include_tag_regex,
-                include_markdown_tag_regex,
-                default_encoding,
-                default_preserve_includer_indent,
-                default_dedent,
-                default_trailing_newlines,
-                default_comments=default_comments,
+                tags,
+                defaults,
                 files_watcher=files_watcher,
                 http_cache=http_cache,
             )
 
             # trailing newlines right stripping
             if not bool_options['trailing-newlines']['value']:
                 new_text_to_include = process.rstrip_trailing_newlines(
@@ -646,32 +515,32 @@
                     source_path=file_path,
                     destination_path=page_src_path,
                 )
 
             # comments
             if bool_options['comments']['value']:
                 new_text_to_include = (
-                    f'{_includer_indent}'
+                    f'{includer_indent}'
                     f'<!-- BEGIN INCLUDE {html.escape(filename)}'
                     f' {start_end_part}-->{separator}{new_text_to_include}'
                     f'{separator}<!-- END INCLUDE -->'
                 )
             else:
                 new_text_to_include = (
-                    f'{_includer_indent}{new_text_to_include}'
+                    f'{includer_indent}{new_text_to_include}'
                 )
 
             # dedent
             if bool_options['dedent']['value']:
                 new_text_to_include = textwrap.dedent(new_text_to_include)
 
             # includer indentation preservation
             if bool_options['preserve-includer-indent']['value']:
                 new_text_to_include = ''.join(
-                    (_empty_includer_indent if i > 0 else '') + line
+                    (empty_includer_indent if i > 0 else '') + line
                     for i, line in enumerate(
                         new_text_to_include.splitlines(keepends=True)
                         or [''],
                     )
                 )
 
             if offset_match:
@@ -700,60 +569,78 @@
                     f' directive at {os.path.relpath(page_src_path, docs_dir)}'
                     f':{lineno} not detected in the file{plural_suffix}'
                     f' {readable_files_to_include}',
                 )
 
         return text_to_include
 
-    markdown = include_tag_regex.sub(
+    markdown = tags['include'].sub(
         found_include_tag,
         markdown,
     )
-    markdown = include_markdown_tag_regex.sub(
+    markdown = tags['include-markdown'].sub(
         found_include_markdown_tag,
         markdown,
     )
     return markdown
 
 
 def on_page_markdown(
-    markdown: str,
-    page: Page,
-    docs_dir: str,
-    config: MutableMapping[str, Any] | None = None,
-    files_watcher: FilesWatcher | None = None,
-    http_cache: Cache | None = None,
+        markdown: str,
+        page: Page,
+        docs_dir: str,
+        config: MutableMapping[str, Any] | None = None,
+        files_watcher: FilesWatcher | None = None,
+        http_cache: Cache | None = None,
 ) -> str:
     """Process markdown content of a page."""
     if config is None:
         config = {}
 
     return get_file_content(
         markdown,
         page.file.abs_src_path,
         docs_dir,
-        config.get(
-            '_include_tag',
-            create_include_tag(
-                config.get('opening_tag', DEFAULT_OPENING_TAG),
-                config.get('closing_tag', DEFAULT_CLOSING_TAG),
+        {
+            'include': config.get(
+                '_include_tag',
+                create_include_tag(
+                    config.get('opening_tag', CONFIG_DEFAULTS['opening-tag']),
+                    config.get('closing_tag', CONFIG_DEFAULTS['closing-tag']),
+                ),
+            ),
+            'include-markdown': config.get(
+                '_include_markdown_tag',
+                create_include_tag(
+                    config.get('opening_tag', CONFIG_DEFAULTS['opening-tag']),
+                    config.get('closing_tag', CONFIG_DEFAULTS['closing-tag']),
+                    tag='include-markdown',
+                ),
+            ),
+        },
+        {
+            'encoding': config.get('encoding', CONFIG_DEFAULTS['encoding']),
+            'preserve-includer-indent': config.get(
+                'preserve_includer_indent',
+                CONFIG_DEFAULTS['preserve-includer-indent'],
+            ),
+            'dedent': config.get('dedent', CONFIG_DEFAULTS['dedent']),
+            'trailing-newlines': config.get(
+                'trailing_newlines',
+                CONFIG_DEFAULTS['trailing-newlines'],
+            ),
+            'comments': config.get('comments', CONFIG_DEFAULTS['comments']),
+            'rewrite-relative-urls': config.get(
+                'rewrite_relative_urls',
+                CONFIG_DEFAULTS['rewrite-relative-urls'],
             ),
-        ),
-        config.get(
-            '_include_markdown_tag',
-            create_include_tag(
-                config.get('opening_tag', DEFAULT_OPENING_TAG),
-                config.get('closing_tag', DEFAULT_CLOSING_TAG),
-                tag='include-markdown',
+            'heading-offset': config.get(
+                'heading_offset',
+                CONFIG_DEFAULTS['heading-offset'],
             ),
-        ),
-        config.get('encoding', CONFIG_DEFAULTS['encoding']),
-        config.get(
-            'preserve_includer_indent',
-            CONFIG_DEFAULTS['preserve_includer_indent'],
-        ),
-        config.get('dedent', CONFIG_DEFAULTS['dedent']),
-        config.get('trailing_newlines', CONFIG_DEFAULTS['trailing_newlines']),
-        default_comments=config.get('comments', CONFIG_DEFAULTS['comments']),
+            'start': config.get('start', CONFIG_DEFAULTS['start']),
+            'end': config.get('end', CONFIG_DEFAULTS['end']),
+            'exclude': config.get('exclude', CONFIG_DEFAULTS['exclude']),
+        },
         files_watcher=files_watcher,
         http_cache=config.get('_cache', http_cache),
     )
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/plugin.py` & `mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/plugin.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,18 +12,16 @@
 
 if TYPE_CHECKING:
     from mkdocs.config.defaults import MkDocsConfig
     from mkdocs.structure.files import Files
     from mkdocs.structure.pages import Page
 
 from mkdocs_include_markdown_plugin.cache import initialize_cache
-from mkdocs_include_markdown_plugin.config import (
-    CONFIG_SCHEME,
-    create_include_tag,
-)
+from mkdocs_include_markdown_plugin.config import CONFIG_SCHEME
+from mkdocs_include_markdown_plugin.directive import create_include_tag
 from mkdocs_include_markdown_plugin.event import (
     on_page_markdown as _on_page_markdown,
 )
 from mkdocs_include_markdown_plugin.files_watcher import FilesWatcher
 
 
 SERVER: LiveReloadServer | None = None
@@ -56,54 +54,51 @@
                 )
             else:
                 cache.clean()
                 self.config['_cache'] = cache
 
         return config
 
-    def _watch_included_files(self) -> None:
+    def _watch_included_files(self) -> None:  # pragma: no cover
         global FILES_WATCHER, SERVER
         SERVER = cast(LiveReloadServer, SERVER)
+        FILES_WATCHER = cast(FilesWatcher, FILES_WATCHER)
+
+        # unwatch previous watched files not needed anymore
+        for filepath in FILES_WATCHER.prev_included_files:
+            if filepath not in FILES_WATCHER.included_files:
+                SERVER.unwatch(filepath)
+        FILES_WATCHER.prev_included_files = (
+            FILES_WATCHER.included_files[:]
+        )
 
-        # compatibility with Mkdocs < 1.4.0
-        if hasattr(SERVER, 'unwatch'):
-            FILES_WATCHER = cast(FilesWatcher, FILES_WATCHER)
-
-            # unwatch previous watched files not needed anymore
-            for filepath in FILES_WATCHER.prev_included_files:
-                if filepath not in FILES_WATCHER.included_files:
-                    SERVER.unwatch(filepath)
-            FILES_WATCHER.prev_included_files = (
-                FILES_WATCHER.included_files[:]
-            )
-
-            # watch new included files
-            for filepath in FILES_WATCHER.included_files:
-                SERVER.watch(filepath, recursive=False)
-            FILES_WATCHER.included_files = []
+        # watch new included files
+        for filepath in FILES_WATCHER.included_files:
+            SERVER.watch(filepath, recursive=False)
+        FILES_WATCHER.included_files = []
 
     def on_page_content(
             self,
             html: str,
             page: Page,
             config: MkDocsConfig,
             files: Files,
     ) -> str:
-        if SERVER is not None:
+        if SERVER is not None:  # pragma: no cover
             self._watch_included_files()
         return html
 
     def on_serve(
             self,
             server: LiveReloadServer,
             config: MkDocsConfig,
             builder: Callable[[Any], Any],
     ) -> None:
         global SERVER
-        if SERVER is None:
+        if SERVER is None:  # pragma: no cover
             SERVER = server
             self._watch_included_files()
 
     @event_priority(100)
     def on_page_markdown(
             self,
             markdown: str,
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/src/mkdocs_include_markdown_plugin/process.py` & `mkdocs_include_markdown_plugin-5.1.0/src/mkdocs_include_markdown_plugin/process.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,21 @@
 from __future__ import annotations
 
 import functools
 import io
 import os
 import re
 from collections.abc import Callable, Iterator
+from typing import TYPE_CHECKING, Any
 from urllib.parse import urlparse, urlunparse
+from urllib.request import Request, urlopen
+
+
+if TYPE_CHECKING:
+    from mkdocs_include_markdown_plugin.cache import Cache
 
 
 # Markdown regular expressions. Taken from the original Markdown.pl by John
 # Gruber, and modified to work in Python
 
 # Matches markdown links.
 # e.g. [scikit-learn](https://github.com/scikit-learn/scikit-learn)
@@ -195,15 +201,17 @@
             _current_fcodeblock_delimiter = ''
         lines.append(line)
 
     return ''.join(lines)
 
 
 def rewrite_relative_urls(
-    markdown: str, source_path: str, destination_path: str,
+        markdown: str,
+        source_path: str,
+        destination_path: str,
 ) -> str:
     """Rewrite relative URLs in a Markdown text.
 
     Rewrites markdown so that relative links that were written at
     ``source_path`` will still work when inserted into a file at
     ``destination_path``.
     """
@@ -272,17 +280,17 @@
     Replaces any standard escape sequences in value with their usual
     meanings as in ordinary Python string literals.
     """
     return value.encode('latin-1', 'backslashreplace').decode('unicode_escape')
 
 
 def filter_inclusions(
-    new_start: str | None,
-    new_end: str | None,
-    text_to_include: str,
+        new_start: str | None,
+        new_end: str | None,
+        text_to_include: str,
 ) -> tuple[str, bool, bool]:
     """Filter inclusions in a text.
 
     Manages inclusions from files using ``start`` and ``end`` directive
     arguments.
     """
     expected_start_not_found, expected_end_not_found = (False, False)
@@ -312,15 +320,15 @@
                     start,
                     maxsplit=1,
                 )[1]
             else:
                 expected_start_not_found = True
         text_to_include = new_text_to_include
 
-    elif new_end is not None:
+    elif new_end is not None:  # pragma: no branch
         end = interpret_escapes(new_end)
         if end in text_to_include:
             text_to_include = text_to_include.split(
                 end,
                 maxsplit=1,
             )[0]
         else:
@@ -369,15 +377,15 @@
     while content.endswith('\n') or content.endswith('\r'):
         content = content.rstrip('\r\n')
     return content
 
 
 def filter_paths(
         filepaths: Iterator[str],
-        ignore_paths: list[str] | None = None,
+        ignore_paths: list[str],
 ) -> list[str]:
     """Filters a list of paths removing those defined in other list of paths.
 
     The paths to filter can be defined in the list of paths to ignore in
     several forms:
 
     - The same string.
@@ -388,17 +396,14 @@
     Args:
         filepaths (list): Set of source paths to filter.
         ignore_paths (list): Paths that must not be included in the response.
 
     Returns:
         list: Non filtered paths ordered alphabetically.
     """
-    if ignore_paths is None:
-        ignore_paths = []
-
     response = []
     for filepath in filepaths:
         # ignore by filepath
         if filepath in ignore_paths:
             continue
 
         # ignore by dirpath (relative or absolute)
@@ -406,7 +411,35 @@
             continue
 
         # ignore if is a directory
         if not os.path.isdir(filepath):
             response.append(filepath)
     response.sort()
     return response
+
+
+def is_url(string: str) -> bool:
+    """Determine if a string is an URL."""
+    try:
+        result = urlparse(string)
+        return all([result.scheme, result.netloc])
+    except ValueError:  # pragma: no cover
+        return False
+
+
+def read_file(file_path: str, encoding: str) -> str:
+    """Read a file and return its content."""
+    with open(file_path, encoding=encoding) as f:
+        return f.read()
+
+
+def read_url(url: str, http_cache: Cache | None) -> Any:  # noqa: U100
+    """Read an HTTP location and return its content."""
+    if http_cache is not None:
+        cached_content = http_cache.get_(url)
+        if cached_content is not None:
+            return cached_content
+    with urlopen(Request(url)) as response:
+        content = response.read().decode('UTF-8')
+    if http_cache is not None:
+        http_cache.set_(url, content)
+    return content
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/LICENSE` & `mkdocs_include_markdown_plugin-5.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs_include_markdown_plugin-5.0.0/README.md` & `mkdocs_include_markdown_plugin-5.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -57,14 +57,19 @@
       opening_tag: "{!"
       closing_tag: "!}"
       encoding: ascii
       preserve_includer_indent: false
       dedent: false
       trailing_newlines: true
       comments: true
+      rewrite_relative_urls: true
+      heading_offset: 0
+      start: <!--start-->
+      end: <!--end-->
+      exclude: LICENSE.md
 ```
 
 The `cache` setting defines a expiration time in seconds for HTTP requests
 when including from URLs.
 
 ```yaml
 plugins:
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/pyproject.toml` & `mkdocs_include_markdown_plugin-5.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "mkdocs-include-markdown-plugin"
-version = "5.0.0"
+version = "5.1.0"
 description = "Mkdocs Markdown includer plugin."
 readme = "README.md"
 license = "Apache-2.0"
 requires-python = ">=3.8,<3.13"
 classifiers = [
   "Development Status :: 5 - Production/Stable",
   "Operating System :: OS Independent",
@@ -107,16 +107,17 @@
   "gh://mondeja/project-config-styles@v4.3/python/tests.json5",
   "gh://mondeja/project-config-styles@v4.3/python/google-docstrings.json5",
   "gh://mondeja/project-config-styles@v4.3/python/mypy.json5",
 ]
 
 [tool.coverage.run]
 source = ["src"]
-omit = ["src/mkdocs_include_markdown_plugin/plugin.py"]
 plugins = ["covdefaults"]
+parallel = true
+data_file = ".coverage/.coverage"
 
 [tool.coverage.report]
 exclude_lines = [
   "def __repr__\\(",
   "@(abc\\.)?abstractmethod",
 ]
 fail_under = 1
```

### Comparing `mkdocs_include_markdown_plugin-5.0.0/PKG-INFO` & `mkdocs_include_markdown_plugin-5.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mkdocs-include-markdown-plugin
-Version: 5.0.0
+Version: 5.1.0
 Summary: Mkdocs Markdown includer plugin.
 Project-URL: Source, https://github.com/mondeja/mkdocs-include-markdown-plugin
 Project-URL: Documentation, https://github.com/mondeja/mkdocs-include-markdown-plugin#documentation
 Project-URL: Bug tracker, https://github.com/mondeja/mkdocs-include-markdown-plugin/issues
 Project-URL: Changelog, https://github.com/mondeja/mkdocs-include-markdown-plugin/releases
 Author: Joe Rickerby
 Author-email: Álvaro Mondéjar Rubio <mondejar1994@gmail.com>
@@ -90,14 +90,19 @@
       opening_tag: "{!"
       closing_tag: "!}"
       encoding: ascii
       preserve_includer_indent: false
       dedent: false
       trailing_newlines: true
       comments: true
+      rewrite_relative_urls: true
+      heading_offset: 0
+      start: <!--start-->
+      end: <!--end-->
+      exclude: LICENSE.md
 ```
 
 The `cache` setting defines a expiration time in seconds for HTTP requests
 when including from URLs.
 
 ```yaml
 plugins:
```

