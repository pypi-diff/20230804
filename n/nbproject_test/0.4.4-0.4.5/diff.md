# Comparing `tmp/nbproject_test-0.4.4.tar.gz` & `tmp/nbproject_test-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbproject_test-0.4.4.tar", last modified: Mon Apr  3 17:03:11 2023, max compression
+gzip compressed data, was "nbproject_test-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `nbproject_test-0.4.4.tar` & `nbproject_test-0.4.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1087 2022-11-27 11:40:01.777395 nbproject_test-0.4.4/.github/workflows/build.yml
--rw-r--r--   0        0        0      135 2022-07-11 10:39:45.798535 nbproject_test-0.4.4/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      622 2022-07-11 10:39:45.804151 nbproject_test-0.4.4/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1309 2022-07-11 10:39:45.811484 nbproject_test-0.4.4/.gitignore
--rw-r--r--   0        0        0     1817 2022-07-11 10:39:45.819141 nbproject_test-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11525 2022-07-11 10:39:45.827559 nbproject_test-0.4.4/LICENSE
--rw-r--r--   0        0        0      245 2022-07-11 10:39:45.839917 nbproject_test-0.4.4/README.md
--rw-r--r--   0        0        0     2502 2023-04-03 17:03:02.555631 nbproject_test-0.4.4/docs/changelog.md
--rw-r--r--   0        0        0      159 2022-07-11 10:39:45.856239 nbproject_test-0.4.4/lamin-project.yaml
--rw-r--r--   0        0        0       98 2023-04-03 17:01:57.911497 nbproject_test-0.4.4/nbproject_test/__init__.py
--rw-r--r--   0        0        0     5359 2023-04-03 17:01:32.654974 nbproject_test-0.4.4/nbproject_test/_core.py
--rw-r--r--   0        0        0      374 2022-11-27 12:23:16.593003 nbproject_test-0.4.4/noxfile.py
--rw-r--r--   0        0        0      696 2023-03-21 17:11:15.118863 nbproject_test-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       95 2022-09-06 12:57:04.932563 nbproject_test-0.4.4/tests/notebooks/index.md
--rw-r--r--   0        0        0     1252 2022-09-06 12:57:04.936586 nbproject_test-0.4.4/tests/notebooks/same_test.ipynb
--rw-r--r--   0        0        0     1247 2022-09-06 12:51:59.657778 nbproject_test-0.4.4/tests/notebooks/test.ipynb
--rw-r--r--   0        0        0       30 2022-09-06 12:57:04.940047 nbproject_test-0.4.4/tests/notebooks/text_test.txt
--rw-r--r--   0        0        0      432 2023-04-03 17:01:32.670612 nbproject_test-0.4.4/tests/test_execute_notebooks.py
--rw-r--r--   0        0        0      109 2022-07-11 10:39:45.885614 nbproject_test-0.4.4/tests/test_import.py
--rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 nbproject_test-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0     1043 2022-12-08 20:13:49.196065 nbproject_test-0.4.5/.github/workflows/build.yml
+-rw-r--r--   0        0        0      133 2022-07-11 09:43:26.561330 nbproject_test-0.4.5/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2022-07-11 09:43:26.561889 nbproject_test-0.4.5/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1201 2022-07-11 09:43:26.544052 nbproject_test-0.4.5/.gitignore
+-rw-r--r--   0        0        0     1753 2022-07-11 09:43:26.540901 nbproject_test-0.4.5/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11324 2022-07-11 09:43:26.539980 nbproject_test-0.4.5/LICENSE
+-rw-r--r--   0        0        0      238 2022-07-11 09:43:26.543073 nbproject_test-0.4.5/README.md
+-rw-r--r--   0        0        0     2637 2023-08-04 20:18:39.345687 nbproject_test-0.4.5/docs/changelog.md
+-rw-r--r--   0        0        0      154 2022-07-11 09:43:26.537412 nbproject_test-0.4.5/lamin-project.yaml
+-rw-r--r--   0        0        0       98 2023-08-04 20:18:47.748432 nbproject_test-0.4.5/nbproject_test/__init__.py
+-rw-r--r--   0        0        0     5455 2023-08-04 20:17:39.935954 nbproject_test-0.4.5/nbproject_test/_core.py
+-rw-r--r--   0        0        0      358 2022-12-08 20:13:51.744209 nbproject_test-0.4.5/noxfile.py
+-rw-r--r--   0        0        0      655 2023-08-04 20:04:39.927430 nbproject_test-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       84 2022-09-20 12:22:44.198709 nbproject_test-0.4.5/tests/notebooks/index.md
+-rw-r--r--   0        0        0     1186 2022-09-20 12:22:44.198803 nbproject_test-0.4.5/tests/notebooks/same_test.ipynb
+-rw-r--r--   0        0        0     1181 2022-08-29 08:21:01.794002 nbproject_test-0.4.5/tests/notebooks/test.ipynb
+-rw-r--r--   0        0        0       29 2022-09-20 12:22:44.198886 nbproject_test-0.4.5/tests/notebooks/text_test.txt
+-rw-r--r--   0        0        0      415 2023-08-04 20:04:39.927844 nbproject_test-0.4.5/tests/test_execute_notebooks.py
+-rw-r--r--   0        0        0      104 2022-07-11 10:10:32.717933 nbproject_test-0.4.5/tests/test_import.py
+-rw-r--r--   0        0        0      785 1970-01-01 00:00:00.000000 nbproject_test-0.4.5/PKG-INFO
```

### Comparing `nbproject_test-0.4.4/.github/workflows/build.yml` & `nbproject_test-0.4.5/.github/workflows/build.yml`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,44 @@
-name: build
-
-on:
-  push:
-    branches: [main]
-  pull_request:
-    branches: [main]
-
-jobs:
-  build:
-    runs-on: ubuntu-latest
-    strategy:
-      fail-fast: false
-      matrix:
-        python-version: ["3.9"]
-
-    steps:
-      - name: Checkout main
-        uses: actions/checkout@v3
-        with:
-          fetch-depth: 0
-      - name: Setup Python
-        uses: actions/setup-python@v3
-        with:
-          python-version: ${{ matrix.python-version }}
-      - name: Cache
-        uses: actions/cache@v3
-        env:
-          cache-name: cache-0
-        with:
-          path: |
-            .nox
-            ~/.cache/pre-commit
-          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
-      - name: Install pip and nox
-        run: |
-          python -m pip install --upgrade pip
-          pip install nox
-      - name: Lint
-        run: |
-          nox -s lint
-      - name: Build
-        run: |
-          nox -s build --python ${{ matrix.python-version }}
+name: build
+
+on:
+  push:
+    branches: [main]
+  pull_request:
+    branches: [main]
+
+jobs:
+  build:
+    runs-on: ubuntu-latest
+    strategy:
+      fail-fast: false
+      matrix:
+        python-version: ["3.9"]
+
+    steps:
+      - name: Checkout main
+        uses: actions/checkout@v3
+        with:
+          fetch-depth: 0
+      - name: Setup Python
+        uses: actions/setup-python@v3
+        with:
+          python-version: ${{ matrix.python-version }}
+      - name: Cache
+        uses: actions/cache@v3
+        env:
+          cache-name: cache-0
+        with:
+          path: |
+            .nox
+            ~/.cache/pre-commit
+          key: ${{ runner.os }}-build-${{ env.cache-name }}-${{ hashFiles('.pre-commit-config.yaml') }}-${{ hashFiles('pyproject.yaml') }}
+      - name: Install pip and nox
+        run: |
+          python -m pip install --upgrade pip
+          pip install nox
+      - name: Lint
+        run: |
+          nox -s lint
+      - name: Build
+        run: |
+          nox -s build --python ${{ matrix.python-version }}
```

