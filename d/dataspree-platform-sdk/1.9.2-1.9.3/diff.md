# Comparing `tmp/dataspree-platform-sdk-1.9.2.tar.gz` & `tmp/dataspree-platform-sdk-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspree-platform-sdk-1.9.2.tar", last modified: Tue Jul 18 17:47:56 2023, max compression
+gzip compressed data, was "dataspree-platform-sdk-1.9.3.tar", last modified: Fri Aug  4 05:35:35 2023, max compression
```

## Comparing `dataspree-platform-sdk-1.9.2.tar` & `dataspree-platform-sdk-1.9.3.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/
--rw-rw-r--   0 x         (1000) x         (1000)     9585 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/LICENSE
--rw-rw-r--   0 x         (1000) x         (1000)       25 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/MANIFEST.in
--rw-r--r--   0 x         (1000) x         (1000)     2759 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)     2228 2022-12-01 12:49:03.000000 dataspree-platform-sdk-1.9.2/README.md
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/dataspree/
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/
--rw-r--r--   0 x         (1000) x         (1000)      613 2023-07-18 17:46:26.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/__init__.py
--rw-r--r--   0 x         (1000) x         (1000)     9594 2022-12-01 12:49:03.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/base_model.py
--rw-rw-r--   0 x         (1000) x         (1000)    12174 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/cli.py
--rw-r--r--   0 x         (1000) x         (1000)    79238 2023-07-18 13:28:10.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/client.py
--rw-r--r--   0 x         (1000) x         (1000)    20820 2022-12-01 13:45:00.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/data_loader.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/
--rw-rw-r--   0 x         (1000) x         (1000)      628 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/__init__.py
--rw-rw-r--   0 x         (1000) x         (1000)     1354 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/base_decoder.py
--rw-rw-r--   0 x         (1000) x         (1000)     4082 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/opencv_decoder.py
--rw-rw-r--   0 x         (1000) x         (1000)     1949 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/pcd_decoder.py
--rw-rw-r--   0 x         (1000) x         (1000)     6731 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/serializer.py
--rw-rw-r--   0 x         (1000) x         (1000)      946 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/http_token_authentication.py
--rw-rw-r--   0 x         (1000) x         (1000)     4771 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/query.py
--rw-rw-r--   0 x         (1000) x         (1000)    33032 2022-10-12 19:41:15.000000 dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/worker.py
-drwxr-xr-x   0 x         (1000) x         (1000)        0 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/
--rw-r--r--   0 x         (1000) x         (1000)     2759 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/PKG-INFO
--rw-r--r--   0 x         (1000) x         (1000)      853 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 x         (1000) x         (1000)        1 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 x         (1000) x         (1000)       54 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/entry_points.txt
--rw-r--r--   0 x         (1000) x         (1000)      161 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/requires.txt
--rw-r--r--   0 x         (1000) x         (1000)       10 2023-07-18 17:47:56.000000 dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/top_level.txt
--rw-rw-r--   0 x         (1000) x         (1000)      121 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/requirements.txt
--rw-r--r--   0 x         (1000) x         (1000)       38 2023-07-18 17:47:56.539783 dataspree-platform-sdk-1.9.2/setup.cfg
--rw-rw-r--   0 x         (1000) x         (1000)     2334 2022-08-26 10:56:53.000000 dataspree-platform-sdk-1.9.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.649604 dataspree-platform-sdk-1.9.3/
+-rw-rw-rw-   0        0        0     9760 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/LICENSE
+-rw-rw-rw-   0        0        0       26 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     2840 2023-08-04 05:35:35.648674 dataspree-platform-sdk-1.9.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2291 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.603570 dataspree-platform-sdk-1.9.3/dataspree/
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.611566 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/
+-rw-rw-rw-   0        0        0      628 2023-08-04 05:28:31.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/__init__.py
+-rw-rw-rw-   0        0        0     9837 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/base_model.py
+-rw-rw-rw-   0        0        0    12429 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/cli.py
+-rw-rw-rw-   0        0        0    81158 2023-08-04 05:28:17.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/client.py
+-rw-rw-rw-   0        0        0    21274 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/data_loader.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.618621 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/
+-rw-rw-rw-   0        0        0      642 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/__init__.py
+-rw-rw-rw-   0        0        0     1401 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/base_decoder.py
+-rw-rw-rw-   0        0        0     4181 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/opencv_decoder.py
+-rw-rw-rw-   0        0        0     2019 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/pcd_decoder.py
+-rw-rw-rw-   0        0        0     6892 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/serializer.py
+-rw-rw-rw-   0        0        0      973 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/http_token_authentication.py
+-rw-rw-rw-   0        0        0     4888 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/query.py
+-rw-rw-rw-   0        0        0    33806 2023-04-03 12:52:11.000000 dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/worker.py
+drwxrwxrwx   0        0        0        0 2023-08-04 05:35:35.645613 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/
+-rw-rw-rw-   0        0        0     2840 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      853 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       54 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      185 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-08-04 05:35:35.000000 dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       69 2023-08-04 05:25:01.000000 dataspree-platform-sdk-1.9.3/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 05:35:35.649604 dataspree-platform-sdk-1.9.3/setup.cfg
+-rw-rw-rw-   0        0        0     2591 2023-08-04 05:25:01.000000 dataspree-platform-sdk-1.9.3/setup.py
```

### Comparing `dataspree-platform-sdk-1.9.2/LICENSE` & `dataspree-platform-sdk-1.9.3/LICENSE`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,176 +1,176 @@
-                               Apache License
-                       Version 2.0, January 2004
-                    http://www.apache.org/licenses/
-
-TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-1. Definitions.
-
-  "License" shall mean the terms and conditions for use, reproduction,
-  and distribution as defined by Sections 1 through 9 of this document.
-
-  "Licensor" shall mean the copyright owner or entity authorized by
-  the copyright owner that is granting the License.
-
-  "Legal Entity" shall mean the union of the acting entity and all
-  other entities that control, are controlled by, or are under common
-  control with that entity. For the purposes of this definition,
-  "control" means (i) the power, direct or indirect, to cause the
-  direction or management of such entity, whether by contract or
-  otherwise, or (ii) ownership of fifty percent (50%) or more of the
-  outstanding shares, or (iii) beneficial ownership of such entity.
-
-  "You" (or "Your") shall mean an individual or Legal Entity
-  exercising permissions granted by this License.
-
-  "Source" form shall mean the preferred form for making modifications,
-  including but not limited to software source code, documentation
-  source, and configuration files.
-
-  "Object" form shall mean any form resulting from mechanical
-  transformation or translation of a Source form, including but
-  not limited to compiled object code, generated documentation,
-  and conversions to other media types.
-
-  "Work" shall mean the work of authorship, whether in Source or
-  Object form, made available under the License, as indicated by a
-  copyright notice that is included in or attached to the work
-  (an example is provided in the Appendix below).
-
-  "Derivative Works" shall mean any work, whether in Source or Object
-  form, that is based on (or derived from) the Work and for which the
-  editorial revisions, annotations, elaborations, or other modifications
-  represent, as a whole, an original work of authorship. For the purposes
-  of this License, Derivative Works shall not include works that remain
-  separable from, or merely link (or bind by name) to the interfaces of,
-  the Work and Derivative Works thereof.
-
-  "Contribution" shall mean any work of authorship, including
-  the original version of the Work and any modifications or additions
-  to that Work or Derivative Works thereof, that is intentionally
-  submitted to Licensor for inclusion in the Work by the copyright owner
-  or by an individual or Legal Entity authorized to submit on behalf of
-  the copyright owner. For the purposes of this definition, "submitted"
-  means any form of electronic, verbal, or written communication sent
-  to the Licensor or its representatives, including but not limited to
-  communication on electronic mailing lists, source code control systems,
-  and issue tracking systems that are managed by, or on behalf of, the
-  Licensor for the purpose of discussing and improving the Work, but
-  excluding communication that is conspicuously marked or otherwise
-  designated in writing by the copyright owner as "Not a Contribution."
-
-  "Contributor" shall mean Licensor and any individual or Legal Entity
-  on behalf of whom a Contribution has been received by Licensor and
-  subsequently incorporated within the Work.
-
-2. Grant of Copyright License. Subject to the terms and conditions of
-  this License, each Contributor hereby grants to You a perpetual,
-  worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-  copyright license to reproduce, prepare Derivative Works of,
-  publicly display, publicly perform, sublicense, and distribute the
-  Work and such Derivative Works in Source or Object form.
-
-3. Grant of Patent License. Subject to the terms and conditions of
-  this License, each Contributor hereby grants to You a perpetual,
-  worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-  (except as stated in this section) patent license to make, have made,
-  use, offer to sell, sell, import, and otherwise transfer the Work,
-  where such license applies only to those patent claims licensable
-  by such Contributor that are necessarily infringed by their
-  Contribution(s) alone or by combination of their Contribution(s)
-  with the Work to which such Contribution(s) was submitted. If You
-  institute patent litigation against any entity (including a
-  cross-claim or counterclaim in a lawsuit) alleging that the Work
-  or a Contribution incorporated within the Work constitutes direct
-  or contributory patent infringement, then any patent licenses
-  granted to You under this License for that Work shall terminate
-  as of the date such litigation is filed.
-
-4. Redistribution. You may reproduce and distribute copies of the
-  Work or Derivative Works thereof in any medium, with or without
-  modifications, and in Source or Object form, provided that You
-  meet the following conditions:
-
-  (a) You must give any other recipients of the Work or
-      Derivative Works a copy of this License; and
-
-  (b) You must cause any modified files to carry prominent notices
-      stating that You changed the files; and
-
-  (c) You must retain, in the Source form of any Derivative Works
-      that You distribute, all copyright, patent, trademark, and
-      attribution notices from the Source form of the Work,
-      excluding those notices that do not pertain to any part of
-      the Derivative Works; and
-
-  (d) If the Work includes a "NOTICE" text file as part of its
-      distribution, then any Derivative Works that You distribute must
-      include a readable copy of the attribution notices contained
-      within such NOTICE file, excluding those notices that do not
-      pertain to any part of the Derivative Works, in at least one
-      of the following places: within a NOTICE text file distributed
-      as part of the Derivative Works; within the Source form or
-      documentation, if provided along with the Derivative Works; or,
-      within a display generated by the Derivative Works, if and
-      wherever such third-party notices normally appear. The contents
-      of the NOTICE file are for informational purposes only and
-      do not modify the License. You may add Your own attribution
-      notices within Derivative Works that You distribute, alongside
-      or as an addendum to the NOTICE text from the Work, provided
-      that such additional attribution notices cannot be construed
-      as modifying the License.
-
-  You may add Your own copyright statement to Your modifications and
-  may provide additional or different license terms and conditions
-  for use, reproduction, or distribution of Your modifications, or
-  for any such Derivative Works as a whole, provided Your use,
-  reproduction, and distribution of the Work otherwise complies with
-  the conditions stated in this License.
-
-5. Submission of Contributions. Unless You explicitly state otherwise,
-  any Contribution intentionally submitted for inclusion in the Work
-  by You to the Licensor shall be under the terms and conditions of
-  this License, without any additional terms or conditions.
-  Notwithstanding the above, nothing herein shall supersede or modify
-  the terms of any separate license agreement you may have executed
-  with Licensor regarding such Contributions.
-
-6. Trademarks. This License does not grant permission to use the trade
-  names, trademarks, service marks, or product names of the Licensor,
-  except as required for reasonable and customary use in describing the
-  origin of the Work and reproducing the content of the NOTICE file.
-
-7. Disclaimer of Warranty. Unless required by applicable law or
-  agreed to in writing, Licensor provides the Work (and each
-  Contributor provides its Contributions) on an "AS IS" BASIS,
-  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-  implied, including, without limitation, any warranties or conditions
-  of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-  PARTICULAR PURPOSE. You are solely responsible for determining the
-  appropriateness of using or redistributing the Work and assume any
-  risks associated with Your exercise of permissions under this License.
-
-8. Limitation of Liability. In no event and under no legal theory,
-  whether in tort (including negligence), contract, or otherwise,
-  unless required by applicable law (such as deliberate and grossly
-  negligent acts) or agreed to in writing, shall any Contributor be
-  liable to You for damages, including any direct, indirect, special,
-  incidental, or consequential damages of any character arising as a
-  result of this License or out of the use or inability to use the
-  Work (including but not limited to damages for loss of goodwill,
-  work stoppage, computer failure or malfunction, or any and all
-  other commercial damages or losses), even if such Contributor
-  has been advised of the possibility of such damages.
-
-9. Accepting Warranty or Additional Liability. While redistributing
-  the Work or Derivative Works thereof, You may choose to offer,
-  and charge a fee for, acceptance of support, warranty, indemnity,
-  or other liability obligations and/or rights consistent with this
-  License. However, in accepting such obligations, You may act only
-  on Your own behalf and on Your sole responsibility, not on behalf
-  of any other Contributor, and only if You agree to indemnify,
-  defend, and hold each Contributor harmless for any liability
-  incurred by, or claims asserted against, such Contributor by reason
-  of your accepting any such warranty or additional liability.
-
+                               Apache License
+                       Version 2.0, January 2004
+                    http://www.apache.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
+
+1. Definitions.
+
+  "License" shall mean the terms and conditions for use, reproduction,
+  and distribution as defined by Sections 1 through 9 of this document.
+
+  "Licensor" shall mean the copyright owner or entity authorized by
+  the copyright owner that is granting the License.
+
+  "Legal Entity" shall mean the union of the acting entity and all
+  other entities that control, are controlled by, or are under common
+  control with that entity. For the purposes of this definition,
+  "control" means (i) the power, direct or indirect, to cause the
+  direction or management of such entity, whether by contract or
+  otherwise, or (ii) ownership of fifty percent (50%) or more of the
+  outstanding shares, or (iii) beneficial ownership of such entity.
+
+  "You" (or "Your") shall mean an individual or Legal Entity
+  exercising permissions granted by this License.
+
+  "Source" form shall mean the preferred form for making modifications,
+  including but not limited to software source code, documentation
+  source, and configuration files.
+
+  "Object" form shall mean any form resulting from mechanical
+  transformation or translation of a Source form, including but
+  not limited to compiled object code, generated documentation,
+  and conversions to other media types.
+
+  "Work" shall mean the work of authorship, whether in Source or
+  Object form, made available under the License, as indicated by a
+  copyright notice that is included in or attached to the work
+  (an example is provided in the Appendix below).
+
+  "Derivative Works" shall mean any work, whether in Source or Object
+  form, that is based on (or derived from) the Work and for which the
+  editorial revisions, annotations, elaborations, or other modifications
+  represent, as a whole, an original work of authorship. For the purposes
+  of this License, Derivative Works shall not include works that remain
+  separable from, or merely link (or bind by name) to the interfaces of,
+  the Work and Derivative Works thereof.
+
+  "Contribution" shall mean any work of authorship, including
+  the original version of the Work and any modifications or additions
+  to that Work or Derivative Works thereof, that is intentionally
+  submitted to Licensor for inclusion in the Work by the copyright owner
+  or by an individual or Legal Entity authorized to submit on behalf of
+  the copyright owner. For the purposes of this definition, "submitted"
+  means any form of electronic, verbal, or written communication sent
+  to the Licensor or its representatives, including but not limited to
+  communication on electronic mailing lists, source code control systems,
+  and issue tracking systems that are managed by, or on behalf of, the
+  Licensor for the purpose of discussing and improving the Work, but
+  excluding communication that is conspicuously marked or otherwise
+  designated in writing by the copyright owner as "Not a Contribution."
+
+  "Contributor" shall mean Licensor and any individual or Legal Entity
+  on behalf of whom a Contribution has been received by Licensor and
+  subsequently incorporated within the Work.
+
+2. Grant of Copyright License. Subject to the terms and conditions of
+  this License, each Contributor hereby grants to You a perpetual,
+  worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+  copyright license to reproduce, prepare Derivative Works of,
+  publicly display, publicly perform, sublicense, and distribute the
+  Work and such Derivative Works in Source or Object form.
+
+3. Grant of Patent License. Subject to the terms and conditions of
+  this License, each Contributor hereby grants to You a perpetual,
+  worldwide, non-exclusive, no-charge, royalty-free, irrevocable
+  (except as stated in this section) patent license to make, have made,
+  use, offer to sell, sell, import, and otherwise transfer the Work,
+  where such license applies only to those patent claims licensable
+  by such Contributor that are necessarily infringed by their
+  Contribution(s) alone or by combination of their Contribution(s)
+  with the Work to which such Contribution(s) was submitted. If You
+  institute patent litigation against any entity (including a
+  cross-claim or counterclaim in a lawsuit) alleging that the Work
+  or a Contribution incorporated within the Work constitutes direct
+  or contributory patent infringement, then any patent licenses
+  granted to You under this License for that Work shall terminate
+  as of the date such litigation is filed.
+
+4. Redistribution. You may reproduce and distribute copies of the
+  Work or Derivative Works thereof in any medium, with or without
+  modifications, and in Source or Object form, provided that You
+  meet the following conditions:
+
+  (a) You must give any other recipients of the Work or
+      Derivative Works a copy of this License; and
+
+  (b) You must cause any modified files to carry prominent notices
+      stating that You changed the files; and
+
+  (c) You must retain, in the Source form of any Derivative Works
+      that You distribute, all copyright, patent, trademark, and
+      attribution notices from the Source form of the Work,
+      excluding those notices that do not pertain to any part of
+      the Derivative Works; and
+
+  (d) If the Work includes a "NOTICE" text file as part of its
+      distribution, then any Derivative Works that You distribute must
+      include a readable copy of the attribution notices contained
+      within such NOTICE file, excluding those notices that do not
+      pertain to any part of the Derivative Works, in at least one
+      of the following places: within a NOTICE text file distributed
+      as part of the Derivative Works; within the Source form or
+      documentation, if provided along with the Derivative Works; or,
+      within a display generated by the Derivative Works, if and
+      wherever such third-party notices normally appear. The contents
+      of the NOTICE file are for informational purposes only and
+      do not modify the License. You may add Your own attribution
+      notices within Derivative Works that You distribute, alongside
+      or as an addendum to the NOTICE text from the Work, provided
+      that such additional attribution notices cannot be construed
+      as modifying the License.
+
+  You may add Your own copyright statement to Your modifications and
+  may provide additional or different license terms and conditions
+  for use, reproduction, or distribution of Your modifications, or
+  for any such Derivative Works as a whole, provided Your use,
+  reproduction, and distribution of the Work otherwise complies with
+  the conditions stated in this License.
+
+5. Submission of Contributions. Unless You explicitly state otherwise,
+  any Contribution intentionally submitted for inclusion in the Work
+  by You to the Licensor shall be under the terms and conditions of
+  this License, without any additional terms or conditions.
+  Notwithstanding the above, nothing herein shall supersede or modify
+  the terms of any separate license agreement you may have executed
+  with Licensor regarding such Contributions.
+
+6. Trademarks. This License does not grant permission to use the trade
+  names, trademarks, service marks, or product names of the Licensor,
+  except as required for reasonable and customary use in describing the
+  origin of the Work and reproducing the content of the NOTICE file.
+
+7. Disclaimer of Warranty. Unless required by applicable law or
+  agreed to in writing, Licensor provides the Work (and each
+  Contributor provides its Contributions) on an "AS IS" BASIS,
+  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
+  implied, including, without limitation, any warranties or conditions
+  of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
+  PARTICULAR PURPOSE. You are solely responsible for determining the
+  appropriateness of using or redistributing the Work and assume any
+  risks associated with Your exercise of permissions under this License.
+
+8. Limitation of Liability. In no event and under no legal theory,
+  whether in tort (including negligence), contract, or otherwise,
+  unless required by applicable law (such as deliberate and grossly
+  negligent acts) or agreed to in writing, shall any Contributor be
+  liable to You for damages, including any direct, indirect, special,
+  incidental, or consequential damages of any character arising as a
+  result of this License or out of the use or inability to use the
+  Work (including but not limited to damages for loss of goodwill,
+  work stoppage, computer failure or malfunction, or any and all
+  other commercial damages or losses), even if such Contributor
+  has been advised of the possibility of such damages.
+
+9. Accepting Warranty or Additional Liability. While redistributing
+  the Work or Derivative Works thereof, You may choose to offer,
+  and charge a fee for, acceptance of support, warranty, indemnity,
+  or other liability obligations and/or rights consistent with this
+  License. However, in accepting such obligations, You may act only
+  on Your own behalf and on Your sole responsibility, not on behalf
+  of any other Contributor, and only if You agree to indemnify,
+  defend, and hold each Contributor harmless for any liability
+  incurred by, or claims asserted against, such Contributor by reason
+  of your accepting any such warranty or additional liability.
+
 END OF TERMS AND CONDITIONS
```

