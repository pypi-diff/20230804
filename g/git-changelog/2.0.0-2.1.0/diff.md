# Comparing `tmp/git_changelog-2.0.0.tar.gz` & `tmp/git_changelog-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "git_changelog-2.0.0.tar", last modified: Mon Jul  3 13:07:07 2023, max compression
+gzip compressed data, was "git_changelog-2.1.0.tar", last modified: Fri Aug  4 13:21:20 2023, max compression
```

## Comparing `git_changelog-2.0.0.tar` & `git_changelog-2.1.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0      754 2023-07-01 10:51:08.684355 git_changelog-2.0.0/LICENSE
--rw-r--r--   0        0        0     8453 2023-07-03 13:00:29.469919 git_changelog-2.0.0/README.md
--rw-r--r--   0        0        0     2723 2023-07-03 13:07:07.133360 git_changelog-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      254 2023-07-01 10:51:08.684355 git_changelog-2.0.0/src/git_changelog/__init__.py
--rw-r--r--   0        0        0      387 2023-07-01 10:51:08.684355 git_changelog-2.0.0/src/git_changelog/__main__.py
--rw-r--r--   0        0        0    15261 2023-07-03 12:39:27.374475 git_changelog-2.0.0/src/git_changelog/build.py
--rw-r--r--   0        0        0    16161 2023-07-03 12:44:30.582591 git_changelog-2.0.0/src/git_changelog/cli.py
--rw-r--r--   0        0        0    13926 2023-07-01 11:37:50.518284 git_changelog-2.0.0/src/git_changelog/commit.py
--rw-r--r--   0        0        0    11252 2023-07-01 11:07:50.369403 git_changelog-2.0.0/src/git_changelog/providers.py
--rw-r--r--   0        0        0        0 2023-07-01 10:51:06.314370 git_changelog-2.0.0/src/git_changelog/py.typed
--rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-2.0.0/src/git_changelog/templates/__init__.py
--rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-2.0.0/src/git_changelog/templates/angular.md.jinja
--rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-2.0.0/src/git_changelog/templates/keepachangelog.md.jinja
--rw-r--r--   0        0        0      166 2023-07-01 10:51:06.304370 git_changelog-2.0.0/tests/__init__.py
--rw-r--r--   0        0        0       47 2023-07-01 10:51:06.304370 git_changelog-2.0.0/tests/conftest.py
--rw-r--r--   0        0        0     2361 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_angular_style.py
--rw-r--r--   0        0        0     2308 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_basic_style.py
--rw-r--r--   0        0        0     1172 2023-07-01 10:51:08.684355 git_changelog-2.0.0/tests/test_cli.py
--rw-r--r--   0        0        0     1079 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_commit.py
--rw-r--r--   0        0        0     5483 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_conventional_commit_style.py
--rw-r--r--   0        0        0     6708 2023-07-03 12:39:27.101147 git_changelog-2.0.0/tests/test_end_to_end.py
--rw-r--r--   0        0        0     1207 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_providers.py
--rw-r--r--   0        0        0      897 2023-07-03 12:39:27.097813 git_changelog-2.0.0/tests/test_release_notes.py
--rw-r--r--   0        0        0     2297 2023-05-10 15:20:51.179724 git_changelog-2.0.0/tests/test_version.py
--rw-r--r--   0        0        0    10008 1970-01-01 00:00:00.000000 git_changelog-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0      754 2023-08-04 13:16:20.562521 git_changelog-2.1.0/LICENSE
+-rw-r--r--   0        0        0     8585 2023-08-04 13:16:20.562521 git_changelog-2.1.0/README.md
+-rw-r--r--   0        0        0     2723 2023-08-04 13:21:20.475985 git_changelog-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      278 2023-08-04 13:16:20.562521 git_changelog-2.1.0/src/git_changelog/__init__.py
+-rw-r--r--   0        0        0      387 2023-08-04 13:16:20.562521 git_changelog-2.1.0/src/git_changelog/__main__.py
+-rw-r--r--   0        0        0    15393 2023-08-04 13:11:59.185352 git_changelog-2.1.0/src/git_changelog/build.py
+-rw-r--r--   0        0        0    16153 2023-08-04 13:16:20.562521 git_changelog-2.1.0/src/git_changelog/cli.py
+-rw-r--r--   0        0        0    13932 2023-08-04 13:11:59.185352 git_changelog-2.1.0/src/git_changelog/commit.py
+-rw-r--r--   0        0        0    14243 2023-08-04 13:11:59.185352 git_changelog-2.1.0/src/git_changelog/providers.py
+-rw-r--r--   0        0        0        0 2023-08-04 13:16:18.062518 git_changelog-2.1.0/src/git_changelog/py.typed
+-rw-r--r--   0        0        0     1122 2023-02-03 19:05:40.815432 git_changelog-2.1.0/src/git_changelog/templates/__init__.py
+-rw-r--r--   0        0        0     1588 2023-02-04 13:50:13.931438 git_changelog-2.1.0/src/git_changelog/templates/angular.md.jinja
+-rw-r--r--   0        0        0     2213 2023-02-04 13:49:16.982323 git_changelog-2.1.0/src/git_changelog/templates/keepachangelog.md.jinja
+-rw-r--r--   0        0        0      166 2023-08-04 13:16:18.052518 git_changelog-2.1.0/tests/__init__.py
+-rw-r--r--   0        0        0       47 2023-08-04 13:16:18.052518 git_changelog-2.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     2361 2023-05-10 15:20:51.179724 git_changelog-2.1.0/tests/test_angular_style.py
+-rw-r--r--   0        0        0     2308 2023-05-10 15:20:51.179724 git_changelog-2.1.0/tests/test_basic_style.py
+-rw-r--r--   0        0        0     1172 2023-08-04 13:16:20.562521 git_changelog-2.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1079 2023-05-10 15:20:51.179724 git_changelog-2.1.0/tests/test_commit.py
+-rw-r--r--   0        0        0     5483 2023-05-10 15:20:51.179724 git_changelog-2.1.0/tests/test_conventional_commit_style.py
+-rw-r--r--   0        0        0     6708 2023-07-03 12:39:27.101147 git_changelog-2.1.0/tests/test_end_to_end.py
+-rw-r--r--   0        0        0     1505 2023-08-04 13:14:50.955733 git_changelog-2.1.0/tests/test_providers.py
+-rw-r--r--   0        0        0      897 2023-07-03 12:39:27.097813 git_changelog-2.1.0/tests/test_release_notes.py
+-rw-r--r--   0        0        0     2297 2023-05-10 15:20:51.179724 git_changelog-2.1.0/tests/test_version.py
+-rw-r--r--   0        0        0    10140 1970-01-01 00:00:00.000000 git_changelog-2.1.0/PKG-INFO
```

### Comparing `git_changelog-2.0.0/LICENSE` & `git_changelog-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/README.md` & `git_changelog-2.1.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
   You get full control over the rendering.
   Built-in [Keep a Changelog][keep-a-changelog] and [Angular][angular] templates
   (also see [Conventional Changelog][conventional-changelog]).
 - Commit styles/conventions parsing.
   Built-in [Angular][angular-convention], [Conventional Commit][conventional-commit], [Atom][atom-convention] and basic conventions.
 - Git service/provider agnostic,
   plus references parsing (issues, commits, etc.).