### Comparing `nbproject_test-0.4.4/LICENSE` & `nbproject_test-0.4.5/LICENSE`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
-Apache License
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
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright [yyyy] [name of copyright owner]
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
+Apache License
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
+   END OF TERMS AND CONDITIONS
+
+   APPENDIX: How to apply the Apache License to your work.
+
+      To apply the Apache License to your work, attach the following
+      boilerplate notice, with the fields enclosed by brackets "[]"
+      replaced with your own identifying information. (Don't include
+      the brackets!)  The text should be enclosed in the appropriate
+      comment syntax for the file format. We also recommend that a
+      file or class name and description of purpose be included on the
+      same "printed page" as the copyright notice for easier
+      identification within third-party archives.
+
+   Copyright [yyyy] [name of copyright owner]
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
```

### Comparing `nbproject_test-0.4.4/docs/changelog.md` & `nbproject_test-0.4.5/docs/changelog.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,20 +1,21 @@
-# Changelog
-
-<!-- prettier-ignore -->
-Name | PR | Developer | Date | Version
---- | --- | --- | --- | ---
-✨ Print outputs for executed cells | [18](https://github.com/laminlabs/nbproject-test/pull/18) | [Koncopd](https://github.com/Koncopd) | 2023-04-03 | 0.4.4
-➕ Move ipykernel to main dependencies | [17](https://github.com/laminlabs/nbproject-test/pull/17) | [Koncopd](https://github.com/Koncopd) | 2023-03-21 | 0.4.3
-💄 Prettify logging | [16](https://github.com/laminlabs/nbproject-test/pull/16) | [falexwolf](https://github.com/falexwolf) | 2022-12-08 |
-🔊 Improve logging | [15](https://github.com/laminlabs/nbproject-test/pull/15) | [Koncopd](https://github.com/Koncopd) | 2022-11-27 | 0.4.1
-🔥 Remove preprocessing | [12](https://github.com/laminlabs/nbproject-test/pull/12) | [falexwolf](https://github.com/falexwolf) | 2022-11-03 | 0.4.0
-✨ Log time to execute notebooks | [11](https://github.com/laminlabs/nbproject-test/pull/11) | [Koncopd](https://github.com/Koncopd) | 2022-10-22 | 0.3.2
-🐛 Ignore dates | [10](https://github.com/laminlabs/nbproject-test/pull/10) | [falexwolf](https://github.com/falexwolf) | 2022-10-18 |
-🚸 Add a preprocessing function that strips prefixes | [commit](https://github.com/laminlabs/nbproject-test/commit/d17e47088aec72acffcf29786369c9f2d041e9b6) | [falexwolf](https://github.com/falexwolf) | 2022-10-08 | 0.3.1
-🚸 Add a preprocessing function that strips prefixes | [8](https://github.com/laminlabs/nbproject-test/pull/8) | [falexwolf](https://github.com/falexwolf) | 2022-10-05 | 0.3.0
-🐛 Fix the error in the last PR | [7](https://github.com/laminlabs/nbproject-test/pull/7) | [Koncopd](https://github.com/Koncopd) | 2022-09-06 | 0.2.2
-🎨 Allow two level markdown files | [6](https://github.com/laminlabs/nbproject-test/pull/6) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-06 | 0.2.1
-✨ Write consecutive cell numbers | [5](https://github.com/laminlabs/nbproject-test/pull/5) | [falexwolf](https://github.com/falexwolf) | 2022-08-29 | 0.2.0
-✨ Allows to execute a single notebook, adds tests | [3](https://github.com/laminlabs/nbproject-test/pull/3) | [Koncopd](https://github.com/Koncopd) | 2022-07-23 |
-♻️ Small refactoring | [2](https://github.com/laminlabs/nbproject-test/pull/2) | [Koncopd](https://github.com/Koncopd) | 2022-07-11 |
-🚚 Add code from nbproject repo | [1](https://github.com/laminlabs/nbproject-test/pull/1) | [falexwolf](https://github.com/falexwolf) | 2022-07-11 | 0.1.0
+# Changelog
+
+<!-- prettier-ignore -->
+Name | PR | Developer | Date | Version
+--- | --- | --- | --- | ---
+♻️ Do not use nested tocs | [19](https://github.com/laminlabs/nbproject-test/pull/19) | [falexwolf](https://github.com/falexwolf) | 2023-08-04 | 0.4.5
+✨ Print outputs for executed cells | [18](https://github.com/laminlabs/nbproject-test/pull/18) | [Koncopd](https://github.com/Koncopd) | 2023-04-03 | 0.4.4
+➕ Move ipykernel to main dependencies | [17](https://github.com/laminlabs/nbproject-test/pull/17) | [Koncopd](https://github.com/Koncopd) | 2023-03-21 | 0.4.3
+💄 Prettify logging | [16](https://github.com/laminlabs/nbproject-test/pull/16) | [falexwolf](https://github.com/falexwolf) | 2022-12-08 |
+🔊 Improve logging | [15](https://github.com/laminlabs/nbproject-test/pull/15) | [Koncopd](https://github.com/Koncopd) | 2022-11-27 | 0.4.1
+🔥 Remove preprocessing | [12](https://github.com/laminlabs/nbproject-test/pull/12) | [falexwolf](https://github.com/falexwolf) | 2022-11-03 | 0.4.0
+✨ Log time to execute notebooks | [11](https://github.com/laminlabs/nbproject-test/pull/11) | [Koncopd](https://github.com/Koncopd) | 2022-10-22 | 0.3.2
+🐛 Ignore dates | [10](https://github.com/laminlabs/nbproject-test/pull/10) | [falexwolf](https://github.com/falexwolf) | 2022-10-18 |
+🚸 Add a preprocessing function that strips prefixes | [commit](https://github.com/laminlabs/nbproject-test/commit/d17e47088aec72acffcf29786369c9f2d041e9b6) | [falexwolf](https://github.com/falexwolf) | 2022-10-08 | 0.3.1
+🚸 Add a preprocessing function that strips prefixes | [8](https://github.com/laminlabs/nbproject-test/pull/8) | [falexwolf](https://github.com/falexwolf) | 2022-10-05 | 0.3.0
+🐛 Fix the error in the last PR | [7](https://github.com/laminlabs/nbproject-test/pull/7) | [Koncopd](https://github.com/Koncopd) | 2022-09-06 | 0.2.2
+🎨 Allow two level markdown files | [6](https://github.com/laminlabs/nbproject-test/pull/6) | [sunnyosun](https://github.com/sunnyosun) | 2022-09-06 | 0.2.1
+✨ Write consecutive cell numbers | [5](https://github.com/laminlabs/nbproject-test/pull/5) | [falexwolf](https://github.com/falexwolf) | 2022-08-29 | 0.2.0
+✨ Allows to execute a single notebook, adds tests | [3](https://github.com/laminlabs/nbproject-test/pull/3) | [Koncopd](https://github.com/Koncopd) | 2022-07-23 |
+♻️ Small refactoring | [2](https://github.com/laminlabs/nbproject-test/pull/2) | [Koncopd](https://github.com/Koncopd) | 2022-07-11 |
+🚚 Add code from nbproject repo | [1](https://github.com/laminlabs/nbproject-test/pull/1) | [falexwolf](https://github.com/falexwolf) | 2022-07-11 | 0.1.0
```

### Comparing `nbproject_test-0.4.4/nbproject_test/_core.py` & `nbproject_test-0.4.5/nbproject_test/_core.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,180 +1,186 @@
-import os
-from pathlib import Path
-from time import perf_counter
-
-from natsort import natsorted
-from nbclient import NotebookClient
-from nbformat import NO_CONVERT
-from nbformat import read as read_nb
-from nbformat import write as write_nb
-
-
-def _list_nbs_in_md(nb_folder, md_filename="index.md"):
-    notebooks = []
-    names = []
-
-    index_path = nb_folder / md_filename
-    if index_path.exists():
-        print(f"Reading {index_path}", flush=True)
-        with open(index_path) as f:
-            index = f.read()
-
-        # parse out indexed file list
-        if "```{toctree}" in index:
-            content = index.split("```{toctree}")[1]
-            content = content.split("\n\n")[1]
-            content = content.split("```")[0]
-
-            # if a file is a notebook, add it
-            # return non-notebook names
-            for name in content.split():
-                nb = nb_folder / f"{name}.ipynb"
-                if nb.exists():
-                    notebooks.append(nb)
-                else:
-                    names.append(name)
-
-    return notebooks, names
-
-
-def add_execution_count(nb):
-    """Add consecutive execution count.
-
-    Notebooks that are executed during CI automatically have consecutive count.
-
-    However, there is no interactive saving. Hence, add this count to the
-    notebook files before executing them.
-
-    Args:
-        nb: Notebook content (`nbproject.dev._notebook.Notebook`).
-    """
-    count = 1
-
-    for icell, cell in enumerate(nb.cells):
-        if cell["cell_type"] != "code" or cell["source"] == []:
-            continue
-
-        nb.cells[icell]["execution_count"] = count
-        count += 1
-
-
-def _print_starting_cell(cell, cell_index):
-    print(f"Starting cell {cell_index}, {cell}.", flush=True)
-
-
-def _print_cell_output(cell, cell_index, execute_reply):
-    txt = f"Executed cell {cell_index}"
-
-    if "source" in cell:
-        txt += f", source: {cell['source']}."
-    else:
-        txt += "."
-
-    if "outputs" in cell:
-        txt += f" Outputs: {cell['outputs']}."
-
-    print(txt, flush=True)
-
-
-def execute_notebooks(
-    nb_file_folder: Path,
-    write: bool = True,
-    print_cells: bool = False,
-    print_outputs: bool = False,
-):
-    """Execute all notebooks in the folder.
-
-    If `write` is `True`, will also add consecutive execution count numbers to
-    make integrity check pass.
-
-    Ignores .ipynb_checkpoints.
-
-    Args:
-        nb_file_folder: Path to folder with notebooks or a notebook to execute.
-        write: If `True`, writes the execution results to the notebooks.
-        print_cells: If `True`, prints cell indices and content
-        on the start of the execution.
-        print_outputs: If `True`, prints cell output for executed cells.
-    """
-    print(f"Executing notebooks in {nb_file_folder}", flush=True)
-
-    t_execute_start = perf_counter()
-
-    env = dict(os.environ)
-
-    if nb_file_folder.is_file():
-        if nb_file_folder.suffix != ".ipynb":
-            print(f"{nb_file_folder} is not a notebook, ignoring", flush=True)
-            return
-
-        nb_folder = nb_file_folder.parent
-
-        notebooks = [nb_file_folder]
-
-    else:
-        nb_folder = nb_file_folder
-
-        # notebooks are part of documentation and indexed
-        # by a sphinx myst index.md file
-        # the order of execution matters!
-        notebooks, names = _list_nbs_in_md(nb_folder, md_filename="index.md")
-        for name in names:
-            md_filename = nb_folder / f"{name}.md"
-            if md_filename.exists():
-                try:
-                    notebooks_, _ = _list_nbs_in_md(nb_folder, md_filename=f"{name}.md")
-                    notebooks += notebooks_
-                except UnicodeDecodeError:
-                    print(f"Ignoring {name}.md due to special characters", flush=True)
-                    continue
-
-        notebooks_unindexed = []
-        for nb in nb_folder.glob("./*.ipynb"):
-            if nb not in notebooks:
-                notebooks_unindexed.append(nb)
-
-        # also for unindexed notebooks the order matters!!!
-        # we'll sort them with natsort so that they can be prefixed
-        notebooks += natsorted(notebooks_unindexed)
-
-    print(f"Scheduled: {[nb.stem for nb in notebooks]}", flush=True)
-
-    os.chdir(nb_folder)
-
-    for nb in notebooks:
-        if ".ipynb_checkpoints/" in str(nb):
-            continue
-
-        t_start = perf_counter()
-
-        nb_content = read_nb(nb, as_version=NO_CONVERT)
-
-        if write:
-            add_execution_count(nb_content)
-            write_nb(nb_content, nb)
-
-        client = NotebookClient(nb_content)
-
-        if print_cells:
-            client.on_cell_start = _print_starting_cell
-        if print_outputs:
-            client.on_cell_executed = _print_cell_output
-
-        print(f"{nb.stem}", end=" ", flush=True)
-
-        env["NBPRJ_TEST_NBPATH"] = str(nb)
-
-        client.execute(env=env)
-
-        if write:
-            write_nb(nb_content, nb)
-
-        t_stop = perf_counter()
-
-        print(f"✓ ({(t_stop - t_start):.3f}s)", flush=True)
-
-    total_time_elapsed = perf_counter() - t_execute_start
-    print(
-        f"Total time: {total_time_elapsed:.3f}s",
-        flush=True,
-    )
+import os
+from pathlib import Path
+from time import perf_counter
+
+from natsort import natsorted
+from nbclient import NotebookClient
+from nbformat import NO_CONVERT
+from nbformat import read as read_nb
+from nbformat import write as write_nb
+
+
+def _list_nbs_in_md(nb_folder, md_filename="index.md"):
+    notebooks = []
+    names = []
+
+    index_path = nb_folder / md_filename
+    if not index_path.exists():
+        # see whether there is a file one level down
+        index_path = Path(nb_folder.as_posix() + ".md")
+    if index_path.exists():
+        print(f"Reading {index_path}", flush=True)
+        with open(index_path) as f:
+            index = f.read()
+
+        # parse out indexed file list
+        if "```{toctree}" in index:
+            content = index.split("```{toctree}")[1]
+            content = content.split("\n\n")[1]
+            content = content.split("```")[0]
+
+            # if a file is a notebook, add it
+            # return non-notebook names
+            for name in content.split():
+                nb = nb_folder / f"{name}.ipynb"
+                if nb.exists():
+                    notebooks.append(nb)
+                else:
+                    names.append(name)
+
+    return notebooks, names
+
+
+def add_execution_count(nb):
+    """Add consecutive execution count.
+
+    Notebooks that are executed during CI automatically have consecutive count.
+
+    However, there is no interactive saving. Hence, add this count to the
+    notebook files before executing them.
+
+    Args:
+        nb: Notebook content (`nbproject.dev._notebook.Notebook`).
+    """
+    count = 1
+
+    for icell, cell in enumerate(nb.cells):
+        if cell["cell_type"] != "code" or cell["source"] == []:
+            continue
+
+        nb.cells[icell]["execution_count"] = count
+        count += 1
+
+
+def _print_starting_cell(cell, cell_index):
+    print(f"Starting cell {cell_index}, {cell}.", flush=True)
+
+
+def _print_cell_output(cell, cell_index, execute_reply):
+    txt = f"Executed cell {cell_index}"
+
+    if "source" in cell:
+        txt += f", source: {cell['source']}."
+    else:
+        txt += "."
+
+    if "outputs" in cell:
+        txt += f" Outputs: {cell['outputs']}."
+
+    print(txt, flush=True)
+
+
+def execute_notebooks(
+    nb_file_folder: Path,
+    write: bool = True,
+    print_cells: bool = False,
+    print_outputs: bool = False,
+):
+    """Execute all notebooks in the folder.
+
+    If `write` is `True`, will also add consecutive execution count numbers
+    to make integrity check pass.
+
+    Ignores .ipynb_checkpoints.
+
+    Args:
+        nb_file_folder: Path to folder with notebooks or a notebook to execute.
+        write: If `True`, writes the execution results to the notebooks.
+        print_cells: If `True`, prints cell indices and content
+        on the start of the execution.
+        print_outputs: If `True`, prints cell output for executed cells.
+    """
+    print(f"Executing notebooks in {nb_file_folder}", flush=True)
+
+    t_execute_start = perf_counter()
+
+    env = dict(os.environ)
+
+    if nb_file_folder.is_file():
+        if nb_file_folder.suffix != ".ipynb":
+            print(f"{nb_file_folder} is not a notebook, ignoring", flush=True)
+            return
+
+        nb_folder = nb_file_folder.parent
+
+        notebooks = [nb_file_folder]
+
+    else:
+        nb_folder = nb_file_folder
+
+        # notebooks are part of documentation and indexed
+        # by a sphinx myst index.md file
+        # the order of execution matters!
+        notebooks, _ = _list_nbs_in_md(nb_folder, md_filename="index.md")
+
+        # nesting is problematic as notebooks might be in other folders but
+        # linked in these markdowns
+        # for name in names:
+        #     md_filename = nb_folder / f"{name}.md"
+        #     if md_filename.exists():
+        #         try:
+        #             notebooks_, _ = _list_nbs_in_md(nb_folder, md_filename=f"{name}.md")  # noqa
+        #             notebooks += notebooks_
+        #         except UnicodeDecodeError:
+        #             print(f"Ignoring {name}.md due to special characters", flush=True)
+        #             continue
+
+        notebooks_unindexed = []
+        for nb in nb_folder.glob("./*.ipynb"):
+            if nb not in notebooks:
+                notebooks_unindexed.append(nb)
+
+        # also for unindexed notebooks the order matters!!!
+        # we'll sort them with natsort so that they can be prefixed
+        notebooks += natsorted(notebooks_unindexed)
+
+    print(f"Scheduled: {[nb.stem for nb in notebooks]}", flush=True)
+
+    os.chdir(nb_folder)
+
+    for nb in notebooks:
+        if ".ipynb_checkpoints/" in str(nb):
+            continue
+
+        t_start = perf_counter()
+
+        nb_content = read_nb(nb, as_version=NO_CONVERT)
+
+        if write:
+            add_execution_count(nb_content)
+            write_nb(nb_content, nb)
+
+        client = NotebookClient(nb_content)
+
+        if print_cells:
+            client.on_cell_start = _print_starting_cell
+        if print_outputs:
+            client.on_cell_executed = _print_cell_output
+
+        print(f"{nb.stem}", end=" ", flush=True)
+
+        env["NBPRJ_TEST_NBPATH"] = str(nb)
+
+        client.execute(env=env)
+
+        if write:
+            write_nb(nb_content, nb)
+
+        t_stop = perf_counter()
+
+        print(f"✓ ({(t_stop - t_start):.3f}s)", flush=True)
+
+    total_time_elapsed = perf_counter() - t_execute_start
+    print(
+        f"Total time: {total_time_elapsed:.3f}s",
+        flush=True,
+    )
```

### Comparing `nbproject_test-0.4.4/pyproject.toml` & `nbproject_test-0.4.5/pyproject.toml`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-[build-system]
-requires = ["flit_core >=3.2,<4"]
-build-backend = "flit_core.buildapi"
-
-[project]
-name = "nbproject_test"
-authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
-readme = "README.md"
-dynamic = ["version", "description"]
-dependencies = [
-    "nbclient",
-    "nbformat",
-    "ipykernel",
-    "natsort"
-]
-
-[project.urls]
-Home = "https://github.com/laminlabs/nbproject-test"
-
-[project.optional-dependencies]
-dev = [
-    "pre-commit",
-    "nox",
-]
-test = [
-    "pytest>=6.0",
-    "pytest-cov"
-]
-
-[tool.black]
-preview = true
-
-[tool.pytest.ini_options]
-testpaths = [
-    "tests",
-]
-
-[tool.coverage.run]
-omit = [
-    "nbproject_test/*",
-]
+[build-system]
+requires = ["flit_core >=3.2,<4"]
+build-backend = "flit_core.buildapi"
+
+[project]
+name = "nbproject_test"
+authors = [{name = "Lamin Labs", email = "laminlabs@gmail.com"}]
+readme = "README.md"
+dynamic = ["version", "description"]
+dependencies = [
+    "nbclient",
+    "nbformat",
+    "ipykernel",
+    "natsort"
+]
+
+[project.urls]
+Home = "https://github.com/laminlabs/nbproject-test"
+
+[project.optional-dependencies]
+dev = [
+    "pre-commit",
+    "nox",
+]
+test = [
+    "pytest>=6.0",
+    "pytest-cov"
+]
+
+[tool.black]
+preview = true
+
+[tool.pytest.ini_options]
+testpaths = [
+    "tests",
+]
+
+[tool.coverage.run]
+omit = [
+    "nbproject_test/*",
+]
```

### Comparing `nbproject_test-0.4.4/PKG-INFO` & `nbproject_test-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbproject_test
-Version: 0.4.4
+Version: 0.4.5
 Summary: Testing for nbproject.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: nbclient
 Requires-Dist: nbformat
 Requires-Dist: ipykernel
 Requires-Dist: natsort
```