### Comparing `dataspree-platform-sdk-1.9.2/PKG-INFO` & `dataspree-platform-sdk-1.9.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,81 +1,81 @@
-Metadata-Version: 2.1
-Name: dataspree-platform-sdk
-Version: 1.9.2
-Summary: Python SDK Data Spree AI Platform
-Home-page: https://data-spree.com/ai
-Author: Data Spree GmbH
-Author-email: info@data-spree.com
-License: Apache-2.0
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: kitti
-Provides-Extra: worker
-Provides-Extra: build
-License-File: LICENSE
-
-# Data Spree AI Platform SDK
-The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
-custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
-* Data Spree
-* KITTI
-* COCO
-
-Furthermore, it is possible to export datasets from the platform.
-
-## Usage
-
-### General Usage
-```
-Usage: ds [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  export
-  import
-```
-
-### Dataset Import
-```
-Usage: ds import [OPTIONS]
-
-Options:
-  --format [dataspree|kitti|coco]  Dataset format to import
-  --dataset_name TEXT         Name of the newly created dataset.
-  --dataset_id INTEGER        ID of the dataset to which new items should be
-                              imported. If set to '-1', a new dataset will be
-                              created
-  --images PATH               Directory containing the images to import.
-                              [required]
-  --annotations PATH          Directory or file containing the annotations to
-                              import.  [required]
-  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
-  --username TEXT             Username for data spree vision platform.
-  --password TEXT             Password for data spree vision platform.
-  --url TEXT                  URL to the API of the platform.
-  --help                      Show this message and exit.
-```
-
-### Dataset Export
-```
-Usage: ds export [OPTIONS]
-
-Options:
-  -o, --output_dir DIRECTORY   Output directory.  [required]
-  -i, --id INTEGER             ID of the dataset to download.
-  -n, --n_items INTEGER        Number of items to download. Download all
-                               items: '-1'  [default: -1]
-  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
-  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
-  --username TEXT              Username for data spree vision platform.
-  --password TEXT              Password for data spree vision platform.
-  --url TEXT                   URL to the API of the platform.
-  --help                       Show this message and exit.
-```
-
-## License
-Apache License 2.0
+Metadata-Version: 2.1
+Name: dataspree-platform-sdk
+Version: 1.9.3
+Summary: Python SDK Data Spree AI Platform
+Home-page: https://data-spree.com/ai
+Author: Data Spree GmbH
+Author-email: info@data-spree.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: kitti
+Provides-Extra: worker
+Provides-Extra: build
+License-File: LICENSE
+
+# Data Spree AI Platform SDK
+The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
+custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
+* Data Spree
+* KITTI
+* COCO
+
+Furthermore, it is possible to export datasets from the platform.
+
+## Usage
+
+### General Usage
+```
+Usage: ds [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  export
+  import
+```
+
+### Dataset Import
+```
+Usage: ds import [OPTIONS]
+
+Options:
+  --format [dataspree|kitti|coco]  Dataset format to import
+  --dataset_name TEXT         Name of the newly created dataset.
+  --dataset_id INTEGER        ID of the dataset to which new items should be
+                              imported. If set to '-1', a new dataset will be
+                              created
+  --images PATH               Directory containing the images to import.
+                              [required]
+  --annotations PATH          Directory or file containing the annotations to
+                              import.  [required]
+  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
+  --username TEXT             Username for data spree vision platform.
+  --password TEXT             Password for data spree vision platform.
+  --url TEXT                  URL to the API of the platform.
+  --help                      Show this message and exit.
+```
+
+### Dataset Export
+```
+Usage: ds export [OPTIONS]
+
+Options:
+  -o, --output_dir DIRECTORY   Output directory.  [required]
+  -i, --id INTEGER             ID of the dataset to download.
+  -n, --n_items INTEGER        Number of items to download. Download all
+                               items: '-1'  [default: -1]
+  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
+  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
+  --username TEXT              Username for data spree vision platform.
+  --password TEXT              Password for data spree vision platform.
+  --url TEXT                   URL to the API of the platform.
+  --help                       Show this message and exit.
+```
+
+## License
+Apache License 2.0
```

### Comparing `dataspree-platform-sdk-1.9.2/README.md` & `dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,63 +1,81 @@
-# Data Spree AI Platform SDK
-The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
-custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
-* Data Spree
-* KITTI
-* COCO
-
-Furthermore, it is possible to export datasets from the platform.
-
-## Usage
-
-### General Usage
-```
-Usage: ds [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --help  Show this message and exit.
-
-Commands:
-  export
-  import
-```
-
-### Dataset Import
-```
-Usage: ds import [OPTIONS]
-
-Options:
-  --format [dataspree|kitti|coco]  Dataset format to import
-  --dataset_name TEXT         Name of the newly created dataset.
-  --dataset_id INTEGER        ID of the dataset to which new items should be
-                              imported. If set to '-1', a new dataset will be
-                              created
-  --images PATH               Directory containing the images to import.
-                              [required]
-  --annotations PATH          Directory or file containing the annotations to
-                              import.  [required]
-  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
-  --username TEXT             Username for data spree vision platform.
-  --password TEXT             Password for data spree vision platform.
-  --url TEXT                  URL to the API of the platform.
-  --help                      Show this message and exit.
-```
-
-### Dataset Export
-```
-Usage: ds export [OPTIONS]
-
-Options:
-  -o, --output_dir DIRECTORY   Output directory.  [required]
-  -i, --id INTEGER             ID of the dataset to download.
-  -n, --n_items INTEGER        Number of items to download. Download all
-                               items: '-1'  [default: -1]
-  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
-  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
-  --username TEXT              Username for data spree vision platform.
-  --password TEXT              Password for data spree vision platform.
-  --url TEXT                   URL to the API of the platform.
-  --help                       Show this message and exit.
-```
-
-## License
-Apache License 2.0
+Metadata-Version: 2.1
+Name: dataspree-platform-sdk
+Version: 1.9.3
+Summary: Python SDK Data Spree AI Platform
+Home-page: https://data-spree.com/ai
+Author: Data Spree GmbH
+Author-email: info@data-spree.com
+License: Apache-2.0
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: kitti
+Provides-Extra: worker
+Provides-Extra: build
+License-File: LICENSE
+
+# Data Spree AI Platform SDK
+The Platform SDK acts as an interface to the Data Spree AI Platform, contains all classes and functions to integrate
+custom models into the platform, and it provides a command-line tool for importing datasets of the following formats:
+* Data Spree
+* KITTI
+* COCO
+
+Furthermore, it is possible to export datasets from the platform.
+
+## Usage
+
+### General Usage
+```
+Usage: ds [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  export
+  import
+```
+
+### Dataset Import
+```
+Usage: ds import [OPTIONS]
+
+Options:
+  --format [dataspree|kitti|coco]  Dataset format to import
+  --dataset_name TEXT         Name of the newly created dataset.
+  --dataset_id INTEGER        ID of the dataset to which new items should be
+                              imported. If set to '-1', a new dataset will be
+                              created
+  --images PATH               Directory containing the images to import.
+                              [required]
+  --annotations PATH          Directory or file containing the annotations to
+                              import.  [required]
+  --http_retries INTEGER      Number of HTTP retries.  [default: 10]
+  --username TEXT             Username for data spree vision platform.
+  --password TEXT             Password for data spree vision platform.
+  --url TEXT                  URL to the API of the platform.
+  --help                      Show this message and exit.
+```
+
+### Dataset Export
+```
+Usage: ds export [OPTIONS]
+
+Options:
+  -o, --output_dir DIRECTORY   Output directory.  [required]
+  -i, --id INTEGER             ID of the dataset to download.
+  -n, --n_items INTEGER        Number of items to download. Download all
+                               items: '-1'  [default: -1]
+  --http_retries INTEGER       Number of HTTP retries.  [default: 10]
+  --parallel_requests INTEGER  Number of parallel requests.  [default: 16]
+  --username TEXT              Username for data spree vision platform.
+  --password TEXT              Password for data spree vision platform.
+  --url TEXT                   URL to the API of the platform.
+  --help                       Show this message and exit.
+```
+
+## License
+Apache License 2.0
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/__init__.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-__version__ = '1.9.2'
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+from .base_decoder import BaseDecoder
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/base_model.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/base_model.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,243 +1,243 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import importlib
-import logging
-import signal
-import sys
-from abc import ABC, abstractmethod
-from queue import Queue, Full, Empty
-from threading import Thread
-from typing import Dict, Optional
-
-import click
-import requests as rq
-
-from dataspree.platform_sdk.client import Client
-
-logger = logging.getLogger(__name__)
-
-
-class BaseModel(ABC):
-    def __init__(self, client: Client, dataset_dir: str, model: Dict,
-                 iterations: int, worker_url: str) -> None:
-        super().__init__()
-        self.client: Client = client
-        self.dataset_dir: str = dataset_dir
-        self.platform_model: Dict = model
-        self.iterations: int = iterations
-        self.worker_url: str = worker_url
-
-        self.run_heartbeat_send_loop = True
-
-        self.heartbeat_queue: Optional[Queue] = None
-        self.heartbeat_sender: Optional[Thread] = None
-        if self.worker_url != '':
-            self.heartbeat_queue = Queue(maxsize=10)
-            self.heartbeat_sender: Thread = Thread(target=self.heartbeat_send_loop)
-            self.heartbeat_sender.start()
-
-    @abstractmethod
-    def run(self) -> None:
-        """
-        Stub for implementing the training and evaluation loop. Regularly, the send_heartbeat function must be
-        called:
-        >>> self.send_heartbeat(status)
-        """
-        pass
-
-    @abstractmethod
-    def shutdown(self) -> None:
-        """
-        Stub for implementing the shutdown. You can use this function for implementing a graceful shutdown of the
-        training. For instance, create a last checkpoint.
-        """
-        pass
-
-    def heartbeat_send_loop(self):
-        while self.run_heartbeat_send_loop:
-            try:
-                status = self.heartbeat_queue.get(timeout=1.0)
-                self.__post_heartbeat(status)
-            except Empty:
-                pass
-
-    def __post_heartbeat(self, status):
-        rq.post(f'{self.worker_url}/model_status', json=status)
-
-    def send_heartbeat(self, status, send_immediately=False) -> None:
-        """
-        Report the status of the model. This callback must be called regularly. Otherwise, the process will be
-        terminated.
-        :param status: Dictionary containing the current number of iterations, one of the following states:
-                       ['init', 'running', 'finished', 'exception'].
-        Example:
-        >>> { 'state': 'running', 'iteration': 350 }
-        :param send_immediately: Directly send the heartbeat and wait for the result. Otherwise, the heartbeat
-                                 will be enqueued to be sent in another thread.
-        """
-        try:
-
-            assert status.get('status') in ('init', 'running', 'finished', 'exception')
-            status.setdefault('iteration', 0)
-            status.setdefault('epoch', 0)
-            status.setdefault('end_iteration', 0)
-            status.setdefault('start_iteration', 0)
-            status.setdefault('eta', 0)
-
-            self.heartbeat_queue.put_nowait(status)
-            if send_immediately:
-                self.__post_heartbeat(status)
-        except Full:
-            pass
-
-    @classmethod
-    def start(cls, job_id: int, username: Optional[str] = None, password: Optional[str] = None,
-              token: Optional[str] = None, server_url: str = '', dataset_dir: str = '',
-              worker_url: str = 'http://localhost:6714') -> None:
-        """
-        Initialize the model and call the run method.
-        :param job_id: ID of the AI platform training job that will be processed.
-        :param username: Username for AI platform server.
-        :param password: Password for AI platform server.
-        :param token: Authentication token for AI platform server (use either username/password or a token).
-        :param server_url: URL to the AI platform server.
-        :param dataset_dir: Directory where dataset items are cached.
-        :param worker_url: URL to the AI platform training worker.
-        """
-
-        # initialize client
-        client = Client(username, password, token, server_url=server_url, verify_ssl=False, verify_s3_ssl=False)
-
-        # load job information (model_id, #iteration)
-        job = client.get_job(job_id)
-        if job is None:
-            return
-
-        # load model information
-        model_id = job.get('model').get('id')
-        platform_model = client.get_model(model_id)
-        model_class_labels = client.get_model_class_labels(model_id)
-        target_class_labels = []
-        target_class_label_ids = []
-        for c in model_class_labels:
-            target_class_label = c['target_class_label']
-            if target_class_label is None:
-                # old class labels have no target (they are the target/there is no remapping)
-                target_class_label = c['class_label']
-            if target_class_label['id'] not in target_class_label_ids:
-                target_class_label_ids.append(target_class_label['id'])
-                target_class_labels.append(target_class_label)
-
-        # "class_labels" contains the original and the target class labels
-        platform_model['class_labels'] = model_class_labels
-
-        # the "target_class_labels" contain only those labels that are predicted by the model
-        platform_model['target_class_labels'] = target_class_labels
-
-        iterations = job.get('iterations')
-        current_iteration = job.get('current_iteration')
-        end_iteration = job.get('end_iteration')
-        if current_iteration is not None and current_iteration > 0 and end_iteration is not None and end_iteration > 0:
-            iterations = end_iteration - current_iteration
-
-        # create model and start training
-        try:
-            model = cls(client, dataset_dir, platform_model, iterations, worker_url)
-        except Exception as e:
-            logger.error(f'Model could not be initialized: {e}')
-            raise e
-
-        def shutdown():
-            model.shutdown()
-            model.run_heartbeat_send_loop = False
-            if model.heartbeat_sender is not None:
-                # join the sender thread
-                model.heartbeat_sender.join()
-
-        def shutdown_handler(signum, frame):
-            logger.info('Received signal to shutdown the model training.')
-            shutdown()
-
-        if hasattr(signal, 'SIGBREAK'):
-            signal.signal(signal.SIGBREAK, shutdown_handler)
-        if hasattr(signal, 'SIGINT'):
-            signal.signal(signal.SIGINT, shutdown_handler)
-
-        shutdown_done = False
-        try:
-            model.run()
-        except KeyboardInterrupt:
-            shutdown()
-            shutdown_done = True
-        except Exception as e:
-            logger.error(f'Model finished due to an exception: {e}')
-            model.send_heartbeat({
-                'status': 'exception',
-                'error': str(e),
-            }, send_immediately=True)
-
-            try:
-                shutdown()
-            finally:
-                raise e
-
-        if not shutdown_done:
-            shutdown()
-
-        logger.info('Model finished.')
-
-
-@click.command()
-@click.option('--job_id', type=int, required=True, help='ID of the training job.',
-              envvar='DS_JOB_ID')
-@click.option('--username', type=str, help='Username for the AI platform.', default=None,
-              envvar='DS_USERNAME')
-@click.option('--password', type=str, help='Password for the AI platform.', default=None,
-              envvar='DS_PASSWORD')
-@click.option('--token', type=str, help='Token for the AI platform.', default=None,
-              envvar='DS_TOKEN')
-@click.option('--server_url', default='https://api.vision.data-spree.com/api', help='URL to the API of the platform.',
-              envvar='DS_SERVER_URL')
-@click.option('--dataset_dir', type=click.Path(file_okay=False), default=None,
-              help='Directory for caching datasets.',
-              envvar='DS_DATASET_DIR')
-@click.option('--worker_url', default='http://localhost:6714', help='URL to the training worker.',
-              envvar='DS_WORKER_URL')
-@click.option('--model_class', 'model_class_abs', type=str, default=None,
-              help='Class name of the Model, e.g. "dldstraining.TrainerModel"',
-              envvar='DS_MODEL_CLASS')
-def main(job_id, username, password, token, server_url, dataset_dir, worker_url, model_class_abs) -> None:
-    log_level = logging.INFO
-    logging.basicConfig(level=log_level, format='%(asctime)s %(name)s %(levelname)-6s %(message)s')
-
-    parts = model_class_abs.split('.')
-    module_name = '.'.join(parts[:-1])
-    class_name = parts[-1]
-    try:
-        model_class = getattr(importlib.import_module(module_name), class_name)
-    except Exception as e:
-        click.echo(f'Could not import "{class_name}" from "{module_name}"')
-        raise e from None
-
-    try:
-        model_class.start(job_id, username, password, token, server_url, dataset_dir, worker_url)
-    except Exception as e:
-        sys.exit(-1)
-
-    print('Training exited')
-
-
-if __name__ == '__main__':
-    main()
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import importlib
+import logging
+import signal
+import sys
+from abc import ABC, abstractmethod
+from queue import Queue, Full, Empty
+from threading import Thread
+from typing import Dict, Optional
+
+import click
+import requests as rq
+
+from dataspree.platform_sdk.client import Client
+
+logger = logging.getLogger(__name__)
+
+
+class BaseModel(ABC):
+    def __init__(self, client: Client, dataset_dir: str, model: Dict,
+                 iterations: int, worker_url: str) -> None:
+        super().__init__()
+        self.client: Client = client
+        self.dataset_dir: str = dataset_dir
+        self.platform_model: Dict = model
+        self.iterations: int = iterations
+        self.worker_url: str = worker_url
+
+        self.run_heartbeat_send_loop = True
+
+        self.heartbeat_queue: Optional[Queue] = None
+        self.heartbeat_sender: Optional[Thread] = None
+        if self.worker_url != '':
+            self.heartbeat_queue = Queue(maxsize=10)
+            self.heartbeat_sender: Thread = Thread(target=self.heartbeat_send_loop)
+            self.heartbeat_sender.start()
+
+    @abstractmethod
+    def run(self) -> None:
+        """
+        Stub for implementing the training and evaluation loop. Regularly, the send_heartbeat function must be
+        called:
+        >>> self.send_heartbeat(status)
+        """
+        pass
+
+    @abstractmethod
+    def shutdown(self) -> None:
+        """
+        Stub for implementing the shutdown. You can use this function for implementing a graceful shutdown of the
+        training. For instance, create a last checkpoint.
+        """
+        pass
+
+    def heartbeat_send_loop(self):
+        while self.run_heartbeat_send_loop:
+            try:
+                status = self.heartbeat_queue.get(timeout=1.0)
+                self.__post_heartbeat(status)
+            except Empty:
+                pass
+
+    def __post_heartbeat(self, status):
+        rq.post(f'{self.worker_url}/model_status', json=status)
+
+    def send_heartbeat(self, status, send_immediately=False) -> None:
+        """
+        Report the status of the model. This callback must be called regularly. Otherwise, the process will be
+        terminated.
+        :param status: Dictionary containing the current number of iterations, one of the following states:
+                       ['init', 'running', 'finished', 'exception'].
+        Example:
+        >>> { 'state': 'running', 'iteration': 350 }
+        :param send_immediately: Directly send the heartbeat and wait for the result. Otherwise, the heartbeat
+                                 will be enqueued to be sent in another thread.
+        """
+        try:
+
+            assert status.get('status') in ('init', 'running', 'finished', 'exception')
+            status.setdefault('iteration', 0)
+            status.setdefault('epoch', 0)
+            status.setdefault('end_iteration', 0)
+            status.setdefault('start_iteration', 0)
+            status.setdefault('eta', 0)
+
+            self.heartbeat_queue.put_nowait(status)
+            if send_immediately:
+                self.__post_heartbeat(status)
+        except Full:
+            pass
+
+    @classmethod
+    def start(cls, job_id: int, username: Optional[str] = None, password: Optional[str] = None,
+              token: Optional[str] = None, server_url: str = '', dataset_dir: str = '',
+              worker_url: str = 'http://localhost:6714') -> None:
+        """
+        Initialize the model and call the run method.
+        :param job_id: ID of the AI platform training job that will be processed.
+        :param username: Username for AI platform server.
+        :param password: Password for AI platform server.
+        :param token: Authentication token for AI platform server (use either username/password or a token).
+        :param server_url: URL to the AI platform server.
+        :param dataset_dir: Directory where dataset items are cached.
+        :param worker_url: URL to the AI platform training worker.
+        """
+
+        # initialize client
+        client = Client(username, password, token, server_url=server_url, verify_ssl=False, verify_s3_ssl=False)
+
+        # load job information (model_id, #iteration)
+        job = client.get_job(job_id)
+        if job is None:
+            return
+
+        # load model information
+        model_id = job.get('model').get('id')
+        platform_model = client.get_model(model_id)
+        model_class_labels = client.get_model_class_labels(model_id)
+        target_class_labels = []
+        target_class_label_ids = []
+        for c in model_class_labels:
+            target_class_label = c['target_class_label']
+            if target_class_label is None:
+                # old class labels have no target (they are the target/there is no remapping)
+                target_class_label = c['class_label']
+            if target_class_label['id'] not in target_class_label_ids:
+                target_class_label_ids.append(target_class_label['id'])
+                target_class_labels.append(target_class_label)
+
+        # "class_labels" contains the original and the target class labels
+        platform_model['class_labels'] = model_class_labels
+
+        # the "target_class_labels" contain only those labels that are predicted by the model
+        platform_model['target_class_labels'] = target_class_labels
+
+        iterations = job.get('iterations')
+        current_iteration = job.get('current_iteration')
+        end_iteration = job.get('end_iteration')
+        if current_iteration is not None and current_iteration > 0 and end_iteration is not None and end_iteration > 0:
+            iterations = end_iteration - current_iteration
+
+        # create model and start training
+        try:
+            model = cls(client, dataset_dir, platform_model, iterations, worker_url)
+        except Exception as e:
+            logger.error(f'Model could not be initialized: {e}')
+            raise e
+
+        def shutdown():
+            model.shutdown()
+            model.run_heartbeat_send_loop = False
+            if model.heartbeat_sender is not None:
+                # join the sender thread
+                model.heartbeat_sender.join()
+
+        def shutdown_handler(signum, frame):
+            logger.info('Received signal to shutdown the model training.')
+            shutdown()
+
+        if hasattr(signal, 'SIGBREAK'):
+            signal.signal(signal.SIGBREAK, shutdown_handler)
+        if hasattr(signal, 'SIGINT'):
+            signal.signal(signal.SIGINT, shutdown_handler)
+
+        shutdown_done = False
+        try:
+            model.run()
+        except KeyboardInterrupt:
+            shutdown()
+            shutdown_done = True
+        except Exception as e:
+            logger.error(f'Model finished due to an exception: {e}')
+            model.send_heartbeat({
+                'status': 'exception',
+                'error': str(e),
+            }, send_immediately=True)
+
+            try:
+                shutdown()
+            finally:
+                raise e
+
+        if not shutdown_done:
+            shutdown()
+
+        logger.info('Model finished.')
+
+
+@click.command()
+@click.option('--job_id', type=int, required=True, help='ID of the training job.',
+              envvar='DS_JOB_ID')
+@click.option('--username', type=str, help='Username for the AI platform.', default=None,
+              envvar='DS_USERNAME')
+@click.option('--password', type=str, help='Password for the AI platform.', default=None,
+              envvar='DS_PASSWORD')
+@click.option('--token', type=str, help='Token for the AI platform.', default=None,
+              envvar='DS_TOKEN')
+@click.option('--server_url', default='https://api.vision.data-spree.com/api', help='URL to the API of the platform.',
+              envvar='DS_SERVER_URL')
+@click.option('--dataset_dir', type=click.Path(file_okay=False), default=None,
+              help='Directory for caching datasets.',
+              envvar='DS_DATASET_DIR')
+@click.option('--worker_url', default='http://localhost:6714', help='URL to the training worker.',
+              envvar='DS_WORKER_URL')
+@click.option('--model_class', 'model_class_abs', type=str, default=None,
+              help='Class name of the Model, e.g. "dldstraining.TrainerModel"',
+              envvar='DS_MODEL_CLASS')
+def main(job_id, username, password, token, server_url, dataset_dir, worker_url, model_class_abs) -> None:
+    log_level = logging.INFO
+    logging.basicConfig(level=log_level, format='%(asctime)s %(name)s %(levelname)-6s %(message)s')
+
+    parts = model_class_abs.split('.')
+    module_name = '.'.join(parts[:-1])
+    class_name = parts[-1]
+    try:
+        model_class = getattr(importlib.import_module(module_name), class_name)
+    except Exception as e:
+        click.echo(f'Could not import "{class_name}" from "{module_name}"')
+        raise e from None
+
+    try:
+        model_class.start(job_id, username, password, token, server_url, dataset_dir, worker_url)
+    except Exception as e:
+        sys.exit(-1)
+
+    print('Training exited')
+
+
+if __name__ == '__main__':
+    main()
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/cli.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/cli.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,255 +1,255 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import csv
-import logging
-from typing import List, Dict
-
-import click
-import requests as rq
-from requests import HTTPError, RequestException
-
-from dataspree.platform_sdk.client import Client
-
-logger = logging.getLogger(__name__)
-
-
-@click.group()
-def cli():
-    pass
-
-
-def check_connection(client):
-    try:
-        client.check_connection()
-    except HTTPError as e:
-        if e.response.status_code in [401, 403]:
-            click.echo('Incorrect username/password.', err=True)
-        else:
-            click.echo(f'Connection error. Status code: {e.response.status_code}', err=True)
-        return False
-    except RequestException as e:
-        click.echo(f'Connection error: {e}', err=True)
-        return False
-    except Exception as e:
-        click.echo(f'Unexpected error: {e}', err=True)
-        return False
-
-    return True
-
-
-@cli.command('export')
-@click.option('-o', '--output_dir', 'output_dir', required=True, help='Output directory.',
-              type=click.Path(exists=False, file_okay=False))
-@click.option('-i', '--id', 'dataset_id', required=False, default=-1, help='ID of the dataset to download.', type=int,
-              prompt='Please enter the ID of the dataset to download')
-@click.option('-n', '--n_items', required=False, default=-1,
-              help='Number of items to download. Download all items: \'-1\'', show_default=True, type=int)
-@click.option('--status', 'accepted_status', required=False, multiple=True,
-              type=click.Choice(['', 'uploaded', 'annotated', 'reviewed', 'ignored']),
-              help='Download only those dataset items with the given status.')
-@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
-@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
-              type=int)
-@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
-@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
-              envvar='DS_PASSWORD')
-@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
-              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
-def export_command(output_dir, dataset_id, n_items, accepted_status, username, password, http_retries,
-                   parallel_requests, server_url):
-    client = Client(username, password, None, http_retries, parallel_requests, server_url)
-    if check_connection(client):
-        if len(accepted_status) == 0:
-            accepted_status = None
-        return client.download_dataset(output_dir, dataset_id, n_items, accepted_status)
-
-
-@cli.command('export_dataset_items')
-@click.option('-o', '--output_file', 'output_file', required=True, help='Output csv file.',
-              type=click.Path(exists=False, dir_okay=False))
-@click.option('-f', '--fields', 'fields', required=False, multiple=True)
-@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
-@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
-              type=int)
-@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
-@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
-              envvar='DS_PASSWORD')
-@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
-              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
-@click.option('-i', '--id', 'dataset_id', required=False, default=-1, help='ID of the dataset to download.', type=int,
-              prompt='Please enter the ID of the dataset to download')
-@click.option('-s', '--status', 'status', required=False, multiple=True)
-def export_dataset_items(output_file, fields, dataset_id, status, username, password, http_retries,
-                         parallel_requests, server_url):
-    client = Client(username, password, None, http_retries, parallel_requests, server_url)
-    if check_connection(client):
-        items: List[Dict] = client.get_dataset_items(dataset_id=dataset_id, status=list(status))
-        # id, created_date, uploaded_date, name
-
-        with open(output_file, 'w') as file:
-            writer = csv.writer(file, delimiter=',')
-            writer.writerow(map(str, fields))
-            for item in items:
-                writer.writerow(map(str, map(item.get, fields)))
-
-
-@cli.command(name='import')
-@click.option('--format', 'dataset_format', type=click.Choice(['dataspree', 'kitti', 'coco', 'class_subdirs']),
-              default='dataspree',
-              help='Dataset format to import')
-@click.option('--dataset_name', help='Name of the newly created dataset.')
-@click.option('--dataset_id', type=int, default=-1,
-              help='ID of the dataset to which new items should be imported. If set to \'-1\', a new dataset will be created')
-@click.option('--images', 'images', required=False, type=click.Path(exists=True),
-              help='Directory containing the images to import.')
-@click.option('--annotations', 'annotations', required=False, type=click.Path(exists=True),
-              help='Directory or file containing the annotations to import.')
-@click.option('--directory', 'directory', required=False, type=click.Path(exists=True),
-              help='Directory or file containing data to import (only used for importing classification data from subdirectories).')
-@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
-@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
-              type=int)
-@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
-@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
-              envvar='DS_PASSWORD')
-@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
-              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
-def import_command(dataset_format, dataset_id, dataset_name, images, annotations, directory, http_retries,
-                   parallel_requests, username, password,
-                   server_url):
-    client = Client(username, password, None, http_retries, parallel_requests, server_url)
-    if check_connection(client):
-        if dataset_format == 'dataspree':
-            return client.import_dataspree(dataset_name, dataset_id, images, annotations)
-        elif dataset_format == 'kitti':
-            return client.import_kitti(dataset_name, dataset_id, images, annotations)
-        elif dataset_format == 'coco':
-            return client.import_coco(dataset_name, dataset_id, images, annotations)
-        elif dataset_format == 'class_subdirs':
-            return client.import_classification_directories(dataset_name, dataset_id, directory)
-
-
-@cli.group()
-@click.option('--url', default='http://localhost:6714', help='Base URL to reach the worker.', envvar='DS_WORKER_URL')
-@click.option('--timeout', default=5, help='Timeout for requests to the worker.')
-@click.pass_context
-def worker(ctx, url, timeout):
-    ctx.ensure_object(dict)
-    ctx.obj['url'] = url
-    ctx.obj['timeout'] = timeout
-
-
-@worker.command()
-@click.pass_context
-def pause(ctx):
-    try:
-        base_url = ctx.obj['url']
-        timeout = ctx.obj['timeout']
-        response = rq.get(f'{base_url}/pause', timeout=timeout)
-        response.raise_for_status()
-        click.echo('Pausing the worker has been initiated. It can take up to one minute until a training checkpoint is '
-                   'created and the training stopped.')
-    except rq.exceptions.HTTPError as e:
-        click.echo(f'HTTP error: {e}')
-    except rq.exceptions.RequestException as e:
-        click.echo(f'Worker is offline. Make sure that the worker is running.')
-
-
-@worker.command()
-@click.pass_context
-def resume(ctx):
-    try:
-        base_url = ctx.obj['url']
-        timeout = ctx.obj['timeout']
-        response = rq.get(f'{base_url}/resume', timeout=timeout)
-        response.raise_for_status()
-        click.echo('Worker has been resumed.')
-    except rq.exceptions.HTTPError as e:
-        click.echo(f'HTTP error: {e}')
-    except rq.exceptions.RequestException as e:
-        click.echo(f'Worker is offline. Make sure that the worker is running.')
-
-
-@worker.command()
-@click.pass_context
-def status(ctx):
-    try:
-        base_url = ctx.obj['url']
-        timeout = ctx.obj['timeout']
-        response = rq.get(f'{base_url}/status', timeout=timeout)
-        response.raise_for_status()
-        worker_status = response.json()
-        iteration = worker_status["iteration"]
-        if iteration is None:
-            iteration = '-'
-        job = worker_status["job"]
-        if job is None:
-            job = '-'
-        click.echo(f'status:\t{worker_status["status"]}\niteration:\t{iteration}\njob:\t{job}')
-    except rq.exceptions.HTTPError as e:
-        click.echo(f'HTTP error: {e}')
-    except rq.exceptions.RequestException as e:
-        click.echo(f'status:\toffline\niteration:\t-\njob:\t-')
-
-
-def do_setup(base_url, timeout):
-    try:
-        # check server status
-        response = rq.get(f'{base_url}/status', timeout=timeout)
-        response.raise_for_status()
-
-        worker_status = response.json()
-        if worker_status['status'] != 'uninitialized':
-            if not click.confirm(
-                    'The worker is already initialized. Do you want to setup the worker anew? A new worker '
-                    'instance will be created in the AI platform and running jobs will be stopped. This can '
-                    'take a minute.'):
-                return
-        auth_method = click.prompt('Which authentication method should be used by the worker?',
-                                   default='username/password',
-                                   type=click.Choice(['username/password', 'token']))
-        setup_data = {}
-        if auth_method == 'username/password':
-            setup_data['username'] = click.prompt('Username', type=str)
-            setup_data['password'] = click.prompt('Password', type=str, hide_input=True)
-        elif auth_method == 'token':
-            setup_data['auth_token'] = click.prompt('Token', type=str)
-
-        setup_data['platform_host'] = click.prompt('AI Platform Host', default='api.vision.data-spree.com', type=str)
-        setup_data['dataset_dir'] = click.prompt('Dataset directory', default='', type=str)
-        click.echo('Setting up...')
-        response = rq.post(f'{base_url}/setup', json=setup_data, timeout=timeout)
-        if response.status_code == 200:
-            click.echo('Setup successful')
-        else:
-            click.echo(f'Setup failed: {response.text}')
-
-    except rq.exceptions.HTTPError as e:
-        click.echo(f'HTTP error: {e}')
-    except rq.exceptions.RequestException as e:
-        click.echo(f'Worker is offline. Make sure that the worker is running.')
-
-
-@worker.command()
-@click.pass_context
-def setup(ctx):
-    base_url = ctx.obj['url']
-    timeout = ctx.obj['timeout']
-    do_setup(base_url, timeout)
-
-
-if __name__ == '__main__':
-    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(name)s %(levelname)-6s %(message)s')
-    cli()
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import csv
+import logging
+from typing import List, Dict
+
+import click
+import requests as rq
+from requests import HTTPError, RequestException
+
+from dataspree.platform_sdk.client import Client
+
+logger = logging.getLogger(__name__)
+
+
+@click.group()
+def cli():
+    pass
+
+
+def check_connection(client):
+    try:
+        client.check_connection()
+    except HTTPError as e:
+        if e.response.status_code in [401, 403]:
+            click.echo('Incorrect username/password.', err=True)
+        else:
+            click.echo(f'Connection error. Status code: {e.response.status_code}', err=True)
+        return False
+    except RequestException as e:
+        click.echo(f'Connection error: {e}', err=True)
+        return False
+    except Exception as e:
+        click.echo(f'Unexpected error: {e}', err=True)
+        return False
+
+    return True
+
+
+@cli.command('export')
+@click.option('-o', '--output_dir', 'output_dir', required=True, help='Output directory.',
+              type=click.Path(exists=False, file_okay=False))
+@click.option('-i', '--id', 'dataset_id', required=False, default=-1, help='ID of the dataset to download.', type=int,
+              prompt='Please enter the ID of the dataset to download')
+@click.option('-n', '--n_items', required=False, default=-1,
+              help='Number of items to download. Download all items: \'-1\'', show_default=True, type=int)
+@click.option('--status', 'accepted_status', required=False, multiple=True,
+              type=click.Choice(['', 'uploaded', 'annotated', 'reviewed', 'ignored']),
+              help='Download only those dataset items with the given status.')
+@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
+@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
+              type=int)
+@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
+@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
+              envvar='DS_PASSWORD')
+@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
+              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
+def export_command(output_dir, dataset_id, n_items, accepted_status, username, password, http_retries,
+                   parallel_requests, server_url):
+    client = Client(username, password, None, http_retries, parallel_requests, server_url)
+    if check_connection(client):
+        if len(accepted_status) == 0:
+            accepted_status = None
+        return client.download_dataset(output_dir, dataset_id, n_items, accepted_status)
+
+
+@cli.command('export_dataset_items')
+@click.option('-o', '--output_file', 'output_file', required=True, help='Output csv file.',
+              type=click.Path(exists=False, dir_okay=False))
+@click.option('-f', '--fields', 'fields', required=False, multiple=True)
+@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
+@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
+              type=int)
+@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
+@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
+              envvar='DS_PASSWORD')
+@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
+              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
+@click.option('-i', '--id', 'dataset_id', required=False, default=-1, help='ID of the dataset to download.', type=int,
+              prompt='Please enter the ID of the dataset to download')
+@click.option('-s', '--status', 'status', required=False, multiple=True)
+def export_dataset_items(output_file, fields, dataset_id, status, username, password, http_retries,
+                         parallel_requests, server_url):
+    client = Client(username, password, None, http_retries, parallel_requests, server_url)
+    if check_connection(client):
+        items: List[Dict] = client.get_dataset_items(dataset_id=dataset_id, status=list(status))
+        # id, created_date, uploaded_date, name
+
+        with open(output_file, 'w') as file:
+            writer = csv.writer(file, delimiter=',')
+            writer.writerow(map(str, fields))
+            for item in items:
+                writer.writerow(map(str, map(item.get, fields)))
+
+
+@cli.command(name='import')
+@click.option('--format', 'dataset_format', type=click.Choice(['dataspree', 'kitti', 'coco', 'class_subdirs']),
+              default='dataspree',
+              help='Dataset format to import')
+@click.option('--dataset_name', help='Name of the newly created dataset.')
+@click.option('--dataset_id', type=int, default=-1,
+              help='ID of the dataset to which new items should be imported. If set to \'-1\', a new dataset will be created')
+@click.option('--images', 'images', required=False, type=click.Path(exists=True),
+              help='Directory containing the images to import.')
+@click.option('--annotations', 'annotations', required=False, type=click.Path(exists=True),
+              help='Directory or file containing the annotations to import.')
+@click.option('--directory', 'directory', required=False, type=click.Path(exists=True),
+              help='Directory or file containing data to import (only used for importing classification data from subdirectories).')
+@click.option('--http_retries', required=False, default=10, help='Number of HTTP retries.', show_default=True, type=int)
+@click.option('--parallel_requests', required=False, default=16, help='Number of parallel requests.', show_default=True,
+              type=int)
+@click.option('--username', prompt='Username', help='Username for data spree vision platform.', envvar='DS_USERNAME')
+@click.option('--password', prompt='Password', hide_input=True, help='Password for data spree vision platform.',
+              envvar='DS_PASSWORD')
+@click.option('--url', 'server_url', default='https://api.vision.data-spree.com/api',
+              help='URL to the API of the platform.', envvar='DS_SERVER_URL')
+def import_command(dataset_format, dataset_id, dataset_name, images, annotations, directory, http_retries,
+                   parallel_requests, username, password,
+                   server_url):
+    client = Client(username, password, None, http_retries, parallel_requests, server_url)
+    if check_connection(client):
+        if dataset_format == 'dataspree':
+            return client.import_dataspree(dataset_name, dataset_id, images, annotations)
+        elif dataset_format == 'kitti':
+            return client.import_kitti(dataset_name, dataset_id, images, annotations)
+        elif dataset_format == 'coco':
+            return client.import_coco(dataset_name, dataset_id, images, annotations)
+        elif dataset_format == 'class_subdirs':
+            return client.import_classification_directories(dataset_name, dataset_id, directory)
+
+
+@cli.group()
+@click.option('--url', default='http://localhost:6714', help='Base URL to reach the worker.', envvar='DS_WORKER_URL')
+@click.option('--timeout', default=5, help='Timeout for requests to the worker.')
+@click.pass_context
+def worker(ctx, url, timeout):
+    ctx.ensure_object(dict)
+    ctx.obj['url'] = url
+    ctx.obj['timeout'] = timeout
+
+
+@worker.command()
+@click.pass_context
+def pause(ctx):
+    try:
+        base_url = ctx.obj['url']
+        timeout = ctx.obj['timeout']
+        response = rq.get(f'{base_url}/pause', timeout=timeout)
+        response.raise_for_status()
+        click.echo('Pausing the worker has been initiated. It can take up to one minute until a training checkpoint is '
+                   'created and the training stopped.')
+    except rq.exceptions.HTTPError as e:
+        click.echo(f'HTTP error: {e}')
+    except rq.exceptions.RequestException as e:
+        click.echo(f'Worker is offline. Make sure that the worker is running.')
+
+
+@worker.command()
+@click.pass_context
+def resume(ctx):
+    try:
+        base_url = ctx.obj['url']
+        timeout = ctx.obj['timeout']
+        response = rq.get(f'{base_url}/resume', timeout=timeout)
+        response.raise_for_status()
+        click.echo('Worker has been resumed.')
+    except rq.exceptions.HTTPError as e:
+        click.echo(f'HTTP error: {e}')
+    except rq.exceptions.RequestException as e:
+        click.echo(f'Worker is offline. Make sure that the worker is running.')
+
+
+@worker.command()
+@click.pass_context
+def status(ctx):
+    try:
+        base_url = ctx.obj['url']
+        timeout = ctx.obj['timeout']
+        response = rq.get(f'{base_url}/status', timeout=timeout)
+        response.raise_for_status()
+        worker_status = response.json()
+        iteration = worker_status["iteration"]
+        if iteration is None:
+            iteration = '-'
+        job = worker_status["job"]
+        if job is None:
+            job = '-'
+        click.echo(f'status:\t{worker_status["status"]}\niteration:\t{iteration}\njob:\t{job}')
+    except rq.exceptions.HTTPError as e:
+        click.echo(f'HTTP error: {e}')
+    except rq.exceptions.RequestException as e:
+        click.echo(f'status:\toffline\niteration:\t-\njob:\t-')
+
+
+def do_setup(base_url, timeout):
+    try:
+        # check server status
+        response = rq.get(f'{base_url}/status', timeout=timeout)
+        response.raise_for_status()
+
+        worker_status = response.json()
+        if worker_status['status'] != 'uninitialized':
+            if not click.confirm(
+                    'The worker is already initialized. Do you want to setup the worker anew? A new worker '
+                    'instance will be created in the AI platform and running jobs will be stopped. This can '
+                    'take a minute.'):
+                return
+        auth_method = click.prompt('Which authentication method should be used by the worker?',
+                                   default='username/password',
+                                   type=click.Choice(['username/password', 'token']))
+        setup_data = {}
+        if auth_method == 'username/password':
+            setup_data['username'] = click.prompt('Username', type=str)
+            setup_data['password'] = click.prompt('Password', type=str, hide_input=True)
+        elif auth_method == 'token':
+            setup_data['auth_token'] = click.prompt('Token', type=str)
+
+        setup_data['platform_host'] = click.prompt('AI Platform Host', default='api.vision.data-spree.com', type=str)
+        setup_data['dataset_dir'] = click.prompt('Dataset directory', default='', type=str)
+        click.echo('Setting up...')
+        response = rq.post(f'{base_url}/setup', json=setup_data, timeout=timeout)
+        if response.status_code == 200:
+            click.echo('Setup successful')
+        else:
+            click.echo(f'Setup failed: {response.text}')
+
+    except rq.exceptions.HTTPError as e:
+        click.echo(f'HTTP error: {e}')
+    except rq.exceptions.RequestException as e:
+        click.echo(f'Worker is offline. Make sure that the worker is running.')
+
+
+@worker.command()
+@click.pass_context
+def setup(ctx):
+    base_url = ctx.obj['url']
+    timeout = ctx.obj['timeout']
+    do_setup(base_url, timeout)
+
+
+if __name__ == '__main__':
+    logging.basicConfig(level=logging.INFO, format='%(asctime)s %(name)s %(levelname)-6s %(message)s')
+    cli()
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/client.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/client.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,1920 +1,1920 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import io
-import json
-import logging
-import math
-import os
-import sys
-import threading
-import traceback
-import datetime
-from typing import Dict, Union, Optional, List, Tuple, Any
-
-import msgpack
-import requests as rq
-from joblib import Parallel, delayed
-from requests.adapters import HTTPAdapter
-from requests.auth import HTTPBasicAuth
-from tqdm import tqdm
-from urllib3 import Retry
-
-from .http_token_authentication import HTTPTokenAuth
-from .query import Condition, Conditions, Equal, GreaterThan, LessThan, Or
-
-logger = logging.getLogger(__name__)
-
-
-def value_or_env(value: Optional[str]):
-    if not value or value[:2] != '[[' or value[-2:] != ']]':
-        return value
-
-    return os.environ[value[2:-2]]
-
-
-class Client:
-    """Client for the Data Spree AI Platform.
-
-    The platform client forms the interface to the AI platform and provides a variety of functions. For instance, it is
-    possible download a whole dataset given its ID or create a new one and upload the corresponding dataset items.
-
-    :param username: Platform username. Required for authentication.
-    :param password: Platform password. Required for authentication.
-    :param auth_token: Platform authentication token.
-    :param http_retries: Number of HTTP retries before error is thrown.
-    :param parallel_requests: Maximum number of parallel HTTP request.
-    :param server_url: URL of the AI platform. Modify this parameter in case you use an on-premise installation.
-
-    """
-
-    def __init__(self, username: Optional[str] = None, password: Optional[str] = None, auth_token: Optional[str] = None,
-                 http_retries: int = 10, parallel_requests: int = 16,
-                 server_url: str = 'https://api.vision.data-spree.com/api', verify_ssl: bool = True,
-                 verify_s3_ssl: bool = True, proxy_servers: Optional[Dict[str, str]] = None):
-
-        self.username = username
-        self.password = password
-        self.auth_token = auth_token
-        self.proxy_servers = proxy_servers
-
-        self.auth = None
-        if auth_token:
-            self.auth = HTTPTokenAuth(auth_token)
-        elif username is not None and password is not None:
-            self.auth = HTTPBasicAuth(value_or_env(username), value_or_env(password))
-
-        if self.auth is None:
-            raise ValueError('Username and password or authentication token must be provided.')
-
-        self.http_retries = http_retries
-        self.server_url = server_url
-        self.parallel_requests = parallel_requests
-        if self.parallel_requests <= 0:
-            raise ValueError(f'Invalid parallel requests: {self.parallel_requests} must be greater than zero.')
-
-        self.http = rq.Session()
-        if not verify_ssl:
-            self.http.verify = False
-        self.s3_http = rq.Session()
-        if not verify_s3_ssl:
-            self.s3_http.verify = False
-        self.http.auth = self.auth
-        retry = Retry(total=http_retries, connect=1, backoff_factor=0.5,
-                      status_forcelist=[500, 502, 503, 504])
-        adapter = HTTPAdapter(pool_maxsize=self.parallel_requests, max_retries=retry)
-
-        if self.proxy_servers is not None:
-            self.http.proxies.update(proxy_servers)
-            self.s3_http.proxies.update(proxy_servers)
-
-        self.http.mount('http://', adapter)
-        self.http.mount('https://', adapter)
-
-    def __reduce__(self):
-        return (Client, (self.username,
-                         self.password,
-                         self.auth_token,
-                         self.http_retries,
-                         self.parallel_requests,
-                         self.server_url,
-                         self.http.verify,
-                         self.s3_http.verify,))
-
-    @staticmethod
-    def get_dataset_item_date_format_string() -> str:
-        return '%Y-%m-%dT%H:%M:%S.%fZ'
-
-    @staticmethod
-    def get_dataset_item_date_format_string_short() -> str:
-        return '%Y-%m-%dT%H:%M:%SZ'
-
-    @staticmethod
-    def parse_dataset_item_date(date_string: Optional[str]) -> Optional[datetime.datetime]:
-        if date_string is None:
-            return None
-
-        try:
-            return datetime.datetime.fromisoformat(date_string)
-        except (TypeError, ValueError, AttributeError):
-            pass
-
-        try:
-            return datetime.datetime.strptime(date_string, Client.get_dataset_item_date_format_string())
-        except (TypeError, ValueError, AttributeError):
-            pass
-
-        try:
-            return datetime.datetime.strptime(date_string, Client.get_dataset_item_date_format_string_short())
-        except (TypeError, ValueError, AttributeError):
-            pass
-
-        return None
-
-    @staticmethod
-    def dataspree_temp_dir(*sub_dirs: str) -> str:
-        temp_dir = os.path.join(Client.dataspree_dir(), 'temp', *sub_dirs)
-        os.makedirs(temp_dir, exist_ok=True)
-        return temp_dir
-
-    @staticmethod
-    def dataspree_dir():
-        base_dir = os.path.expanduser('~')
-        dir = os.path.join(base_dir, '.dataspree')
-        if sys.platform in ['win32', 'cygwin'] and os.getlogin() == 'SYSTEM':
-            # on windows in case the 'user' is SYSTEM, e.g. when started as a windows service
-            dir = os.path.join(os.getenv('ALLUSERSPROFILE'), 'Data Spree', 'AI Platform')
-        try:
-            os.makedirs(dir)
-        except FileExistsError:
-            pass
-        return dir
-
-    def check_connection(self):
-        response = self.http.get(f'{self.server_url}/auth/users/me/')
-        response.raise_for_status()
-        return response.json()
-
-    def server_status(self):
-        response = self.http.get(f'{self.server_url}/server')
-        response.raise_for_status()
-        return response.json()
-
-    def create_dataset(self,
-                       dataset_name,
-                       classification_class_label_ids=None,
-                       key_point_ids=None,
-                       roi_classification_class_label_ids=None,
-                       roi_key_point_ids=None,
-                       object_detection_class_label_ids=None,
-                       object_detection_key_point_ids=None,
-                       object_detection_masks=False,
-                       semantic_segmentation_class_label_ids=None):
-        """Create a new dataset.
-
-        :param dataset_name: Name of the new dataset.
-        :param classification_class_label_ids: IDs of the class labels for the classification of the whole image.
-        :param key_point_ids: IDs of the key points that can be annotated for the whole image.
-        :param roi_classification_class_label_ids: IDs of the class label for the classification of regions of interest.
-        :param roi_key_point_ids: IDs of the key points that can be annotated for each region of interest.
-        :param object_detection_class_label_ids: IDs of the class labels for object annotations.
-        :param object_detection_key_point_ids: IDs of the key points that can be annotated for individual objects.
-        :param object_detection_masks: Set to True if it should be possible to annotate individual objects with segmentation masks.
-        :param semantic_segmentation_class_label_ids: IDs of the class labels for annotating each pixel with a class label (semantic segmentation of the image).
-        :return: ID of the newly created dataset or -1 if dataset creation fails.
-        """
-
-        dataset = {
-            'name': dataset_name,
-            'classification': classification_class_label_ids is not None,
-            'key_points': key_point_ids is not None,
-            'roi_classification': roi_classification_class_label_ids is not None,
-            'roi_key_points': roi_key_point_ids is not None,
-            'object_detection': object_detection_class_label_ids is not None,
-            'object_detection_key_points': object_detection_key_point_ids is not None,
-            'object_detection_mask': object_detection_masks,
-            'semantic_segmentation': semantic_segmentation_class_label_ids is not None,
-        }
-
-        if dataset['classification']:
-            dataset['classification_class_label_ids'] = classification_class_label_ids
-
-        if dataset['key_points']:
-            dataset['key_point_ids'] = key_point_ids
-
-        if dataset['roi_classification']:
-            dataset['roi_classification_class_label_ids'] = roi_classification_class_label_ids
-
-        if dataset['roi_key_points']:
-            dataset['roi_key_point_ids'] = roi_key_point_ids
-
-        if dataset['object_detection']:
-            dataset['object_detection_class_label_ids'] = object_detection_class_label_ids,
-
-        if dataset['object_detection_key_points']:
-            dataset['object_detection_key_point_ids'] = object_detection_key_point_ids
-
-        if dataset['semantic_segmentation']:
-            dataset['semantic_segmentation_class_label_ids'] = semantic_segmentation_class_label_ids
-
-        try:
-            response = self.http.post(self.server_url + '/datasets/', data=dataset)
-            response.raise_for_status()
-            data = response.json()
-            return data['id']
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return -1
-
-    def get_dataset(self, dataset_id: int):
-        """Get information about a dataset.
-
-        Example:
-            >>> {
-            >>>    'id': 46,
-            >>>    'total_items': 104,
-            >>>    'uploaded_items': 0,
-            >>>    'annotated_items': 0,
-            >>>    'reviewed_items': 104,
-            >>>    'ignored_items': 0,
-            >>>    'created_by': {'id': 1, 'username': 'admin'},
-            >>>    'name': 'Traffic II',
-            >>>    'created_date': '2019-07-29T10:06:22.454871Z',
-            >>>    'updated_date': '2019-07-29T10:06:22.454914Z',
-            >>>    'classification': False,
-            >>>    'key_points': False,
-            >>>    'roi_classification': False,
-            >>>    'roi_key_points': False,
-            >>>    'object_detection': True,
-            >>>    'object_detection_key_points': False,
-            >>>    'object_detection_mask': False,
-            >>>    'semantic_segmentation': False,
-            >>>    'classification_class_labels': [],
-            >>>    'key_point_names': [],
-            >>>    'roi_classification_class_labels': [],
-            >>>    'roi_key_points_names': [],
-            >>>    'object_detection_class_labels': [{'id': 4, 'name': 'car'},
-            >>>     {'id': 6, 'name': 'truck'},
-            >>>     {'id': 7, 'name': 'pedestrian'},
-            >>>     {'id': 9, 'name': 'cyclist'},
-            >>>     {'id': 41, 'name': 'traffic light'},
-            >>>     {'id': 119, 'name': 'traffic sign'}],
-            >>>    'object_detection_key_point_names': [],
-            >>>    'semantic_segmentation_class_labels': []
-            >>> }
-
-        :param dataset_id: ID of the dataset to receive information.
-        :return: Dictionary containing information of the requested datatset.
-        """
-        request: str = self.server_url + '/datasets/{}/'.format(dataset_id)
-        try:
-            response = self.http.get(request)
-            if response.status_code == 200:
-                dataset = response.json()
-                return dataset
-        except rq.exceptions.RequestException as e:
-            logger.error(f'An error occurred during GET request: {request}: {e}')
-
-        return None
-
-    def get_dataset_items_url(self, dataset_id: Optional[int] = None,
-                              class_id: Optional[int] = None,
-                              subset_id: Optional[Union[str, int]] = None,
-                              created_date_since: Optional[Union[str, datetime.datetime]] = None,
-                              created_date_until: Optional[Union[str, datetime.datetime]] = None,
-                              status: Optional[List[str]] = None,
-                              query_expression: Optional[Condition] = None,
-                              free_query_str: Optional[str] = None, *, return_query: bool = False,
-                              max_items: Optional[int] = None) -> str:
-        items_per_request: int = min(5000, max_items) if max_items is not None else 5000
-
-        def format_time(t: Optional[Union[str, datetime.datetime]]) -> Optional[str]:
-            return t if t is None or type(t) == str else t.isoformat()
-
-        # Compile conditions
-        condition_str: str = Conditions.create(Equal(var='class', val=class_id),
-                                               Equal(var='dataset__id', val=dataset_id),
-                                               Equal(var='page_size', val=items_per_request),
-                                               Equal(var='data_subsets__id', val=subset_id),
-                                               GreaterThan(var='created_date', val=format_time(created_date_since)),
-                                               LessThan(var='created_date', val=format_time(created_date_until)),
-                                               Or(*(Equal(var='status', val=s) for s in status)) if status else None,
-                                               query_expression, exclude_empty=True, do_url_escape=True)
-
-        if free_query_str:
-            if not free_query_str.startswith('&'):
-                free_query_str = f'&{free_query_str}'
-            condition_str += free_query_str
-
-        # Compile URL
-        return f'{self.server_url}/dataset-items/?{condition_str}'
-
-    def get_dataset_items(self, dataset_id: Optional[int] = None,
-                          class_id: Optional[int] = None,
-                          subset_id: Optional[Union[str, int]] = None,
-                          created_date_since: Optional[Union[str, datetime.datetime]] = None,
-                          created_date_until: Optional[Union[str, datetime.datetime]] = None,
-                          status: Optional[List[str]] = None,
-                          query_expression: Optional[Condition] = None,
-                          free_query_str: Optional[str] = None, *, return_query: bool = False,
-                          max_items: Optional[int] = None) \
-            -> Union[Optional[List[Dict]], Tuple[Optional[List[Dict]], str]]:
-        """
-        Return all dataset items that match the filter compiled from this functions' parameters.
-
-        :param dataset_id:          Identifier of the dataset whose content be downloaded.
-        :param subset_id:           Identifier of the subset whose content be downloaded or None if you don't want
-                                    to filter by subset. "null()" if you would like to receive every dataset item
-                                    that is not part of any subset.
-        :param class_id:            Set this to only download items of the specified class_id
-        :param created_date_since:  Set this to filter out dataset items created at created_date_since or earlier.
-        :param created_date_until:  Set this to filter out dataset items created at created_date_until or later.
-        :param status:              If not set, return the dataset items irrespective of their status.
-                                    Otherwise, add an OR filter to the query on the content of the status list.
-        :param query_expression:    Set this field to supply a custom query expression to the query.
-        :param free_query_str:      Set this field to supply a custom query expression as a string to the query.
-        :param return_query:        Return first query if enabled as second return argument
-        :param max_items:           Max number of items to be returned.
-        :return:                    A list of dataset items or None, if a problem occurred.
-        """
-        # Compile URL
-        url: Optional[str] = self.get_dataset_items_url(dataset_id=dataset_id, class_id=class_id, subset_id=subset_id,
-                                                        created_date_since=created_date_since,
-                                                        created_date_until=created_date_until, status=status,
-                                                        query_expression=query_expression,
-                                                        free_query_str=free_query_str, max_items=max_items)
-        first_url: str = url
-
-        all_items: List[Dict] = list()
-        while url is not None:
-
-            logger.debug(f'Get dataset items from "{url}"')
-            try:
-                response: rq.models.Response = self.http.get(url)
-                response.raise_for_status()
-                response_json = response.json()
-
-                items: Optional[List[Dict]] = response_json.get('results')
-                url = response_json.get('next')
-
-                if not items:
-                    break
-
-                all_items.extend(items)
-
-                if max_items is not None and len(all_items) >= max_items:
-                    break
-
-            except rq.exceptions.RequestException as e:
-                logger.error(f'An error occurred during GET request: {url}: {e}')
-
-                if return_query:
-                    return None, first_url
-                return None
-
-        if return_query:
-            return all_items, first_url
-        return all_items
-
-    def delete_dataset(self, dataset_id):
-        """Delete a dataset.
-
-        :param dataset_id: id of the dataset
-        :return: 'True' if success else 'False'
-        """
-
-        try:
-            request: str = f'{self.server_url}/datasets/{dataset_id}'
-            response = self.http.delete(request)
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(f'An error occurred during HTTP delete request: {request}: {e}')
-
-        return False
-
-    def download_dataset(self, directory, dataset_id, n_items=-1, accepted_status=None):
-        """Download a dataset from data spree vision platform.
-
-        :param directory:  Directory to download dataset items (images and annotations)
-        :param dataset_id: ID of the dataset that should be downloaded.
-        :param n_items: Maximum number of items to download. Set to -1 to download all items.
-        :param accepted_status: Download only items with the provided status (list of strings). Set to None to accept all status.
-        """
-
-        logger.info('Download dataset. Dataset ID: {}'.format(dataset_id))
-
-        # download list of dataset items
-        dataset_items = self.get_dataset_items(dataset_id)
-        if dataset_items is None:
-            logger.error('Could not get list of dataset items for dataset with ID {}'.format(dataset_id))
-
-        # create output directories
-        try:
-            os.makedirs(directory)
-        except FileExistsError:
-            pass
-        try:
-            os.makedirs(os.path.join(directory, 'images'))
-        except FileExistsError:
-            pass
-        image_dir = os.path.join(directory, 'images')
-        try:
-            os.makedirs(os.path.join(directory, 'annotations'))
-        except FileExistsError:
-            pass
-
-        annotation_dir = os.path.join(directory, 'annotations')
-
-        if n_items != -1:
-            dataset_items = dataset_items[:n_items]
-
-        # use only those dataset items from the list, that are not yet downloaded
-        new_dataset_items = []
-        for item in dataset_items:
-            image_name = item['name'].split('/')[-1]
-            image_name = '{}_{}_{}'.format(dataset_id, item['id'], image_name)
-            image_file_path = os.path.join(image_dir, image_name)
-
-            annotation_file_name = os.path.splitext(image_name)[0] + '.json'
-            annotation_file_path = os.path.join(annotation_dir, annotation_file_name)
-
-            if not os.path.exists(image_file_path) or not os.path.exists(annotation_file_path):
-                new_dataset_items.append(item)
-
-        logger.info(
-            '{} items available in dataset {}. {} already downloaded'.format(len(dataset_items), dataset_id,
-                                                                             len(dataset_items) - len(
-                                                                                 new_dataset_items)))
-
-        if len(new_dataset_items) != 0:
-            with open(os.path.join(directory, 'items.json'), 'w') as f:
-                json.dump(dataset_items, f, indent=2)
-
-            if self.parallel_requests > 1:
-                Parallel(n_jobs=self.parallel_requests, prefer='threads')(
-                    delayed(self.download_dataset_item)(item['id'], image_dir, annotation_dir, accepted_status)
-                    for item in tqdm(new_dataset_items))
-            else:
-                for item in tqdm(new_dataset_items):
-                    self.download_dataset_item(item['id'], image_dir, annotation_dir, accepted_status)
-
-        logger.info('Download completed. (dataset ID: {})'.format(dataset_id))
-
-    def create_data_subset(self, subset_name, dataset_id, description=''):
-        """Add a subset to an existing dataset.
-
-        :param subset_name: name of the subset
-        :param dataset_id: id of the parent dataset
-        :param description: string description
-        :return: newly created subset or 'None' if subset creation fails.
-        """
-
-        subset_dict = {
-            'name': subset_name,
-            'description': description,
-            'dataset': dataset_id,
-        }
-
-        try:
-            request: str = f'{self.server_url}/data-subsets/'
-            response = self.http.post(request, data=subset_dict)
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(f'An error occurred during HTTP post request: {request}: {e}')
-
-        return None
-
-    def get_data_subset(self, subset_id):
-        """Get information about a dataset.
-
-        Example:
-            >>> {
-            >>>    'id': 46,
-            >>>    'total_items': 104,
-            >>>    'name': 'Traffic II',
-            >>>    'description': str,
-            >>>    'dataset': 24,
-            >>> }
-
-        :param subset_id: ID of the subset to receive information.
-        :return: Dictionary containing information of the requested subset.
-        """
-        try:
-            request = self.server_url + '/data-subsets/{}/'.format(subset_id)
-            response = self.http.get(request)
-            if response.status_code == 200:
-                subset = response.json()
-                return subset
-        except rq.exceptions.RequestException as e:
-            logger.error(f'An error occurred during HTTP get request: {request}: {e}')
-
-        return None
-
-    def get_data_subset_items(self, subset_id) -> List[Dict]:
-        """
-        Get all subset items for the subset given by its ID.
-        :see get_dataset_items
-        """
-        return self.get_dataset_items(subset_id=subset_id)
-
-    def delete_data_subset(self, subset_id):
-        """Delete a subset to an existing dataset.
-
-        :param subset_id: id of the subset
-        :return: 'True' if success else 'False'
-        """
-
-        try:
-            request = f'{self.server_url}/data-subsets/{subset_id}'
-            response = self.http.delete(request)
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(f'An error occurred during HTTP delete request: {request}: {e}')
-
-        return False
-
-    def create_dataset_item(self,
-                            image_file,
-                            dataset_id,
-                            annotations=None,
-                            image_file_name=None,
-                            status=None,
-                            created_date=None):
-        """Create a new dataset item including the image and the associated annotations.
-
-        :param image_file: File path to the image or image bytes to upload that belongs to the new item.
-        :param dataset_id: The new item will be created for the provided dataset ID.
-        :param annotations: Dictionary of the annotations
-        :param image_file_name: Name of the image that should be uploaded. Set to `None` to use the file name derived from `image_file` if provided as a path, otherwise a name is required.
-        :param status: Status of the newly created item. Should be one of `['uploaded', 'annotated', 'reviewed', 'ignored']`. Set to `None` to automatically set to `reviewed` or `uploaded` in case the annotations are empty.
-        :param created_date: Creation date and time as datetime object or number (seconds, POSIX timestamp) of the dataset item (upload time is used if not provided).
-        :return: ID of the newly created item or `-1` in case it could not be created.
-        """
-
-        if annotations is None:
-            annotations = {}
-        if isinstance(image_file, bytes):
-            if not isinstance(image_file_name, str):
-                raise ValueError('If an image is passed in bytes form, an "image_file_name" (str) has to be provided.')
-            files = {
-                'data': (image_file_name, image_file)
-            }
-        else:
-            if image_file_name is None:
-                image_file_name = os.path.split(image_file)[-1]
-
-            files = {
-                'data': (image_file_name, open(image_file, 'rb'))
-            }
-
-        if status is None:
-            status = 'reviewed' if annotations else 'uploaded'
-
-        dataset_item = {
-            'dataset_id': dataset_id,
-            'annotations': json.dumps(annotations),
-            'status': status
-        }
-
-        if created_date is not None:
-            if type(created_date) in (int, float):
-                created_date_dt = datetime.datetime.fromtimestamp(created_date)
-            else:
-                created_date_dt = created_date
-
-            if type(created_date_dt) != datetime.datetime:
-                raise ValueError('"created_date" must be a datetime object or a number')
-
-            created_date_str = created_date_dt.isoformat()
-            dataset_item['created_date'] = created_date_str
-
-        try:
-            response = self.http.post(self.server_url + '/dataset-items/', data=dataset_item, files=files)
-            response.raise_for_status()
-            data = response.json()
-            return data['id']
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            traceback.print_exc()
-        except Exception as e:
-            logger.error(e)
-            traceback.print_exc()
-
-        return -1
-
-    def get_dataset_item(self, item_id):
-        """Get a dataset item given its ID.
-        :param item_id: ID of the item to be retrieved.
-        :return: Dictionary containing the item details (e.g., ID, name, status).
-        >>> {
-        >>>     "id": 137594,
-        >>>     "dataset_id": 46,
-        >>>     "name": "dataset/46/frame_1563809032073.png",
-        >>>     "status": "reviewed",
-        >>>     "thumbnail": "https://...",
-        >>>     "data": "https://...",
-        >>>     "annotations": {
-        >>>         "classes": [],
-        >>>         "objects": []
-        >>>     }
-        >>> }
-
-        """
-        # load item details
-        try:
-            response = self.http.get(self.server_url + '/dataset-items/{}'.format(item_id))
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        item_details = json.loads(response.content)
-
-        return item_details
-
-    def delete_dataset_item(self, item_id):
-        """Delete a dataset item.
-
-        :param item_id: id of the dataset item
-        :return: 'True' if success else 'False'
-        """
-
-        try:
-            response = self.http.delete(f'{self.server_url}/dataset-items/{item_id}')
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return False
-
-    def download_dataset_item(self, item_id, image_dir: Optional[str] = None,
-                              metainformation_directory: Optional[str] = None,
-                              accepted_status=None, return_item: bool = False):
-        """Download a dataset item into the specified directories (image and metainformation).
-
-        :param item_id: ID of the dataset item to download.
-        :param image_dir: Output directory for the image.
-        :param metainformation_directory: Output directory for the metainformation.
-        :param accepted_status: List of accepted status. If the item status is not in this list, it will not be downloaded.
-        :return:
-        """
-        if image_dir is None and metainformation_directory is None and not return_item:
-            raise ValueError('arguments not correct')
-
-        # load item details
-        try:
-            response = self.http.get(self.server_url + '/dataset-items/{}'.format(item_id))
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        item_details = json.loads(response.content)
-        if accepted_status is not None:
-            if item_details['status'] not in accepted_status:
-                return None
-        image_url = item_details['data']
-
-        # download image
-        try:
-            response = self.s3_http.get(image_url, stream=True)
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        item_id = item_details['id']
-        dataset_id = item_details['dataset']
-        item_name = item_details['name'].split('/')[-1]
-        item_name = '{}_{}_{}'.format(dataset_id, item_id, item_name)
-
-        image_bytes: Optional[bytes] = response.content
-        if image_bytes is None:
-            image_bytes = bytes()
-            for chunk in response.iter_content(4096):
-                image_bytes += chunk
-
-        if image_dir:
-            try:
-                os.makedirs(image_dir)
-            except FileExistsError:
-                pass
-            image_file_path = os.path.join(image_dir, item_name)
-
-            with open(image_file_path, 'wb') as f:
-                f.write(image_bytes)
-
-        if metainformation_directory:
-            os.makedirs(metainformation_directory, exist_ok=True)
-
-            # write annotations to file
-            details = dict(item_details)
-
-            # remove unimportant clutter.
-            for key in ('data', 'thumbnail'):
-                if key in details:
-                    del details[key]
-
-            metainformation_file_name = os.path.splitext(item_name)[0] + '.json'
-            metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
-            with open(metainformation_path, 'w') as f:
-                json.dump(details, f, indent=2)
-
-        if return_item:
-            item_details['image'] = image_bytes
-            return item_details
-
-        return None
-
-    def add_dataset_items_to_subset(self, item_ids, subset_id):
-        """Add an existing dataset item to a subset.
-
-        :param item_ids: List of item IDs or a single item ID to be added
-        :param subset_id: ID of target subset
-        :return: 'True' if success, else 'False'
-        """
-        if not isinstance(item_ids, list):
-            if isinstance(item_ids, int):
-                item_ids = [item_ids]
-            else:
-                raise ValueError('Item IDs has to be a list of integers or an integer')
-
-        items = {
-            'items': item_ids
-        }
-
-        try:
-            response = self.http.post(f'{self.server_url}/data-subsets/{subset_id}/items/', json=items)
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return False
-
-    def remove_dataset_items_from_subset(self, item_ids, subset_id):
-        """Remove a dataset item from a subset.
-
-        :param item_ids: List of item IDs or a single item ID to be removed
-        :param subset_id: ID of target subset
-        :return: 'True' if success, else 'False'
-        """
-        if not isinstance(item_ids, list):
-            if isinstance(item_ids, int):
-                item_ids = [item_ids]
-            else:
-                raise ValueError('Item IDs has to be a list of integers or an integer')
-
-        items = {
-            'items': item_ids
-        }
-
-        try:
-            response = self.http.post(f'{self.server_url}/data-subsets/{subset_id}/remove_items/', json=items)
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return False
-
-    def get_model(self, model_id):
-        """Get information about a model.
-
-        Example:
-            >>> {
-            >>>     'id': 41,
-            >>>     'created_by': {'id': 1, 'username': 'admin'},
-            >>>     'worker_id': None,
-            >>>     'pretrained_checkpoint_id': None,
-            >>>     'name': 'SSD MobileNet V2 & MSF 300x300',
-            >>>     'created_date': '2019-07-01T10:02:15.856145Z',
-            >>>     'updated_date': '2019-07-29T13:19:32.190259Z',
-            >>>     'network_type': 'object_detection',
-            >>>     'status': 'open',
-            >>>     'progress': 0.0,
-            >>>     'model_data': None,
-            >>>     'inference_data': None,
-            >>>     'network_config_option': 1,
-            >>>     'datasets': [7]
-            >>> }
-
-        :param model_id: ID of the model to receive information.
-        :return: Dictionary containing information of the requested model.
-        """
-
-        try:
-            response = self.http.get(self.server_url + '/models/{}/'.format(model_id))
-            if response.status_code == 200:
-                model = response.json()
-                return model
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def get_model_class_labels(self, model_id):
-        """Get all class labels of a model.
-
-        Example:
-           >>> [
-           >>>     {
-           >>>         "class_label": { "id": 80, "name": "orange" },
-           >>>         "target_class_label": { "id": 80, "name": "orange" }
-           >>>     },
-           >>>     {
-           >>>         "class_label": { "id": 80, "name": "orange" },
-           >>>         "target_class_label": { "id": 79, "name": "fruit" }
-           >>>     }
-           >>> ]
-
-        :param model_id: ID of the model to receive the class labels.
-        :return: List of model class labels (see example) including the original class label and the target label. The
-                 target label is intended for remapping the label from the dataset to a new one for training. For
-                 example, you have created specific labels but you would like to combine multiple labels into one to
-                 train a more general model.
-        """
-
-        try:
-            response = self.http.get(f'{self.server_url}/models/{model_id}/class_labels/')
-            if response.status_code == 200:
-                model = response.json()
-                return model
-
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def get_model_parameters(self, model_id):
-        """Get the parameters of a model.
-
-        Example:
-            >>> {
-            >>>     'augmentation': {'horizontal_flip': {'probability': 0.5},
-            >>>                      'random_scale_crop': {'aspect_ratio_max': 2,
-            >>>                                            'aspect_ratio_min': 0.5,
-            >>>                                            'probability': 0.8,
-            >>>                                            'scaling_factor_max': 1,
-            >>>                                            'scaling_factor_min': 0.5}},
-            >>>     'dataset': {'input_height': 300, 'input_width': 300, 'training_split': 0.98},
-            >>>     'detection': {'anchors': {'parameters': [...], 'position_offset': False},
-            >>>                   'matching': {'threshold': 0.5},
-            >>>                   'network': 'mobilenet_v2_msf'},
-            >>>     'evaluation': {'interval': 500},
-            >>>     'learning_rate': {'initial': 0.001, 'selection': 'constant'},
-            >>>     'optimizer': {'amsgrad': False,
-            >>>                   'beta1': 0.9,
-            >>>                   'beta2': 0.999,
-            >>>                   'epsilon': 1e-08,
-            >>>                   'selection': 'adam',
-            >>>                   'weight_decay': 4e-05},
-            >>>     'training': {'batch_size': 96, 'checkpoints': {'interval': 100}}
-            >>> }
-
-        :param model_id: ID of the model to receive the parameters.
-        :return: Dictionary containing all model parameters.
-        """
-
-        try:
-            response = self.http.get(self.server_url + '/models/{}/parameters/'.format(model_id))
-            if response.status_code == 200:
-                model = response.json()
-                return model
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def get_model_checkpoints(self, model_id):
-        """Get information about all checkpoints of a model.
-
-        Example:
-            >>> [{'checkpoint_file': '...',
-            >>>  'created_date': '2019-07-22T23:02:19.362520Z',
-            >>>  'id': 5,
-            >>>  'iteration': 38700,
-            >>>  'network_model': 59,
-            >>>  'updated_date': '2019-07-27T13:24:42.951453Z'}]
-
-        :param model_id: ID of the model to receive the checkpoints.
-        :return: List with checkpoints.
-        """
-        try:
-            response = self.http.get(self.server_url + '/models/{}/checkpoints/'.format(model_id))
-            if response.status_code == 200:
-                checkpoints = response.json()
-                return checkpoints
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return []
-
-    def get_cloud_deployment(self, id):
-        """Get information about a cloud deployment.
-
-        Example:
-            >>> {
-            >>>     'id': 1,
-            >>>     'name': 'Deployment Example',
-            >>>     'last_online': '2019-12-12T14:00:00Z',
-            >>>     'created_date': '2019-12-12T13:30:00.00Z',
-            >>>     'updated_date': '2019-12-12T13:30:00.00Z',
-            >>>     'parameters': {},
-            >>>     'network_model': 123
-            >>> }
-
-        :param id: ID of the cloud deployment to receive information.
-        :return: Dictionary containing information of the requested cloud deployment.
-        """
-
-        try:
-            response = self.http.get(self.server_url + '/cloud-deployments/{}/'.format(id))
-            if response.status_code == 200:
-                return response.json()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def download_latest_model_checkpoint(self, model_id, output_file_path):
-        """Download the latest checkpoint of the given model and write it to the given `output_file_path`.
-
-        :param model_id: ID of the model whose latest checkpoint is download.
-        :param output_file_path: Output file path (no directory!).
-        :return: Information about the latest checkpoint or `None` if no checkpoint is available or an error occurred.
-        """
-        checkpoints = self.get_model_checkpoints(model_id)
-
-        if len(checkpoints) == 0:
-            return None
-
-        latest_checkpoint = checkpoints[-1]
-        if latest_checkpoint['checkpoint_file'] is None:
-            return None
-
-        try:
-            response = self.s3_http.get(latest_checkpoint['checkpoint_file'], stream=True)
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        with open(output_file_path, 'wb') as f:
-            for chunk in response.iter_content(4096):
-                f.write(chunk)
-        return latest_checkpoint
-
-    def download_model_checkpoint(self, checkpoint_id, output_file_path):
-        """Download a model checkpoint given by the checkpoint ID.
-
-        :param checkpoint_id: ID of the checkpoint to download.
-        :param output_file_path:  Output file path (no directory!).
-        :return: Information about the downloaded checkpoint or `None` if no checkpoint is available or an error occurred.
-        """
-        logger.info('Download model checkpoint with ID: {}'.format(checkpoint_id))
-
-        try:
-            response = self.http.get(self.server_url + '/model-checkpoints/' + str(checkpoint_id))
-            response.raise_for_status()
-            checkpoint = response.json()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        if checkpoint is None:
-            return None
-
-        try:
-            response = self.s3_http.get(checkpoint['checkpoint_file'], stream=True)
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return None
-
-        with open(output_file_path, 'wb') as f:
-            for chunk in response.iter_content(4096):
-                f.write(chunk)
-
-        logger.info('Downloaded model checkpoint with ID: {} to: {}'.format(checkpoint_id, output_file_path))
-
-        return checkpoint
-
-    def create_model_checkpoint(self, model_id, iteration):
-        """Create a new checkpoint for a model without uploading the checkpoint file.
-
-        :param model_id: ID of the model for which a checkpoint is created.
-        :param iteration: Training iteration of the checkpoint.
-        :return: Newly created checkpoint or `None` in case it could not be created.
-        """
-        model_checkpoint = {
-            'network_model': model_id,
-            'iteration': iteration
-        }
-
-        try:
-            response = self.http.post(self.server_url + '/model-checkpoints/', data=model_checkpoint)
-            response.raise_for_status()
-            return response.json()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def upload_model_checkpoint(self, checkpoint_id, iteration, file_path):
-        """Upload a model checkpoint.
-
-        :param checkpoint_id: ID of the checkpoint to which the files are uploaded.
-        :param iteration: Training iteration of the checkpoint.
-        :param file_path: File path to the checkpoint file.
-        :return: Updated checkpoint information or `None` in case of errors.
-        """
-
-        file_name = os.path.split(file_path)[-1]
-        files = {
-            'checkpoint_file': (file_name, open(file_path, 'rb'))
-        }
-        model_checkpoint = {
-            'iteration': iteration
-        }
-
-        try:
-            response = self.http.patch(self.server_url + '/model-checkpoints/{}/'.format(checkpoint_id),
-                                       data=model_checkpoint, files=files)
-            response.raise_for_status()
-            logger.info('Model checkpoint uploaded: {}'.format(file_name))
-            return response.json()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def upload_latest_model_checkpoint_async(self, model_id, iteration, file_path):
-        """Asynchronous update of the latest model checkpoint (largest iteration) including uploading a new checkpoint file.
-
-        :param model_id: ID of the model for which the latest checkpoint is updated.
-        :param iteration: Training iteration of the checkpoint.
-        :param file_path: File path to the checkpoint file.
-        """
-        threading.Thread(target=self.upload_latest_model_checkpoint, args=(model_id, iteration, file_path)).start()
-
-    def upload_latest_model_checkpoint(self, model_id, iteration, file_path):
-        """Update of the latest model checkpoint (largest iteration) including uploading a new checkpoint file.
-
-        :param model_id: ID of the model for which the latest checkpoint is updated.
-        :param iteration: Training iteration of the checkpoint.
-        :param file_path: File path to the checkpoint file.
-        :return: Updated checkpoint information or `None` in case of errors.
-        """
-        checkpoints = self.get_model_checkpoints(model_id)
-
-        if len(checkpoints) == 0:
-            checkpoint = self.create_model_checkpoint(model_id, iteration)
-        else:
-            checkpoint = checkpoints[-1]
-
-        if checkpoint is None:
-            return None
-
-        return self.upload_model_checkpoint(checkpoint['id'], iteration, file_path)
-
-    def upload_inference_data_async(self, model_id, file_path):
-        """Asynchronous upload of the inference data for the model given by its ID.
-
-        :param model_id: ID of the model for which the latest checkpoint is updated.
-        :param file_path: File path to the inference data file.
-        """
-        threading.Thread(target=self.upload_inference_data, args=(model_id, file_path)).start()
-
-    def upload_inference_data(self, model_id, file_path):
-        # TODO: FIXME: "upload_infernece_data" is confusion. this endpoint uploads the model (onnx) and accompanying files
-        # maybe rename to "upload_model_data" or something ? -> openAPI says "partial_update_network_model"
-        """Upload the inference data for the model given by its ID.
-
-        :param model_id: ID of the model for which the inference data is updated.
-        :param file_path: File path to the inference data file.
-        :return: Updated model information or `None` in case of errors.
-        """
-
-        file_name = os.path.split(file_path)[-1]
-        files = {'inference_data': (file_name, open(file_path, 'rb'))}
-
-        try:
-            response = self.http.patch(self.server_url + '/models/{}/'.format(model_id), files=files)
-            response.raise_for_status()
-            return True
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return False
-
-    def upload_model_statistics_async(self, statistics, timestamp, iteration, model_id):
-        """Asynchronous upload of model statistics (e.g., during training and evaluation) for a given model.
-
-        :param statistics: Dictionary of model statistics that must be serializable as JSON.
-        :param timestamp: Creation timestamp of the statistics.
-        :param iteration: Iteration of the statistics.
-        :param model_id: ID of the model the statistics belong to.
-        """
-        threading.Thread(target=self.upload_model_statistics, args=(statistics, timestamp, iteration, model_id)).start()
-
-    def upload_model_statistics(self, statistics, timestamp, iteration, model_id):
-        """Asynchronous upload of model statistics (e.g., during training and evaluation) for a given model.
-
-        :param statistics: Dictionary of model statistics that must be serializable as JSON.
-        :param timestamp: Creation timestamp of the statistics.
-        :param iteration: Iteration of the statistics.
-        :param model_id: ID of the model the statistics belong to.
-        """
-
-        logger.info('Upload model statistics')
-
-        statistics_entry = {
-            "timestamp": timestamp,
-            "iteration": iteration,
-            "statistics": json.dumps(statistics),
-            "network_model": model_id
-        }
-
-        try:
-            response = self.http.post(self.server_url + '/model-statistics/', data=statistics_entry)
-            response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            return
-
-        logger.info('Uploaded model statistics')
-
-    def get_inference_results_by_dataset_item_id(self, dataset_id: Optional[int] = None,
-                                                 iteration: Optional[int] = None,
-                                                 network_model_id: Optional[int] = None,
-                                                 max_items: Optional[int] = None,
-                                                 page_size: int = 100, **kwargs: Any) -> Dict[int, Dict[str, Any]]:
-
-        inference_results: List[Dict[str, Any]] = self.get_inference_results(
-            dataset_id=dataset_id, iteration=iteration, network_model_id=network_model_id,
-            max_items=max_items, page_size=page_size, **kwargs)
-
-        return {ir['dataset_item']['id']: ir for ir in inference_results}
-
-    def get_inference_results(self, dataset_id: Optional[int] = None, iteration: Optional[int] = None,
-                              network_model_id: Optional[int] = None, max_items: Optional[int] = None,
-                              page_size: int = 100, **kwargs: Any) -> List[Dict[str, Any]]:
-
-        url: str = f'{self.server_url}/inference-results/'
-        params: Dict[str, Any] = {'page_size': page_size}
-
-        if dataset_id is not None:
-            params['dataset_item__dataset__id'] = dataset_id
-
-        if iteration is not None:
-            params['iteration'] = iteration
-
-        if iteration is not None:
-            params['network_model_id'] = network_model_id
-
-        params.update(kwargs)
-
-        all_inference_results: List[Dict[str, Any]] = list()
-        while url is not None:
-
-            logger.debug(f'Get dataset items from "{url}"')
-            response: rq.models.Response = self.http.get(url, params=params)
-            response.raise_for_status()
-            response_json = response.json()
-
-            inference_results: Optional[List[Dict]] = response_json.get('results')
-            url = response_json.get('next')
-            params = None
-
-            if not inference_results:
-                break
-
-            all_inference_results.extend(inference_results)
-
-            if max_items is not None and len(all_inference_results) >= max_items:
-                break
-
-        return all_inference_results
-
-    def upload_inference_results_async(self, results, timestamp, iteration, model_id):
-        """Asynchronous upload of inference results (e.g., during evaluation) for a given model.
-
-        :param results: List of results. See :func:`~platform_sdk.Client.upload_inference_results` for details.
-        :param timestamp: Creation timestamp of the inference results.
-        :param iteration: Iteration of the inference results.
-        :param model_id: ID of the model the inference results belong to.
-        """
-        threading.Thread(target=self.upload_inference_results,
-                         args=(results, timestamp, iteration, model_id)).start()
-
-    def upload_inference_results(self, results, timestamp, iteration, model_id, *args):
-        """Upload of inference results (e.g., during evaluation) for a given model.
-
-        :param results: List of results.
-
-        Example:
-        >>> [
-        >>>     {
-        >>>         'dataset_item': 42,             # ID of the dataset item the result belongs to
-        >>>         'classification': {
-        >>>             'classes': [],              # list of platform class IDs (for classification)
-        >>>             'class_confidences': [...]  # list containing class confidences (ordered according to 'classes')
-        >>>         },
-        >>>         'detection': {
-        >>>             'boxes': [...]              # list of arrays representing the box coordinates and positions [x, y, width, height, orientation (optional)]
-        >>>                                         # x, y, width, and height must be scaled to the interval [0, 1] (the point (1, 1) corresponds to the lower right corner)
-        >>>             'classes': [...]            # list of platform class IDs (for detection)
-        >>>             'class_confidences': [...]  # 2-dimensional array containing class confidences (ordered according to 'classes') for each box
-        >>>         }
-        >>>     }
-        >>> ]
-
-        :param timestamp: Creation timestamp of the inference results.
-        :param iteration: Iteration of the inference results.
-        :param model_id: ID of the model the inference results belong to.
-        """
-
-        logger.info('Upload inference results')
-
-        msg_bytes = io.BytesIO()
-
-        # add meta data
-        msg_bytes.write(msgpack.packb(dict(timestamp=timestamp,
-                                           iteration=iteration,
-                                           model_id=model_id,
-                                           results=len(results))))
-
-        for i, result in enumerate(results):
-            msg_bytes.write(msgpack.packb(result))
-
-        response = self.http.post(f'{self.server_url}/bulk-data/',
-                                  data=dict(data_type=0),
-                                  files=dict(
-                                      data=(f'inference-data-{timestamp}-{model_id}.msgpack', msg_bytes.getvalue())))
-        response.raise_for_status()
-
-    def get_class_labels(self):
-        """Get a list of all available class labels of the platform sorted by name.
-
-        Example:
-        >>> [{'id': 37, 'name': 'airplane'},
-        >>>  {'id': 78, 'name': 'apple'},
-        >>>  {'id': 56, 'name': 'backpack'},
-        >>>  {'id': 77, 'name': 'banana'},
-        >>>  ...
-        >>> ]
-
-        :return: List of class labels or `None` in case of errors.
-        """
-        try:
-            response = self.http.get(self.server_url + '/class-labels/')
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def create_class_label(self, name, public=False):
-        """Create a new class label.
-
-        :param name: Name of the new class label.
-        :param public: Indicates if the label shall be globally accessible (by all users).
-        :return: Newly created class label or `None` in case of errors.
-        """
-
-        class_label = {'name': name, 'public': False}
-
-        try:
-            response = self.http.post(self.server_url + '/class-labels/', data=class_label)
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def get_jobs(self, worker_id):
-        """Get list of jobs for a particular worker.
-
-        :param worker_id: Jobs of this worker are returned.
-        :return: List of jobs or None.
-        """
-
-        try:
-            response = self.http.get(self.server_url + '/workers/{}/jobs/'.format(worker_id))
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def get_job(self, job_id):
-        """Get job details given its ID.
-
-        :param job_id: Job details.
-        :return: Job information or None.
-        """
-
-        try:
-            response = self.http.get(self.server_url + '/jobs/{}/'.format(job_id))
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def update_job(self, job):
-        """Update the job.
-
-        :param job: Fields to update. Must include the job ID.
-        :return: Job information or None.
-        """
-
-        job_id = job.get('id')
-        if job_id is None:
-            return None
-
-        try:
-            response = self.http.patch(self.server_url + '/jobs/{}/'.format(job_id), data=job)
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-        return None
-
-    def delete_job(self, job_id):
-        """Delete a specific job.
-
-        :param job_id: ID of the job that is to be removed.
-        """
-
-        try:
-            response = self.http.delete(self.server_url + '/jobs/{}/'.format(job_id))
-            if response.status_code == 404:
-                logger.info('Job could not be deleted because it did not exist.')
-            else:
-                response.raise_for_status()
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-
-    def create_labels_and_dataset(self, dataset_name, classification_class_labels=None,
-                                  object_detection_class_labels=None):
-        """Create a new dataset with all given class labels as detection class labels.
-
-        A new dataset is created and those class labels that do not exist yet are automatically created as well.
-
-        :param dataset_name: Name of the new dataset.
-        :param object_detection_class_labels: List of strings of the object detection class labels for the new dataset.
-        :return: ID of the newly created dataset or status code (see :func:`~platform_sdk.Client.create_dataset` for details).
-        """
-
-        # load list of all available class labels
-        all_class_labels = self.get_class_labels()
-
-        if all_class_labels is None:
-            logger.error('Could not retrieve available class labels')
-            return -1
-
-        # dictionary containing mapping from class names to class label ids
-        class_label_maps = {
-            'classification': None,
-            'object_detection': None
-        }
-
-        task_class_label_map = {}
-        if classification_class_labels is not None:
-            task_class_label_map['classification'] = classification_class_labels
-
-        if object_detection_class_labels is not None:
-            task_class_label_map['object_detection'] = object_detection_class_labels
-
-        for task in task_class_label_map:
-
-            class_label_names = task_class_label_map[task]
-            class_label_map = {}
-
-            # contains class names that do not yet exist on the platform
-            new_class_labels = []
-
-            # compare class labels of the dataset with existing class labels
-            for class_label in class_label_names:
-                is_new = True
-                for cl in all_class_labels:
-                    if class_label == cl['name']:
-                        is_new = False
-                        class_label_map[class_label] = cl['id']
-                        break
-
-                if is_new:
-                    new_class_labels.append(class_label)
-
-            # create new class labels
-            for new_class_label in new_class_labels:
-                id = self.create_class_label(new_class_label)
-                if id is None:
-                    logger.error('Could not create new class label ({}).'.format(new_class_label))
-                    return -1
-                class_label_map[new_class_label] = id
-
-            class_label_maps[task] = class_label_map.values()
-
-        logger.debug('Create new dataset')
-        return self.create_dataset(dataset_name,
-                                   classification_class_label_ids=class_label_maps['classification'],
-                                   object_detection_class_label_ids=class_label_maps['object_detection'])
-
-    def get_detection_class_label_map(self, dataset_id):
-        """Retrieve a dictionary that maps class label names to their IDs.
-
-        Example:
-        >>> {'car': 4,
-        >>>     'cyclist': 9,
-        >>>     'motorcycle': 36,
-        >>>     'pedestrian': 7,
-        >>>     'traffic light': 41,
-        >>>     'traffic sign': 119,
-        >>>     'truck': 6
-        >>> }
-
-        :param dataset_id: The mapping is loaded for class labels of this dataset.
-        :return: Class label map or `None` in case of errors.
-        """
-
-        dataset = self.get_dataset(dataset_id)
-
-        if dataset is None:
-            logger.error('Could not get dataset with ID {} for retrieving class labels'.format(dataset_id))
-            return None
-
-        class_labels = dataset['object_detection_class_labels']
-        class_label_map = {}
-        for class_label in class_labels:
-            class_label_map[class_label['name']] = class_label['id']
-        return class_label_map
-
-    def get_classification_class_label_map(self, dataset_id):
-        """Retrieve a dictionary that maps class label names to their IDs.
-
-        Example:
-        >>> {'car': 4,
-        >>>     'cyclist': 9,
-        >>>     'motorcycle': 36,
-        >>>     'pedestrian': 7,
-        >>>     'traffic light': 41,
-        >>>     'traffic sign': 119,
-        >>>     'truck': 6
-        >>> }
-
-        :param dataset_id: The mapping is loaded for class labels of this dataset.
-        :return: Class label map or `None` in case of errors.
-        """
-
-        dataset = self.get_dataset(dataset_id)
-
-        if dataset is None:
-            logger.error('Could not get dataset with ID {} for retrieving class labels'.format(dataset_id))
-            return None
-
-        class_labels = dataset['classification_class_labels']
-        class_label_map = {}
-        for class_label in class_labels:
-            class_label_map[class_label['name']] = class_label['id']
-        return class_label_map
-
-    def create_worker(self, name):
-        """Create a new training worker.
-
-        :return: ID of the newly created worker or `None`.
-        """
-
-        try:
-            worker = {
-                'name': name,
-                'status': '',
-                'details': {}
-            }
-            response = self.http.post(self.server_url + '/workers/', data=worker)
-            response.raise_for_status()
-            data = response.json()
-            return data
-        except rq.exceptions.RequestException as e:
-            logger.error(e)
-            raise e
-
-    def import_dataspree(self, dataset_name, dataset_id, images, annotations):
-        """Import a dataset that is available in the dataspree format.
-
-        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
-        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
-        :param images: Directory containing all images.
-        :param annotations: Directory containing the annotations.
-        :return: Status code. 0: import completed, -1: error
-        """
-        logger.info('Import dataspree data')
-
-        # create new dataset if no id is given
-        if dataset_id == -1:
-            # iterate over all items and determine used class labels (only for object detection for now)
-            logger.debug('Retrieve used class labels')
-            class_label_ids = set()
-            annotation_files = os.listdir(annotations)
-            for annotation_file in annotation_files:
-                with open(os.path.join(annotations, annotation_file), 'r') as f:
-                    annotation = json.load(f)
-                    for o in annotation['objects']:
-                        class_label_ids.add(o['label'])
-
-            logger.debug('Create new dataset')
-            dataset_id = self.create_dataset(dataset_name, object_detection_class_label_ids=class_label_ids)
-        else:
-            dataset = self.get_dataset(dataset_id)
-            if dataset is None:
-                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
-                return -1
-
-        if dataset_id == -1:
-            logger.error('Dataset ID not provided and could not create new dataset.')
-            return -1
-
-        dataset_items = self.get_dataset_items(dataset_id)
-        dataset_item_names = []
-
-        for item in dataset_items:
-            dataset_item_name = item['name'].split('/')[-1]
-            dataset_item_names.append(dataset_item_name)
-
-        # upload dataset items
-        annotation_files = os.listdir(annotations)
-        annotation_files.sort()
-
-        image_files = os.listdir(images)
-        image_files.sort()
-
-        logger.info('Upload dataset items')
-        for image_file in tqdm(image_files):
-
-            # do not upload in case the dataset item exits already
-            if image_file in dataset_item_names:
-                continue
-
-            base_name, image_extension = os.path.splitext(image_file)
-            annotation_file = '{}.{}'.format(base_name, 'json')
-
-            image_file_path = os.path.join(images, image_file)
-            base_name_split = base_name.split('_')
-
-            # first two elements of base_name_split contain dataset_id and item_id
-            image_file_name = '{}{}'.format('_'.join(base_name_split[2:]), image_extension)
-
-            annotation = {}
-            # load annotations if they exist
-            if annotation_file in annotation_files:
-                annotation_files.remove(annotation_file)
-
-                with open(os.path.join(annotations, annotation_file), 'r') as f:
-                    annotation = json.load(f)
-
-            if self.create_dataset_item(image_file_path, dataset_id, annotation, image_file_name) == -1:
-                logger.error('Error during creation of dataset item.')
-                return -1
-
-        return 0
-
-    def import_classification_directories(self, dataset_name, dataset_id, directory):
-        """Import a dataset for classification where each subfolder represents a class. The folder names need to match the class names that are available in the DLSD platform.
-
-                :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
-                :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
-                :param directory: Directory containing image subfolders.
-                :return: Status code. 0: import completed, -1: error
-                """
-        logger.info('Import classification directories')
-
-        subfolders = os.listdir(directory)
-
-        # create new dataset if no id is given
-        if dataset_id == -1:
-            # iterate over all items and determine used class labels
-            logger.debug('Retrieve used class labels')
-            class_labels = set()
-            for subfolder in subfolders:
-                class_labels.add(subfolder.lower())
-
-            dataset_id = self.create_labels_and_dataset(dataset_name, classification_class_labels=class_labels)
-        else:
-            dataset = self.get_dataset(dataset_id)
-            if dataset is None:
-                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
-                return -1
-
-        if dataset_id == -1:
-            logger.error('Dataset ID not provided and could not create new dataset.')
-            return -1
-
-        class_label_map = self.get_classification_class_label_map(dataset_id)
-
-        dataset_items = self.get_dataset_items(dataset_id)
-        dataset_item_names = []
-
-        for item in dataset_items:
-            dataset_item_name = item['name'].split('/')[-1]
-            dataset_item_names.append(dataset_item_name)
-
-        logger.info('Upload dataset items')
-        # upload dataset items
-        for subfolder in subfolders:
-            class_label_name = subfolder.lower()
-            logger.info('Import {}'.format(class_label_name))
-
-            image_files = os.listdir(os.path.join(directory, subfolder))
-
-            class_annotation = {
-                'classes': [class_label_map[class_label_name]]
-            }
-
-            for image_file in tqdm(image_files):
-
-                # do not upload in case the dataset item exits already
-                if image_file in dataset_item_names:
-                    continue
-
-                image_file_path = os.path.join(directory, subfolder, image_file)
-
-                if self.create_dataset_item(image_file_path, dataset_id, class_annotation) == -1:
-                    logger.error('Error during creation of dataset item.')
-                    return -1
-
-        return 0
-
-    def import_kitti(self, dataset_name, dataset_id, images, annotations):
-        """Import a dataset that is available in the KITTI format [1].
-
-        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
-        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
-        :param images: Directory containing all images.
-        :param annotations: Directory containing the annotations.
-        :return: Status code. 0: import completed, -1: error
-
-        [1] Geiger et al., "Are we ready for Autonomous Driving? The KITTI Vision Benchmark Suite", 2012.
-            http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=2d
-        """
-        logger.info('Import KITTI data')
-
-        # we import Pillow here as it is not required for other endpoints
-        from PIL import Image
-
-        # create new dataset if no id is given
-        if dataset_id == -1:
-            # iterate over all items and determine used class labels
-            logger.debug('Retrieve used class labels')
-            class_labels = set()
-            annotation_files = os.listdir(annotations)
-            for annotation_file in annotation_files:
-                with open(os.path.join(annotations, annotation_file), 'r') as f:
-                    file_content = f.readlines()
-                    for line in file_content:
-                        class_label = line.split(' ')[0].lower()
-                        # skip all objects with label 'dontcare'
-                        if class_label == 'dontcare' or class_label == 'misc':
-                            continue
-                        class_labels.add(class_label.lower())
-
-            dataset_id = self.create_labels_and_dataset(dataset_name, object_detection_class_labels=class_labels)
-        else:
-            dataset = self.get_dataset(dataset_id)
-            if dataset is None:
-                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
-                return -1
-
-        if dataset_id == -1:
-            logger.error('Dataset ID not provided and could not create new dataset.')
-            return -1
-
-        class_label_map = self.get_detection_class_label_map(dataset_id)
-
-        dataset_items = self.get_dataset_items(dataset_id)
-        dataset_item_names = []
-
-        for item in dataset_items:
-            dataset_item_name = item['name'].split('/')[-1]
-            dataset_item_names.append(dataset_item_name)
-
-        def convert_kitti_annotation(image_width, image_height, file_content):
-            normalizer = max(image_width, image_height)
-            objects = []
-
-            for i, line in enumerate(file_content):
-                attributes = line.split(' ')
-
-                class_label = attributes[0].lower()
-                # skip all objects with label 'dontcare'
-                if class_label == 'dontcare' or class_label == 'misc':
-                    continue
-
-                class_label_id = class_label_map[class_label]
-
-                left_x = float(attributes[4])
-                top_y = float(attributes[5])
-                right_x = float(attributes[6])
-                bottom_y = float(attributes[7])
-
-                x = ((left_x + right_x) / 2.0) / normalizer
-                y = ((top_y + bottom_y) / 2.0) / normalizer
-                w = (right_x - left_x) / normalizer
-                h = (bottom_y - top_y) / normalizer
-
-                o = {
-                    'id': i,
-                    'label': class_label_id,
-                    'x': x,
-                    'y': y,
-                    'width': w,
-                    'height': h,
-                    'orientation': 0
-                }
-
-                objects.append(o)
-
-            return objects
-
-        # upload dataset items
-        annotation_files = os.listdir(annotations)
-        image_files = os.listdir(images)
-
-        logger.info('Upload dataset items')
-        for image_file in tqdm(image_files):
-
-            # do not upload in case the dataset item exits already
-            if image_file in dataset_item_names:
-                continue
-
-            base_name = os.path.splitext(image_file)[0]
-            annotation_file = '{}.{}'.format(base_name, 'txt')
-
-            # only upload if image and annotation exists
-            if annotation_file in annotation_files:
-                annotation_files.remove(annotation_file)
-                image_file_path = os.path.join(images, image_file)
-
-                # We need to open the image to retrieve its width and height
-                # Image.open is a lazy operation - hence, the complete image
-                # data is not read immediately.
-                image = Image.open(image_file_path)
-                image_width, image_height = image.size
-
-                with open(os.path.join(annotations, annotation_file), 'r') as f:
-                    objects = convert_kitti_annotation(image_width, image_height, f.readlines())
-                    annotation = {
-                        'objects': objects
-                    }
-
-                if self.create_dataset_item(image_file_path, dataset_id, annotation) == -1:
-                    logger.error('Error during creation of dataset item.')
-                    return -1
-
-        return 0
-
-    def import_coco(self, dataset_name, dataset_id, images, annotations):
-        """Import a dataset that is available in the COCO format [1].
-
-        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
-        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
-        :param images: Directory containing all images.
-        :param annotations: Directory containing the annotations.
-        :return: Status code. 0: import completed, -1: error
-
-        [1] Lin et al., "Microsoft COCO: Common Objects in Context", 2014.
-            https://cocodataset.org/
-        """
-
-        logger.info('Import COCO data')
-
-        with open(annotations, 'r') as f:
-            coco = json.load(f)
-
-        coco_class_id_map = {}
-        for c in coco['categories']:
-            coco_class_id_map[c['id']] = c['name']
-
-        # create new dataset if no id is given
-        if dataset_id == -1:
-            # iterate over all items and determine used class labels
-            logger.debug('Retrieve used class labels')
-            dataset_id = self.create_labels_and_dataset(dataset_name,
-                                                        object_detection_class_labels=coco_class_id_map.values())
-            logger.info('Created dataset with ID {}.'.format(dataset_id))
-        else:
-            dataset = self.get_dataset(dataset_id)
-            if dataset is None:
-                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
-                return -1
-
-        if dataset_id == -1:
-            logger.error('Dataset ID not provided and could not create new dataset.')
-            return -1
-
-        class_label_map = self.get_detection_class_label_map(dataset_id)
-        dataset_items = self.get_dataset_items(dataset_id)
-        dataset_item_names = []
-
-        for item in dataset_items:
-            dataset_item_name = item['name'].split('/')[-1]
-            dataset_item_names.append(dataset_item_name)
-
-        # upload dataset items
-        logger.info('Upload dataset items')
-
-        coco_annotations = {}
-        coco_annotation_ids = {}
-        for a in coco['annotations']:
-            coco_annotations[a['id']] = a
-            image_id = a['image_id']
-            if image_id not in coco_annotation_ids:
-                coco_annotation_ids[image_id] = []
-            coco_annotation_ids[image_id].append(a['id'])
-
-        if self.parallel_requests > 1:
-            Parallel(n_jobs=self.parallel_requests, prefer='threads')(
-                delayed(self.upload_item_coco)(coco_image, images, coco_annotation_ids, coco_annotations,
-                                               coco_class_id_map,
-                                               class_label_map, dataset_id, dataset_item_names) for coco_image in
-                tqdm(coco['images']))
-        else:
-            for coco_image in tqdm(coco['images']):
-                self.upload_item_coco(coco_image, images, coco_annotation_ids, coco_annotations, coco_class_id_map,
-                                      class_label_map, dataset_id, dataset_item_names)
-
-        return 0
-
-    def upload_item_coco(self, coco_image, images, coco_annotation_ids, coco_annotations, coco_class_id_map,
-                         class_label_map, dataset_id, dataset_item_names):
-        image_id = coco_image['id']
-        image_file_name = coco_image['file_name']
-
-        # do not upload in case the dataset item exits already
-        if image_file_name in dataset_item_names:
-            return
-
-        image_file_path = os.path.join(images, image_file_name)
-        image_width = coco_image['width']
-        image_height = coco_image['height']
-        normalizer = max(image_width, image_height)
-
-        # get corresponding annotations
-        objects = []
-        if image_id not in coco_annotation_ids:
-            return
-        for i, cid in enumerate(coco_annotation_ids[image_id]):
-            a = coco_annotations[cid]
-
-            coco_class_id = a['category_id']
-            class_label_name = coco_class_id_map[coco_class_id]
-            class_label_id = class_label_map[class_label_name]
-            x = (a['bbox'][0] + 0.5 * a['bbox'][2]) / normalizer
-            y = (a['bbox'][1] + 0.5 * a['bbox'][3]) / normalizer
-            w = a['bbox'][2] / normalizer
-            h = a['bbox'][3] / normalizer
-            o = {
-                'id': i,
-                'label': class_label_id,
-                'x': x,
-                'y': y,
-                'width': w,
-                'height': h,
-                'orientation': 0
-            }
-            objects.append(o)
-
-        annotation = {
-            'objects': objects
-        }
-
-        if self.create_dataset_item(image_file_path, dataset_id, annotation) == -1:
-            logger.error('Error during creation of dataset item.')
-            return -1
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import io
+import json
+import logging
+import math
+import os
+import sys
+import threading
+import traceback
+import datetime
+from typing import Dict, Union, Optional, List, Tuple, Any
+
+import msgpack
+import requests as rq
+from joblib import Parallel, delayed
+from requests.adapters import HTTPAdapter
+from requests.auth import HTTPBasicAuth
+from tqdm import tqdm
+from urllib3 import Retry
+
+from .http_token_authentication import HTTPTokenAuth
+from .query import Condition, Conditions, Equal, GreaterThan, LessThan, Or
+
+logger = logging.getLogger(__name__)
+
+
+def value_or_env(value: Optional[str]):
+    if not value or value[:2] != '[[' or value[-2:] != ']]':
+        return value
+
+    return os.environ[value[2:-2]]
+
+
+class Client:
+    """Client for the Data Spree AI Platform.
+
+    The platform client forms the interface to the AI platform and provides a variety of functions. For instance, it is
+    possible download a whole dataset given its ID or create a new one and upload the corresponding dataset items.
+
+    :param username: Platform username. Required for authentication.
+    :param password: Platform password. Required for authentication.
+    :param auth_token: Platform authentication token.
+    :param http_retries: Number of HTTP retries before error is thrown.
+    :param parallel_requests: Maximum number of parallel HTTP request.
+    :param server_url: URL of the AI platform. Modify this parameter in case you use an on-premise installation.
+
+    """
+
+    def __init__(self, username: Optional[str] = None, password: Optional[str] = None, auth_token: Optional[str] = None,
+                 http_retries: int = 10, parallel_requests: int = 16,
+                 server_url: str = 'https://api.vision.data-spree.com/api', verify_ssl: bool = True,
+                 verify_s3_ssl: bool = True, proxy_servers: Optional[Dict[str, str]] = None):
+
+        self.username = username
+        self.password = password
+        self.auth_token = auth_token
+        self.proxy_servers = proxy_servers
+
+        self.auth = None
+        if auth_token:
+            self.auth = HTTPTokenAuth(auth_token)
+        elif username is not None and password is not None:
+            self.auth = HTTPBasicAuth(value_or_env(username), value_or_env(password))
+
+        if self.auth is None:
+            raise ValueError('Username and password or authentication token must be provided.')
+
+        self.http_retries = http_retries
+        self.server_url = server_url
+        self.parallel_requests = parallel_requests
+        if self.parallel_requests <= 0:
+            raise ValueError(f'Invalid parallel requests: {self.parallel_requests} must be greater than zero.')
+
+        self.http = rq.Session()
+        if not verify_ssl:
+            self.http.verify = False
+        self.s3_http = rq.Session()
+        if not verify_s3_ssl:
+            self.s3_http.verify = False
+        self.http.auth = self.auth
+        retry = Retry(total=http_retries, connect=1, backoff_factor=0.5,
+                      status_forcelist=[500, 502, 503, 504])
+        adapter = HTTPAdapter(pool_maxsize=self.parallel_requests, max_retries=retry)
+
+        if self.proxy_servers is not None:
+            self.http.proxies.update(proxy_servers)
+            self.s3_http.proxies.update(proxy_servers)
+
+        self.http.mount('http://', adapter)
+        self.http.mount('https://', adapter)
+
+    def __reduce__(self):
+        return (Client, (self.username,
+                         self.password,
+                         self.auth_token,
+                         self.http_retries,
+                         self.parallel_requests,
+                         self.server_url,
+                         self.http.verify,
+                         self.s3_http.verify,))
+
+    @staticmethod
+    def get_dataset_item_date_format_string() -> str:
+        return '%Y-%m-%dT%H:%M:%S.%fZ'
+
+    @staticmethod
+    def get_dataset_item_date_format_string_short() -> str:
+        return '%Y-%m-%dT%H:%M:%SZ'
+
+    @staticmethod
+    def parse_dataset_item_date(date_string: Optional[str]) -> Optional[datetime.datetime]:
+        if date_string is None:
+            return None
+
+        try:
+            return datetime.datetime.fromisoformat(date_string)
+        except (TypeError, ValueError, AttributeError):
+            pass
+
+        try:
+            return datetime.datetime.strptime(date_string, Client.get_dataset_item_date_format_string())
+        except (TypeError, ValueError, AttributeError):
+            pass
+
+        try:
+            return datetime.datetime.strptime(date_string, Client.get_dataset_item_date_format_string_short())
+        except (TypeError, ValueError, AttributeError):
+            pass
+
+        return None
+
+    @staticmethod
+    def dataspree_temp_dir(*sub_dirs: str) -> str:
+        temp_dir = os.path.join(Client.dataspree_dir(), 'temp', *sub_dirs)
+        os.makedirs(temp_dir, exist_ok=True)
+        return temp_dir
+
+    @staticmethod
+    def dataspree_dir():
+        base_dir = os.path.expanduser('~')
+        dir = os.path.join(base_dir, '.dataspree')
+        if sys.platform in ['win32', 'cygwin'] and os.getlogin() == 'SYSTEM':
+            # on windows in case the 'user' is SYSTEM, e.g. when started as a windows service
+            dir = os.path.join(os.getenv('ALLUSERSPROFILE'), 'Data Spree', 'AI Platform')
+        try:
+            os.makedirs(dir)
+        except FileExistsError:
+            pass
+        return dir
+
+    def check_connection(self):
+        response = self.http.get(f'{self.server_url}/auth/users/me/')
+        response.raise_for_status()
+        return response.json()
+
+    def server_status(self):
+        response = self.http.get(f'{self.server_url}/server')
+        response.raise_for_status()
+        return response.json()
+
+    def create_dataset(self,
+                       dataset_name,
+                       classification_class_label_ids=None,
+                       key_point_ids=None,
+                       roi_classification_class_label_ids=None,
+                       roi_key_point_ids=None,
+                       object_detection_class_label_ids=None,
+                       object_detection_key_point_ids=None,
+                       object_detection_masks=False,
+                       semantic_segmentation_class_label_ids=None):
+        """Create a new dataset.
+
+        :param dataset_name: Name of the new dataset.
+        :param classification_class_label_ids: IDs of the class labels for the classification of the whole image.
+        :param key_point_ids: IDs of the key points that can be annotated for the whole image.
+        :param roi_classification_class_label_ids: IDs of the class label for the classification of regions of interest.
+        :param roi_key_point_ids: IDs of the key points that can be annotated for each region of interest.
+        :param object_detection_class_label_ids: IDs of the class labels for object annotations.
+        :param object_detection_key_point_ids: IDs of the key points that can be annotated for individual objects.
+        :param object_detection_masks: Set to True if it should be possible to annotate individual objects with segmentation masks.
+        :param semantic_segmentation_class_label_ids: IDs of the class labels for annotating each pixel with a class label (semantic segmentation of the image).
+        :return: ID of the newly created dataset or -1 if dataset creation fails.
+        """
+
+        dataset = {
+            'name': dataset_name,
+            'classification': classification_class_label_ids is not None,
+            'key_points': key_point_ids is not None,
+            'roi_classification': roi_classification_class_label_ids is not None,
+            'roi_key_points': roi_key_point_ids is not None,
+            'object_detection': object_detection_class_label_ids is not None,
+            'object_detection_key_points': object_detection_key_point_ids is not None,
+            'object_detection_mask': object_detection_masks,
+            'semantic_segmentation': semantic_segmentation_class_label_ids is not None,
+        }
+
+        if dataset['classification']:
+            dataset['classification_class_label_ids'] = classification_class_label_ids
+
+        if dataset['key_points']:
+            dataset['key_point_ids'] = key_point_ids
+
+        if dataset['roi_classification']:
+            dataset['roi_classification_class_label_ids'] = roi_classification_class_label_ids
+
+        if dataset['roi_key_points']:
+            dataset['roi_key_point_ids'] = roi_key_point_ids
+
+        if dataset['object_detection']:
+            dataset['object_detection_class_label_ids'] = object_detection_class_label_ids,
+
+        if dataset['object_detection_key_points']:
+            dataset['object_detection_key_point_ids'] = object_detection_key_point_ids
+
+        if dataset['semantic_segmentation']:
+            dataset['semantic_segmentation_class_label_ids'] = semantic_segmentation_class_label_ids
+
+        try:
+            response = self.http.post(self.server_url + '/datasets/', data=dataset)
+            response.raise_for_status()
+            data = response.json()
+            return data['id']
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return -1
+
+    def get_dataset(self, dataset_id: int):
+        """Get information about a dataset.
+
+        Example:
+            >>> {
+            >>>    'id': 46,
+            >>>    'total_items': 104,
+            >>>    'uploaded_items': 0,
+            >>>    'annotated_items': 0,
+            >>>    'reviewed_items': 104,
+            >>>    'ignored_items': 0,
+            >>>    'created_by': {'id': 1, 'username': 'admin'},
+            >>>    'name': 'Traffic II',
+            >>>    'created_date': '2019-07-29T10:06:22.454871Z',
+            >>>    'updated_date': '2019-07-29T10:06:22.454914Z',
+            >>>    'classification': False,
+            >>>    'key_points': False,
+            >>>    'roi_classification': False,
+            >>>    'roi_key_points': False,
+            >>>    'object_detection': True,
+            >>>    'object_detection_key_points': False,
+            >>>    'object_detection_mask': False,
+            >>>    'semantic_segmentation': False,
+            >>>    'classification_class_labels': [],
+            >>>    'key_point_names': [],
+            >>>    'roi_classification_class_labels': [],
+            >>>    'roi_key_points_names': [],
+            >>>    'object_detection_class_labels': [{'id': 4, 'name': 'car'},
+            >>>     {'id': 6, 'name': 'truck'},
+            >>>     {'id': 7, 'name': 'pedestrian'},
+            >>>     {'id': 9, 'name': 'cyclist'},
+            >>>     {'id': 41, 'name': 'traffic light'},
+            >>>     {'id': 119, 'name': 'traffic sign'}],
+            >>>    'object_detection_key_point_names': [],
+            >>>    'semantic_segmentation_class_labels': []
+            >>> }
+
+        :param dataset_id: ID of the dataset to receive information.
+        :return: Dictionary containing information of the requested datatset.
+        """
+        request: str = self.server_url + '/datasets/{}/'.format(dataset_id)
+        try:
+            response = self.http.get(request)
+            if response.status_code == 200:
+                dataset = response.json()
+                return dataset
+        except rq.exceptions.RequestException as e:
+            logger.error(f'An error occurred during GET request: {request}: {e}')
+
+        return None
+
+    def get_dataset_items_url(self, dataset_id: Optional[int] = None,
+                              class_id: Optional[int] = None,
+                              subset_id: Optional[Union[str, int]] = None,
+                              created_date_since: Optional[Union[str, datetime.datetime]] = None,
+                              created_date_until: Optional[Union[str, datetime.datetime]] = None,
+                              status: Optional[List[str]] = None,
+                              query_expression: Optional[Condition] = None,
+                              free_query_str: Optional[str] = None, *, return_query: bool = False,
+                              max_items: Optional[int] = None) -> str:
+        items_per_request: int = min(5000, max_items) if max_items is not None else 5000
+
+        def format_time(t: Optional[Union[str, datetime.datetime]]) -> Optional[str]:
+            return t if t is None or type(t) == str else t.isoformat()
+
+        # Compile conditions
+        condition_str: str = Conditions.create(Equal(var='class', val=class_id),
+                                               Equal(var='dataset__id', val=dataset_id),
+                                               Equal(var='page_size', val=items_per_request),
+                                               Equal(var='data_subsets__id', val=subset_id),
+                                               GreaterThan(var='created_date', val=format_time(created_date_since)),
+                                               LessThan(var='created_date', val=format_time(created_date_until)),
+                                               Or(*(Equal(var='status', val=s) for s in status)) if status else None,
+                                               query_expression, exclude_empty=True, do_url_escape=True)
+
+        if free_query_str:
+            if not free_query_str.startswith('&'):
+                free_query_str = f'&{free_query_str}'
+            condition_str += free_query_str
+
+        # Compile URL
+        return f'{self.server_url}/dataset-items/?{condition_str}'
+
+    def get_dataset_items(self, dataset_id: Optional[int] = None,
+                          class_id: Optional[int] = None,
+                          subset_id: Optional[Union[str, int]] = None,
+                          created_date_since: Optional[Union[str, datetime.datetime]] = None,
+                          created_date_until: Optional[Union[str, datetime.datetime]] = None,
+                          status: Optional[List[str]] = None,
+                          query_expression: Optional[Condition] = None,
+                          free_query_str: Optional[str] = None, *, return_query: bool = False,
+                          max_items: Optional[int] = None) \
+            -> Union[Optional[List[Dict]], Tuple[Optional[List[Dict]], str]]:
+        """
+        Return all dataset items that match the filter compiled from this functions' parameters.
+
+        :param dataset_id:          Identifier of the dataset whose content be downloaded.
+        :param subset_id:           Identifier of the subset whose content be downloaded or None if you don't want
+                                    to filter by subset. "null()" if you would like to receive every dataset item
+                                    that is not part of any subset.
+        :param class_id:            Set this to only download items of the specified class_id
+        :param created_date_since:  Set this to filter out dataset items created at created_date_since or earlier.
+        :param created_date_until:  Set this to filter out dataset items created at created_date_until or later.
+        :param status:              If not set, return the dataset items irrespective of their status.
+                                    Otherwise, add an OR filter to the query on the content of the status list.
+        :param query_expression:    Set this field to supply a custom query expression to the query.
+        :param free_query_str:      Set this field to supply a custom query expression as a string to the query.
+        :param return_query:        Return first query if enabled as second return argument
+        :param max_items:           Max number of items to be returned.
+        :return:                    A list of dataset items or None, if a problem occurred.
+        """
+        # Compile URL
+        url: Optional[str] = self.get_dataset_items_url(dataset_id=dataset_id, class_id=class_id, subset_id=subset_id,
+                                                        created_date_since=created_date_since,
+                                                        created_date_until=created_date_until, status=status,
+                                                        query_expression=query_expression,
+                                                        free_query_str=free_query_str, max_items=max_items)
+        first_url: str = url
+
+        all_items: List[Dict] = list()
+        while url is not None:
+
+            logger.debug(f'Get dataset items from "{url}"')
+            try:
+                response: rq.models.Response = self.http.get(url)
+                response.raise_for_status()
+                response_json = response.json()
+
+                items: Optional[List[Dict]] = response_json.get('results')
+                url = response_json.get('next')
+
+                if not items:
+                    break
+
+                all_items.extend(items)
+
+                if max_items is not None and len(all_items) >= max_items:
+                    break
+
+            except rq.exceptions.RequestException as e:
+                logger.error(f'An error occurred during GET request: {url}: {e}')
+
+                if return_query:
+                    return None, first_url
+                return None
+
+        if return_query:
+            return all_items, first_url
+        return all_items
+
+    def delete_dataset(self, dataset_id):
+        """Delete a dataset.
+
+        :param dataset_id: id of the dataset
+        :return: 'True' if success else 'False'
+        """
+
+        try:
+            request: str = f'{self.server_url}/datasets/{dataset_id}'
+            response = self.http.delete(request)
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(f'An error occurred during HTTP delete request: {request}: {e}')
+
+        return False
+
+    def download_dataset(self, directory, dataset_id, n_items=-1, accepted_status=None):
+        """Download a dataset from data spree vision platform.
+
+        :param directory:  Directory to download dataset items (images and annotations)
+        :param dataset_id: ID of the dataset that should be downloaded.
+        :param n_items: Maximum number of items to download. Set to -1 to download all items.
+        :param accepted_status: Download only items with the provided status (list of strings). Set to None to accept all status.
+        """
+
+        logger.info('Download dataset. Dataset ID: {}'.format(dataset_id))
+
+        # download list of dataset items
+        dataset_items = self.get_dataset_items(dataset_id)
+        if dataset_items is None:
+            logger.error('Could not get list of dataset items for dataset with ID {}'.format(dataset_id))
+
+        # create output directories
+        try:
+            os.makedirs(directory)
+        except FileExistsError:
+            pass
+        try:
+            os.makedirs(os.path.join(directory, 'images'))
+        except FileExistsError:
+            pass
+        image_dir = os.path.join(directory, 'images')
+        try:
+            os.makedirs(os.path.join(directory, 'annotations'))
+        except FileExistsError:
+            pass
+
+        annotation_dir = os.path.join(directory, 'annotations')
+
+        if n_items != -1:
+            dataset_items = dataset_items[:n_items]
+
+        # use only those dataset items from the list, that are not yet downloaded
+        new_dataset_items = []
+        for item in dataset_items:
+            image_name = item['name'].split('/')[-1]
+            image_name = '{}_{}_{}'.format(dataset_id, item['id'], image_name)
+            image_file_path = os.path.join(image_dir, image_name)
+
+            annotation_file_name = os.path.splitext(image_name)[0] + '.json'
+            annotation_file_path = os.path.join(annotation_dir, annotation_file_name)
+
+            if not os.path.exists(image_file_path) or not os.path.exists(annotation_file_path):
+                new_dataset_items.append(item)
+
+        logger.info(
+            '{} items available in dataset {}. {} already downloaded'.format(len(dataset_items), dataset_id,
+                                                                             len(dataset_items) - len(
+                                                                                 new_dataset_items)))
+
+        if len(new_dataset_items) != 0:
+            with open(os.path.join(directory, 'items.json'), 'w') as f:
+                json.dump(dataset_items, f, indent=2)
+
+            if self.parallel_requests > 1:
+                Parallel(n_jobs=self.parallel_requests, prefer='threads')(
+                    delayed(self.download_dataset_item)(item['id'], image_dir, annotation_dir, accepted_status)
+                    for item in tqdm(new_dataset_items))
+            else:
+                for item in tqdm(new_dataset_items):
+                    self.download_dataset_item(item['id'], image_dir, annotation_dir, accepted_status)
+
+        logger.info('Download completed. (dataset ID: {})'.format(dataset_id))
+
+    def create_data_subset(self, subset_name, dataset_id, description=''):
+        """Add a subset to an existing dataset.
+
+        :param subset_name: name of the subset
+        :param dataset_id: id of the parent dataset
+        :param description: string description
+        :return: newly created subset or 'None' if subset creation fails.
+        """
+
+        subset_dict = {
+            'name': subset_name,
+            'description': description,
+            'dataset': dataset_id,
+        }
+
+        try:
+            request: str = f'{self.server_url}/data-subsets/'
+            response = self.http.post(request, data=subset_dict)
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(f'An error occurred during HTTP post request: {request}: {e}')
+
+        return None
+
+    def get_data_subset(self, subset_id):
+        """Get information about a dataset.
+
+        Example:
+            >>> {
+            >>>    'id': 46,
+            >>>    'total_items': 104,
+            >>>    'name': 'Traffic II',
+            >>>    'description': str,
+            >>>    'dataset': 24,
+            >>> }
+
+        :param subset_id: ID of the subset to receive information.
+        :return: Dictionary containing information of the requested subset.
+        """
+        try:
+            request = self.server_url + '/data-subsets/{}/'.format(subset_id)
+            response = self.http.get(request)
+            if response.status_code == 200:
+                subset = response.json()
+                return subset
+        except rq.exceptions.RequestException as e:
+            logger.error(f'An error occurred during HTTP get request: {request}: {e}')
+
+        return None
+
+    def get_data_subset_items(self, subset_id) -> List[Dict]:
+        """
+        Get all subset items for the subset given by its ID.
+        :see get_dataset_items
+        """
+        return self.get_dataset_items(subset_id=subset_id)
+
+    def delete_data_subset(self, subset_id):
+        """Delete a subset to an existing dataset.
+
+        :param subset_id: id of the subset
+        :return: 'True' if success else 'False'
+        """
+
+        try:
+            request = f'{self.server_url}/data-subsets/{subset_id}'
+            response = self.http.delete(request)
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(f'An error occurred during HTTP delete request: {request}: {e}')
+
+        return False
+
+    def create_dataset_item(self,
+                            image_file,
+                            dataset_id,
+                            annotations=None,
+                            image_file_name=None,
+                            status=None,
+                            created_date=None):
+        """Create a new dataset item including the image and the associated annotations.
+
+        :param image_file: File path to the image or image bytes to upload that belongs to the new item.
+        :param dataset_id: The new item will be created for the provided dataset ID.
+        :param annotations: Dictionary of the annotations
+        :param image_file_name: Name of the image that should be uploaded. Set to `None` to use the file name derived from `image_file` if provided as a path, otherwise a name is required.
+        :param status: Status of the newly created item. Should be one of `['uploaded', 'annotated', 'reviewed', 'ignored']`. Set to `None` to automatically set to `reviewed` or `uploaded` in case the annotations are empty.
+        :param created_date: Creation date and time as datetime object or number (seconds, POSIX timestamp) of the dataset item (upload time is used if not provided).
+        :return: ID of the newly created item or `-1` in case it could not be created.
+        """
+
+        if annotations is None:
+            annotations = {}
+        if isinstance(image_file, bytes):
+            if not isinstance(image_file_name, str):
+                raise ValueError('If an image is passed in bytes form, an "image_file_name" (str) has to be provided.')
+            files = {
+                'data': (image_file_name, image_file)
+            }
+        else:
+            if image_file_name is None:
+                image_file_name = os.path.split(image_file)[-1]
+
+            files = {
+                'data': (image_file_name, open(image_file, 'rb'))
+            }
+
+        if status is None:
+            status = 'reviewed' if annotations else 'uploaded'
+
+        dataset_item = {
+            'dataset_id': dataset_id,
+            'annotations': json.dumps(annotations),
+            'status': status
+        }
+
+        if created_date is not None:
+            if type(created_date) in (int, float):
+                created_date_dt = datetime.datetime.fromtimestamp(created_date)
+            else:
+                created_date_dt = created_date
+
+            if type(created_date_dt) != datetime.datetime:
+                raise ValueError('"created_date" must be a datetime object or a number')
+
+            created_date_str = created_date_dt.isoformat()
+            dataset_item['created_date'] = created_date_str
+
+        try:
+            response = self.http.post(self.server_url + '/dataset-items/', data=dataset_item, files=files)
+            response.raise_for_status()
+            data = response.json()
+            return data['id']
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            traceback.print_exc()
+        except Exception as e:
+            logger.error(e)
+            traceback.print_exc()
+
+        return -1
+
+    def get_dataset_item(self, item_id):
+        """Get a dataset item given its ID.
+        :param item_id: ID of the item to be retrieved.
+        :return: Dictionary containing the item details (e.g., ID, name, status).
+        >>> {
+        >>>     "id": 137594,
+        >>>     "dataset_id": 46,
+        >>>     "name": "dataset/46/frame_1563809032073.png",
+        >>>     "status": "reviewed",
+        >>>     "thumbnail": "https://...",
+        >>>     "data": "https://...",
+        >>>     "annotations": {
+        >>>         "classes": [],
+        >>>         "objects": []
+        >>>     }
+        >>> }
+
+        """
+        # load item details
+        try:
+            response = self.http.get(self.server_url + '/dataset-items/{}'.format(item_id))
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        item_details = json.loads(response.content)
+
+        return item_details
+
+    def delete_dataset_item(self, item_id):
+        """Delete a dataset item.
+
+        :param item_id: id of the dataset item
+        :return: 'True' if success else 'False'
+        """
+
+        try:
+            response = self.http.delete(f'{self.server_url}/dataset-items/{item_id}')
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return False
+
+    def download_dataset_item(self, item_id, image_dir: Optional[str] = None,
+                              metainformation_directory: Optional[str] = None,
+                              accepted_status=None, return_item: bool = False):
+        """Download a dataset item into the specified directories (image and metainformation).
+
+        :param item_id: ID of the dataset item to download.
+        :param image_dir: Output directory for the image.
+        :param metainformation_directory: Output directory for the metainformation.
+        :param accepted_status: List of accepted status. If the item status is not in this list, it will not be downloaded.
+        :return:
+        """
+        if image_dir is None and metainformation_directory is None and not return_item:
+            raise ValueError('arguments not correct')
+
+        # load item details
+        try:
+            response = self.http.get(self.server_url + '/dataset-items/{}'.format(item_id))
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        item_details = json.loads(response.content)
+        if accepted_status is not None:
+            if item_details['status'] not in accepted_status:
+                return None
+        image_url = item_details['data']
+
+        # download image
+        try:
+            response = self.s3_http.get(image_url, stream=True)
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        item_id = item_details['id']
+        dataset_id = item_details['dataset']
+        item_name = item_details['name'].split('/')[-1]
+        item_name = '{}_{}_{}'.format(dataset_id, item_id, item_name)
+
+        image_bytes: Optional[bytes] = response.content
+        if image_bytes is None:
+            image_bytes = bytes()
+            for chunk in response.iter_content(4096):
+                image_bytes += chunk
+
+        if image_dir:
+            try:
+                os.makedirs(image_dir)
+            except FileExistsError:
+                pass
+            image_file_path = os.path.join(image_dir, item_name)
+
+            with open(image_file_path, 'wb') as f:
+                f.write(image_bytes)
+
+        if metainformation_directory:
+            os.makedirs(metainformation_directory, exist_ok=True)
+
+            # write annotations to file
+            details = dict(item_details)
+
+            # remove unimportant clutter.
+            for key in ('data', 'thumbnail'):
+                if key in details:
+                    del details[key]
+
+            metainformation_file_name = os.path.splitext(item_name)[0] + '.json'
+            metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
+            with open(metainformation_path, 'w') as f:
+                json.dump(details, f, indent=2)
+
+        if return_item:
+            item_details['image'] = image_bytes
+            return item_details
+
+        return None
+
+    def add_dataset_items_to_subset(self, item_ids, subset_id):
+        """Add an existing dataset item to a subset.
+
+        :param item_ids: List of item IDs or a single item ID to be added
+        :param subset_id: ID of target subset
+        :return: 'True' if success, else 'False'
+        """
+        if not isinstance(item_ids, list):
+            if isinstance(item_ids, int):
+                item_ids = [item_ids]
+            else:
+                raise ValueError('Item IDs has to be a list of integers or an integer')
+
+        items = {
+            'items': item_ids
+        }
+
+        try:
+            response = self.http.post(f'{self.server_url}/data-subsets/{subset_id}/items/', json=items)
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return False
+
+    def remove_dataset_items_from_subset(self, item_ids, subset_id):
+        """Remove a dataset item from a subset.
+
+        :param item_ids: List of item IDs or a single item ID to be removed
+        :param subset_id: ID of target subset
+        :return: 'True' if success, else 'False'
+        """
+        if not isinstance(item_ids, list):
+            if isinstance(item_ids, int):
+                item_ids = [item_ids]
+            else:
+                raise ValueError('Item IDs has to be a list of integers or an integer')
+
+        items = {
+            'items': item_ids
+        }
+
+        try:
+            response = self.http.post(f'{self.server_url}/data-subsets/{subset_id}/remove_items/', json=items)
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return False
+
+    def get_model(self, model_id):
+        """Get information about a model.
+
+        Example:
+            >>> {
+            >>>     'id': 41,
+            >>>     'created_by': {'id': 1, 'username': 'admin'},
+            >>>     'worker_id': None,
+            >>>     'pretrained_checkpoint_id': None,
+            >>>     'name': 'SSD MobileNet V2 & MSF 300x300',
+            >>>     'created_date': '2019-07-01T10:02:15.856145Z',
+            >>>     'updated_date': '2019-07-29T13:19:32.190259Z',
+            >>>     'network_type': 'object_detection',
+            >>>     'status': 'open',
+            >>>     'progress': 0.0,
+            >>>     'model_data': None,
+            >>>     'inference_data': None,
+            >>>     'network_config_option': 1,
+            >>>     'datasets': [7]
+            >>> }
+
+        :param model_id: ID of the model to receive information.
+        :return: Dictionary containing information of the requested model.
+        """
+
+        try:
+            response = self.http.get(self.server_url + '/models/{}/'.format(model_id))
+            if response.status_code == 200:
+                model = response.json()
+                return model
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def get_model_class_labels(self, model_id):
+        """Get all class labels of a model.
+
+        Example:
+           >>> [
+           >>>     {
+           >>>         "class_label": { "id": 80, "name": "orange" },
+           >>>         "target_class_label": { "id": 80, "name": "orange" }
+           >>>     },
+           >>>     {
+           >>>         "class_label": { "id": 80, "name": "orange" },
+           >>>         "target_class_label": { "id": 79, "name": "fruit" }
+           >>>     }
+           >>> ]
+
+        :param model_id: ID of the model to receive the class labels.
+        :return: List of model class labels (see example) including the original class label and the target label. The
+                 target label is intended for remapping the label from the dataset to a new one for training. For
+                 example, you have created specific labels but you would like to combine multiple labels into one to
+                 train a more general model.
+        """
+
+        try:
+            response = self.http.get(f'{self.server_url}/models/{model_id}/class_labels/')
+            if response.status_code == 200:
+                model = response.json()
+                return model
+
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def get_model_parameters(self, model_id):
+        """Get the parameters of a model.
+
+        Example:
+            >>> {
+            >>>     'augmentation': {'horizontal_flip': {'probability': 0.5},
+            >>>                      'random_scale_crop': {'aspect_ratio_max': 2,
+            >>>                                            'aspect_ratio_min': 0.5,
+            >>>                                            'probability': 0.8,
+            >>>                                            'scaling_factor_max': 1,
+            >>>                                            'scaling_factor_min': 0.5}},
+            >>>     'dataset': {'input_height': 300, 'input_width': 300, 'training_split': 0.98},
+            >>>     'detection': {'anchors': {'parameters': [...], 'position_offset': False},
+            >>>                   'matching': {'threshold': 0.5},
+            >>>                   'network': 'mobilenet_v2_msf'},
+            >>>     'evaluation': {'interval': 500},
+            >>>     'learning_rate': {'initial': 0.001, 'selection': 'constant'},
+            >>>     'optimizer': {'amsgrad': False,
+            >>>                   'beta1': 0.9,
+            >>>                   'beta2': 0.999,
+            >>>                   'epsilon': 1e-08,
+            >>>                   'selection': 'adam',
+            >>>                   'weight_decay': 4e-05},
+            >>>     'training': {'batch_size': 96, 'checkpoints': {'interval': 100}}
+            >>> }
+
+        :param model_id: ID of the model to receive the parameters.
+        :return: Dictionary containing all model parameters.
+        """
+
+        try:
+            response = self.http.get(self.server_url + '/models/{}/parameters/'.format(model_id))
+            if response.status_code == 200:
+                model = response.json()
+                return model
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def get_model_checkpoints(self, model_id):
+        """Get information about all checkpoints of a model.
+
+        Example:
+            >>> [{'checkpoint_file': '...',
+            >>>  'created_date': '2019-07-22T23:02:19.362520Z',
+            >>>  'id': 5,
+            >>>  'iteration': 38700,
+            >>>  'network_model': 59,
+            >>>  'updated_date': '2019-07-27T13:24:42.951453Z'}]
+
+        :param model_id: ID of the model to receive the checkpoints.
+        :return: List with checkpoints.
+        """
+        try:
+            response = self.http.get(self.server_url + '/models/{}/checkpoints/'.format(model_id))
+            if response.status_code == 200:
+                checkpoints = response.json()
+                return checkpoints
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return []
+
+    def get_cloud_deployment(self, id):
+        """Get information about a cloud deployment.
+
+        Example:
+            >>> {
+            >>>     'id': 1,
+            >>>     'name': 'Deployment Example',
+            >>>     'last_online': '2019-12-12T14:00:00Z',
+            >>>     'created_date': '2019-12-12T13:30:00.00Z',
+            >>>     'updated_date': '2019-12-12T13:30:00.00Z',
+            >>>     'parameters': {},
+            >>>     'network_model': 123
+            >>> }
+
+        :param id: ID of the cloud deployment to receive information.
+        :return: Dictionary containing information of the requested cloud deployment.
+        """
+
+        try:
+            response = self.http.get(self.server_url + '/cloud-deployments/{}/'.format(id))
+            if response.status_code == 200:
+                return response.json()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def download_latest_model_checkpoint(self, model_id, output_file_path):
+        """Download the latest checkpoint of the given model and write it to the given `output_file_path`.
+
+        :param model_id: ID of the model whose latest checkpoint is download.
+        :param output_file_path: Output file path (no directory!).
+        :return: Information about the latest checkpoint or `None` if no checkpoint is available or an error occurred.
+        """
+        checkpoints = self.get_model_checkpoints(model_id)
+
+        if len(checkpoints) == 0:
+            return None
+
+        latest_checkpoint = checkpoints[-1]
+        if latest_checkpoint['checkpoint_file'] is None:
+            return None
+
+        try:
+            response = self.s3_http.get(latest_checkpoint['checkpoint_file'], stream=True)
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        with open(output_file_path, 'wb') as f:
+            for chunk in response.iter_content(4096):
+                f.write(chunk)
+        return latest_checkpoint
+
+    def download_model_checkpoint(self, checkpoint_id, output_file_path):
+        """Download a model checkpoint given by the checkpoint ID.
+
+        :param checkpoint_id: ID of the checkpoint to download.
+        :param output_file_path:  Output file path (no directory!).
+        :return: Information about the downloaded checkpoint or `None` if no checkpoint is available or an error occurred.
+        """
+        logger.info('Download model checkpoint with ID: {}'.format(checkpoint_id))
+
+        try:
+            response = self.http.get(self.server_url + '/model-checkpoints/' + str(checkpoint_id))
+            response.raise_for_status()
+            checkpoint = response.json()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        if checkpoint is None:
+            return None
+
+        try:
+            response = self.s3_http.get(checkpoint['checkpoint_file'], stream=True)
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return None
+
+        with open(output_file_path, 'wb') as f:
+            for chunk in response.iter_content(4096):
+                f.write(chunk)
+
+        logger.info('Downloaded model checkpoint with ID: {} to: {}'.format(checkpoint_id, output_file_path))
+
+        return checkpoint
+
+    def create_model_checkpoint(self, model_id, iteration):
+        """Create a new checkpoint for a model without uploading the checkpoint file.
+
+        :param model_id: ID of the model for which a checkpoint is created.
+        :param iteration: Training iteration of the checkpoint.
+        :return: Newly created checkpoint or `None` in case it could not be created.
+        """
+        model_checkpoint = {
+            'network_model': model_id,
+            'iteration': iteration
+        }
+
+        try:
+            response = self.http.post(self.server_url + '/model-checkpoints/', data=model_checkpoint)
+            response.raise_for_status()
+            return response.json()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def upload_model_checkpoint(self, checkpoint_id, iteration, file_path):
+        """Upload a model checkpoint.
+
+        :param checkpoint_id: ID of the checkpoint to which the files are uploaded.
+        :param iteration: Training iteration of the checkpoint.
+        :param file_path: File path to the checkpoint file.
+        :return: Updated checkpoint information or `None` in case of errors.
+        """
+
+        file_name = os.path.split(file_path)[-1]
+        files = {
+            'checkpoint_file': (file_name, open(file_path, 'rb'))
+        }
+        model_checkpoint = {
+            'iteration': iteration
+        }
+
+        try:
+            response = self.http.patch(self.server_url + '/model-checkpoints/{}/'.format(checkpoint_id),
+                                       data=model_checkpoint, files=files)
+            response.raise_for_status()
+            logger.info('Model checkpoint uploaded: {}'.format(file_name))
+            return response.json()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def upload_latest_model_checkpoint_async(self, model_id, iteration, file_path):
+        """Asynchronous update of the latest model checkpoint (largest iteration) including uploading a new checkpoint file.
+
+        :param model_id: ID of the model for which the latest checkpoint is updated.
+        :param iteration: Training iteration of the checkpoint.
+        :param file_path: File path to the checkpoint file.
+        """
+        threading.Thread(target=self.upload_latest_model_checkpoint, args=(model_id, iteration, file_path)).start()
+
+    def upload_latest_model_checkpoint(self, model_id, iteration, file_path):
+        """Update of the latest model checkpoint (largest iteration) including uploading a new checkpoint file.
+
+        :param model_id: ID of the model for which the latest checkpoint is updated.
+        :param iteration: Training iteration of the checkpoint.
+        :param file_path: File path to the checkpoint file.
+        :return: Updated checkpoint information or `None` in case of errors.
+        """
+        checkpoints = self.get_model_checkpoints(model_id)
+
+        if len(checkpoints) == 0:
+            checkpoint = self.create_model_checkpoint(model_id, iteration)
+        else:
+            checkpoint = checkpoints[-1]
+
+        if checkpoint is None:
+            return None
+
+        return self.upload_model_checkpoint(checkpoint['id'], iteration, file_path)
+
+    def upload_inference_data_async(self, model_id, file_path):
+        """Asynchronous upload of the inference data for the model given by its ID.
+
+        :param model_id: ID of the model for which the latest checkpoint is updated.
+        :param file_path: File path to the inference data file.
+        """
+        threading.Thread(target=self.upload_inference_data, args=(model_id, file_path)).start()
+
+    def upload_inference_data(self, model_id, file_path):
+        # TODO: FIXME: "upload_infernece_data" is confusion. this endpoint uploads the model (onnx) and accompanying files
+        # maybe rename to "upload_model_data" or something ? -> openAPI says "partial_update_network_model"
+        """Upload the inference data for the model given by its ID.
+
+        :param model_id: ID of the model for which the inference data is updated.
+        :param file_path: File path to the inference data file.
+        :return: Updated model information or `None` in case of errors.
+        """
+
+        file_name = os.path.split(file_path)[-1]
+        files = {'inference_data': (file_name, open(file_path, 'rb'))}
+
+        try:
+            response = self.http.patch(self.server_url + '/models/{}/'.format(model_id), files=files)
+            response.raise_for_status()
+            return True
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return False
+
+    def upload_model_statistics_async(self, statistics, timestamp, iteration, model_id):
+        """Asynchronous upload of model statistics (e.g., during training and evaluation) for a given model.
+
+        :param statistics: Dictionary of model statistics that must be serializable as JSON.
+        :param timestamp: Creation timestamp of the statistics.
+        :param iteration: Iteration of the statistics.
+        :param model_id: ID of the model the statistics belong to.
+        """
+        threading.Thread(target=self.upload_model_statistics, args=(statistics, timestamp, iteration, model_id)).start()
+
+    def upload_model_statistics(self, statistics, timestamp, iteration, model_id):
+        """Asynchronous upload of model statistics (e.g., during training and evaluation) for a given model.
+
+        :param statistics: Dictionary of model statistics that must be serializable as JSON.
+        :param timestamp: Creation timestamp of the statistics.
+        :param iteration: Iteration of the statistics.
+        :param model_id: ID of the model the statistics belong to.
+        """
+
+        logger.info('Upload model statistics')
+
+        statistics_entry = {
+            "timestamp": timestamp,
+            "iteration": iteration,
+            "statistics": json.dumps(statistics),
+            "network_model": model_id
+        }
+
+        try:
+            response = self.http.post(self.server_url + '/model-statistics/', data=statistics_entry)
+            response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            return
+
+        logger.info('Uploaded model statistics')
+
+    def get_inference_results_by_dataset_item_id(self, dataset_id: Optional[int] = None,
+                                                 iteration: Optional[int] = None,
+                                                 network_model_id: Optional[int] = None,
+                                                 max_items: Optional[int] = None,
+                                                 page_size: int = 100, **kwargs: Any) -> Dict[int, Dict[str, Any]]:
+
+        inference_results: List[Dict[str, Any]] = self.get_inference_results(
+            dataset_id=dataset_id, iteration=iteration, network_model_id=network_model_id,
+            max_items=max_items, page_size=page_size, **kwargs)
+
+        return {ir['dataset_item']['id']: ir for ir in inference_results}
+
+    def get_inference_results(self, dataset_id: Optional[int] = None, iteration: Optional[int] = None,
+                              network_model_id: Optional[int] = None, max_items: Optional[int] = None,
+                              page_size: int = 100, **kwargs: Any) -> List[Dict[str, Any]]:
+
+        url: str = f'{self.server_url}/inference-results/'
+        params: Dict[str, Any] = {'page_size': page_size}
+
+        if dataset_id is not None:
+            params['dataset_item__dataset__id'] = dataset_id
+
+        if iteration is not None:
+            params['iteration'] = iteration
+
+        if iteration is not None:
+            params['network_model_id'] = network_model_id
+
+        params.update(kwargs)
+
+        all_inference_results: List[Dict[str, Any]] = list()
+        while url is not None:
+
+            logger.debug(f'Get dataset items from "{url}"')
+            response: rq.models.Response = self.http.get(url, params=params)
+            response.raise_for_status()
+            response_json = response.json()
+
+            inference_results: Optional[List[Dict]] = response_json.get('results')
+            url = response_json.get('next')
+            params = None
+
+            if not inference_results:
+                break
+
+            all_inference_results.extend(inference_results)
+
+            if max_items is not None and len(all_inference_results) >= max_items:
+                break
+
+        return all_inference_results
+
+    def upload_inference_results_async(self, results, timestamp, iteration, model_id):
+        """Asynchronous upload of inference results (e.g., during evaluation) for a given model.
+
+        :param results: List of results. See :func:`~platform_sdk.Client.upload_inference_results` for details.
+        :param timestamp: Creation timestamp of the inference results.
+        :param iteration: Iteration of the inference results.
+        :param model_id: ID of the model the inference results belong to.
+        """
+        threading.Thread(target=self.upload_inference_results,
+                         args=(results, timestamp, iteration, model_id)).start()
+
+    def upload_inference_results(self, results, timestamp, iteration, model_id, *args):
+        """Upload of inference results (e.g., during evaluation) for a given model.
+
+        :param results: List of results.
+
+        Example:
+        >>> [
+        >>>     {
+        >>>         'dataset_item': 42,             # ID of the dataset item the result belongs to
+        >>>         'classification': {
+        >>>             'classes': [],              # list of platform class IDs (for classification)
+        >>>             'class_confidences': [...]  # list containing class confidences (ordered according to 'classes')
+        >>>         },
+        >>>         'detection': {
+        >>>             'boxes': [...]              # list of arrays representing the box coordinates and positions [x, y, width, height, orientation (optional)]
+        >>>                                         # x, y, width, and height must be scaled to the interval [0, 1] (the point (1, 1) corresponds to the lower right corner)
+        >>>             'classes': [...]            # list of platform class IDs (for detection)
+        >>>             'class_confidences': [...]  # 2-dimensional array containing class confidences (ordered according to 'classes') for each box
+        >>>         }
+        >>>     }
+        >>> ]
+
+        :param timestamp: Creation timestamp of the inference results.
+        :param iteration: Iteration of the inference results.
+        :param model_id: ID of the model the inference results belong to.
+        """
+
+        logger.info('Upload inference results')
+
+        msg_bytes = io.BytesIO()
+
+        # add meta data
+        msg_bytes.write(msgpack.packb(dict(timestamp=timestamp,
+                                           iteration=iteration,
+                                           model_id=model_id,
+                                           results=len(results))))
+
+        for i, result in enumerate(results):
+            msg_bytes.write(msgpack.packb(result))
+
+        response = self.http.post(f'{self.server_url}/bulk-data/',
+                                  data=dict(data_type=0),
+                                  files=dict(
+                                      data=(f'inference-data-{timestamp}-{model_id}.msgpack', msg_bytes.getvalue())))
+        response.raise_for_status()
+
+    def get_class_labels(self):
+        """Get a list of all available class labels of the platform sorted by name.
+
+        Example:
+        >>> [{'id': 37, 'name': 'airplane'},
+        >>>  {'id': 78, 'name': 'apple'},
+        >>>  {'id': 56, 'name': 'backpack'},
+        >>>  {'id': 77, 'name': 'banana'},
+        >>>  ...
+        >>> ]
+
+        :return: List of class labels or `None` in case of errors.
+        """
+        try:
+            response = self.http.get(self.server_url + '/class-labels/')
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def create_class_label(self, name, public=False):
+        """Create a new class label.
+
+        :param name: Name of the new class label.
+        :param public: Indicates if the label shall be globally accessible (by all users).
+        :return: Newly created class label or `None` in case of errors.
+        """
+
+        class_label = {'name': name, 'public': False}
+
+        try:
+            response = self.http.post(self.server_url + '/class-labels/', data=class_label)
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def get_jobs(self, worker_id):
+        """Get list of jobs for a particular worker.
+
+        :param worker_id: Jobs of this worker are returned.
+        :return: List of jobs or None.
+        """
+
+        try:
+            response = self.http.get(self.server_url + '/workers/{}/jobs/'.format(worker_id))
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def get_job(self, job_id):
+        """Get job details given its ID.
+
+        :param job_id: Job details.
+        :return: Job information or None.
+        """
+
+        try:
+            response = self.http.get(self.server_url + '/jobs/{}/'.format(job_id))
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def update_job(self, job):
+        """Update the job.
+
+        :param job: Fields to update. Must include the job ID.
+        :return: Job information or None.
+        """
+
+        job_id = job.get('id')
+        if job_id is None:
+            return None
+
+        try:
+            response = self.http.patch(self.server_url + '/jobs/{}/'.format(job_id), data=job)
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+        return None
+
+    def delete_job(self, job_id):
+        """Delete a specific job.
+
+        :param job_id: ID of the job that is to be removed.
+        """
+
+        try:
+            response = self.http.delete(self.server_url + '/jobs/{}/'.format(job_id))
+            if response.status_code == 404:
+                logger.info('Job could not be deleted because it did not exist.')
+            else:
+                response.raise_for_status()
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+
+    def create_labels_and_dataset(self, dataset_name, classification_class_labels=None,
+                                  object_detection_class_labels=None):
+        """Create a new dataset with all given class labels as detection class labels.
+
+        A new dataset is created and those class labels that do not exist yet are automatically created as well.
+
+        :param dataset_name: Name of the new dataset.
+        :param object_detection_class_labels: List of strings of the object detection class labels for the new dataset.
+        :return: ID of the newly created dataset or status code (see :func:`~platform_sdk.Client.create_dataset` for details).
+        """
+
+        # load list of all available class labels
+        all_class_labels = self.get_class_labels()
+
+        if all_class_labels is None:
+            logger.error('Could not retrieve available class labels')
+            return -1
+
+        # dictionary containing mapping from class names to class label ids
+        class_label_maps = {
+            'classification': None,
+            'object_detection': None
+        }
+
+        task_class_label_map = {}
+        if classification_class_labels is not None:
+            task_class_label_map['classification'] = classification_class_labels
+
+        if object_detection_class_labels is not None:
+            task_class_label_map['object_detection'] = object_detection_class_labels
+
+        for task in task_class_label_map:
+
+            class_label_names = task_class_label_map[task]
+            class_label_map = {}
+
+            # contains class names that do not yet exist on the platform
+            new_class_labels = []
+
+            # compare class labels of the dataset with existing class labels
+            for class_label in class_label_names:
+                is_new = True
+                for cl in all_class_labels:
+                    if class_label == cl['name']:
+                        is_new = False
+                        class_label_map[class_label] = cl['id']
+                        break
+
+                if is_new:
+                    new_class_labels.append(class_label)
+
+            # create new class labels
+            for new_class_label in new_class_labels:
+                id = self.create_class_label(new_class_label)
+                if id is None:
+                    logger.error('Could not create new class label ({}).'.format(new_class_label))
+                    return -1
+                class_label_map[new_class_label] = id
+
+            class_label_maps[task] = class_label_map.values()
+
+        logger.debug('Create new dataset')
+        return self.create_dataset(dataset_name,
+                                   classification_class_label_ids=class_label_maps['classification'],
+                                   object_detection_class_label_ids=class_label_maps['object_detection'])
+
+    def get_detection_class_label_map(self, dataset_id):
+        """Retrieve a dictionary that maps class label names to their IDs.
+
+        Example:
+        >>> {'car': 4,
+        >>>     'cyclist': 9,
+        >>>     'motorcycle': 36,
+        >>>     'pedestrian': 7,
+        >>>     'traffic light': 41,
+        >>>     'traffic sign': 119,
+        >>>     'truck': 6
+        >>> }
+
+        :param dataset_id: The mapping is loaded for class labels of this dataset.
+        :return: Class label map or `None` in case of errors.
+        """
+
+        dataset = self.get_dataset(dataset_id)
+
+        if dataset is None:
+            logger.error('Could not get dataset with ID {} for retrieving class labels'.format(dataset_id))
+            return None
+
+        class_labels = dataset['object_detection_class_labels']
+        class_label_map = {}
+        for class_label in class_labels:
+            class_label_map[class_label['name']] = class_label['id']
+        return class_label_map
+
+    def get_classification_class_label_map(self, dataset_id):
+        """Retrieve a dictionary that maps class label names to their IDs.
+
+        Example:
+        >>> {'car': 4,
+        >>>     'cyclist': 9,
+        >>>     'motorcycle': 36,
+        >>>     'pedestrian': 7,
+        >>>     'traffic light': 41,
+        >>>     'traffic sign': 119,
+        >>>     'truck': 6
+        >>> }
+
+        :param dataset_id: The mapping is loaded for class labels of this dataset.
+        :return: Class label map or `None` in case of errors.
+        """
+
+        dataset = self.get_dataset(dataset_id)
+
+        if dataset is None:
+            logger.error('Could not get dataset with ID {} for retrieving class labels'.format(dataset_id))
+            return None
+
+        class_labels = dataset['classification_class_labels']
+        class_label_map = {}
+        for class_label in class_labels:
+            class_label_map[class_label['name']] = class_label['id']
+        return class_label_map
+
+    def create_worker(self, name):
+        """Create a new training worker.
+
+        :return: ID of the newly created worker or `None`.
+        """
+
+        try:
+            worker = {
+                'name': name,
+                'status': '',
+                'details': {}
+            }
+            response = self.http.post(self.server_url + '/workers/', data=worker)
+            response.raise_for_status()
+            data = response.json()
+            return data
+        except rq.exceptions.RequestException as e:
+            logger.error(e)
+            raise e
+
+    def import_dataspree(self, dataset_name, dataset_id, images, annotations):
+        """Import a dataset that is available in the dataspree format.
+
+        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
+        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
+        :param images: Directory containing all images.
+        :param annotations: Directory containing the annotations.
+        :return: Status code. 0: import completed, -1: error
+        """
+        logger.info('Import dataspree data')
+
+        # create new dataset if no id is given
+        if dataset_id == -1:
+            # iterate over all items and determine used class labels (only for object detection for now)
+            logger.debug('Retrieve used class labels')
+            class_label_ids = set()
+            annotation_files = os.listdir(annotations)
+            for annotation_file in annotation_files:
+                with open(os.path.join(annotations, annotation_file), 'r') as f:
+                    annotation = json.load(f)
+                    for o in annotation['objects']:
+                        class_label_ids.add(o['label'])
+
+            logger.debug('Create new dataset')
+            dataset_id = self.create_dataset(dataset_name, object_detection_class_label_ids=class_label_ids)
+        else:
+            dataset = self.get_dataset(dataset_id)
+            if dataset is None:
+                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
+                return -1
+
+        if dataset_id == -1:
+            logger.error('Dataset ID not provided and could not create new dataset.')
+            return -1
+
+        dataset_items = self.get_dataset_items(dataset_id)
+        dataset_item_names = []
+
+        for item in dataset_items:
+            dataset_item_name = item['name'].split('/')[-1]
+            dataset_item_names.append(dataset_item_name)
+
+        # upload dataset items
+        annotation_files = os.listdir(annotations)
+        annotation_files.sort()
+
+        image_files = os.listdir(images)
+        image_files.sort()
+
+        logger.info('Upload dataset items')
+        for image_file in tqdm(image_files):
+
+            # do not upload in case the dataset item exits already
+            if image_file in dataset_item_names:
+                continue
+
+            base_name, image_extension = os.path.splitext(image_file)
+            annotation_file = '{}.{}'.format(base_name, 'json')
+
+            image_file_path = os.path.join(images, image_file)
+            base_name_split = base_name.split('_')
+
+            # first two elements of base_name_split contain dataset_id and item_id
+            image_file_name = '{}{}'.format('_'.join(base_name_split[2:]), image_extension)
+
+            annotation = {}
+            # load annotations if they exist
+            if annotation_file in annotation_files:
+                annotation_files.remove(annotation_file)
+
+                with open(os.path.join(annotations, annotation_file), 'r') as f:
+                    annotation = json.load(f)
+
+            if self.create_dataset_item(image_file_path, dataset_id, annotation, image_file_name) == -1:
+                logger.error('Error during creation of dataset item.')
+                return -1
+
+        return 0
+
+    def import_classification_directories(self, dataset_name, dataset_id, directory):
+        """Import a dataset for classification where each subfolder represents a class. The folder names need to match the class names that are available in the DLSD platform.
+
+                :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
+                :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
+                :param directory: Directory containing image subfolders.
+                :return: Status code. 0: import completed, -1: error
+                """
+        logger.info('Import classification directories')
+
+        subfolders = os.listdir(directory)
+
+        # create new dataset if no id is given
+        if dataset_id == -1:
+            # iterate over all items and determine used class labels
+            logger.debug('Retrieve used class labels')
+            class_labels = set()
+            for subfolder in subfolders:
+                class_labels.add(subfolder.lower())
+
+            dataset_id = self.create_labels_and_dataset(dataset_name, classification_class_labels=class_labels)
+        else:
+            dataset = self.get_dataset(dataset_id)
+            if dataset is None:
+                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
+                return -1
+
+        if dataset_id == -1:
+            logger.error('Dataset ID not provided and could not create new dataset.')
+            return -1
+
+        class_label_map = self.get_classification_class_label_map(dataset_id)
+
+        dataset_items = self.get_dataset_items(dataset_id)
+        dataset_item_names = []
+
+        for item in dataset_items:
+            dataset_item_name = item['name'].split('/')[-1]
+            dataset_item_names.append(dataset_item_name)
+
+        logger.info('Upload dataset items')
+        # upload dataset items
+        for subfolder in subfolders:
+            class_label_name = subfolder.lower()
+            logger.info('Import {}'.format(class_label_name))
+
+            image_files = os.listdir(os.path.join(directory, subfolder))
+
+            class_annotation = {
+                'classes': [class_label_map[class_label_name]]
+            }
+
+            for image_file in tqdm(image_files):
+
+                # do not upload in case the dataset item exits already
+                if image_file in dataset_item_names:
+                    continue
+
+                image_file_path = os.path.join(directory, subfolder, image_file)
+
+                if self.create_dataset_item(image_file_path, dataset_id, class_annotation) == -1:
+                    logger.error('Error during creation of dataset item.')
+                    return -1
+
+        return 0
+
+    def import_kitti(self, dataset_name, dataset_id, images, annotations):
+        """Import a dataset that is available in the KITTI format [1].
+
+        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
+        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
+        :param images: Directory containing all images.
+        :param annotations: Directory containing the annotations.
+        :return: Status code. 0: import completed, -1: error
+
+        [1] Geiger et al., "Are we ready for Autonomous Driving? The KITTI Vision Benchmark Suite", 2012.
+            http://www.cvlibs.net/datasets/kitti/eval_object.php?obj_benchmark=2d
+        """
+        logger.info('Import KITTI data')
+
+        # we import Pillow here as it is not required for other endpoints
+        from PIL import Image
+
+        # create new dataset if no id is given
+        if dataset_id == -1:
+            # iterate over all items and determine used class labels
+            logger.debug('Retrieve used class labels')
+            class_labels = set()
+            annotation_files = os.listdir(annotations)
+            for annotation_file in annotation_files:
+                with open(os.path.join(annotations, annotation_file), 'r') as f:
+                    file_content = f.readlines()
+                    for line in file_content:
+                        class_label = line.split(' ')[0].lower()
+                        # skip all objects with label 'dontcare'
+                        if class_label == 'dontcare' or class_label == 'misc':
+                            continue
+                        class_labels.add(class_label.lower())
+
+            dataset_id = self.create_labels_and_dataset(dataset_name, object_detection_class_labels=class_labels)
+        else:
+            dataset = self.get_dataset(dataset_id)
+            if dataset is None:
+                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
+                return -1
+
+        if dataset_id == -1:
+            logger.error('Dataset ID not provided and could not create new dataset.')
+            return -1
+
+        class_label_map = self.get_detection_class_label_map(dataset_id)
+
+        dataset_items = self.get_dataset_items(dataset_id)
+        dataset_item_names = []
+
+        for item in dataset_items:
+            dataset_item_name = item['name'].split('/')[-1]
+            dataset_item_names.append(dataset_item_name)
+
+        def convert_kitti_annotation(image_width, image_height, file_content):
+            normalizer = max(image_width, image_height)
+            objects = []
+
+            for i, line in enumerate(file_content):
+                attributes = line.split(' ')
+
+                class_label = attributes[0].lower()
+                # skip all objects with label 'dontcare'
+                if class_label == 'dontcare' or class_label == 'misc':
+                    continue
+
+                class_label_id = class_label_map[class_label]
+
+                left_x = float(attributes[4])
+                top_y = float(attributes[5])
+                right_x = float(attributes[6])
+                bottom_y = float(attributes[7])
+
+                x = ((left_x + right_x) / 2.0) / normalizer
+                y = ((top_y + bottom_y) / 2.0) / normalizer
+                w = (right_x - left_x) / normalizer
+                h = (bottom_y - top_y) / normalizer
+
+                o = {
+                    'id': i,
+                    'label': class_label_id,
+                    'x': x,
+                    'y': y,
+                    'width': w,
+                    'height': h,
+                    'orientation': 0
+                }
+
+                objects.append(o)
+
+            return objects
+
+        # upload dataset items
+        annotation_files = os.listdir(annotations)
+        image_files = os.listdir(images)
+
+        logger.info('Upload dataset items')
+        for image_file in tqdm(image_files):
+
+            # do not upload in case the dataset item exits already
+            if image_file in dataset_item_names:
+                continue
+
+            base_name = os.path.splitext(image_file)[0]
+            annotation_file = '{}.{}'.format(base_name, 'txt')
+
+            # only upload if image and annotation exists
+            if annotation_file in annotation_files:
+                annotation_files.remove(annotation_file)
+                image_file_path = os.path.join(images, image_file)
+
+                # We need to open the image to retrieve its width and height
+                # Image.open is a lazy operation - hence, the complete image
+                # data is not read immediately.
+                image = Image.open(image_file_path)
+                image_width, image_height = image.size
+
+                with open(os.path.join(annotations, annotation_file), 'r') as f:
+                    objects = convert_kitti_annotation(image_width, image_height, f.readlines())
+                    annotation = {
+                        'objects': objects
+                    }
+
+                if self.create_dataset_item(image_file_path, dataset_id, annotation) == -1:
+                    logger.error('Error during creation of dataset item.')
+                    return -1
+
+        return 0
+
+    def import_coco(self, dataset_name, dataset_id, images, annotations):
+        """Import a dataset that is available in the COCO format [1].
+
+        :param dataset_name: Name of the dataset that should be created. Set `None` if no new dataset should be created.
+        :param dataset_id: ID of an existing dataset to which items should be imported. Set `-1` if a new dataset should be created.
+        :param images: Directory containing all images.
+        :param annotations: Directory containing the annotations.
+        :return: Status code. 0: import completed, -1: error
+
+        [1] Lin et al., "Microsoft COCO: Common Objects in Context", 2014.
+            https://cocodataset.org/
+        """
+
+        logger.info('Import COCO data')
+
+        with open(annotations, 'r') as f:
+            coco = json.load(f)
+
+        coco_class_id_map = {}
+        for c in coco['categories']:
+            coco_class_id_map[c['id']] = c['name']
+
+        # create new dataset if no id is given
+        if dataset_id == -1:
+            # iterate over all items and determine used class labels
+            logger.debug('Retrieve used class labels')
+            dataset_id = self.create_labels_and_dataset(dataset_name,
+                                                        object_detection_class_labels=coco_class_id_map.values())
+            logger.info('Created dataset with ID {}.'.format(dataset_id))
+        else:
+            dataset = self.get_dataset(dataset_id)
+            if dataset is None:
+                logger.error('Dataset with ID {} does not exist.'.format(dataset_id))
+                return -1
+
+        if dataset_id == -1:
+            logger.error('Dataset ID not provided and could not create new dataset.')
+            return -1
+
+        class_label_map = self.get_detection_class_label_map(dataset_id)
+        dataset_items = self.get_dataset_items(dataset_id)
+        dataset_item_names = []
+
+        for item in dataset_items:
+            dataset_item_name = item['name'].split('/')[-1]
+            dataset_item_names.append(dataset_item_name)
+
+        # upload dataset items
+        logger.info('Upload dataset items')
+
+        coco_annotations = {}
+        coco_annotation_ids = {}
+        for a in coco['annotations']:
+            coco_annotations[a['id']] = a
+            image_id = a['image_id']
+            if image_id not in coco_annotation_ids:
+                coco_annotation_ids[image_id] = []
+            coco_annotation_ids[image_id].append(a['id'])
+
+        if self.parallel_requests > 1:
+            Parallel(n_jobs=self.parallel_requests, prefer='threads')(
+                delayed(self.upload_item_coco)(coco_image, images, coco_annotation_ids, coco_annotations,
+                                               coco_class_id_map,
+                                               class_label_map, dataset_id, dataset_item_names) for coco_image in
+                tqdm(coco['images']))
+        else:
+            for coco_image in tqdm(coco['images']):
+                self.upload_item_coco(coco_image, images, coco_annotation_ids, coco_annotations, coco_class_id_map,
+                                      class_label_map, dataset_id, dataset_item_names)
+
+        return 0
+
+    def upload_item_coco(self, coco_image, images, coco_annotation_ids, coco_annotations, coco_class_id_map,
+                         class_label_map, dataset_id, dataset_item_names):
+        image_id = coco_image['id']
+        image_file_name = coco_image['file_name']
+
+        # do not upload in case the dataset item exits already
+        if image_file_name in dataset_item_names:
+            return
+
+        image_file_path = os.path.join(images, image_file_name)
+        image_width = coco_image['width']
+        image_height = coco_image['height']
+        normalizer = max(image_width, image_height)
+
+        # get corresponding annotations
+        objects = []
+        if image_id not in coco_annotation_ids:
+            return
+        for i, cid in enumerate(coco_annotation_ids[image_id]):
+            a = coco_annotations[cid]
+
+            coco_class_id = a['category_id']
+            class_label_name = coco_class_id_map[coco_class_id]
+            class_label_id = class_label_map[class_label_name]
+            x = (a['bbox'][0] + 0.5 * a['bbox'][2]) / normalizer
+            y = (a['bbox'][1] + 0.5 * a['bbox'][3]) / normalizer
+            w = a['bbox'][2] / normalizer
+            h = a['bbox'][3] / normalizer
+            o = {
+                'id': i,
+                'label': class_label_id,
+                'x': x,
+                'y': y,
+                'width': w,
+                'height': h,
+                'orientation': 0
+            }
+            objects.append(o)
+
+        annotation = {
+            'objects': objects
+        }
+
+        if self.create_dataset_item(image_file_path, dataset_id, annotation) == -1:
+            logger.error('Error during creation of dataset item.')
+            return -1
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/data_loader.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/data_loader.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,454 +1,454 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import json
-import logging
-import os
-import numpy as np
-from copy import copy, deepcopy
-from enum import Enum
-from time import sleep
-from typing import Optional, Dict, List
-
-from tqdm import tqdm
-
-from dataspree.platform_sdk.client import Client
-from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
-from dataspree.platform_sdk.decoder.pcd_decoder import PcdDecoder
-from dataspree.platform_sdk.decoder.opencv_decoder import OpencvDecoder
-
-logger = logging.getLogger(__name__)
-
-
-class LoadMode(Enum):
-    PRELOAD = 0
-    ADHOC = 1
-    ADHOC_CACHED = 2
-
-
-class DataLoader:
-    """Data loader for data from the Data Spree AI Platform"""
-
-    def __init__(self, client: Client, network_model: Dict, dataset_directory: str,
-                 mode: LoadMode = LoadMode.ADHOC_CACHED,
-                 allowed_status=('annotated', 'reviewed'), decoders: Optional[List[BaseDecoder]] = None,
-                 distinct_items_per_category: bool = True):
-        self._client = client
-        self._network_model = network_model
-        self._dataset_directory = dataset_directory
-        self._mode = mode
-        self._allowed_status = allowed_status
-        self._decoders = []
-        self._distinct_items_per_category = distinct_items_per_category
-        self._max_retries = 10
-
-        if self._dataset_directory == '':
-            logger.info('Switching to adhoc mode because no dataset directory is provided.')
-            self._mode = LoadMode.ADHOC
-
-        if decoders is None:
-            decoders = [PcdDecoder(), OpencvDecoder()]
-            # decoders=[PcdDecoder(), OpencvDecoder(), PlyDecoder()] # TODO: Test Me
-
-        for decoder in decoders:
-            self.add_decoder(decoder)
-
-        self._items = {}
-
-        # load class label ids and names that are used within this model
-        self._model_class_labels: List[Dict] = client.get_model_class_labels(network_model['id'])
-        self._mapped_class_labels: Dict[int, List[int]] = dict()
-        self._target_class_labels: List[Dict] = []
-        target_class_label_ids = []
-        for c in self._model_class_labels:
-            target_class_label = c['target_class_label']
-            if target_class_label is None:
-                # old class labels have no target (they are the target/there is no remapping)
-                target_class_label = c['class_label']
-            if target_class_label['id'] not in target_class_label_ids:
-                target_class_label_ids.append(target_class_label['id'])
-                self._target_class_labels.append(target_class_label)
-            class_label = c['class_label']
-            mapped_labels = self._mapped_class_labels.setdefault(class_label['id'], [])
-            if target_class_label['id'] not in mapped_labels:
-                mapped_labels.append(target_class_label['id'])
-
-        # get all categories and aggregate the respective subset IDs
-        self._subsets_ids_by_category = {}
-        for entry in network_model['data_subsets']:
-            if entry['category'] not in self._subsets_ids_by_category.keys():
-                self._subsets_ids_by_category[entry['category']] = []
-            if entry['data_subset']['id'] not in self._subsets_ids_by_category[entry['category']]:
-                self._subsets_ids_by_category[entry['category']].append(entry['data_subset']['id'])
-
-        # get all subset IDs
-        subset_ids = []
-        condensed_subset_ids = [self._subsets_ids_by_category[cat] for cat in self._subsets_ids_by_category.keys()]
-        for subset_id in [item for sublist in condensed_subset_ids for item in sublist]:
-            subset_ids.append(subset_id)
-
-        # get all item IDs
-        self._item_ids = set()
-        self._item_ids_by_subset = {}
-        for subset_id in subset_ids:
-            if subset_id not in self._item_ids_by_subset:
-                self._item_ids_by_subset[subset_id] = []
-
-            ## FIXME: only get items that have the reqested class IDs.
-            # TODO: figure out the most efficient way to get those items.
-            # SUGGESTIONS A: client.get_dataset_items with specified class_id for all IDs. Probably slow when a lot of labels are required
-            # SUGGESTIONS B: client.get_dataset_items with specified class_id in filter query (?, this is also limited in DLDS isn't it?)
-            subset_item_details = self._client.get_dataset_items(subset_id=subset_id, status=self._allowed_status)
-            for item in subset_item_details:
-                # del item['name']
-                # del item['updated_date']
-                if item['status'] in self._allowed_status:
-                    item['exists'] = False
-                    self._items[item['id']] = item
-                    self._item_ids_by_subset[subset_id].append(item['id'])
-                    self._item_ids.add(item['id'])
-
-        self._item_ids = list(self._item_ids)
-        if not len(self._item_ids):
-            raise ValueError('No items loaded for training. Exit. Maybe you did not update the item\'s status?')
-
-        self._item_ids_by_category = {}
-        for category in self._subsets_ids_by_category.keys():
-            for subset_id in self._subsets_ids_by_category[category]:
-                if category not in self._item_ids_by_category:
-                    if distinct_items_per_category:
-                        self._item_ids_by_category[category] = set()
-                    else:
-                        self._item_ids_by_category[category] = list()
-
-                if distinct_items_per_category:
-                    self._item_ids_by_category[category].update(self._item_ids_by_subset[subset_id])
-                else:
-                    self._item_ids_by_category[category].extend(self._item_ids_by_subset[subset_id])
-
-            if distinct_items_per_category:
-                self._item_ids_by_category[category] = list(self._item_ids_by_category[category])
-
-        if self._mode == LoadMode.PRELOAD:
-            for item_id in tqdm(self._item_ids):
-                image_directory = os.path.join(self._dataset_directory, str(self._items[item_id]['dataset']), 'images')
-                metainformation_directory = os.path.join(self._dataset_directory, str(self._items[item_id]['dataset']),
-                                                         'metainformation')
-
-                item = self._items[item_id]
-                dataset_id = item['dataset']
-                item_name = item['name'].split('/')[-1]
-                image_file_name = f'{dataset_id}_{item_id}_{item_name}'
-                metainformation_file_name = image_file_name.split('.')[0] + '.json'
-                image_path = os.path.join(image_directory, image_file_name)
-                metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
-                if os.path.exists(image_path) and os.path.exists(metainformation_path):
-                    item['exists'] = True
-                else:
-                    self._client.download_dataset_item(item_id, image_dir=image_directory,
-                                                            metainformation_directory=metainformation_directory,
-                                                            accepted_status=self._allowed_status,
-                                                            return_item=False)
-
-    def __reduce__(self):
-        return (DataLoader, (self._client,
-                             self._network_model,
-                             self._dataset_directory,
-                             self._mode,
-                             self._allowed_status,
-                             self._decoders,
-                             self._distinct_items_per_category,))
-
-    def add_decoder(self, decoder):
-        self._decoders.append(decoder)
-
-    def get_class_labels(self) -> List[Dict]:
-        """Get the list of class labels that are selected for the loaded model.
-
-        :return: List containing the class labels with ID and name.
-        """
-        return copy(self._target_class_labels)
-
-    def get_categories(self) -> List[str]:
-        """List containing the names of all categories.
-
-        :return: List of category names.
-        """
-        return list(self._item_ids_by_category.keys())
-
-    def get_subset_ids_by_category(self, category) -> List[str]:
-        """List containing the ids of all subsets in that categories.
-
-        :return: List of subset ids.
-        """
-        return self._subsets_ids_by_category.get(category, [])
-
-    def get_subset_ids(self, category=None) -> List[int]:
-        """List containing the IDs of the subsets of the specified category or all subsets.
-
-        :param category: Category to filter the subset IDs.
-        :return: List of subset IDs.
-        """
-
-        if category is None:
-            return list(self._item_ids_by_subset.keys())
-        else:
-            return list(self._subsets_ids_by_category[category])
-
-    def get_item_ids(self) -> List[int]:
-        """List containing the IDs of all items.
-
-        This list contains unique item IDs, e.g. an item that belongs to multiple subsets is only listed once.
-
-        :return: List of item IDs.
-        """
-        return copy(list(set(self._item_ids)))
-
-    def get_item_ids_by_category(self, category) -> List[int]:
-        """Get the IDs of all items that belong to the specified category.
-
-        :param category: Category to filter the item IDs.
-        :return: List of item IDs.
-        """
-        return copy(self._item_ids_by_category.get(category, []))
-
-    def apply_label_remapping(self, annotations):
-        """Remap dataset labels to model target labels.
-
-        :param annotations: Dataset item annotations.
-        :return: Updated annotations.
-        """
-        mcl = self._mapped_class_labels
-
-        # update all image class labels
-        classes = annotations.get('classes')
-        new_classes = []
-        if classes is not None:
-            for label in classes:
-                new_labels = mcl.get(label, [label])
-                new_classes.extend(new_labels)
-            annotations['classes'] = new_classes
-
-        # update all object class labels
-        new_objects = []
-        objects = annotations.get('objects')
-        if objects is not None:
-            for obj in objects:
-                label = obj['label']
-                new_labels = mcl.get(label, [label])
-                # update the label of the existing object
-                new_label = new_labels[0]
-                obj['label'] = new_label
-
-                # add new objects with mapped labels if needed
-                for l in new_labels[1:]:
-                    new_obj = copy(obj)
-                    new_obj['label'] = l
-                    new_objects.append(new_obj)
-            objects.extend(new_objects)
-        return annotations
-
-    def get_item_ids_by_subset(self, subset_id):
-        """Get the IDs of all items that belong to the specified subset.
-
-        :param subset_id: ID of a subset.
-        :return: List of item IDs.
-        """
-        return copy(self._item_ids_by_subset.get(subset_id, []))
-
-    def get_item(self, item_id, n_retries=0, store_binary: bool = False) -> Optional[Dict]:
-        """Get dataset item given its ID.
-
-        :param item_id: ID of the item.
-        :param store_binary:
-        :return: Dictionary containing the image and meta data or None if the item does not exist.
-        >>> {
-        >>> 'id': int,
-        >>> 'image': [],
-        >>> 'annotations': Dict
-        >>> }
-        """
-
-        logger.debug(f'get item {item_id}')
-
-        loading_error = False
-
-        item_serialized = None
-        decoded_image_path = None
-        if self._mode == LoadMode.ADHOC:
-            item_serialized = self._client.download_dataset_item(item_id, image_dir=None,
-                                                                      metainformation_directory=None,
-                                                                      accepted_status=self._allowed_status,
-                                                                      return_item=True)
-        else:
-            # get item details (if it exists already)
-            item = self._items.get(item_id)
-            if item is None:
-                item = self._client.get_dataset_item(item_id)
-                self._items[item_id] = item
-
-            if item is not None:
-                dataset_id = item['dataset']
-                image_directory = os.path.join(self._dataset_directory, str(dataset_id), 'images')
-                metainformation_directory = os.path.join(self._dataset_directory, str(dataset_id), 'metainformation')
-
-                item_name = item['name'].split('/')[-1]
-                image_file_name = f'{dataset_id}_{item_id}_{item_name}'
-
-                metainformation_file_name = os.path.splitext(image_file_name)[0] + '.json'
-                image_path = os.path.join(image_directory, image_file_name)
-                decoded_image_path = os.path.join(image_directory, f'{image_file_name}.bin') if store_binary else None
-                metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
-
-                item['image_path'] = image_path
-                item['decoded_image_path'] = decoded_image_path
-                item['metainformation_path'] = metainformation_path
-                item_serialized = deepcopy(item)
-
-                if (os.path.exists(image_path)
-                    or (decoded_image_path is not None and os.path.exists(decoded_image_path))) \
-                        and os.path.exists(metainformation_path):
-                    item['exists'] = True
-
-                    if decoded_image_path is not None and os.path.exists(decoded_image_path):
-                        try:
-                            with open(decoded_image_path, 'rb') as f:
-                                item_serialized['decoded_image'] = np.load(f)
-                        except Exception:
-                            logger.warning(f'could not  decode bianry image file {decoded_image_path}.')
-
-                    if 'decoded_image' not in item_serialized:
-                        if os.path.exists(image_path):
-                            with open(image_path, 'rb') as f:
-                                item_serialized['image'] = f.read()
-                        else:
-                            loading_error = True
-
-                    with open(metainformation_path, 'r') as f:
-                        try:
-                            loaded = json.load(f)
-
-                            str_changed_date_json = loaded.get('updated_date')
-                            str_changed_date_item = item.get('updated_date')
-
-                            if str_changed_date_json is None or str_changed_date_item is None:
-                                logger.warning(f'Could not extract modified date from item {item_id}:'
-                                               f'"{str_changed_date_json}", "{str_changed_date_item}"')
-
-                            changed_date_json = None
-                            changed_date_item = None
-
-                            if str_changed_date_json is not None and str_changed_date_item is not None:
-                                changed_date_item = Client.parse_dataset_item_date(str_changed_date_item)
-                                changed_date_json = Client.parse_dataset_item_date(str_changed_date_json)
-
-                            if changed_date_json is not None and changed_date_item is not None \
-                                    and changed_date_json > changed_date_item:
-                                logger.warning('The item\'s cached metainformation are newer than those from the '
-                                               'platform. Expecting an error and downloading the current item again. ')
-
-                            item['exists'] = changed_date_item is not None and changed_date_json is not None \
-                                             and changed_date_item == changed_date_json
-
-                            if item['exists']:
-                                item_serialized['annotations'] = loaded['annotations']
-
-                        except json.JSONDecodeError:
-                            logger.warning(f'Could not load metainformation for item {item_id}')
-                            loading_error = True
-
-                else:
-                    item['exists'] = False
-
-                if not item['exists']:
-                    item_serialized: Optional[Dict] = self._client.download_dataset_item(
-                        item_id, image_dir=image_directory, metainformation_directory=metainformation_directory,
-                        accepted_status=self._allowed_status, return_item=True)
-                    if item_serialized is not None:
-                        item_serialized['exists'] = True
-                        item_serialized['image_path'] = image_path
-                        item_serialized['metainformation_path'] = metainformation_directory
-
-        if item_serialized is None:
-            loading_error = True
-        else:
-            # decode
-
-            item_file_extension = os.path.splitext(item_serialized['name'])[1].lower().replace('.', '')
-            if item_file_extension == '':
-                # assume jpg if no file extension
-                item_file_extension = 'jpg'
-            if self._decoders:
-
-                if 'decoded_image' in item_serialized:
-                    item_serialized['image'] = item_serialized['decoded_image']
-                    item_serialized['data_type'] = item_file_extension
-
-                else:
-                    loading_error = True
-                    for decoder in self._decoders:
-                        extensions = decoder.get_file_extensions()
-                        if item_file_extension in extensions:
-                            try:
-                                item_serialized['image'], item_serialized['metadata'] = decoder(
-                                    item_serialized['image'])
-                                item_serialized['data_type'] = item_file_extension
-
-                                if decoded_image_path is not None:
-                                    with open(decoded_image_path, 'wb') as f:
-                                        np.save(f, item_serialized['image'])
-                                loading_error = False
-                            except Exception as e:
-                                logger.warning(f'Could not decode image for item {item_id}: {type(e)}: {e}')
-                                #loading_error = True
-                            break
-                    if loading_error: return None
-
-        if loading_error:
-            if n_retries < self._max_retries:
-                # sleep for 1, 2, 4, 8, ... milliseconds (maximum 2 seconds)
-                sleep(min(2.0, 1e-3 * 2 ** n_retries))
-
-                if item_serialized is not None and item_serialized.get('exists', False):
-                    if 'image_path' in item_serialized:
-                        try:
-                            os.remove(item_serialized['image_path'])
-                        except Exception as e:
-                            logger.error(f'Exception occurred while removing {item_serialized["image_path"]}\n{e}')
-                    if 'metainformation_path' in item_serialized:
-                        try:
-                            os.remove(item_serialized['metainformation_path'])
-                        except Exception as e:
-                            logger.error(f'Exception occurred while removing '
-                                         f'{item_serialized["metainformation_path"]}\n{e}')
-
-                return self.get_item(item_id, n_retries + 1)
-            else:
-                return None
-
-        image = item_serialized['image']
-        data_type = item_serialized['data_type']
-        annotations = item_serialized['annotations']
-
-        # update annotations based on the label remapping
-        annotations = self.apply_label_remapping(annotations)
-
-        sample = {
-            'id': item_id,
-            'image': image,
-            'data_type': data_type,
-            'annotations': annotations
-        }
-
-        return sample
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import json
+import logging
+import os
+import numpy as np
+from copy import copy, deepcopy
+from enum import Enum
+from time import sleep
+from typing import Optional, Dict, List
+
+from tqdm import tqdm
+
+from dataspree.platform_sdk.client import Client
+from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
+from dataspree.platform_sdk.decoder.pcd_decoder import PcdDecoder
+from dataspree.platform_sdk.decoder.opencv_decoder import OpencvDecoder
+
+logger = logging.getLogger(__name__)
+
+
+class LoadMode(Enum):
+    PRELOAD = 0
+    ADHOC = 1
+    ADHOC_CACHED = 2
+
+
+class DataLoader:
+    """Data loader for data from the Data Spree AI Platform"""
+
+    def __init__(self, client: Client, network_model: Dict, dataset_directory: str,
+                 mode: LoadMode = LoadMode.ADHOC_CACHED,
+                 allowed_status=('annotated', 'reviewed'), decoders: Optional[List[BaseDecoder]] = None,
+                 distinct_items_per_category: bool = True):
+        self._client = client
+        self._network_model = network_model
+        self._dataset_directory = dataset_directory
+        self._mode = mode
+        self._allowed_status = allowed_status
+        self._decoders = []
+        self._distinct_items_per_category = distinct_items_per_category
+        self._max_retries = 10
+
+        if self._dataset_directory == '':
+            logger.info('Switching to adhoc mode because no dataset directory is provided.')
+            self._mode = LoadMode.ADHOC
+
+        if decoders is None:
+            decoders = [PcdDecoder(), OpencvDecoder()]
+            # decoders=[PcdDecoder(), OpencvDecoder(), PlyDecoder()] # TODO: Test Me
+
+        for decoder in decoders:
+            self.add_decoder(decoder)
+
+        self._items = {}
+
+        # load class label ids and names that are used within this model
+        self._model_class_labels: List[Dict] = client.get_model_class_labels(network_model['id'])
+        self._mapped_class_labels: Dict[int, List[int]] = dict()
+        self._target_class_labels: List[Dict] = []
+        target_class_label_ids = []
+        for c in self._model_class_labels:
+            target_class_label = c['target_class_label']
+            if target_class_label is None:
+                # old class labels have no target (they are the target/there is no remapping)
+                target_class_label = c['class_label']
+            if target_class_label['id'] not in target_class_label_ids:
+                target_class_label_ids.append(target_class_label['id'])
+                self._target_class_labels.append(target_class_label)
+            class_label = c['class_label']
+            mapped_labels = self._mapped_class_labels.setdefault(class_label['id'], [])
+            if target_class_label['id'] not in mapped_labels:
+                mapped_labels.append(target_class_label['id'])
+
+        # get all categories and aggregate the respective subset IDs
+        self._subsets_ids_by_category = {}
+        for entry in network_model['data_subsets']:
+            if entry['category'] not in self._subsets_ids_by_category.keys():
+                self._subsets_ids_by_category[entry['category']] = []
+            if entry['data_subset']['id'] not in self._subsets_ids_by_category[entry['category']]:
+                self._subsets_ids_by_category[entry['category']].append(entry['data_subset']['id'])
+
+        # get all subset IDs
+        subset_ids = []
+        condensed_subset_ids = [self._subsets_ids_by_category[cat] for cat in self._subsets_ids_by_category.keys()]
+        for subset_id in [item for sublist in condensed_subset_ids for item in sublist]:
+            subset_ids.append(subset_id)
+
+        # get all item IDs
+        self._item_ids = set()
+        self._item_ids_by_subset = {}
+        for subset_id in subset_ids:
+            if subset_id not in self._item_ids_by_subset:
+                self._item_ids_by_subset[subset_id] = []
+
+            ## FIXME: only get items that have the reqested class IDs.
+            # TODO: figure out the most efficient way to get those items.
+            # SUGGESTIONS A: client.get_dataset_items with specified class_id for all IDs. Probably slow when a lot of labels are required
+            # SUGGESTIONS B: client.get_dataset_items with specified class_id in filter query (?, this is also limited in DLDS isn't it?)
+            subset_item_details = self._client.get_dataset_items(subset_id=subset_id, status=self._allowed_status)
+            for item in subset_item_details:
+                # del item['name']
+                # del item['updated_date']
+                if item['status'] in self._allowed_status:
+                    item['exists'] = False
+                    self._items[item['id']] = item
+                    self._item_ids_by_subset[subset_id].append(item['id'])
+                    self._item_ids.add(item['id'])
+
+        self._item_ids = list(self._item_ids)
+        if not len(self._item_ids):
+            raise ValueError('No items loaded for training. Exit. Maybe you did not update the item\'s status?')
+
+        self._item_ids_by_category = {}
+        for category in self._subsets_ids_by_category.keys():
+            for subset_id in self._subsets_ids_by_category[category]:
+                if category not in self._item_ids_by_category:
+                    if distinct_items_per_category:
+                        self._item_ids_by_category[category] = set()
+                    else:
+                        self._item_ids_by_category[category] = list()
+
+                if distinct_items_per_category:
+                    self._item_ids_by_category[category].update(self._item_ids_by_subset[subset_id])
+                else:
+                    self._item_ids_by_category[category].extend(self._item_ids_by_subset[subset_id])
+
+            if distinct_items_per_category:
+                self._item_ids_by_category[category] = list(self._item_ids_by_category[category])
+
+        if self._mode == LoadMode.PRELOAD:
+            for item_id in tqdm(self._item_ids):
+                image_directory = os.path.join(self._dataset_directory, str(self._items[item_id]['dataset']), 'images')
+                metainformation_directory = os.path.join(self._dataset_directory, str(self._items[item_id]['dataset']),
+                                                         'metainformation')
+
+                item = self._items[item_id]
+                dataset_id = item['dataset']
+                item_name = item['name'].split('/')[-1]
+                image_file_name = f'{dataset_id}_{item_id}_{item_name}'
+                metainformation_file_name = image_file_name.split('.')[0] + '.json'
+                image_path = os.path.join(image_directory, image_file_name)
+                metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
+                if os.path.exists(image_path) and os.path.exists(metainformation_path):
+                    item['exists'] = True
+                else:
+                    self._client.download_dataset_item(item_id, image_dir=image_directory,
+                                                            metainformation_directory=metainformation_directory,
+                                                            accepted_status=self._allowed_status,
+                                                            return_item=False)
+
+    def __reduce__(self):
+        return (DataLoader, (self._client,
+                             self._network_model,
+                             self._dataset_directory,
+                             self._mode,
+                             self._allowed_status,
+                             self._decoders,
+                             self._distinct_items_per_category,))
+
+    def add_decoder(self, decoder):
+        self._decoders.append(decoder)
+
+    def get_class_labels(self) -> List[Dict]:
+        """Get the list of class labels that are selected for the loaded model.
+
+        :return: List containing the class labels with ID and name.
+        """
+        return copy(self._target_class_labels)
+
+    def get_categories(self) -> List[str]:
+        """List containing the names of all categories.
+
+        :return: List of category names.
+        """
+        return list(self._item_ids_by_category.keys())
+
+    def get_subset_ids_by_category(self, category) -> List[str]:
+        """List containing the ids of all subsets in that categories.
+
+        :return: List of subset ids.
+        """
+        return self._subsets_ids_by_category.get(category, [])
+
+    def get_subset_ids(self, category=None) -> List[int]:
+        """List containing the IDs of the subsets of the specified category or all subsets.
+
+        :param category: Category to filter the subset IDs.
+        :return: List of subset IDs.
+        """
+
+        if category is None:
+            return list(self._item_ids_by_subset.keys())
+        else:
+            return list(self._subsets_ids_by_category[category])
+
+    def get_item_ids(self) -> List[int]:
+        """List containing the IDs of all items.
+
+        This list contains unique item IDs, e.g. an item that belongs to multiple subsets is only listed once.
+
+        :return: List of item IDs.
+        """
+        return copy(list(set(self._item_ids)))
+
+    def get_item_ids_by_category(self, category) -> List[int]:
+        """Get the IDs of all items that belong to the specified category.
+
+        :param category: Category to filter the item IDs.
+        :return: List of item IDs.
+        """
+        return copy(self._item_ids_by_category.get(category, []))
+
+    def apply_label_remapping(self, annotations):
+        """Remap dataset labels to model target labels.
+
+        :param annotations: Dataset item annotations.
+        :return: Updated annotations.
+        """
+        mcl = self._mapped_class_labels
+
+        # update all image class labels
+        classes = annotations.get('classes')
+        new_classes = []
+        if classes is not None:
+            for label in classes:
+                new_labels = mcl.get(label, [label])
+                new_classes.extend(new_labels)
+            annotations['classes'] = new_classes
+
+        # update all object class labels
+        new_objects = []
+        objects = annotations.get('objects')
+        if objects is not None:
+            for obj in objects:
+                label = obj['label']
+                new_labels = mcl.get(label, [label])
+                # update the label of the existing object
+                new_label = new_labels[0]
+                obj['label'] = new_label
+
+                # add new objects with mapped labels if needed
+                for l in new_labels[1:]:
+                    new_obj = copy(obj)
+                    new_obj['label'] = l
+                    new_objects.append(new_obj)
+            objects.extend(new_objects)
+        return annotations
+
+    def get_item_ids_by_subset(self, subset_id):
+        """Get the IDs of all items that belong to the specified subset.
+
+        :param subset_id: ID of a subset.
+        :return: List of item IDs.
+        """
+        return copy(self._item_ids_by_subset.get(subset_id, []))
+
+    def get_item(self, item_id, n_retries=0, store_binary: bool = False) -> Optional[Dict]:
+        """Get dataset item given its ID.
+
+        :param item_id: ID of the item.
+        :param store_binary:
+        :return: Dictionary containing the image and meta data or None if the item does not exist.
+        >>> {
+        >>> 'id': int,
+        >>> 'image': [],
+        >>> 'annotations': Dict
+        >>> }
+        """
+
+        logger.debug(f'get item {item_id}')
+
+        loading_error = False
+
+        item_serialized = None
+        decoded_image_path = None
+        if self._mode == LoadMode.ADHOC:
+            item_serialized = self._client.download_dataset_item(item_id, image_dir=None,
+                                                                      metainformation_directory=None,
+                                                                      accepted_status=self._allowed_status,
+                                                                      return_item=True)
+        else:
+            # get item details (if it exists already)
+            item = self._items.get(item_id)
+            if item is None:
+                item = self._client.get_dataset_item(item_id)
+                self._items[item_id] = item
+
+            if item is not None:
+                dataset_id = item['dataset']
+                image_directory = os.path.join(self._dataset_directory, str(dataset_id), 'images')
+                metainformation_directory = os.path.join(self._dataset_directory, str(dataset_id), 'metainformation')
+
+                item_name = item['name'].split('/')[-1]
+                image_file_name = f'{dataset_id}_{item_id}_{item_name}'
+
+                metainformation_file_name = os.path.splitext(image_file_name)[0] + '.json'
+                image_path = os.path.join(image_directory, image_file_name)
+                decoded_image_path = os.path.join(image_directory, f'{image_file_name}.bin') if store_binary else None
+                metainformation_path = os.path.join(metainformation_directory, metainformation_file_name)
+
+                item['image_path'] = image_path
+                item['decoded_image_path'] = decoded_image_path
+                item['metainformation_path'] = metainformation_path
+                item_serialized = deepcopy(item)
+
+                if (os.path.exists(image_path)
+                    or (decoded_image_path is not None and os.path.exists(decoded_image_path))) \
+                        and os.path.exists(metainformation_path):
+                    item['exists'] = True
+
+                    if decoded_image_path is not None and os.path.exists(decoded_image_path):
+                        try:
+                            with open(decoded_image_path, 'rb') as f:
+                                item_serialized['decoded_image'] = np.load(f)
+                        except Exception:
+                            logger.warning(f'could not  decode bianry image file {decoded_image_path}.')
+
+                    if 'decoded_image' not in item_serialized:
+                        if os.path.exists(image_path):
+                            with open(image_path, 'rb') as f:
+                                item_serialized['image'] = f.read()
+                        else:
+                            loading_error = True
+
+                    with open(metainformation_path, 'r') as f:
+                        try:
+                            loaded = json.load(f)
+
+                            str_changed_date_json = loaded.get('updated_date')
+                            str_changed_date_item = item.get('updated_date')
+
+                            if str_changed_date_json is None or str_changed_date_item is None:
+                                logger.warning(f'Could not extract modified date from item {item_id}:'
+                                               f'"{str_changed_date_json}", "{str_changed_date_item}"')
+
+                            changed_date_json = None
+                            changed_date_item = None
+
+                            if str_changed_date_json is not None and str_changed_date_item is not None:
+                                changed_date_item = Client.parse_dataset_item_date(str_changed_date_item)
+                                changed_date_json = Client.parse_dataset_item_date(str_changed_date_json)
+
+                            if changed_date_json is not None and changed_date_item is not None \
+                                    and changed_date_json > changed_date_item:
+                                logger.warning('The item\'s cached metainformation are newer than those from the '
+                                               'platform. Expecting an error and downloading the current item again. ')
+
+                            item['exists'] = changed_date_item is not None and changed_date_json is not None \
+                                             and changed_date_item == changed_date_json
+
+                            if item['exists']:
+                                item_serialized['annotations'] = loaded['annotations']
+
+                        except json.JSONDecodeError:
+                            logger.warning(f'Could not load metainformation for item {item_id}')
+                            loading_error = True
+
+                else:
+                    item['exists'] = False
+
+                if not item['exists']:
+                    item_serialized: Optional[Dict] = self._client.download_dataset_item(
+                        item_id, image_dir=image_directory, metainformation_directory=metainformation_directory,
+                        accepted_status=self._allowed_status, return_item=True)
+                    if item_serialized is not None:
+                        item_serialized['exists'] = True
+                        item_serialized['image_path'] = image_path
+                        item_serialized['metainformation_path'] = metainformation_directory
+
+        if item_serialized is None:
+            loading_error = True
+        else:
+            # decode
+
+            item_file_extension = os.path.splitext(item_serialized['name'])[1].lower().replace('.', '')
+            if item_file_extension == '':
+                # assume jpg if no file extension
+                item_file_extension = 'jpg'
+            if self._decoders:
+
+                if 'decoded_image' in item_serialized:
+                    item_serialized['image'] = item_serialized['decoded_image']
+                    item_serialized['data_type'] = item_file_extension
+
+                else:
+                    loading_error = True
+                    for decoder in self._decoders:
+                        extensions = decoder.get_file_extensions()
+                        if item_file_extension in extensions:
+                            try:
+                                item_serialized['image'], item_serialized['metadata'] = decoder(
+                                    item_serialized['image'])
+                                item_serialized['data_type'] = item_file_extension
+
+                                if decoded_image_path is not None:
+                                    with open(decoded_image_path, 'wb') as f:
+                                        np.save(f, item_serialized['image'])
+                                loading_error = False
+                            except Exception as e:
+                                logger.warning(f'Could not decode image for item {item_id}: {type(e)}: {e}')
+                                #loading_error = True
+                            break
+                    if loading_error: return None
+
+        if loading_error:
+            if n_retries < self._max_retries:
+                # sleep for 1, 2, 4, 8, ... milliseconds (maximum 2 seconds)
+                sleep(min(2.0, 1e-3 * 2 ** n_retries))
+
+                if item_serialized is not None and item_serialized.get('exists', False):
+                    if 'image_path' in item_serialized:
+                        try:
+                            os.remove(item_serialized['image_path'])
+                        except Exception as e:
+                            logger.error(f'Exception occurred while removing {item_serialized["image_path"]}\n{e}')
+                    if 'metainformation_path' in item_serialized:
+                        try:
+                            os.remove(item_serialized['metainformation_path'])
+                        except Exception as e:
+                            logger.error(f'Exception occurred while removing '
+                                         f'{item_serialized["metainformation_path"]}\n{e}')
+
+                return self.get_item(item_id, n_retries + 1)
+            else:
+                return None
+
+        image = item_serialized['image']
+        data_type = item_serialized['data_type']
+        annotations = item_serialized['annotations']
+
+        # update annotations based on the label remapping
+        annotations = self.apply_label_remapping(annotations)
+
+        sample = {
+            'id': item_id,
+            'image': image,
+            'data_type': data_type,
+            'annotations': annotations
+        }
+
+        return sample
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/base_decoder.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/base_decoder.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,47 +1,47 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-from abc import ABC, abstractmethod
-
-from typing import List, Tuple, Optional, Dict, Any
-
-import numpy as np
-
-
-class BaseDecoder(ABC):
-    def __init__(self) -> None:
-        super().__init__()
-
-    @abstractmethod
-    def __call__(self, data: bytes) -> Tuple[np.ndarray, Optional[Dict[str, Any]]]:
-        """
-        Stub for implementing the decoding procedure
-        called:
-        >>> decoder = BaseDecoder()
-        >>> decoder(encoded_bytes)
-
-        :return Decoded data, metainformation
-        """
-        pass
-
-    @staticmethod
-    @abstractmethod
-    def get_file_extensions() -> List[str]:
-        """
-        Stub for returning allowed file endings
-        """
-        pass
-
-    def __reduce__(self) -> Tuple:
-        return BaseDecoder, tuple()
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+from abc import ABC, abstractmethod
+
+from typing import List, Tuple, Optional, Dict, Any
+
+import numpy as np
+
+
+class BaseDecoder(ABC):
+    def __init__(self) -> None:
+        super().__init__()
+
+    @abstractmethod
+    def __call__(self, data: bytes) -> Tuple[np.ndarray, Optional[Dict[str, Any]]]:
+        """
+        Stub for implementing the decoding procedure
+        called:
+        >>> decoder = BaseDecoder()
+        >>> decoder(encoded_bytes)
+
+        :return Decoded data, metainformation
+        """
+        pass
+
+    @staticmethod
+    @abstractmethod
+    def get_file_extensions() -> List[str]:
+        """
+        Stub for returning allowed file endings
+        """
+        pass
+
+    def __reduce__(self) -> Tuple:
+        return BaseDecoder, tuple()
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/opencv_decoder.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/opencv_decoder.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,100 +1,100 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import io
-from enum import Enum
-from typing import Tuple, Dict, Any, List, Optional
-
-import cv2
-import numpy as np
-from numpy.lib.recfunctions import unstructured_to_structured
-from PIL import ExifTags, Image
-
-from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
-
-
-class ReadingMode(Enum):
-    GRAYSCALE = 1
-    RGB = 2
-    RGBA = 3
-    ANY = 4
-
-
-class OpencvDecoder(BaseDecoder):
-    def __init__(self) -> None:
-        super().__init__()
-
-        self.exif_orientation_tag = None
-        for orientation in ExifTags.TAGS.keys():
-            if ExifTags.TAGS[orientation] == 'Orientation':
-                self.exif_orientation_tag = orientation
-                break
-
-    def __call__(self, data: bytes) -> Tuple[np.ndarray, Optional[Dict[str, Any]]]:
-        image = cv2.imdecode(np.asarray(bytearray(data), dtype=np.uint8), cv2.IMREAD_UNCHANGED)
-
-        # rotate the image according to the exif orientation
-        if self.exif_orientation_tag is not None:
-            # unfortunately, opencv does not expose the exif flags, so that we open the image with pillow
-            # fortunately, pillow opens images in a lazy fashion
-            image_pil = Image.open(io.BytesIO(data))
-            if hasattr(image_pil, '_getexif'):
-                exif = image_pil._getexif()
-                if exif is not None:
-                    exif = dict(exif.items())
-                    if self.exif_orientation_tag in exif:
-                        if exif[self.exif_orientation_tag] == 3:
-                            image = cv2.rotate(image, cv2.ROTATE_180)
-                        elif exif[self.exif_orientation_tag] == 6:
-                            image = cv2.rotate(image, cv2.ROTATE_90_CLOCKWISE)
-                        elif exif[self.exif_orientation_tag] == 8:
-                            image = cv2.rotate(image, cv2.ROTATE_90_COUNTERCLOCKWISE)
-
-        image = self.create_sturctured_array(image)
-
-        return image, dict()
-
-    def __reduce__(self) -> Tuple:
-        return OpencvDecoder, tuple()
-
-    @staticmethod
-    def get_file_extensions() -> List[str]:
-        return ['bmp', 'dib', 'jpeg', 'jpg', 'jpe', 'jp2', 'png', 'pdm', 'pgm', 'ppm', 'sr', 'ras', 'tiff', 'tif']
-
-    @staticmethod
-    def create_sturctured_array(image: np.ndarray, n_chans = None) -> np.ndarray:
-        ### FIXME : remove n_chans kwarg -> bad quick fix
-        ### TODO: check if image is valid (has hight/widht, shape-len is 2 or 3)
-        if n_chans is not None:
-            n_channels = n_chans
-        else:
-            n_channels = image.shape[-1] if len(image.shape) == 3 else 1
-            if len(image.shape) == 2:
-                image = image[:,:,True]
-        if n_channels == 3:
-            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
-        elif n_channels == 4:
-            image = cv2.cvtColor(image, cv2.COLOR_BGRA2RGBA)
-
-        if n_channels == 1:
-            image = unstructured_to_structured(image, np.dtype([('gray', image.dtype)]))
-        elif n_channels == 3:
-            image = unstructured_to_structured(image, np.dtype(
-                [('red', image.dtype), ('green', image.dtype), ('blue', image.dtype)]))
-        elif n_channels == 4:
-            image = unstructured_to_structured(image, np.dtype(
-                [('red', image.dtype), ('green', image.dtype), ('blue', image.dtype), ('alpha', image.dtype)]))
-        else:
-            raise ValueError(f'Cannot decode channel semantics of {image.shape[-1]} channel image.')
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import io
+from enum import Enum
+from typing import Tuple, Dict, Any, List, Optional
+
+import cv2
+import numpy as np
+from numpy.lib.recfunctions import unstructured_to_structured
+from PIL import ExifTags, Image
+
+from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
+
+
+class ReadingMode(Enum):
+    GRAYSCALE = 1
+    RGB = 2
+    RGBA = 3
+    ANY = 4
+
+
+class OpencvDecoder(BaseDecoder):
+    def __init__(self) -> None:
+        super().__init__()
+
+        self.exif_orientation_tag = None
+        for orientation in ExifTags.TAGS.keys():
+            if ExifTags.TAGS[orientation] == 'Orientation':
+                self.exif_orientation_tag = orientation
+                break
+
+    def __call__(self, data: bytes) -> Tuple[np.ndarray, Optional[Dict[str, Any]]]:
+        image = cv2.imdecode(np.asarray(bytearray(data), dtype=np.uint8), cv2.IMREAD_UNCHANGED)
+
+        # rotate the image according to the exif orientation
+        if self.exif_orientation_tag is not None:
+            # unfortunately, opencv does not expose the exif flags, so that we open the image with pillow
+            # fortunately, pillow opens images in a lazy fashion
+            image_pil = Image.open(io.BytesIO(data))
+            if hasattr(image_pil, '_getexif'):
+                exif = image_pil._getexif()
+                if exif is not None:
+                    exif = dict(exif.items())
+                    if self.exif_orientation_tag in exif:
+                        if exif[self.exif_orientation_tag] == 3:
+                            image = cv2.rotate(image, cv2.ROTATE_180)
+                        elif exif[self.exif_orientation_tag] == 6:
+                            image = cv2.rotate(image, cv2.ROTATE_90_CLOCKWISE)
+                        elif exif[self.exif_orientation_tag] == 8:
+                            image = cv2.rotate(image, cv2.ROTATE_90_COUNTERCLOCKWISE)
+
+        image = self.create_sturctured_array(image)
+
+        return image, dict()
+
+    def __reduce__(self) -> Tuple:
+        return OpencvDecoder, tuple()
+
+    @staticmethod
+    def get_file_extensions() -> List[str]:
+        return ['bmp', 'dib', 'jpeg', 'jpg', 'jpe', 'jp2', 'png', 'pdm', 'pgm', 'ppm', 'sr', 'ras', 'tiff', 'tif']
+
+    @staticmethod
+    def create_sturctured_array(image: np.ndarray, n_chans = None) -> np.ndarray:
+        ### FIXME : remove n_chans kwarg -> bad quick fix
+        ### TODO: check if image is valid (has hight/widht, shape-len is 2 or 3)
+        if n_chans is not None:
+            n_channels = n_chans
+        else:
+            n_channels = image.shape[-1] if len(image.shape) == 3 else 1
+            if len(image.shape) == 2:
+                image = image[:,:,True]
+        if n_channels == 3:
+            image = cv2.cvtColor(image, cv2.COLOR_BGR2RGB)
+        elif n_channels == 4:
+            image = cv2.cvtColor(image, cv2.COLOR_BGRA2RGBA)
+
+        if n_channels == 1:
+            image = unstructured_to_structured(image, np.dtype([('gray', image.dtype)]))
+        elif n_channels == 3:
+            image = unstructured_to_structured(image, np.dtype(
+                [('red', image.dtype), ('green', image.dtype), ('blue', image.dtype)]))
+        elif n_channels == 4:
+            image = unstructured_to_structured(image, np.dtype(
+                [('red', image.dtype), ('green', image.dtype), ('blue', image.dtype), ('alpha', image.dtype)]))
+        else:
+            raise ValueError(f'Cannot decode channel semantics of {image.shape[-1]} channel image.')
         return image
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/decoder/pcd_decoder.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/decoder/pcd_decoder.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-#  Copyright 2021 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-import logging
-from enum import Enum
-from typing import Tuple, Dict, Any, List
-
-import numpy as np
-from PIL import ExifTags
-
-from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
-from dataspree.platform_sdk.decoder.serializer import load_pcd, load_ply
-
-logger = logging.getLogger(__name__)
-
-
-class ReadingMode(Enum):
-    GRAYSCALE = 1
-    RGB = 2
-    RGBA = 3
-    ANY = 4
-
-
-class PcdDecoder(BaseDecoder):
-    def __init__(self) -> None:
-        super().__init__()
-
-        # TODO: Document me!
-        self.exif_orientation_tag = None
-        for orientation in ExifTags.TAGS.keys():
-            if ExifTags.TAGS[orientation] == 'Orientation':
-                self.exif_orientation_tag = orientation
-                break
-
-    def __call__(self, data) -> Tuple[np.ndarray, Dict[str, Any]]:
-        return load_pcd(data)
-
-    def __reduce__(self) -> Tuple:
-        return PcdDecoder, tuple()
-
-    @staticmethod
-    def get_file_extensions() -> List[str]:
-        return ['pcd']
-
-
-class PlyDecoder(PcdDecoder):
-    # TODO: Test me!
-    def __init__(self) -> None:
-        super().__init__()
-
-    def __call__(self, data) -> Tuple[np.ndarray, Dict[str, Any]]:
-        return load_ply(data)
-
-    def __reduce__(self) -> Tuple:
-        return PlyDecoder, tuple()
-
-    @staticmethod
-    def get_file_extensions() -> List[str]:
-        return ['ply']
+#  Copyright 2021 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+import logging
+from enum import Enum
+from typing import Tuple, Dict, Any, List
+
+import numpy as np
+from PIL import ExifTags
+
+from dataspree.platform_sdk.decoder.base_decoder import BaseDecoder
+from dataspree.platform_sdk.decoder.serializer import load_pcd, load_ply
+
+logger = logging.getLogger(__name__)
+
+
+class ReadingMode(Enum):
+    GRAYSCALE = 1
+    RGB = 2
+    RGBA = 3
+    ANY = 4
+
+
+class PcdDecoder(BaseDecoder):
+    def __init__(self) -> None:
+        super().__init__()
+
+        # TODO: Document me!
+        self.exif_orientation_tag = None
+        for orientation in ExifTags.TAGS.keys():
+            if ExifTags.TAGS[orientation] == 'Orientation':
+                self.exif_orientation_tag = orientation
+                break
+
+    def __call__(self, data) -> Tuple[np.ndarray, Dict[str, Any]]:
+        return load_pcd(data)
+
+    def __reduce__(self) -> Tuple:
+        return PcdDecoder, tuple()
+
+    @staticmethod
+    def get_file_extensions() -> List[str]:
+        return ['pcd']
+
+
+class PlyDecoder(PcdDecoder):
+    # TODO: Test me!
+    def __init__(self) -> None:
+        super().__init__()
+
+    def __call__(self, data) -> Tuple[np.ndarray, Dict[str, Any]]:
+        return load_ply(data)
+
+    def __reduce__(self) -> Tuple:
+        return PlyDecoder, tuple()
+
+    @staticmethod
+    def get_file_extensions() -> List[str]:
+        return ['ply']
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/http_token_authentication.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/http_token_authentication.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,27 +1,27 @@
-#  Copyright 2022 Data Spree GmbH
-#
-#  Licensed under the Apache License, Version 2.0 (the "License");
-#  you may not use this file except in compliance with the License.
-#  You may obtain a copy of the License at
-#
-#       http://www.apache.org/licenses/LICENSE-2.0
-#
-#  Unless required by applicable law or agreed to in writing, software
-#  distributed under the License is distributed on an "AS IS" BASIS,
-#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-#  See the License for the specific language governing permissions and
-#  limitations under the License.
-
-from requests.auth import AuthBase
-
-
-class HTTPTokenAuth(AuthBase):
-    """Attaches Token Authentication to the given Request object."""
-
-    def __init__(self, token):
-        self.token = token
-
-    def __call__(self, r):
-        # add authentication header with token
-        r.headers['Authorization'] = 'Token {}'.format(self.token)
-        return r
+#  Copyright 2022 Data Spree GmbH
+#
+#  Licensed under the Apache License, Version 2.0 (the "License");
+#  you may not use this file except in compliance with the License.
+#  You may obtain a copy of the License at
+#
+#       http://www.apache.org/licenses/LICENSE-2.0
+#
+#  Unless required by applicable law or agreed to in writing, software
+#  distributed under the License is distributed on an "AS IS" BASIS,
+#  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
+#  See the License for the specific language governing permissions and
+#  limitations under the License.
+
+from requests.auth import AuthBase
+
+
+class HTTPTokenAuth(AuthBase):
+    """Attaches Token Authentication to the given Request object."""
+
+    def __init__(self, token):
+        self.token = token
+
+    def __call__(self, r):
+        # add authentication header with token
+        r.headers['Authorization'] = 'Token {}'.format(self.token)
+        return r
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree/platform_sdk/query.py` & `dataspree-platform-sdk-1.9.3/dataspree/platform_sdk/query.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,117 +1,117 @@
-from abc import ABC, abstractmethod
-from typing import Any, List, Optional, Tuple, Union
-
-from urllib.parse import quote
-
-
-class Condition(ABC):
-    """
-    Class which combines all conditions that can be specified in a query.
-    """
-
-    @abstractmethod
-    def __call__(self, do_url_escape: bool) -> str:
-        """ :return:  The compiled output of the condition """
-        ...
-
-    @staticmethod
-    def create(*args: 'Condition', exclude_empty: bool = True, do_url_escape: bool = True) -> str:
-        """
-        :param args:                The set of Conditions that is to be combined .
-
-        :param exclude_empty:       If true, conditions that are empty (according to the Condition's implementation)
-                                    are removed from the query.
-
-        :param do_url_escape:       Escape variable comparator assignment characters in url if necessary.
-
-        :return:                    The joined compiled output of the arguments.
-        """
-        list_conditions: List[Conditions] = []
-        list_condition: List[Condition] = []
-
-        for arg in args:
-            if arg is not None and (not exclude_empty or arg):
-                (list_conditions if isinstance(arg, Conditions) else list_condition).append(arg)
-
-        if len(list_condition):
-            list_conditions.append(Conditions(*list_condition))
-
-        return '&'.join((c(do_url_escape=do_url_escape) for c in list_conditions))
-
-
-class Conditions(Condition):
-    """ Combination of multiple conditions. """
-
-    def __init__(self, *args: Condition) -> None: self.args: Tuple[(Condition,) * len(args)] = (*args,)
-
-    def __call__(self, do_url_escape: bool) -> str: return '&'.join(a(do_url_escape) for a in self.args if a)
-
-    def __bool__(self) -> bool: return any((a for a in self.args))
-
-
-class Comparator(Condition):
-    """ Condition that expresses a comparison of a variable and a value. """
-
-    def __init__(self, var: str, val: Any, attribute: Any = None, prefix: str = '', infix: str = ',',
-                 suffix: str = ')') -> None:
-        self.var: str = var
-        self.val: Optional[str] = val if val is None else str(val)
-        self.attribute: Optional[str] = None if attribute is None else str(attribute)
-        self.prefix: str = prefix
-        self.infix: str = infix
-        self.suffix: str = suffix
-
-    def __call__(self, do_url_escape: bool) -> str:
-        val, var = (self.val, self.var) if self.attribute is None else (f'{self.var}:{self.val}', self.attribute)
-        val = val if not do_url_escape else quote(val)
-        return ''.join([self.prefix, var, self.infix, val, self.suffix])
-
-    def __bool__(self) -> bool: return self.val is not None
-
-
-class Equal(Comparator):
-    """ Checks equality between a variable and a value. The variable can be part of an attribute. """
-
-    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
-        if attribute is None:
-            super(Equal, self).__init__(var=var, val=val, infix='=', suffix='', attribute=attribute)
-        else:
-            super(Equal, self).__init__(var=var, val=val, prefix='eq(', attribute=attribute)
-
-
-class LessThan(Comparator):
-    """ Checks if a variable is less than a value. The variable can be part of an attribute. """
-
-    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
-        super(LessThan, self).__init__(var=var, val=val, attribute=attribute, prefix='lt(')
-
-
-class GreaterThan(Comparator):
-    """ Checks if a variable is greater than a value. The variable can be part of an attribute. """
-
-    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
-        super(GreaterThan, self).__init__(var=var, val=val, attribute=attribute, prefix='gt(')
-
-
-class LogicalExpression(Condition):
-    """ Condition that expresses a logical combination of multiple child expressions. """
-
-    def __init__(self, op: str, *args: Condition) -> None:
-        self.op = op
-        self.args: Tuple[(Condition,) * len(args)] = (*args,)
-
-    def __call__(self, do_url_escape: bool) -> str:
-        return f'{self.op}(' + ','.join((a(do_url_escape=do_url_escape) for a in self.args)) + ')' \
-            if len(self.args) > 1 else self.args[0](do_url_escape)
-
-
-class And(LogicalExpression):
-    """ Checks if all the child conditions yield true. """
-
-    def __init__(self, arg0: Condition, *args: Condition) -> None: super(And, self).__init__('and', arg0, *args)
-
-
-class Or(LogicalExpression):
-    """ Checks  if any of the child conditions yield true. """
-
-    def __init__(self, arg0: Condition, *args: Condition) -> None: super(Or, self).__init__('or', arg0, *args)
+from abc import ABC, abstractmethod
+from typing import Any, List, Optional, Tuple, Union
+
+from urllib.parse import quote
+
+
+class Condition(ABC):
+    """
+    Class which combines all conditions that can be specified in a query.
+    """
+
+    @abstractmethod
+    def __call__(self, do_url_escape: bool) -> str:
+        """ :return:  The compiled output of the condition """
+        ...
+
+    @staticmethod
+    def create(*args: 'Condition', exclude_empty: bool = True, do_url_escape: bool = True) -> str:
+        """
+        :param args:                The set of Conditions that is to be combined .
+
+        :param exclude_empty:       If true, conditions that are empty (according to the Condition's implementation)
+                                    are removed from the query.
+
+        :param do_url_escape:       Escape variable comparator assignment characters in url if necessary.
+
+        :return:                    The joined compiled output of the arguments.
+        """
+        list_conditions: List[Conditions] = []
+        list_condition: List[Condition] = []
+
+        for arg in args:
+            if arg is not None and (not exclude_empty or arg):
+                (list_conditions if isinstance(arg, Conditions) else list_condition).append(arg)
+
+        if len(list_condition):
+            list_conditions.append(Conditions(*list_condition))
+
+        return '&'.join((c(do_url_escape=do_url_escape) for c in list_conditions))
+
+
+class Conditions(Condition):
+    """ Combination of multiple conditions. """
+
+    def __init__(self, *args: Condition) -> None: self.args: Tuple[(Condition,) * len(args)] = (*args,)
+
+    def __call__(self, do_url_escape: bool) -> str: return '&'.join(a(do_url_escape) for a in self.args if a)
+
+    def __bool__(self) -> bool: return any((a for a in self.args))
+
+
+class Comparator(Condition):
+    """ Condition that expresses a comparison of a variable and a value. """
+
+    def __init__(self, var: str, val: Any, attribute: Any = None, prefix: str = '', infix: str = ',',
+                 suffix: str = ')') -> None:
+        self.var: str = var
+        self.val: Optional[str] = val if val is None else str(val)
+        self.attribute: Optional[str] = None if attribute is None else str(attribute)
+        self.prefix: str = prefix
+        self.infix: str = infix
+        self.suffix: str = suffix
+
+    def __call__(self, do_url_escape: bool) -> str:
+        val, var = (self.val, self.var) if self.attribute is None else (f'{self.var}:{self.val}', self.attribute)
+        val = val if not do_url_escape else quote(val)
+        return ''.join([self.prefix, var, self.infix, val, self.suffix])
+
+    def __bool__(self) -> bool: return self.val is not None
+
+
+class Equal(Comparator):
+    """ Checks equality between a variable and a value. The variable can be part of an attribute. """
+
+    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
+        if attribute is None:
+            super(Equal, self).__init__(var=var, val=val, infix='=', suffix='', attribute=attribute)
+        else:
+            super(Equal, self).__init__(var=var, val=val, prefix='eq(', attribute=attribute)
+
+
+class LessThan(Comparator):
+    """ Checks if a variable is less than a value. The variable can be part of an attribute. """
+
+    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
+        super(LessThan, self).__init__(var=var, val=val, attribute=attribute, prefix='lt(')
+
+
+class GreaterThan(Comparator):
+    """ Checks if a variable is greater than a value. The variable can be part of an attribute. """
+
+    def __init__(self, var: str, val: Optional[Union[str, Any]], attribute: Optional[Union[str, Any]] = None) -> None:
+        super(GreaterThan, self).__init__(var=var, val=val, attribute=attribute, prefix='gt(')
+
+
+class LogicalExpression(Condition):
+    """ Condition that expresses a logical combination of multiple child expressions. """
+
+    def __init__(self, op: str, *args: Condition) -> None:
+        self.op = op
+        self.args: Tuple[(Condition,) * len(args)] = (*args,)
+
+    def __call__(self, do_url_escape: bool) -> str:
+        return f'{self.op}(' + ','.join((a(do_url_escape=do_url_escape) for a in self.args)) + ')' \
+            if len(self.args) > 1 else self.args[0](do_url_escape)
+
+
+class And(LogicalExpression):
+    """ Checks if all the child conditions yield true. """
+
+    def __init__(self, arg0: Condition, *args: Condition) -> None: super(And, self).__init__('and', arg0, *args)
+
+
+class Or(LogicalExpression):
+    """ Checks  if any of the child conditions yield true. """
+
+    def __init__(self, arg0: Condition, *args: Condition) -> None: super(Or, self).__init__('or', arg0, *args)
```

### Comparing `dataspree-platform-sdk-1.9.2/dataspree_platform_sdk.egg-info/SOURCES.txt` & `dataspree-platform-sdk-1.9.3/dataspree_platform_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