-  Built-in [GitHub][github-refs] and [Gitlab][gitlab-refs] support.
+  Built-in [GitHub][github-refs], [Gitlab][gitlab-refs] and [Bitbucket][bitbucket-refs] support.
 - Understands [Semantic Versioning][semantic-versioning]:
   major/minor/patch for versions and commits.
   Guesses next version based on last commits.
 - Parses [Git trailers][git-trailers], allowing to reference
   issues, PRs, etc., in your commit messages
   in a clean, provider-agnostic way.
 
@@ -40,14 +40,15 @@
 [conventional-changelog]: https://github.com/conventional-changelog/conventional-changelog
 [semantic-versioning]:    http://semver.org/spec/v2.0.0.html
 [atom-convention]:        https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages
 [angular-convention]:     https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
 [conventional-commit]:    https://www.conventionalcommits.org/en/v1.0.0/
 [github-refs]:            https://help.github.com/articles/autolinked-references-and-urls/
 [gitlab-refs]:            https://docs.gitlab.com/ce/user/markdown.html#special-gitlab-references
+[bitbucket-refs]:         https://support.atlassian.com/bitbucket-cloud/docs/markup-comments
 [git-trailers]:           https://git-scm.com/docs/git-interpret-trailers
 
 [issue-14]: https://github.com/pawamoy/git-changelog/issues/14
 [issue-15]: https://github.com/pawamoy/git-changelog/issues/15
 [issue-16]: https://github.com/pawamoy/git-changelog/issues/16
 [issue-17]: https://github.com/pawamoy/git-changelog/issues/17
 [issue-19]: https://github.com/pawamoy/git-changelog/issues/19
@@ -164,15 +165,15 @@
                         missing from changelog). If two marker lines are
                         present in the changelog, the contents between those
                         two lines will be overwritten (useful to update an
                         'Unreleased' entry for example). Default: <!--
                         insertion marker -->.
   -o, --output OUTPUT   Output to given file. Default: stdout.
   -r, --parse-refs      Parse provider-specific references in commit messages
-                        (GitHub/GitLab issues, PRs, etc.). Default: False.
+                        (GitHub/GitLab/Bitbucket issues, PRs, etc.). Default: False.
   -R, --release-notes   Output release notes to stdout based on the last entry
                         in the changelog. Default: False.
   -I, --input INPUT     Read from given file when creating release notes.
                         Default: CHANGELOG.md.
   -c, --style, --commit-style, --convention {angular,atom,conventional,basic}
                         The commit convention to match against. Default:
                         basic.
```

### Comparing `git_changelog-2.0.0/pyproject.toml` & `git_changelog-2.1.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     "Topic :: Utilities",
     "Typing :: Typed",
 ]
 dependencies = [
     "Jinja2>=2.10,<4",
     "semver>=2.13",
 ]
-version = "2.0.0"
+version = "2.1.0"
 
 [project.license]
 text = "ISC"
 
 [project.urls]
 Homepage = "https://pawamoy.github.io/git-changelog"
 Documentation = "https://pawamoy.github.io/git-changelog"
@@ -80,15 +80,15 @@
 ci-tests = [
     "git-changelog[duty,tests]",
 ]
 docs = [
     "black>=23.1",
     "markdown-callouts>=0.2",
     "markdown-exec>=0.5",
-    "mkdocs>=1.3",
+    "mkdocs>=1.5",
     "mkdocs-coverage>=0.2",
     "mkdocs-gen-files>=0.3",
     "mkdocs-git-committers-plugin-2>=1.1",
     "mkdocs-literate-nav>=0.4",
     "mkdocs-material>=7.3",
     "mkdocs-minify-plugin>=0.6.4",
     "mkdocstrings[python]>=0.18",
```

### Comparing `git_changelog-2.0.0/src/git_changelog/build.py` & `git_changelog-2.1.0/src/git_changelog/build.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     AngularConvention,
     AtomConvention,
     BasicConvention,
     Commit,
     CommitConvention,
     ConventionalCommitConvention,
 )
-from git_changelog.providers import GitHub, GitLab, ProviderRefParser
+from git_changelog.providers import Bitbucket, GitHub, GitLab, ProviderRefParser
 
 if TYPE_CHECKING:
     from pathlib import Path
 
 ConventionType = Union[str, CommitConvention, Type[CommitConvention]]
 
 
@@ -193,14 +193,16 @@
             split = remote_url.split("/")
             provider_url = "/".join(split[:3])
             namespace, project = "/".join(split[3:-1]), split[-1]
             if "github" in provider_url:
                 provider = GitHub(namespace, project, url=provider_url)
             elif "gitlab" in provider_url:
                 provider = GitLab(namespace, project, url=provider_url)
+            elif "bitbucket" in provider_url:
+                provider = Bitbucket(namespace, project, url=provider_url)
             self.remote_url: str = remote_url
         self.provider = provider
 
         # set convention
         if isinstance(convention, str):
             try:
                 convention = self.CONVENTION[convention]()
```

### Comparing `git_changelog-2.0.0/src/git_changelog/cli.py` & `git_changelog-2.1.0/src/git_changelog/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -167,15 +167,15 @@
     )
     parser.add_argument(
         "-r",
         "--parse-refs",
         action="store_true",
         dest="parse_refs",
         default=False,
-        help="Parse provider-specific references in commit messages (GitHub/GitLab issues, PRs, etc.). Default: %(default)s.",
+        help="Parse provider-specific references in commit messages (GitHub/GitLab/Bitbucket issues, PRs, etc.). Default: %(default)s.",
     )
     parser.add_argument(
         "-R",
         "--release-notes",
         action="store_true",
         dest="release_notes",
         default=False,
@@ -326,18 +326,18 @@
             version_regex = DEFAULT_VERSION_REGEX
             marker_line = DEFAULT_MARKER_LINE
 
         # only keep new entries (missing from changelog)
         last_released = _latest(lines, re.compile(version_regex))
         if last_released:
             # check if the latest version is already in the changelog
-            if (
-                last_released == changelog.versions_list[0].tag
-                or last_released == changelog.versions_list[0].planned_tag
-            ):
+            if last_released in [
+                changelog.versions_list[0].tag,
+                changelog.versions_list[0].planned_tag,
+            ]:
                 raise ValueError(f"Version {last_released} already in changelog")
             changelog.versions_list = _unreleased(
                 changelog.versions_list,
                 last_released,
             )
 
         # render new entries
```

### Comparing `git_changelog-2.0.0/src/git_changelog/commit.py` & `git_changelog-2.1.0/src/git_changelog/commit.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from __future__ import annotations
 
 import re
 from abc import ABC, abstractmethod
 from collections import defaultdict
 from contextlib import suppress
-from datetime import datetime
+from datetime import datetime, timezone
 from typing import TYPE_CHECKING, Any, ClassVar, Pattern
 
 if TYPE_CHECKING:
     from git_changelog.providers import ProviderRefParser, Ref
 
 
 def _clean_body(lines: list[str]) -> list[str]:
@@ -55,19 +55,19 @@
             body: The commit message body.
             url: The commit URL.
             parse_trailers: Whether to parse Git trailers.
         """
         if not author_date:
             author_date = datetime.now()  # noqa: DTZ005
         elif isinstance(author_date, str):
-            author_date = datetime.utcfromtimestamp(float(author_date))  # noqa: DTZ004
+            author_date = datetime.fromtimestamp(float(author_date), tz=timezone.utc)
         if not committer_date:
             committer_date = datetime.now()  # noqa: DTZ005
         elif isinstance(committer_date, str):
-            committer_date = datetime.utcfromtimestamp(float(committer_date))  # noqa: DTZ004
+            committer_date = datetime.fromtimestamp(float(committer_date), tz=timezone.utc)
 
         self.hash: str = commit_hash
         self.author_name: str = author_name
         self.author_email: str = author_email
         self.author_date: datetime = author_date
         self.committer_name: str = committer_name
         self.committer_email: str = committer_email
```

### Comparing `git_changelog-2.0.0/src/git_changelog/providers.py` & `git_changelog-2.1.0/src/git_changelog/providers.py`

 * *Files 8% similar despite different names*

```diff
@@ -298,7 +298,82 @@
         return super().build_ref_url(ref_type, match_dict)
 
     def get_tag_url(self, tag: str = "") -> str:  # noqa: D102
         return self.tag_url.format(base_url=self.url, namespace=self.namespace, project=self.project, ref=tag)
 
     def get_compare_url(self, base: str, target: str) -> str:  # noqa: D102 (use parent docstring)
         return self.build_ref_url("commits_ranges", {"ref": f"{base}...{target}"})
+
+
+class Bitbucket(ProviderRefParser):
+    """A parser for the Bitbucket references."""
+
+    url: str = "https://bitbucket.org"
+    project_url: str = "{base_url}/{namespace}/{project}"
+    tag_url: str = "{base_url}/{namespace}/{project}/commits/tag/{ref}"
+
+    commit_min_length = 8
+    commit_max_length = 40
+
+    REF: ClassVar[dict[str, RefDef]] = {
+        "issues": RefDef(
+            regex=re.compile(RefRe.BB + RefRe.NP + "?issue\\s*" + RefRe.ID.format(symbol="#"), re.I),
+            url_string="{base_url}/{namespace}/{project}/issues/{ref}",
+        ),
+        "merge_requests": RefDef(
+            regex=re.compile(RefRe.BB + RefRe.NP + "?pull request\\s*" + RefRe.ID.format(symbol=r"#"), re.I),
+            url_string="{base_url}/{namespace}/{project}/pull-request/{ref}",
+        ),
+        "commits": RefDef(
+            regex=re.compile(
+                RefRe.BB
+                + r"(?:{np}@)?{commit}{ba}".format(
+                    np=RefRe.NP,
+                    commit=RefRe.COMMIT.format(min=commit_min_length, max=commit_max_length),
+                    ba=RefRe.BA,
+                ),
+                re.I,
+            ),
+            url_string="{base_url}/{namespace}/{project}/commits/{ref}",
+        ),
+        "commits_ranges": RefDef(
+            regex=re.compile(
+                RefRe.BB
+                + r"(?:{np}@)?{commit_range}".format(
+                    np=RefRe.NP,
+                    commit_range=RefRe.COMMIT_RANGE.format(min=commit_min_length, max=commit_max_length),
+                ),
+                re.I,
+            ),
+            url_string="{base_url}/{namespace}/{project}/branches/compare/{ref}#diff",
+        ),
+        "mentions": RefDef(
+            regex=re.compile(RefRe.BB + RefRe.MENTION, re.I),
+            url_string="{base_url}/{ref}",
+        ),
+    }
+
+    def __init__(self, namespace: str, project: str, url: str = url):
+        """Initialization method.
+
+        Arguments:
+            namespace: The Bitbucket namespace.
+            project: The Bitbucket project.
+            url: The Bitbucket URL.
+        """
+        self.namespace: str = namespace
+        self.project: str = project
+        self.url: str = url  # (shadowing but uses class' as default)
+
+    def build_ref_url(self, ref_type: str, match_dict: dict[str, str]) -> str:  # noqa: D102 (use parent docstring)
+        match_dict["base_url"] = self.url
+        if not match_dict.get("namespace"):
+            match_dict["namespace"] = self.namespace
+        if not match_dict.get("project"):
+            match_dict["project"] = self.project
+        return super().build_ref_url(ref_type, match_dict)
+
+    def get_tag_url(self, tag: str = "") -> str:  # noqa: D102
+        return self.tag_url.format(base_url=self.url, namespace=self.namespace, project=self.project, ref=tag)
+
+    def get_compare_url(self, base: str, target: str) -> str:  # noqa: D102 (use parent docstring)
+        return self.build_ref_url("commits_ranges", {"ref": f"{target}..{base}"})
```

### Comparing `git_changelog-2.0.0/src/git_changelog/templates/__init__.py` & `git_changelog-2.1.0/src/git_changelog/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/src/git_changelog/templates/angular.md.jinja` & `git_changelog-2.1.0/src/git_changelog/templates/angular.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/src/git_changelog/templates/keepachangelog.md.jinja` & `git_changelog-2.1.0/src/git_changelog/templates/keepachangelog.md.jinja`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_angular_style.py` & `git_changelog-2.1.0/tests/test_angular_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_basic_style.py` & `git_changelog-2.1.0/tests/test_basic_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_cli.py` & `git_changelog-2.1.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_commit.py` & `git_changelog-2.1.0/tests/test_commit.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_conventional_commit_style.py` & `git_changelog-2.1.0/tests/test_conventional_commit_style.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_end_to_end.py` & `git_changelog-2.1.0/tests/test_end_to_end.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_providers.py` & `git_changelog-2.1.0/tests/test_providers.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 A mention: @hello
 A commit git-changelog@06abf793
 A longer commit 3879fabda896da89954adec8
 A commit range: 00000000...11111111
 A snippet: $45
 Some labels: ~18, ~bug, ~"multi word label"
 Some milestones: %2, %version1, %"awesome version"
+A Bitbucket PR: Pull request #1
+A Bitbucket issue: Issue #1
 """
 
 
 def test_github_issue_parsing() -> None:
     """GitHub issues are correctly parsed."""  # (first word *is* correctly capitalized)
     github = git_changelog.GitHub("pawamoy", "git-changelog")
     for ref in github.REF:
@@ -35,7 +37,14 @@
 
 
 def test_gitlab_issue_parsing() -> None:
     """GitLab issues are correctly parsed."""  # (first word *is* correctly capitalized)
     gitlab = git_changelog.GitLab("pawamoy", "git-changelog")
     for ref in gitlab.REF:
         assert gitlab.get_refs(ref, text)
+
+
+def test_bitbucket_issue_parsing() -> None:
+    """Bitbucket issues are correctly parsed."""
+    bitbucket = git_changelog.Bitbucket("pawamoy", "git-changelog")
+    for ref in bitbucket.REF:
+        assert bitbucket.get_refs(ref, text)
```

### Comparing `git_changelog-2.0.0/tests/test_release_notes.py` & `git_changelog-2.1.0/tests/test_release_notes.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/tests/test_version.py` & `git_changelog-2.1.0/tests/test_version.py`

 * *Files identical despite different names*

### Comparing `git_changelog-2.0.0/PKG-INFO` & `git_changelog-2.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: git-changelog
-Version: 2.0.0
+Version: 2.1.0
 Summary: Automatic Changelog generator using Jinja2 templates.
 Keywords: git changelog changelog-generator commit-style commit-convention
 Author-Email: Timothée Mazzucotelli <pawamoy@pm.me>
 License: ISC
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
@@ -48,15 +48,15 @@
   You get full control over the rendering.
   Built-in [Keep a Changelog][keep-a-changelog] and [Angular][angular] templates
   (also see [Conventional Changelog][conventional-changelog]).
 - Commit styles/conventions parsing.
   Built-in [Angular][angular-convention], [Conventional Commit][conventional-commit], [Atom][atom-convention] and basic conventions.
 - Git service/provider agnostic,
   plus references parsing (issues, commits, etc.).
-  Built-in [GitHub][github-refs] and [Gitlab][gitlab-refs] support.
+  Built-in [GitHub][github-refs], [Gitlab][gitlab-refs] and [Bitbucket][bitbucket-refs] support.
 - Understands [Semantic Versioning][semantic-versioning]:
   major/minor/patch for versions and commits.
   Guesses next version based on last commits.
 - Parses [Git trailers][git-trailers], allowing to reference
   issues, PRs, etc., in your commit messages
   in a clean, provider-agnostic way.
 
@@ -74,14 +74,15 @@
 [conventional-changelog]: https://github.com/conventional-changelog/conventional-changelog
 [semantic-versioning]:    http://semver.org/spec/v2.0.0.html
 [atom-convention]:        https://github.com/atom/atom/blob/master/CONTRIBUTING.md#git-commit-messages
 [angular-convention]:     https://github.com/angular/angular/blob/master/CONTRIBUTING.md#commit
 [conventional-commit]:    https://www.conventionalcommits.org/en/v1.0.0/
 [github-refs]:            https://help.github.com/articles/autolinked-references-and-urls/
 [gitlab-refs]:            https://docs.gitlab.com/ce/user/markdown.html#special-gitlab-references
+[bitbucket-refs]:         https://support.atlassian.com/bitbucket-cloud/docs/markup-comments
 [git-trailers]:           https://git-scm.com/docs/git-interpret-trailers
 
 [issue-14]: https://github.com/pawamoy/git-changelog/issues/14
 [issue-15]: https://github.com/pawamoy/git-changelog/issues/15
 [issue-16]: https://github.com/pawamoy/git-changelog/issues/16
 [issue-17]: https://github.com/pawamoy/git-changelog/issues/17
 [issue-19]: https://github.com/pawamoy/git-changelog/issues/19
@@ -198,15 +199,15 @@
                         missing from changelog). If two marker lines are
                         present in the changelog, the contents between those
                         two lines will be overwritten (useful to update an
                         'Unreleased' entry for example). Default: <!--
                         insertion marker -->.
   -o, --output OUTPUT   Output to given file. Default: stdout.
   -r, --parse-refs      Parse provider-specific references in commit messages
-                        (GitHub/GitLab issues, PRs, etc.). Default: False.
+                        (GitHub/GitLab/Bitbucket issues, PRs, etc.). Default: False.
   -R, --release-notes   Output release notes to stdout based on the last entry
                         in the changelog. Default: False.
   -I, --input INPUT     Read from given file when creating release notes.
                         Default: CHANGELOG.md.
   -c, --style, --commit-style, --convention {angular,atom,conventional,basic}
                         The commit convention to match against. Default:
                         basic.
```

