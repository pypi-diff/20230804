# Comparing `tmp/wizata-dsapi-0.2.9.tar.gz` & `tmp/wizata-dsapi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wizata-dsapi-0.2.9.tar", last modified: Wed Jul 12 20:16:16 2023, max compression
+gzip compressed data, was "wizata-dsapi-0.3.1.tar", last modified: Fri Aug  4 10:58:25 2023, max compression
```

## Comparing `wizata-dsapi-0.2.9.tar` & `wizata-dsapi-0.3.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.624118 wizata-dsapi-0.2.9/
--rw-rw-rw-   0        0        0    11556 2023-03-03 13:11:49.000000 wizata-dsapi-0.2.9/LICENSE.txt
--rw-rw-rw-   0        0        0      176 2023-07-12 20:16:16.621516 wizata-dsapi-0.2.9/PKG-INFO
--rw-rw-rw-   0        0        0      323 2023-05-23 08:41:25.000000 wizata-dsapi-0.2.9/README.rst
--rw-rw-rw-   0        0        0       42 2023-07-12 20:16:16.624118 wizata-dsapi-0.2.9/setup.cfg
--rw-rw-rw-   0        0        0     1241 2023-07-12 20:15:59.000000 wizata-dsapi-0.2.9/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.572322 wizata-dsapi-0.2.9/wizata_dsapi/
--rw-rw-rw-   0        0        0     1014 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/__init__.py
--rw-rw-rw-   0        0        0      632 2023-03-25 08:43:45.000000 wizata-dsapi-0.2.9/wizata_dsapi/api_dto.py
--rw-rw-rw-   0        0        0     5763 2023-06-18 19:31:22.000000 wizata-dsapi-0.2.9/wizata_dsapi/dataframe_toolkit.py
--rw-rw-rw-   0        0        0     6145 2023-07-12 07:57:04.000000 wizata-dsapi-0.2.9/wizata_dsapi/datapoint.py
--rw-rw-rw-   0        0        0     1877 2023-05-07 10:55:37.000000 wizata-dsapi-0.2.9/wizata_dsapi/ds_dataframe.py
--rw-rw-rw-   0        0        0     2846 2023-03-20 14:32:36.000000 wizata-dsapi-0.2.9/wizata_dsapi/dsapi_json_encoder.py
--rw-rw-rw-   0        0        0    14903 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/execution.py
--rw-rw-rw-   0        0        0     3810 2023-06-01 19:11:05.000000 wizata-dsapi-0.2.9/wizata_dsapi/experiment.py
--rw-rw-rw-   0        0        0     9999 2023-06-20 18:59:20.000000 wizata-dsapi-0.2.9/wizata_dsapi/mlmodel.py
--rw-rw-rw-   0        0        0     1594 2023-06-20 16:08:31.000000 wizata-dsapi-0.2.9/wizata_dsapi/model_toolkit.py
--rw-rw-rw-   0        0        0    17900 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/pipeline.py
--rw-rw-rw-   0        0        0     2136 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.9/wizata_dsapi/plot.py
--rw-rw-rw-   0        0        0    18221 2023-07-10 09:09:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/request.py
--rw-rw-rw-   0        0        0     8716 2023-06-14 12:20:26.000000 wizata-dsapi-0.2.9/wizata_dsapi/script.py
--rw-rw-rw-   0        0        0     7221 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/template.py
--rw-rw-rw-   0        0        0     2599 2023-07-03 10:20:49.000000 wizata-dsapi-0.2.9/wizata_dsapi/twin.py
--rw-rw-rw-   0        0        0     2762 2023-07-10 13:54:24.000000 wizata-dsapi-0.2.9/wizata_dsapi/twinregistration.py
--rw-rw-rw-   0        0        0      489 2023-03-28 10:24:12.000000 wizata-dsapi-0.2.9/wizata_dsapi/wizard_function.py
--rw-rw-rw-   0        0        0    56573 2023-07-12 20:15:59.000000 wizata-dsapi-0.2.9/wizata_dsapi/wizata_dsapi_client.py
-drwxrwxrwx   0        0        0        0 2023-07-12 20:16:16.614691 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/
--rw-rw-rw-   0        0        0      176 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      730 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      555 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-07-12 20:16:16.000000 wizata-dsapi-0.2.9/wizata_dsapi.egg-info/top_level.txt
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 10:58:25.442745 wizata-dsapi-0.3.1/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    11356 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/LICENSE.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 10:58:25.442631 wizata-dsapi-0.3.1/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      315 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/README.rst
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       38 2023-08-04 10:58:25.442786 wizata-dsapi-0.3.1/setup.cfg
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1203 2023-08-04 10:58:07.000000 wizata-dsapi-0.3.1/setup.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 10:58:25.441394 wizata-dsapi-0.3.1/wizata_dsapi/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1029 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.1/wizata_dsapi/__init__.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      605 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/api_dto.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3807 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.1/wizata_dsapi/context.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5588 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/dataframe_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     5933 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/datapoint.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1815 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/ds_dataframe.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2772 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/dsapi_json_encoder.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    14533 2023-08-04 10:57:55.000000 wizata-dsapi-0.3.1/wizata_dsapi/execution.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     3711 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/experiment.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    10306 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.1/wizata_dsapi/mlmodel.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     1552 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/model_toolkit.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    18380 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.1/wizata_dsapi/pipeline.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2067 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/plot.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    17759 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/request.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     8485 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/script.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     7110 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.1/wizata_dsapi/template.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     2517 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/twin.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)     4675 2023-08-02 08:42:21.000000 wizata-dsapi-0.3.1/wizata_dsapi/twinregistration.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      471 2023-07-20 17:32:08.000000 wizata-dsapi-0.3.1/wizata_dsapi/wizard_function.py
+-rw-r--r--   0 wizata.jph   (502) staff       (20)    57650 2023-07-31 10:14:43.000000 wizata-dsapi-0.3.1/wizata_dsapi/wizata_dsapi_client.py
+drwxr-xr-x   0 wizata.jph   (502) staff       (20)        0 2023-08-04 10:58:25.442449 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      169 2023-08-04 10:58:25.000000 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/PKG-INFO
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      754 2023-08-04 10:58:25.000000 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)        1 2023-08-04 10:58:25.000000 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)      555 2023-08-04 10:58:25.000000 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/requires.txt
+-rw-r--r--   0 wizata.jph   (502) staff       (20)       13 2023-08-04 10:58:25.000000 wizata-dsapi-0.3.1/wizata_dsapi.egg-info/top_level.txt
```

### Comparing `wizata-dsapi-0.2.9/LICENSE.txt` & `wizata-dsapi-0.3.1/LICENSE.txt`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,201 +1,201 @@
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
    limitations under the License.
```

### Comparing `wizata-dsapi-0.2.9/setup.py` & `wizata-dsapi-0.3.1/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from setuptools import setup
-
-setup(
-    name='wizata-dsapi',
-    version='0.2.9',
-    description='Wizata Data Science Toolkit',
-    author='Wizata S.A.',
-    author_email='info@wizata.com',
-    packages=['wizata_dsapi'],
-    install_requires=[
-        'dill==0.3.6',
-        'pandas==1.5.3',
-        'numpy==1.23.5',
-        'matplotlib==3.7.1',
-        'protobuf==3.19.6',
-        "tensorflow==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "tensorflow-macos==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
-        "keras==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
-        "keras==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
-        'tensorflow_probability==0.15.0',
-        'scikit-learn==1.2.2',
-        'plotly==5.13.1',
-        'adtk==0.6.2',
-        'scipy==1.10.1',
-        'xgboost==1.7.4',
-        'joblib==1.2.0',
-        'requests==2.28.2',
-        'setuptools==67.6.0',
-        'explainerdashboard==0.4.2.1',
-        'ipywidgets==8.0.4',
-        'kaleido==0.2.1',
-        'pytest==7.2.2',
-        'pytest-cov==4.0.0',
-        'shapely==2.0.1',
-        'pyodbc==4.0.35',
-        'msal==1.21.0'
-    ]
-)
+from setuptools import setup
+
+setup(
+    name='wizata-dsapi',
+    version='0.3.1',
+    description='Wizata Data Science Toolkit',
+    author='Wizata S.A.',
+    author_email='info@wizata.com',
+    packages=['wizata_dsapi'],
+    install_requires=[
+        'dill==0.3.6',
+        'pandas==1.5.3',
+        'numpy==1.23.5',
+        'matplotlib==3.7.1',
+        'protobuf==3.19.6',
+        "tensorflow==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "tensorflow-macos==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        "keras==2.7; sys_platform != 'darwin' or platform_machine != 'arm64'",
+        "keras==2.11.0; sys_platform == 'darwin' and platform_machine == 'arm64'",
+        'tensorflow_probability==0.15.0',
+        'scikit-learn==1.2.2',
+        'plotly==5.13.1',
+        'adtk==0.6.2',
+        'scipy==1.10.1',
+        'xgboost==1.7.4',
+        'joblib==1.2.0',
+        'requests==2.28.2',
+        'setuptools==67.6.0',
+        'explainerdashboard==0.4.2.1',
+        'ipywidgets==8.0.4',
+        'kaleido==0.2.1',
+        'pytest==7.2.2',
+        'pytest-cov==4.0.0',
+        'shapely==2.0.1',
+        'pyodbc==4.0.35',
+        'msal==1.21.0'
+    ]
+)
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/dataframe_toolkit.py` & `wizata-dsapi-0.3.1/wizata_dsapi/dataframe_toolkit.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,175 +1,175 @@
-import pandas
-import io
-from datetime import datetime, timedelta, timezone
-import re
-
-
-def validate(df: pandas.DataFrame) -> pandas.DataFrame:
-    """
-    validate dataframe format to match supported Wizata format.
-    :param df: dataframe to validate.
-    :return: validated and formatted df - raise error if not valid.
-    """
-    if not isinstance(df.index, pandas.DatetimeIndex):
-        raise TypeError(f'df.index is not a DatatimeIndex {df.index}')
-
-    if df.index.name != "Timestamp":
-        df.index.name = "Timestamp"
-
-    if len(df.axes) < 2 or df.axes[1].name != "sensorId":
-        df.rename_axis("sensorId", axis="columns", inplace=True)
-
-    df = df.astype(float)
-
-    return df
-
-
-def df_to_csv(df: pandas.DataFrame) -> bytes:
-    """
-    Convert the DataFrame to a strongly formatted CSV.
-    :param df: pandas DataFrame compatible with Wizata standards.
-    :return: bytes containing the full CSV file.
-    """
-    b_buf = io.BytesIO()
-
-    df.to_csv(b_buf,
-              date_format="%Y-%m-%d-%H-%M-%S-%f",
-              sep=",",
-              decimal=".",
-              encoding="utf-8")
-
-    b_buf.seek(0)
-    return b_buf.read()
-
-
-def df_from_csv(b_data: bytes) -> pandas.DataFrame:
-    """
-    Convert the bytes to a pandas.DataFrame.
-    :param b_data: bytes representing a CSV file.
-    :return: pandas DataFrame formatted.
-    """
-    b_buf = io.BytesIO(b_data)
-
-    df = pandas.read_csv(b_buf,
-                         sep=",",
-                         decimal=".",
-                         encoding="utf-8")
-
-    # detect timestamp column
-    if "timestamp" in df.columns:
-        df = df.rename(columns={'timestamp': 'Timestamp'})
-    if "Timestamp" not in df.columns:
-        raise ValueError('Cannot read dataframe as no Timestamp columns exists.')
-
-    # detect timestamp type
-    if df['Timestamp'].dtypes == 'int64':
-        df['Timestamp'] = pandas.to_datetime(df['Timestamp'], unit="ms")
-    elif df['Timestamp'].dtypes == 'object':
-        df['Timestamp'] = df['Timestamp'].apply(lambda _: datetime.strptime(_, "%Y-%m-%d-%H-%M-%S-%f"))
-
-    df = df.set_index('Timestamp')
-    df.rename_axis("sensorId", axis="columns", inplace=True)
-
-    return df
-
-
-def df_from_json(json):
-    """
-    Convert a dictionary dataframe using JSON convention into a panda Dataframe.
-
-    Dataframe must contain a timestamp column and be compatible to float data types.
-
-    :param json: JSON formatted dataframe.
-    :return: panda Dataframe
-    """
-    df = pandas.DataFrame.from_dict(json, orient='columns')
-    df = df.set_index('Timestamp')
-
-    if df.index.dtype == 'int64':
-        df.index = [datetime.fromtimestamp(i) for i in (df.index / 1000).astype(int)]
-        df.index.name = 'Timestamp'
-    if not isinstance(df.index, pandas.DatetimeIndex):
-        raise TypeError("Unexpected type {0}".format(df.index))
-
-    df.rename_axis("sensorId", axis="columns", inplace=True)
-    return df
-
-
-def df_to_json(df: pandas.DataFrame):
-    """
-    Convert a panda Dataframe to a JSON compatible dictionary.
-
-    Dataframe must be compatible to Wizata format using Timestamp index and float data types.
-
-    :param df: panda Dataframe to convert.
-    :return: dictionary representing JSON compatible dataframe.
-    """
-    df_json = {
-        "Timestamp": list(df.index)
-    }
-    for col in list(df.columns):
-        if col != 'Timestamp':
-            df_json[col] = list(df[col].values.astype(float))
-        else:
-            df_json[col] = list(df[col].values)
-    return df_json
-
-
-def generate_epoch(formatted_string: str, now=None):
-    """
-    generate an epoch based on a formatted string (e.g. now+6h) - see documentation.
-    * now = datetime.utcnow() can be override
-    * units = 'y' = 365d, 'M'=30d , 'w'=7d , 'd'=24h , 'h'=60m, 'm'=60s , 's'=1000'ms'
-    * operators = '+' or '-'
-    :param formatted_string: formatted epoch representation using relative time.
-    :param now: override now datetime.
-    :return: epoch in ms.
-    """
-    if now is None:
-        now = datetime.utcnow()
-
-    pattern = r'^now([+-]\d+([yMwdHhms]{1,2}))?$'
-    match = re.match(pattern, formatted_string)
-    if not match:
-        raise ValueError(f"invalid time delay format {formatted_string}")
-
-    operator = match.group(1)[0] if match.group(1) else None
-    value_unit_str = match.group(1)[1:] if match.group(1) else None
-
-    if value_unit_str:
-        value_str = re.search(r'\d+', value_unit_str).group()
-        unit_str = re.search(r'[yMwdHhms]{1,2}', value_unit_str).group()
-
-        value = int(value_str)
-
-        if unit_str == 'y':
-            delta = timedelta(days=365) * value
-        elif unit_str == 'M':
-            delta = timedelta(days=30) * value
-        elif unit_str == 'w':
-            delta = timedelta(days=7) * value
-        elif unit_str == 'd':
-            delta = timedelta(days=value)
-        elif unit_str == 'H' or unit_str == 'h':
-            delta = timedelta(hours=value)
-        elif unit_str == 'm':
-            delta = timedelta(minutes=value)
-        elif unit_str == 's':
-            delta = timedelta(seconds=value)
-        elif unit_str == 'ms':
-            delta = timedelta(milliseconds=value)
-        else:
-            raise ValueError("invalid time unit")
-
-        if operator == '+':
-            timestamp = now + delta
-        elif operator == '-':
-            timestamp = now - delta
-        else:
-            raise ValueError("invalid time delay format")
-    else:
-        timestamp = now
-
-    epoch = datetime.utcfromtimestamp(0)
-    timestamp_ms = int((timestamp - epoch).total_seconds() * 1000)
-    return timestamp_ms
+import pandas
+import io
+from datetime import datetime, timedelta, timezone
+import re
+
+
+def validate(df: pandas.DataFrame) -> pandas.DataFrame:
+    """
+    validate dataframe format to match supported Wizata format.
+    :param df: dataframe to validate.
+    :return: validated and formatted df - raise error if not valid.
+    """
+    if not isinstance(df.index, pandas.DatetimeIndex):
+        raise TypeError(f'df.index is not a DatatimeIndex {df.index}')
+
+    if df.index.name != "Timestamp":
+        df.index.name = "Timestamp"
+
+    if len(df.axes) < 2 or df.axes[1].name != "sensorId":
+        df.rename_axis("sensorId", axis="columns", inplace=True)
+
+    df = df.astype(float)
+
+    return df
+
+
+def df_to_csv(df: pandas.DataFrame) -> bytes:
+    """
+    Convert the DataFrame to a strongly formatted CSV.
+    :param df: pandas DataFrame compatible with Wizata standards.
+    :return: bytes containing the full CSV file.
+    """
+    b_buf = io.BytesIO()
+
+    df.to_csv(b_buf,
+              date_format="%Y-%m-%d-%H-%M-%S-%f",
+              sep=",",
+              decimal=".",
+              encoding="utf-8")
+
+    b_buf.seek(0)
+    return b_buf.read()
+
+
+def df_from_csv(b_data: bytes) -> pandas.DataFrame:
+    """
+    Convert the bytes to a pandas.DataFrame.
+    :param b_data: bytes representing a CSV file.
+    :return: pandas DataFrame formatted.
+    """
+    b_buf = io.BytesIO(b_data)
+
+    df = pandas.read_csv(b_buf,
+                         sep=",",
+                         decimal=".",
+                         encoding="utf-8")
+
+    # detect timestamp column
+    if "timestamp" in df.columns:
+        df = df.rename(columns={'timestamp': 'Timestamp'})
+    if "Timestamp" not in df.columns:
+        raise ValueError('Cannot read dataframe as no Timestamp columns exists.')
+
+    # detect timestamp type
+    if df['Timestamp'].dtypes == 'int64':
+        df['Timestamp'] = pandas.to_datetime(df['Timestamp'], unit="ms")
+    elif df['Timestamp'].dtypes == 'object':
+        df['Timestamp'] = df['Timestamp'].apply(lambda _: datetime.strptime(_, "%Y-%m-%d-%H-%M-%S-%f"))
+
+    df = df.set_index('Timestamp')
+    df.rename_axis("sensorId", axis="columns", inplace=True)
+
+    return df
+
+
+def df_from_json(json):
+    """
+    Convert a dictionary dataframe using JSON convention into a panda Dataframe.
+
+    Dataframe must contain a timestamp column and be compatible to float data types.
+
+    :param json: JSON formatted dataframe.
+    :return: panda Dataframe
+    """
+    df = pandas.DataFrame.from_dict(json, orient='columns')
+    df = df.set_index('Timestamp')
+
+    if df.index.dtype == 'int64':
+        df.index = [datetime.fromtimestamp(i) for i in (df.index / 1000).astype(int)]
+        df.index.name = 'Timestamp'
+    if not isinstance(df.index, pandas.DatetimeIndex):
+        raise TypeError("Unexpected type {0}".format(df.index))
+
+    df.rename_axis("sensorId", axis="columns", inplace=True)
+    return df
+
+
+def df_to_json(df: pandas.DataFrame):
+    """
+    Convert a panda Dataframe to a JSON compatible dictionary.
+
+    Dataframe must be compatible to Wizata format using Timestamp index and float data types.
+
+    :param df: panda Dataframe to convert.
+    :return: dictionary representing JSON compatible dataframe.
+    """
+    df_json = {
+        "Timestamp": list(df.index)
+    }
+    for col in list(df.columns):
+        if col != 'Timestamp':
+            df_json[col] = list(df[col].values.astype(float))
+        else:
+            df_json[col] = list(df[col].values)
+    return df_json
+
+
+def generate_epoch(formatted_string: str, now=None):
+    """
+    generate an epoch based on a formatted string (e.g. now+6h) - see documentation.
+    * now = datetime.utcnow() can be override
+    * units = 'y' = 365d, 'M'=30d , 'w'=7d , 'd'=24h , 'h'=60m, 'm'=60s , 's'=1000'ms'
+    * operators = '+' or '-'
+    :param formatted_string: formatted epoch representation using relative time.
+    :param now: override now datetime.
+    :return: epoch in ms.
+    """
+    if now is None:
+        now = datetime.utcnow()
+
+    pattern = r'^now([+-]\d+([yMwdHhms]{1,2}))?$'
+    match = re.match(pattern, formatted_string)
+    if not match:
+        raise ValueError(f"invalid time delay format {formatted_string}")
+
+    operator = match.group(1)[0] if match.group(1) else None
+    value_unit_str = match.group(1)[1:] if match.group(1) else None
+
+    if value_unit_str:
+        value_str = re.search(r'\d+', value_unit_str).group()
+        unit_str = re.search(r'[yMwdHhms]{1,2}', value_unit_str).group()
+
+        value = int(value_str)
+
+        if unit_str == 'y':
+            delta = timedelta(days=365) * value
+        elif unit_str == 'M':
+            delta = timedelta(days=30) * value
+        elif unit_str == 'w':
+            delta = timedelta(days=7) * value
+        elif unit_str == 'd':
+            delta = timedelta(days=value)
+        elif unit_str == 'H' or unit_str == 'h':
+            delta = timedelta(hours=value)
+        elif unit_str == 'm':
+            delta = timedelta(minutes=value)
+        elif unit_str == 's':
+            delta = timedelta(seconds=value)
+        elif unit_str == 'ms':
+            delta = timedelta(milliseconds=value)
+        else:
+            raise ValueError("invalid time unit")
+
+        if operator == '+':
+            timestamp = now + delta
+        elif operator == '-':
+            timestamp = now - delta
+        else:
+            raise ValueError("invalid time delay format")
+    else:
+        timestamp = now
+
+    epoch = datetime.utcfromtimestamp(0)
+    timestamp_ms = int((timestamp - epoch).total_seconds() * 1000)
+    return timestamp_ms
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/ds_dataframe.py` & `wizata-dsapi-0.3.1/wizata_dsapi/ds_dataframe.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,62 @@
-import uuid
-import pandas
-from .api_dto import ApiDto
-
-
-class DSDataFrame(ApiDto):
-    """
-    A DS Dataframe is a definition of a pandas Dataframe that can be stored and shared on Wizata.
-
-    :ivar df_id: The UUID of the dataframe.
-    :ivar generatedById: The UUID of the Execution from which the dataframe was created.
-    :ivar dataframe: Pandas Dataframe.
-    """
-
-    def __init__(self, df_id=None, dataframe=None):
-        if df_id is None:
-            self.df_id = uuid.uuid4()
-        else:
-            self.df_id = df_id
-        self.generatedById = None
-        self.dataframe = dataframe
-
-    def api_id(self) -> str:
-        """
-        Id of the dataframe (df_id)
-
-        :return: string formatted UUID of the dataframe.
-        """
-        return str(self.df_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate dataframes.
-        :return: Endpoint name.
-        """
-        return "Dataframes"
-
-    def from_json(self, obj):
-        """
-        Load the Dataframe entity from a dictionary representation of the dataframe.
-        Doesn't load the dataframe itself, you can use df_from_json to fetch it from JSON, CSV or other formats.
-
-        :param obj: Dict version of the Dataframe.
-        """
-        if "id" in obj.keys():
-            self.df_id = uuid.UUID(obj["id"])
-        if "generatedById" in obj.keys():
-            self.generatedById = obj["generatedById"]
-
-    def to_json(self):
-        """
-        Convert the dataframe to a dictionary compatible to JSON format.
-
-        :return: dictionary representation of the Dataframe object.
-        """
-        obj = {
-            "id": str(self.df_id)
-        }
-        if self.generatedById is not None:
-            obj["generatedById"] = str(self.generatedById)
-        return obj
-
+import uuid
+import pandas
+from .api_dto import ApiDto
+
+
+class DSDataFrame(ApiDto):
+    """
+    A DS Dataframe is a definition of a pandas Dataframe that can be stored and shared on Wizata.
+
+    :ivar df_id: The UUID of the dataframe.
+    :ivar generatedById: The UUID of the Execution from which the dataframe was created.
+    :ivar dataframe: Pandas Dataframe.
+    """
+
+    def __init__(self, df_id=None, dataframe=None):
+        if df_id is None:
+            self.df_id = uuid.uuid4()
+        else:
+            self.df_id = df_id
+        self.generatedById = None
+        self.dataframe = dataframe
+
+    def api_id(self) -> str:
+        """
+        Id of the dataframe (df_id)
+
+        :return: string formatted UUID of the dataframe.
+        """
+        return str(self.df_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate dataframes.
+        :return: Endpoint name.
+        """
+        return "Dataframes"
+
+    def from_json(self, obj):
+        """
+        Load the Dataframe entity from a dictionary representation of the dataframe.
+        Doesn't load the dataframe itself, you can use df_from_json to fetch it from JSON, CSV or other formats.
+
+        :param obj: Dict version of the Dataframe.
+        """
+        if "id" in obj.keys():
+            self.df_id = uuid.UUID(obj["id"])
+        if "generatedById" in obj.keys():
+            self.generatedById = obj["generatedById"]
+
+    def to_json(self):
+        """
+        Convert the dataframe to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Dataframe object.
+        """
+        obj = {
+            "id": str(self.df_id)
+        }
+        if self.generatedById is not None:
+            obj["generatedById"] = str(self.generatedById)
+        return obj
+
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/execution.py` & `wizata-dsapi-0.3.1/wizata_dsapi/execution.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,394 +1,395 @@
-import json
-import pickle
-import uuid
-
-import string
-import random
-import pandas
-import wizata_dsapi
-from enum import Enum
-
-from .dataframe_toolkit import df_to_json, df_from_json
-from .api_dto import ApiDto
-from .ds_dataframe import DSDataFrame
-from .mlmodel import MLModel
-from .plot import Plot
-from .request import Request
-from .script import Script
-from .pipeline import Pipeline
-from .experiment import Experiment
-
-
-class ExecutionStatus(Enum):
-    RECEIVED = "received"
-    QUEUED = "queued"
-    STARTED = "started"
-    COMPLETED = "completed"
-    FAILED = "failed"
-
-
-class Execution(ApiDto):
-    """
-    Execution Context defining an experimentation historical run.
-
-    Execution can be run in the platform or directly within your script.
-    Used also as context within a Script function, used the following method:
-        - append_model - To store a generated model
-        - append_plot - To store a plot
-        - result_dataframe - To set the panda Dataframe as output
-
-    :ivar execution_id: UUID of the Execution on Wizata App.
-    :ivar experiment_id: UUID of the Experiment on which this Experiment is linked.
-    :ivar warnings: Warning about the Execution.
-
-    Data
-
-    :ivar request: Request or JSON formatted object to fecth data on Wizata App.
-    :ivar input_ds_dataframe: DS Dataframe containing the panda Dataframe input.
-    :ivar dataframe: shortcut to Pandas DataFrame used as input.
-
-    Inputs
-
-    :ivar script: Script to execute against the input data.
-    :ivar ml_model: Trained ML Model to use against the input data.
-    :ivar function: Name of a Wizata built-in function.
-    :ivar isAnomalyDetection: True if this execution triggers integrated Anomaly Detection within Wizata.
-    :ivar properties: configuration and variables.
-
-    Outputs
-
-    :ivar models: Trained Machine Learning Models.
-    :ivar plots: Figures generated with Plotly.
-    :ivar anomalies: Anomalies detected.
-    :ivar output_ds_dataframe: Output dataframe generated by the Script or Model.
-    """
-
-    keys = [
-        'target_feat',
-        'sensitivity',
-        'aggregations',
-        'restart_filter',
-        'interval'
-    ]
-
-    def __init__(self, execution_id=None, properties: dict = None, pipeline: Pipeline = None, experiment: Experiment = None):
-
-        # Id
-        if execution_id is None:
-            execution_id = uuid.uuid4()
-        self.execution_id = execution_id
-
-        # Experiment
-        if experiment is not None:
-            self.experiment_id = experiment.experiment_id
-        else:
-            self.experiment_id = None
-
-        # Inputs Properties (load)
-        self.script = None
-        self.request = None
-
-        if properties is None:
-            properties = {}
-        self.properties = properties
-
-        self.input_ds_dataframe = None
-        self.ml_model = None
-        self.function = None
-        self.isAnomalyDetection = False
-        self.pipeline = pipeline
-        self.status = None
-
-        # created/updated
-        self.createdById = None
-        self.createdDate = None
-        self.updatedById = None
-        self.updatedDate = None
-
-        # Outputs Properties (generated by Execution)
-        self.models = []
-        self.anomalies = []
-        self.plots = []
-        self.dataframes = []
-        self.output_ds_dataframe = None
-        self.warnings = None
-
-    def _get_dataframe(self):
-        if self.input_ds_dataframe is None:
-            return None
-        else:
-            return self.input_ds_dataframe.dataframe
-
-    def _set_dataframe(self, value):
-        if not isinstance(value, pandas.DataFrame):
-            raise ValueError("dataframe must be a panda dataframe.")
-        self.input_ds_dataframe = DSDataFrame()
-        self.input_ds_dataframe.dataframe = value
-
-    def _del_dataframe(self):
-        del self.input_ds_dataframe
-
-    dataframe = property(
-        fget=_get_dataframe,
-        fset=_set_dataframe,
-        fdel=_del_dataframe,
-        doc="Input Pandas Dataframe (for id fetch 'input_ds_dataframe.df_id')"
-    )
-
-    def _get_result_dataframe(self):
-        if self.output_ds_dataframe is None:
-            return None
-        else:
-            return self.output_ds_dataframe.dataframe
-
-    def _set_result_dataframe(self, value):
-        if not isinstance(value, pandas.DataFrame):
-            raise ValueError("dataframe must be a panda dataframe.")
-        self.output_ds_dataframe = DSDataFrame()
-        self.output_ds_dataframe.dataframe = value
-
-    def _del_result_dataframe(self):
-        del self.output_ds_dataframe
-
-    result_dataframe = property(
-        fget=_get_result_dataframe,
-        fset=_set_result_dataframe,
-        fdel=_del_result_dataframe,
-        doc="Output Pandas Dataframe (for id fetch 'output_ds_dataframe.df_id')"
-    )
-
-    def append_plot(self, figure, name="Unkwown"):
-        """
-        Append a plot to the context.
-
-        :param figure: Plotly figure.
-        :param name: Name of the plot.
-        :return: Plot object prepared.
-        """
-        plot = Plot()
-        plot.name = name
-        plot.experiment_id = self.experiment_id
-        plot.figure = figure
-        self.plots.append(plot)
-        return plot
-
-    def append_model(self, trained_model, input_columns, key=None, output_columns=None, has_anomalies=False, scaler=None):
-        """
-        Append a Trained ML Model to the context.
-
-        :param key: Model key to logically identify the model - if not provided a random
-        :param trained_model: Trained Model to be stored as a pickled object.
-        :param input_columns: List of str defining input columns to call the model (df.columns)
-        :param output_columns: List of output columns - Optional as can be detected automatically during validation.
-        :param has_anomalies: False by default, define if the model set anomalies
-        :param scaler: Scaler to be stored if necessary.
-        :return: ML Model object prepared.
-        """
-        ml_model = MLModel()
-
-        if key is None:
-            key = generate_key()
-        ml_model.key = key
-        ml_model.trained_model = trained_model
-        ml_model.scaler = scaler
-
-        ml_model.input_columns = input_columns
-        ml_model.output_columns = output_columns
-
-        ml_model.has_anomalies = has_anomalies
-
-        self.models.append(ml_model)
-        return ml_model
-
-    def api_id(self) -> str:
-        """
-        Id of the execution (execution_id)
-
-        :return: string formatted UUID of the Execution.
-        """
-        return str(self.execution_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate execution.
-        :return: Endpoint name.
-        """
-        return "Executions"
-
-    def to_json(self):
-        """
-        Convert to a json version of Execution definition.
-        By default, use DS API format.
-        """
-        obj = {
-            "id": str(self.execution_id)
-        }
-        if self.experiment_id is not None:
-            obj["experimentId"] = str(self.experiment_id)
-        if self.request is not None:
-            obj["request"] = json.dumps(self.request.to_json())
-        if self.properties is not None:
-            obj["properties"] = json.dumps(self.properties)
-        if self.dataframe is not None:
-            obj["dataframe"] = df_to_json(self.dataframe)
-        # if self.input_ds_dataframe is not None:
-        #     obj["dataframeId"] = str(self.input_ds_dataframe.df_id)
-        if self.script is not None:
-            obj["scriptId"] = str(self.script.script_id)
-        if self.ml_model is not None:
-            obj["mlModelId"] = str(self.ml_model.model_id)
-        if self.pipeline is not None:
-            obj["pipelineId"] = str(self.pipeline.pipeline_id)
-        if self.function is not None:
-            obj["function"] = self.function
-        if self.isAnomalyDetection:
-            obj["isAnomalyDetection"] = str(True)
-        if self.plots is not None:
-            plots_ids = []
-            for plot in self.plots:
-                plots_ids.append(
-                    {
-                        "id": str(plot.plot_id)
-                    }
-                )
-            obj["plots"] = plots_ids
-        if self.models is not None:
-            models_json = []
-            for ml_model in self.models:
-                models_json.append({"id": str(ml_model.model_id)})
-            obj["models"] = models_json
-        if self.anomalies is not None:
-            obj["anomaliesList"] = json.dumps(self.anomalies)
-        # if self.result_dataframe is not None:
-        #     obj["resultDataframe"] = {
-        #         "id": str(self.output_ds_dataframe.df_id)
-        #     }
-        if self.createdById is not None:
-            obj["createdById"] = self.createdById
-        if self.createdDate is not None:
-            obj["createdDate"] = self.createdDate
-        if self.updatedById is not None:
-            obj["updatedById"] = self.updatedById
-        if self.updatedDate is not None:
-            obj["updatedDate"] = self.updatedDate
-        if self.warnings is not None:
-            obj["warnings"] = self.warnings
-        if self.status is not None and isinstance(self.status, ExecutionStatus):
-            obj["status"] = self.status.value
-        return obj
-
-    def from_json(self, obj):
-        """
-        Load an execution from a stored JSON model.
-        :param obj: dictionnary representing an execution.
-        """
-        if "id" in obj.keys():
-            self.execution_id = uuid.UUID(obj["id"])
-        if "experimentId" in obj.keys() and obj["experimentId"] is not None:
-            self.experiment_id = uuid.UUID(obj["experimentId"])
-        if "request" in obj.keys() and obj["request"] is not None:
-            self.request = Request()
-            if isinstance(obj["request"], str):
-                self.request.from_json(json.loads(obj["request"]))
-                self.copy_properties(json.loads(obj["request"]))
-            else:
-                self.request.from_json(obj["request"])
-                self.copy_properties(obj["request"])
-        if "properties" in obj.keys() and obj["properties"] is not None:
-            if isinstance(obj["properties"], str):
-                self.add_properties(json.loads(obj["properties"]))
-            else:
-                self.add_properties(obj["properties"])
-        if "dataframe" in obj.keys() and obj["dataframe"] is not None:
-            if isinstance(obj["dataframe"], str):
-                self.request.from_json(json.loads(obj["dataframe"]))
-            else:
-                self.dataframe = df_from_json(obj["dataframe"])
-        # elif "dataframeId" in obj.keys() and obj["dataframeId"] is not None:
-        #     self.input_ds_dataframe = DSDataFrame(df_id=uuid.UUID(obj["dataframeId"]))
-        if "scriptId" in obj.keys() and obj["scriptId"] is not None:
-            self.script = Script()
-            self.script.script_id = uuid.UUID(obj["scriptId"])
-        if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
-            self.pipeline = Pipeline()
-            self.pipeline.pipeline_id = uuid.UUID(obj["pipelineId"])
-        if "mlModelId" in obj.keys() and obj["mlModelId"] is not None:
-            self.ml_model = MLModel()
-            self.ml_model.model_id = uuid.UUID(obj["mlModelId"])
-        if "function" in obj.keys() and obj["function"] is not None:
-            self.function = obj["function"]
-        if "isAnomalyDetection" in obj.keys() and obj["isAnomalyDetection"] is not None:
-            if isinstance(obj["isAnomalyDetection"], bool):
-                self.isAnomalyDetection = obj["isAnomalyDetection"]
-            else:
-                self.isAnomalyDetection = obj["isAnomalyDetection"] == 'True'
-        if "createdById" in obj.keys() and obj["createdById"] is not None:
-            self.createdById = obj["createdById"]
-        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
-            self.createdDate = obj["createdDate"]
-        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
-            self.updatedById = obj["updatedById"]
-        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
-            self.updatedDate = obj["updatedDate"]
-        if "warnings" in obj.keys() and obj["warnings"] is not None:
-            self.warnings = obj["warnings"]
-        if "anomaliesList" in obj.keys() and obj["anomaliesList"] is not None:
-            if isinstance(obj["anomaliesList"], str):
-                self.anomalies = json.loads(obj["anomaliesList"])
-            else:
-                self.anomalies = obj["anomaliesList"]
-        if "status" in obj.keys():
-            self.status = ExecutionStatus(str(obj["status"]))
-
-    def to_pickle(self):
-        """
-        Convert the Execution to a pickle object.
-        :return: Pickle object.
-        """
-        return pickle.dumps(self)
-
-    def add_properties(self, obj: dict):
-        """
-        load properties from a dictionary
-
-        :param obj: dictionary with potential properties
-        """
-        for key in obj.keys():
-            if self.properties is None:
-                self.properties = {}
-            self.properties[key] = obj[key]
-
-    def copy_properties(self, obj: dict):
-        """
-        copy properties from a dictionary originating from a Request object.
-        filtering on specific properties (Execution.keys)
-
-        :param obj: dictionary with potential properties
-        """
-        for key in Execution.keys:
-            if key in obj:
-                if self.properties is None:
-                    self.properties = {}
-                self.properties[key] = obj[key]
-
-    def get_interval(self) -> int:
-        """
-        Determine interval from either request, properties or loaded dataframe.
-        :return:
-        """
-        if self.request is not None:
-            interval = self.request.interval
-        elif self.properties['aggregations'] is not None \
-                and self.properties['aggregations']['interval'] is not None:
-            interval = int(self.properties["aggregations"]["interval"] / 1000)
-        elif self.properties['interval'] is not None:
-            interval = int(self.properties['interval'] / 1000)
-        else:
-            raise KeyError("No interval have been loaded - please set an interval in properties.")
-        return interval
-
-
-def generate_key():
-    # choose from all lowercase letter
-    letters = string.ascii_lowercase
-    result_str = ''.join(random.choice(letters) for i in range(10))
+import json
+import pickle
+import uuid
+
+import string
+import random
+import pandas
+import wizata_dsapi
+from enum import Enum
+
+from .dataframe_toolkit import df_to_json, df_from_json
+from .api_dto import ApiDto
+from .ds_dataframe import DSDataFrame
+from .mlmodel import MLModel
+from .plot import Plot
+from .request import Request
+from .script import Script
+from .pipeline import Pipeline
+from .experiment import Experiment
+
+
+class ExecutionStatus(Enum):
+    RECEIVED = "received"
+    QUEUED = "queued"
+    STARTED = "started"
+    COMPLETED = "completed"
+    FAILED = "failed"
+
+
+class Execution(ApiDto):
+    """
+    Execution Context defining an experimentation historical run.
+
+    Execution can be run in the platform or directly within your script.
+    Used also as context within a Script function, used the following method:
+        - append_model - To store a generated model
+        - append_plot - To store a plot
+        - result_dataframe - To set the panda Dataframe as output
+
+    :ivar execution_id: UUID of the Execution on Wizata App.
+    :ivar experiment_id: UUID of the Experiment on which this Experiment is linked.
+    :ivar warnings: Warning about the Execution.
+
+    Data
+
+    :ivar request: Request or JSON formatted object to fecth data on Wizata App.
+    :ivar input_ds_dataframe: DS Dataframe containing the panda Dataframe input.
+    :ivar dataframe: shortcut to Pandas DataFrame used as input.
+
+    Inputs
+
+    :ivar script: Script to execute against the input data.
+    :ivar ml_model: Trained ML Model to use against the input data.
+    :ivar function: Name of a Wizata built-in function.
+    :ivar isAnomalyDetection: True if this execution triggers integrated Anomaly Detection within Wizata.
+    :ivar properties: configuration and variables.
+
+    Outputs
+
+    :ivar models: Trained Machine Learning Models.
+    :ivar plots: Figures generated with Plotly.
+    :ivar anomalies: Anomalies detected.
+    :ivar output_ds_dataframe: Output dataframe generated by the Script or Model.
+    """
+
+    keys = [
+        'target_feat',
+        'sensitivity',
+        'aggregations',
+        'restart_filter',
+        'interval'
+    ]
+
+    def __init__(self, execution_id=None, properties: dict = None, pipeline: Pipeline = None, experiment: Experiment = None):
+
+        # Id
+        if execution_id is None:
+            execution_id = uuid.uuid4()
+        self.execution_id = execution_id
+
+        # Experiment
+        if experiment is not None:
+            self.experiment_id = experiment.experiment_id
+        else:
+            self.experiment_id = None
+
+        # Inputs Properties (load)
+        self.script = None
+        self.request = None
+
+        if properties is None:
+            properties = {}
+        self.properties = properties
+
+        self.input_ds_dataframe = None
+        self.ml_model = None
+        self.function = None
+        self.isAnomalyDetection = False
+        self.pipeline = pipeline
+        self.status = None
+
+        # created/updated
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
+
+        # Outputs Properties (generated by Execution)
+        self.models = []
+        self.anomalies = []
+        self.plots = []
+        self.dataframes = []
+        self.output_ds_dataframe = None
+        self.warnings = None
+
+    def _get_dataframe(self):
+        if self.input_ds_dataframe is None:
+            return None
+        else:
+            return self.input_ds_dataframe.dataframe
+
+    def _set_dataframe(self, value):
+        if not isinstance(value, pandas.DataFrame):
+            raise ValueError("dataframe must be a panda dataframe.")
+        self.input_ds_dataframe = DSDataFrame()
+        self.input_ds_dataframe.dataframe = value
+
+    def _del_dataframe(self):
+        del self.input_ds_dataframe
+
+    dataframe = property(
+        fget=_get_dataframe,
+        fset=_set_dataframe,
+        fdel=_del_dataframe,
+        doc="Input Pandas Dataframe (for id fetch 'input_ds_dataframe.df_id')"
+    )
+
+    def _get_result_dataframe(self):
+        if self.output_ds_dataframe is None:
+            return None
+        else:
+            return self.output_ds_dataframe.dataframe
+
+    def _set_result_dataframe(self, value):
+        if not isinstance(value, pandas.DataFrame):
+            raise ValueError("dataframe must be a panda dataframe.")
+        self.output_ds_dataframe = DSDataFrame()
+        self.output_ds_dataframe.dataframe = value
+
+    def _del_result_dataframe(self):
+        del self.output_ds_dataframe
+
+    result_dataframe = property(
+        fget=_get_result_dataframe,
+        fset=_set_result_dataframe,
+        fdel=_del_result_dataframe,
+        doc="Output Pandas Dataframe (for id fetch 'output_ds_dataframe.df_id')"
+    )
+
+    def append_plot(self, figure, name="Unkwown"):
+        """
+        Append a plot to the context.
+
+        :param figure: Plotly figure.
+        :param name: Name of the plot.
+        :return: Plot object prepared.
+        """
+        plot = Plot()
+        plot.name = name
+        plot.experiment_id = self.experiment_id
+        plot.figure = figure
+        self.plots.append(plot)
+        return plot
+
+    def append_model(self, trained_model, input_columns, key=None, output_columns=None, has_anomalies=False, scaler=None):
+        """
+        Append a Trained ML Model to the context.
+
+        :param key: Model key to logically identify the model - if not provided a random
+        :param trained_model: Trained Model to be stored as a pickled object.
+        :param input_columns: List of str defining input columns to call the model (df.columns)
+        :param output_columns: List of output columns - Optional as can be detected automatically during validation.
+        :param has_anomalies: False by default, define if the model set anomalies
+        :param scaler: Scaler to be stored if necessary.
+        :return: ML Model object prepared.
+        """
+        ml_model = MLModel()
+
+        if key is None:
+            key = generate_key()
+        ml_model.key = key
+        ml_model.trained_model = trained_model
+        ml_model.scaler = scaler
+
+        ml_model.input_columns = input_columns
+        ml_model.output_columns = output_columns
+
+        ml_model.has_anomalies = has_anomalies
+
+        self.models.append(ml_model)
+        return ml_model
+
+    def api_id(self) -> str:
+        """
+        Id of the execution (execution_id)
+
+        :return: string formatted UUID of the Execution.
+        """
+        return str(self.execution_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate execution.
+        :return: Endpoint name.
+        """
+        return "Executions"
+
+    def to_json(self):
+        """
+        Convert to a json version of Execution definition.
+        By default, use DS API format.
+        """
+        obj = {
+            "id": str(self.execution_id)
+        }
+        if self.experiment_id is not None:
+            obj["experimentId"] = str(self.experiment_id)
+        if self.request is not None:
+            obj["request"] = json.dumps(self.request.to_json())
+        if self.properties is not None:
+            obj["properties"] = json.dumps(self.properties)
+        if self.dataframe is not None:
+            obj["dataframe"] = df_to_json(self.dataframe)
+        # if self.input_ds_dataframe is not None:
+        #     obj["dataframeId"] = str(self.input_ds_dataframe.df_id)
+        if self.script is not None:
+            obj["scriptId"] = str(self.script.script_id)
+        if self.ml_model is not None:
+            obj["mlModelId"] = str(self.ml_model.model_id)
+        if self.pipeline is not None:
+            obj["pipelineId"] = str(self.pipeline.pipeline_id)
+        if self.function is not None:
+            obj["function"] = self.function
+        if self.isAnomalyDetection:
+            obj["isAnomalyDetection"] = str(True)
+        if self.plots is not None:
+            plots_ids = []
+            for plot in self.plots:
+                plots_ids.append(
+                    {
+                        "id": str(plot.plot_id)
+                    }
+                )
+            obj["plots"] = plots_ids
+        if self.models is not None:
+            models_json = []
+            for ml_model in self.models:
+                models_json.append({"id": str(ml_model.model_id)})
+            obj["models"] = models_json
+        if self.anomalies is not None:
+            obj["anomaliesList"] = json.dumps(self.anomalies)
+        # if self.result_dataframe is not None:
+        #     obj["resultDataframe"] = {
+        #         "id": str(self.output_ds_dataframe.df_id)
+        #     }
+        if self.createdById is not None:
+            obj["createdById"] = self.createdById
+        if self.createdDate is not None:
+            obj["createdDate"] = self.createdDate
+        if self.updatedById is not None:
+            obj["updatedById"] = self.updatedById
+        if self.updatedDate is not None:
+            obj["updatedDate"] = self.updatedDate
+        if self.warnings is not None:
+            obj["warnings"] = self.warnings
+        if self.status is not None and isinstance(self.status, ExecutionStatus):
+            obj["status"] = self.status.value
+        return obj
+
+    def from_json(self, obj):
+        """
+        Load an execution from a stored JSON model.
+        :param obj: dictionnary representing an execution.
+        """
+        if "id" in obj.keys():
+            self.execution_id = uuid.UUID(obj["id"])
+        if "experimentId" in obj.keys() and obj["experimentId"] is not None:
+            self.experiment_id = uuid.UUID(obj["experimentId"])
+        if "request" in obj.keys() and obj["request"] is not None:
+            self.request = Request()
+            if isinstance(obj["request"], str):
+                self.request.from_json(json.loads(obj["request"]))
+                self.copy_properties(json.loads(obj["request"]))
+            else:
+                self.request.from_json(obj["request"])
+                self.copy_properties(obj["request"])
+        if "properties" in obj.keys() and obj["properties"] is not None:
+            if isinstance(obj["properties"], str):
+                self.add_properties(json.loads(obj["properties"]))
+            else:
+                self.add_properties(obj["properties"])
+        if "dataframe" in obj.keys() and obj["dataframe"] is not None:
+            if isinstance(obj["dataframe"], str):
+                self.request.from_json(json.loads(obj["dataframe"]))
+            else:
+                self.dataframe = df_from_json(obj["dataframe"])
+        # elif "dataframeId" in obj.keys() and obj["dataframeId"] is not None:
+        #     self.input_ds_dataframe = DSDataFrame(df_id=uuid.UUID(obj["dataframeId"]))
+        if "scriptId" in obj.keys() and obj["scriptId"] is not None:
+            self.script = Script()
+            self.script.script_id = uuid.UUID(obj["scriptId"])
+        if "pipelineId" in obj.keys() and obj["pipelineId"] is not None:
+            self.pipeline = Pipeline()
+            self.pipeline.pipeline_id = uuid.UUID(obj["pipelineId"])
+        if "mlModelId" in obj.keys() and obj["mlModelId"] is not None:
+            self.ml_model = MLModel()
+            self.ml_model.model_id = uuid.UUID(obj["mlModelId"])
+        if "function" in obj.keys() and obj["function"] is not None:
+            self.function = obj["function"]
+        if "isAnomalyDetection" in obj.keys() and obj["isAnomalyDetection"] is not None:
+            if isinstance(obj["isAnomalyDetection"], bool):
+                self.isAnomalyDetection = obj["isAnomalyDetection"]
+            else:
+                self.isAnomalyDetection = obj["isAnomalyDetection"] == 'True'
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
+        if "warnings" in obj.keys() and obj["warnings"] is not None:
+            self.warnings = obj["warnings"]
+        if "anomaliesList" in obj.keys() and obj["anomaliesList"] is not None:
+            if isinstance(obj["anomaliesList"], str):
+                self.anomalies = json.loads(obj["anomaliesList"])
+            else:
+                self.anomalies = obj["anomaliesList"]
+        if "status" in obj.keys():
+            self.status = ExecutionStatus(str(obj["status"]))
+
+    def to_pickle(self):
+        """
+        Convert the Execution to a pickle object.
+        :return: Pickle object.
+        """
+        return pickle.dumps(self)
+
+    def add_properties(self, obj: dict):
+        """
+        load properties from a dictionary
+
+        :param obj: dictionary with potential properties
+        """
+        for key in obj.keys():
+            if self.properties is None:
+                self.properties = {}
+            self.properties[key] = obj[key]
+
+    def copy_properties(self, obj: dict):
+        """
+        copy properties from a dictionary originating from a Request object.
+        filtering on specific properties (Execution.keys)
+
+        :param obj: dictionary with potential properties
+        """
+        for key in Execution.keys:
+            if key in obj:
+                if self.properties is None:
+                    self.properties = {}
+                self.properties[key] = obj[key]
+
+    def get_interval(self) -> int:
+        """
+        Determine interval from either request, properties or loaded dataframe.
+        :return:
+        """
+        if self.request is not None:
+            interval = self.request.interval
+        elif self.properties['aggregations'] is not None \
+                and self.properties['aggregations']['interval'] is not None:
+            interval = int(self.properties["aggregations"]["interval"] / 1000)
+        elif self.properties['interval'] is not None:
+            interval = int(self.properties['interval'] / 1000)
+        else:
+            raise KeyError("No interval have been loaded - please set an interval in properties.")
+        return interval
+
+
+def generate_key():
+    # choose from all lowercase letter
+    letters = string.ascii_lowercase
+    result_str = ''.join(random.choice(letters) for i in range(10))
+    return result_str
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/experiment.py` & `wizata-dsapi-0.3.1/wizata_dsapi/experiment.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,99 @@
-import uuid
-from .api_dto import ApiDto
-
-
-class Experiment(ApiDto):
-    """
-    An experiment is a container to track all executions made in the same context.
-
-    :ivar experiment_id: The UUID of the Experiment.
-    :ivar key: Logical String ID of the Experiment
-    :ivar name: A simple name helping the user identifying the experiment.
-    """
-    def __init__(self, experiment_id=None, key=None, name=None, description=None):
-        if experiment_id is None:
-            self.experiment_id = uuid.uuid4()
-        else:
-            self.experiment_id = experiment_id
-        self.key = key
-        self.name = name
-        self.description = description
-        self.templateId = None
-        self.twinId = None
-        self.twinGraphId = None
-        self.createdById = None
-        self.createdDate = None
-        self.updatedById = None
-        self.updatedDate = None
-
-    def api_id(self) -> str:
-        """
-        Id of the experiment (experiment_id)
-
-        :return: string formatted UUID of the Experiment.
-        """
-        return str(self.experiment_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate execution.
-        :return: Endpoint name.
-        """
-        return "Experiments"
-
-    def to_json(self):
-        """
-        Convert to a json version of Experiment definition.
-        """
-        obj = {
-            "id": str(self.experiment_id)
-        }
-        if self.key is not None:
-            obj["key"] = str(self.key)
-        if self.name is not None:
-            obj["name"] = str(self.name)
-        if self.description is not None:
-            obj["description"] = str(self.description)
-        if self.templateId is not None:
-            obj["templateId"] = str(self.templateId)
-        if self.twinId is not None:
-            obj["twinId"] = str(self.twinId)
-        if self.twinGraphId is not None:
-            obj["twinGraphId"] = str(self.twinGraphId)
-        if self.createdById is not None:
-            obj["createdById"] = str(self.createdById)
-        if self.createdDate is not None:
-            obj["createdDate"] = str(self.createdDate)
-        if self.updatedById is not None:
-            obj["updatedById"] = str(self.updatedById)
-        if self.updatedDate is not None:
-            obj["updatedDate"] = str(self.updatedDate)
-        return obj
-
-    def from_json(self, obj):
-        """
-        Load an experiment from a stored JSON object.
-        """
-        if "id" in obj.keys():
-            self.experiment_id = uuid.UUID(obj["id"])
-        if "key" in obj.keys() and obj["key"] is not None:
-            self.key = obj["key"]
-        if "name" in obj.keys() and obj["name"] is not None:
-            self.name = obj["name"]
-        if "description" in obj.keys() and obj["description"] is not None:
-            self.description = obj["description"]
-        if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.templateId = obj["templateId"]
-        if "twinId" in obj.keys() and obj["twinId"] is not None:
-            self.twinId = obj["twinId"]
-        if "twinGraphId" in obj.keys() and obj["twinGraphId"] is not None:
-            self.twinGraphId = obj["twinGraphId"]
-        if "createdById" in obj.keys() and obj["createdById"] is not None:
-            self.createdById = obj["createdById"]
-        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
-            self.createdDate = obj["createdDate"]
-        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
-            self.updatedById = obj["updatedById"]
-        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
-            self.updatedDate = obj["updatedDate"]
-
+import uuid
+from .api_dto import ApiDto
+
+
+class Experiment(ApiDto):
+    """
+    An experiment is a container to track all executions made in the same context.
+
+    :ivar experiment_id: The UUID of the Experiment.
+    :ivar key: Logical String ID of the Experiment
+    :ivar name: A simple name helping the user identifying the experiment.
+    """
+    def __init__(self, experiment_id=None, key=None, name=None, description=None):
+        if experiment_id is None:
+            self.experiment_id = uuid.uuid4()
+        else:
+            self.experiment_id = experiment_id
+        self.key = key
+        self.name = name
+        self.description = description
+        self.templateId = None
+        self.twinId = None
+        self.twinGraphId = None
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
+
+    def api_id(self) -> str:
+        """
+        Id of the experiment (experiment_id)
+
+        :return: string formatted UUID of the Experiment.
+        """
+        return str(self.experiment_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate execution.
+        :return: Endpoint name.
+        """
+        return "Experiments"
+
+    def to_json(self):
+        """
+        Convert to a json version of Experiment definition.
+        """
+        obj = {
+            "id": str(self.experiment_id)
+        }
+        if self.key is not None:
+            obj["key"] = str(self.key)
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.description is not None:
+            obj["description"] = str(self.description)
+        if self.templateId is not None:
+            obj["templateId"] = str(self.templateId)
+        if self.twinId is not None:
+            obj["twinId"] = str(self.twinId)
+        if self.twinGraphId is not None:
+            obj["twinGraphId"] = str(self.twinGraphId)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
+        return obj
+
+    def from_json(self, obj):
+        """
+        Load an experiment from a stored JSON object.
+        """
+        if "id" in obj.keys():
+            self.experiment_id = uuid.UUID(obj["id"])
+        if "key" in obj.keys() and obj["key"] is not None:
+            self.key = obj["key"]
+        if "name" in obj.keys() and obj["name"] is not None:
+            self.name = obj["name"]
+        if "description" in obj.keys() and obj["description"] is not None:
+            self.description = obj["description"]
+        if "templateId" in obj.keys() and obj["templateId"] is not None:
+            self.templateId = obj["templateId"]
+        if "twinId" in obj.keys() and obj["twinId"] is not None:
+            self.twinId = obj["twinId"]
+        if "twinGraphId" in obj.keys() and obj["twinGraphId"] is not None:
+            self.twinGraphId = obj["twinGraphId"]
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
+
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/model_toolkit.py` & `wizata-dsapi-0.3.1/wizata_dsapi/model_toolkit.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-import pandas
-from .mlmodel import MLModel
-
-
-def predict(df: pandas.DataFrame, ml_model: MLModel, mapping_table=None):
-    """
-    Execute a Machine Learning models locally.
-
-    :param df: dataframe to use as input.
-    :param ml_model: trained machine learning model.
-    :param mapping_table: Optional mapping table.
-    :return: output dataframe with predicted values.
-    """
-    if ml_model is None or ml_model.trained_model is None or ml_model.input_columns is None:
-        raise ValueError("Please download your model from DS API before using it.")
-    old_index = df.index
-    df.index = pandas.to_datetime(df.index)
-    df_result = pandas.DataFrame(index=df.index)
-    features = ml_model.input_columns
-    if ml_model.has_target_feat is True:
-        df_result['result'] = ml_model.trained_model.detect(df[features]).astype(float)
-    else:
-        df_result['result'] = ml_model.trained_model.predict(df[features]).astype(float)
-    if ml_model.label_counts != 0:
-        df_result[__generate_label_columns(ml_model.label_counts)] = \
-            ml_model.trained_model.predict_proba(df[features]).astype(float)
-    df_result = df_result.set_index(old_index)
-    return df_result
-
-
-def __generate_label_columns(label_count):
-    """
-    Generate a list of columns based on number of desired labels.
-    :param label_count: Number of desired labels.
-    :return: list of labels generated.
-    """
-    i = 0
-    columns = []
-    while i < label_count:
-        columns.append("prob_" + str(i) + "_label")
-        i = i + 1
-    return columns
+import pandas
+from .mlmodel import MLModel
+
+
+def predict(df: pandas.DataFrame, ml_model: MLModel, mapping_table=None):
+    """
+    Execute a Machine Learning models locally.
+
+    :param df: dataframe to use as input.
+    :param ml_model: trained machine learning model.
+    :param mapping_table: Optional mapping table.
+    :return: output dataframe with predicted values.
+    """
+    if ml_model is None or ml_model.trained_model is None or ml_model.input_columns is None:
+        raise ValueError("Please download your model from DS API before using it.")
+    old_index = df.index
+    df.index = pandas.to_datetime(df.index)
+    df_result = pandas.DataFrame(index=df.index)
+    features = ml_model.input_columns
+    if ml_model.has_target_feat is True:
+        df_result['result'] = ml_model.trained_model.detect(df[features]).astype(float)
+    else:
+        df_result['result'] = ml_model.trained_model.predict(df[features]).astype(float)
+    if ml_model.label_counts != 0:
+        df_result[__generate_label_columns(ml_model.label_counts)] = \
+            ml_model.trained_model.predict_proba(df[features]).astype(float)
+    df_result = df_result.set_index(old_index)
+    return df_result
+
+
+def __generate_label_columns(label_count):
+    """
+    Generate a list of columns based on number of desired labels.
+    :param label_count: Number of desired labels.
+    :return: list of labels generated.
+    """
+    i = 0
+    columns = []
+    while i < label_count:
+        columns.append("prob_" + str(i) + "_label")
+        i = i + 1
+    return columns
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/pipeline.py` & `wizata-dsapi-0.3.1/wizata_dsapi/pipeline.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,476 +1,504 @@
-import uuid
-import json
-
-from .api_dto import ApiDto
-from .script import ScriptConfig, Script
-from .request import Request
-from .mlmodel import MLModelConfig
-
-from enum import Enum
-
-
-class VarType(Enum):
-    STRING = "string"
-    INTEGER = "integer"
-    DATETIME = "datetime"
-    RELATIVE = "relative"
-    DATAPOINT = "datapoint"
-    FLOAT = "float"
-
-
-class StepType(Enum):
-    QUERY = 'query'
-    SCRIPT = 'script'
-    MODEL = 'model'
-    WRITE = 'write'
-
-
-class WriteConfig:
-
-    def __init__(self, config_id = None, datapoints: dict = None):
-        if config_id is None:
-            config_id = uuid.uuid4()
-        self.config_id = config_id
-        self.datapoints = datapoints
-
-    def from_json(self, obj):
-        if "id" in obj:
-            self.config_id = obj["id"]
-        if "datapoints" in obj:
-            self.datapoints = obj["datapoints"]
-
-    def to_json(self):
-        obj = {
-            "id": str(self.config_id)
-        }
-        if self.datapoints is not None:
-            obj["datapoints"] = self.datapoints
-        return obj
-
-
-class PipelineStep(ApiDto):
-    """
-    Step of a pipeline.
-    """
-
-    def __init__(self,
-                 step_id: uuid.UUID = None,
-                 step_type: StepType = None,
-                 config=None,
-                 inputs=None,
-                 outputs=None):
-
-        if outputs is None:
-            outputs = []
-        if inputs is None:
-            inputs = []
-        if step_id is None:
-            step_id = uuid.uuid4()
-        self.step_id = step_id
-        self.step_type = step_type
-        self.config = config
-        self.inputs = inputs
-        self.outputs = outputs
-
-    def from_json(self, obj):
-        """
-        load from JSON dictionary representation
-        """
-        if "id" in obj.keys():
-            self.step_id = uuid.UUID(obj["id"])
-
-        if "type" in obj.keys():
-            if obj["type"] in ['query', 'script', 'model', 'write']:
-                self.step_type = StepType(obj["type"])
-            else:
-                raise TypeError(f'unsupported step type {obj["type"]}')
-        else:
-            raise TypeError(f'pipeline step must have a type.')
-        if "config" in obj.keys():
-            if self.step_type == StepType.SCRIPT:
-                self.config = ScriptConfig()
-                self.config.from_json(obj['config'])
-            elif self.step_type == StepType.QUERY:
-                self.config = Request()
-                self.config.from_json(obj['config'])
-            elif self.step_type == StepType.WRITE:
-                self.config = WriteConfig()
-                self.config.from_json(obj['config'])
-            elif self.step_type == StepType.MODEL:
-                self.config = MLModelConfig()
-                self.config.from_json(obj['config'])
-            else:
-                self.config = obj['config']
-        self.inputs = []
-        if "inputs" in obj.keys():
-            for step_input in obj["inputs"]:
-                if isinstance(step_input, dict):
-                    self.inputs.append(step_input)
-                else:
-                    raise TypeError(f'unsupported input type {step_input.__class__.__name__}')
-
-        self.outputs = []
-        if "outputs" in obj.keys():
-            for step_output in obj["outputs"]:
-                if isinstance(step_output, dict):
-                    self.outputs.append(step_output)
-                else:
-                    raise TypeError(f'unsupported output type {step_output.__class__.__name__}')
-
-    def to_json(self):
-        obj = {
-            "id": str(self.step_id)
-        }
-        if self.step_type is not None:
-            obj["type"] = str(self.step_type.value)
-        if self.config is not None:
-            if self.step_type == StepType.SCRIPT:
-                obj["config"] = self.config.to_json()
-            elif self.step_type == StepType.QUERY:
-                obj["config"] = self.config.to_json()
-            elif self.step_type == StepType.WRITE:
-                obj["config"] = self.config.to_json()
-            elif self.step_type == StepType.MODEL:
-                obj["config"] = self.config.to_json()
-            else:
-                obj["config"] = self.config
-        if self.inputs is not None:
-            obj["inputs"] = self.inputs
-        if self.outputs is not None:
-            obj["outputs"] = self.outputs
-        return obj
-
-    def inputs_names(self, f_type: str = None) -> list:
-        """
-        get a list str representing inputs names
-        :param f_type: filter on a type
-        :return: list str
-        """
-        names = []
-        for d_key in self.inputs:
-            if not isinstance(d_key, dict):
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-            if "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
-                names.append(d_key["dataframe"])
-            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
-                names.append(d_key["model"])
-            elif f_type is None:
-                raise TypeError(f'unsupported input type {d_key} expected dataframe or model')
-        return names
-
-    def outputs_names(self, f_type: str = None) -> list:
-        """
-        get a list str representing outputs names
-        :param f_type: filter on a type
-        :return: list str
-        """
-        names = []
-        for d_key in self.outputs:
-            if not isinstance(d_key, dict):
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-            elif "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
-                names.append(d_key["dataframe"])
-            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
-                names.append(d_key["model"])
-            elif f_type is None:
-                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
-        return names
-
-    def get_input(self, name: str) -> dict:
-        """
-        get input dict based on value name.
-        :param name: value name to find.
-        :return: input dict
-        """
-        for d_input in self.inputs:
-            if name in d_input.values():
-                return d_input
-
-    def get_output(self, name: str) -> dict:
-        """
-        get output dict based on value name.
-        :param name: value name to find.
-        :return: input dict
-        """
-        for d_output in self.outputs:
-            if name in d_output.values():
-                return d_output
-
-
-class Pipeline(ApiDto):
-
-    def __init__(self,
-                 pipeline_id: uuid.UUID = None,
-                 key: str = None,
-                 variables: list = None,
-                 steps: list = None,
-                 plots: list = None,
-                 template_id: uuid.UUID = None,
-                 experiment_id: uuid.UUID = None):
-
-        if pipeline_id is None:
-            pipeline_id = uuid.uuid4()
-        self.pipeline_id = pipeline_id
-        self.key = key
-        if variables is None:
-            variables = {}
-        self.variables = variables
-        self.template_id = template_id
-        self.experiment_id = experiment_id
-        self.createdById = None
-        self.createdDate = None
-        self.updatedById = None
-        self.updatedDate = None
-        self.plots = plots
-        if plots is None:
-            self.plots = []
-        if steps is not None:
-            for step in steps:
-                if not isinstance(step, PipelineStep):
-                    raise TypeError(f'step expected PipelineStep but received {step.__class__.__name__}')
-            self.steps = steps
-        else:
-            self.steps = []
-
-    def check_path(self) -> bool:
-        """
-        validate that steps create a valid path.
-        return true if path is valid, otherwise raise errors
-        """
-
-        followed = []  # all steps already followed
-        produced = []  # all outputs already produced
-
-        steps_to_follow = self._next_steps(followed, produced)
-        if len(steps_to_follow) == 0:
-            raise ValueError('path does not contains any initial steps producing outputs')
-
-        while len(steps_to_follow) > 0:
-            for step in steps_to_follow:
-                self._follow_step(step, followed, produced)
-            steps_to_follow = []
-            if len(followed) < len(self.steps):
-                steps_to_follow = self._next_steps(followed, produced)
-
-        if len(followed) == len(self.steps):
-            return True
-        else:
-            raise RuntimeError(f'missing {len(self.steps)-len(followed)} step(s) that could not be followed')
-
-    def _follow_step(self,
-                     step: PipelineStep,
-                     followed: list,
-                     produced: list):
-        """
-        simulate that step have been followed.
-        """
-        if step in followed:
-            raise RuntimeError(f'path cannot pass two times through same step {step.step_id}')
-        followed.append(step)
-        if step.step_type == StepType.QUERY and len(step.outputs) != 1:
-            raise RuntimeError(f'query step must have exactly one output and be of type dataframe')
-        if step.step_type == StepType.WRITE and (len(step.inputs) != 1 or len(step.outputs) > 0):
-            raise RuntimeError(f'write step must have exactly one input and no outputs')
-        for output in step.outputs_names():
-            if output in produced:
-                raise RuntimeError(f'output {output} is already produced.')
-            produced.append(output)
-
-    def _next_steps(self, followed, produced):
-        """
-        find all next steps that are ready to be executed
-        """
-        next_steps = []
-        step: PipelineStep
-        for step in self.steps:
-            if all(s_input in produced for s_input in step.inputs_names()) and step not in followed:
-                next_steps.append(step)
-        return next_steps
-
-    def add_query(self, request: Request, df_name: str):
-        """
-        add a query step
-        :param request: request definition to add.
-        :param df_name: output name ot use for the dataframe.
-        """
-        if request is None:
-            raise ValueError('please provide a request.')
-        if df_name is None:
-            raise ValueError('please name the output')
-        step = PipelineStep()
-        step.step_type = StepType.QUERY
-        step.config = request
-        step.outputs.append({'dataframe': df_name})
-        self.steps.append(step)
-
-    def add_transformation(self, script, input_df_names: list, output_df_names: list):
-        """
-        add a transformation script
-        :param script: name, Script or ScriptConfig.
-        :param input_df_names: list of str for dataframe input.
-        :param output_df_names: list of str for dataframe output.
-        """
-        if script is None:
-            raise ValueError('please provide a script.')
-
-        step = PipelineStep()
-        step.step_type = StepType.SCRIPT
-        if isinstance(script, str):
-            step.config = ScriptConfig(function=script)
-        elif isinstance(script, ScriptConfig):
-            step.config = script
-        elif isinstance(script, Script):
-            name = script.name
-            if name is None:
-                raise ValueError('please fetch your script or set a function name directly')
-            step.config = ScriptConfig(function=name)
-        else:
-            raise TypeError(f'unsupported type of script {script.__class__.__name__}')
-        for input_df_name in input_df_names:
-            if not isinstance(input_df_name, str):
-                raise TypeError(f'unsupported type of input df name {input_df_name.__class__.__name__}')
-            step.inputs.append({'dataframe': input_df_name})
-        for output_df_name in output_df_names:
-            if not isinstance(output_df_name, str):
-                raise TypeError(f'unsupported type of input df name {output_df_name.__class__.__name__}')
-            step.outputs.append({'dataframe': output_df_name})
-        self.steps.append(step)
-
-    def add_plot(self, script, df_name: str):
-        """
-        add a plot to the pipeline.
-        :param script: name, Script or ScriptConfig.
-        :param df_name: name of the dataframe to plot.
-        """
-
-        if script is None:
-            raise ValueError('please provide a script.')
-
-        script_name = None
-        if isinstance(script, str):
-            script_name = ScriptConfig(function=script)
-        elif isinstance(script, ScriptConfig):
-            script_name = script
-        elif isinstance(script, Script):
-            script_name = script.name
-            if script_name is None:
-                raise ValueError('please fetch your script or set a function name directly')
-        else:
-            raise TypeError(f'unsupported type of script {script.__class__.__name__}')
-
-        if df_name is None:
-            raise ValueError(f'please provide a dataframe name')
-
-        self.plots.append({'dataframe': df_name, 'script': script_name})
-
-    def check_variables(self):
-        """
-        verify that variables dict is a valid { "name" : "VarType" } dictionary.
-        """
-        if self.variables is None:
-            self.variables = {}
-        elif not isinstance(self.variables, dict):
-            raise TypeError(f'variables must be empty nor a valid dictionary')
-        for key in self.variables:
-            # check if valid type (trigger an error if not)
-            VarType(self.variables[key])
-
-    def api_id(self) -> str:
-        """
-        Id of the pipeline
-
-        :return: string formatted UUID of the Pipeline.
-        """
-        return str(self.pipeline_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate pipeline.
-        :return: Endpoint name.
-        """
-        return "Pipelines"
-
-    def from_json(self, obj):
-        """
-        load from JSON dictionary representation
-        """
-        if "id" in obj.keys():
-            self.pipeline_id = uuid.UUID(obj["id"])
-        if "key" in obj.keys():
-            self.key = str(obj['key'])
-        if "id" not in obj.keys() and "key" not in obj.keys():
-            raise KeyError("at least id or key must be set on a pipeline")
-        if "templateId" in obj.keys() and obj["templateId"] is not None:
-            self.template_id = uuid.UUID(obj["templateId"])
-        if "experimentKey" in obj.keys() and obj["experimentKey"] is not None:
-            self.experiment_id = uuid.UUID(obj["experimentKey"])
-        if "variables" in obj.keys():
-            if isinstance(obj["variables"], str):
-                self.variables = json.loads(obj["variables"])
-            else:
-                self.variables = obj["variables"]
-            if self.variables is not None or not isinstance(self.variables, dict):
-                if isinstance(self.variables, list) and len(self.variables) == 0:
-                    self.variables = {}
-            self.check_variables()
-        if "steps" in obj.keys():
-            if isinstance(obj["steps"], str):
-                steps = json.loads(obj["steps"])
-            else:
-                steps = obj["steps"]
-            for obj_step in steps:
-                step = PipelineStep()
-                step.from_json(obj_step)
-                self.steps.append(step)
-        if "plots" in obj.keys():
-            if isinstance(obj["plots"], str):
-                self.plots = json.loads(obj["plots"])
-            else:
-                self.plots = obj["plots"]
-        if "createdById" in obj.keys() and obj["createdById"] is not None:
-            self.createdById = obj["createdById"]
-        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
-            self.createdDate = obj["createdDate"]
-        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
-            self.updatedById = obj["updatedById"]
-        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
-            self.updatedDate = obj["updatedDate"]
-
-    def to_json(self):
-        """
-        Convert to a json version of Execution definition.
-        By default, use DS API format.
-        """
-        obj = {
-            "id": str(self.pipeline_id)
-        }
-        if self.key is not None:
-            obj["key"] = self.key
-        if self.steps is not None:
-            obj_steps = []
-            step: PipelineStep
-            for step in self.steps:
-                obj_steps.append(step.to_json())
-            obj["steps"] = json.dumps(obj_steps)
-        if self.plots is not None:
-            obj["plots"] = json.dumps(self.plots)
-        if self.variables is not None:
-            self.check_variables()
-            obj["variables"] = json.dumps(self.variables)
-        if self.template_id is not None:
-            obj["templateId"] = str(self.template_id)
-        if self.experiment_id is not None:
-            obj["experimentKey"] = str(self.experiment_id)
-        if self.createdById is not None:
-            obj["createdById"] = str(self.createdById)
-        if self.createdDate is not None:
-            obj["createdDate"] = str(self.createdDate)
-        if self.updatedById is not None:
-            obj["updatedById"] = str(self.updatedById)
-        if self.updatedDate is not None:
-            obj["updatedDate"] = str(self.updatedDate)
-        return obj
-
-
-
-
+import uuid
+import json
+
+from .api_dto import ApiDto
+from .script import ScriptConfig, Script
+from .request import Request
+from .mlmodel import MLModelConfig
+
+from enum import Enum
+
+
+class VarType(Enum):
+    STRING = "string"
+    INTEGER = "integer"
+    DATETIME = "datetime"
+    RELATIVE = "relative"
+    DATAPOINT = "datapoint"
+    FLOAT = "float"
+    JSON = "json"
+
+
+class StepType(Enum):
+    QUERY = 'query'
+    SCRIPT = 'script'
+    MODEL = 'model'
+    WRITE = 'write'
+
+
+class WriteConfig:
+
+    def __init__(self, config_id = None, datapoints: dict = None):
+        if config_id is None:
+            config_id = uuid.uuid4()
+        self.config_id = config_id
+        self.datapoints = datapoints
+
+    def from_json(self, obj):
+        if "id" in obj:
+            self.config_id = obj["id"]
+        if "datapoints" in obj:
+            self.datapoints = obj["datapoints"]
+
+    def to_json(self):
+        obj = {
+            "id": str(self.config_id)
+        }
+        if self.datapoints is not None:
+            obj["datapoints"] = self.datapoints
+        return obj
+
+
+class PipelineStep(ApiDto):
+    """
+    Step of a pipeline.
+    """
+
+    def __init__(self,
+                 step_id: uuid.UUID = None,
+                 step_type: StepType = None,
+                 config=None,
+                 inputs=None,
+                 outputs=None):
+
+        if outputs is None:
+            outputs = []
+        if inputs is None:
+            inputs = []
+        if step_id is None:
+            step_id = uuid.uuid4()
+        self.step_id = step_id
+        self.step_type = step_type
+        self.config = config
+        self.inputs = inputs
+        self.outputs = outputs
+
+    def from_json(self, obj):
+        """
+        load from JSON dictionary representation
+        """
+        if "id" in obj.keys():
+            self.step_id = uuid.UUID(obj["id"])
+
+        if "type" in obj.keys():
+            if obj["type"] in ['query', 'script', 'model', 'write']:
+                self.step_type = StepType(obj["type"])
+            else:
+                raise TypeError(f'unsupported step type {obj["type"]}')
+        else:
+            raise TypeError(f'pipeline step must have a type.')
+        if "config" in obj.keys():
+            if self.step_type == StepType.SCRIPT:
+                self.config = ScriptConfig()
+                self.config.from_json(obj['config'])
+            elif self.step_type == StepType.QUERY:
+                self.config = Request()
+                self.config.from_json(obj['config'])
+            elif self.step_type == StepType.WRITE:
+                self.config = WriteConfig()
+                self.config.from_json(obj['config'])
+            elif self.step_type == StepType.MODEL:
+                self.config = MLModelConfig()
+                self.config.from_json(obj['config'])
+            else:
+                self.config = obj['config']
+        self.inputs = []
+        if "inputs" in obj.keys():
+            for step_input in obj["inputs"]:
+                if isinstance(step_input, dict):
+                    self.inputs.append(step_input)
+                else:
+                    raise TypeError(f'unsupported input type {step_input.__class__.__name__}')
+
+        self.outputs = []
+        if "outputs" in obj.keys():
+            for step_output in obj["outputs"]:
+                if isinstance(step_output, dict):
+                    self.outputs.append(step_output)
+                else:
+                    raise TypeError(f'unsupported output type {step_output.__class__.__name__}')
+
+    def to_json(self):
+        obj = {
+            "id": str(self.step_id)
+        }
+        if self.step_type is not None:
+            obj["type"] = str(self.step_type.value)
+        if self.config is not None:
+            if self.step_type == StepType.SCRIPT:
+                obj["config"] = self.config.to_json()
+            elif self.step_type == StepType.QUERY:
+                obj["config"] = self.config.to_json()
+            elif self.step_type == StepType.WRITE:
+                obj["config"] = self.config.to_json()
+            elif self.step_type == StepType.MODEL:
+                obj["config"] = self.config.to_json()
+            else:
+                obj["config"] = self.config
+        if self.inputs is not None:
+            obj["inputs"] = self.inputs
+        if self.outputs is not None:
+            obj["outputs"] = self.outputs
+        return obj
+
+    def inputs_names(self, f_type: str = None) -> list:
+        """
+        get a list str representing inputs names
+        :param f_type: filter on a type
+        :return: list str
+        """
+        names = []
+        for d_key in self.inputs:
+            if not isinstance(d_key, dict):
+                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
+            if "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
+                names.append(d_key["dataframe"])
+            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
+                names.append(d_key["model"])
+            elif f_type is None:
+                raise TypeError(f'unsupported input type {d_key} expected dataframe or model')
+        return names
+
+    def outputs_names(self, f_type: str = None) -> list:
+        """
+        get a list str representing outputs names
+        :param f_type: filter on a type
+        :return: list str
+        """
+        names = []
+        for d_key in self.outputs:
+            if not isinstance(d_key, dict):
+                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
+            elif "dataframe" in d_key.keys() and (f_type is None or f_type == 'dataframe'):
+                names.append(d_key["dataframe"])
+            elif "model" in d_key.keys() and (f_type is None or f_type == 'model'):
+                names.append(d_key["model"])
+            elif f_type is None:
+                raise TypeError(f'unsupported output type {d_key} expected dataframe or model')
+        return names
+
+    def get_input(self, name: str) -> dict:
+        """
+        get input dict based on value name.
+        :param name: value name to find.
+        :return: input dict
+        """
+        for d_input in self.inputs:
+            if name in d_input.values():
+                return d_input
+
+    def get_output(self, name: str) -> dict:
+        """
+        get output dict based on value name.
+        :param name: value name to find.
+        :return: input dict
+        """
+        for d_output in self.outputs:
+            if name in d_output.values():
+                return d_output
+
+
+class Pipeline(ApiDto):
+
+    def __init__(self,
+                 pipeline_id: uuid.UUID = None,
+                 key: str = None,
+                 variables: dict = None,
+                 steps: list = None,
+                 plots: list = None,
+                 template_id: uuid.UUID = None,
+                 experiment_id: uuid.UUID = None):
+
+        if pipeline_id is None:
+            pipeline_id = uuid.uuid4()
+        self.pipeline_id = pipeline_id
+        self.key = key
+        if variables is None:
+            variables = {}
+        self.variables = variables
+        self.template_id = template_id
+        self.experiment_id = experiment_id
+        self.createdById = None
+        self.createdDate = None
+        self.updatedById = None
+        self.updatedDate = None
+        self.plots = plots
+        if plots is None:
+            self.plots = []
+        if steps is not None:
+            for step in steps:
+                if not isinstance(step, PipelineStep):
+                    raise TypeError(f'step expected PipelineStep but received {step.__class__.__name__}')
+            self.steps = steps
+        else:
+            self.steps = []
+
+    def check_path(self) -> bool:
+        """
+        validate that steps create a valid path.
+        return true if path is valid, otherwise raise errors
+        """
+
+        followed = []  # all steps already followed
+        produced = []  # all outputs already produced
+
+        steps_to_follow = self._next_steps(followed, produced)
+        if len(steps_to_follow) == 0:
+            raise ValueError('path does not contains any initial steps producing outputs')
+
+        while len(steps_to_follow) > 0:
+            for step in steps_to_follow:
+                self._follow_step(step, followed, produced)
+            steps_to_follow = []
+            if len(followed) < len(self.steps):
+                steps_to_follow = self._next_steps(followed, produced)
+
+        if len(followed) == len(self.steps):
+            return True
+        else:
+            raise RuntimeError(f'missing {len(self.steps)-len(followed)} step(s) that could not be followed')
+
+    def _follow_step(self,
+                     step: PipelineStep,
+                     followed: list,
+                     produced: list):
+        """
+        simulate that step have been followed.
+        """
+        if step in followed:
+            raise RuntimeError(f'path cannot pass two times through same step {step.step_id}')
+        followed.append(step)
+        if step.step_type == StepType.QUERY and len(step.outputs) != 1:
+            raise RuntimeError(f'query step must have exactly one output and be of type dataframe')
+        if step.step_type == StepType.WRITE and (len(step.inputs) != 1 or len(step.outputs) > 0):
+            raise RuntimeError(f'write step must have exactly one input and no outputs')
+        for output in step.outputs_names():
+            if output in produced:
+                raise RuntimeError(f'output {output} is already produced.')
+            produced.append(output)
+
+    def _next_steps(self, followed, produced):
+        """
+        find all next steps that are ready to be executed
+        """
+        next_steps = []
+        step: PipelineStep
+        for step in self.steps:
+            if all(s_input in produced for s_input in step.inputs_names()) and step not in followed:
+                next_steps.append(step)
+        return next_steps
+
+    def add_query(self, request: Request, df_name: str):
+        """
+        add a query step
+        :param request: request definition to add.
+        :param df_name: output name ot use for the dataframe.
+        """
+        if request is None:
+            raise ValueError('please provide a request.')
+        if df_name is None:
+            raise ValueError('please name the output')
+        step = PipelineStep()
+        step.step_type = StepType.QUERY
+        step.config = request
+        step.outputs.append({'dataframe': df_name})
+        self.steps.append(step)
+
+    def add_transformation(self, script, input_df_names: list, output_df_names: list):
+        """
+        add a transformation script
+        :param script: name, Script or ScriptConfig.
+        :param input_df_names: list of str for dataframe input.
+        :param output_df_names: list of str for dataframe output.
+        """
+        if script is None:
+            raise ValueError('please provide a script.')
+
+        step = PipelineStep()
+        step.step_type = StepType.SCRIPT
+        if isinstance(script, str):
+            step.config = ScriptConfig(function=script)
+        elif isinstance(script, ScriptConfig):
+            step.config = script
+        elif isinstance(script, Script):
+            name = script.name
+            if name is None:
+                raise ValueError('please fetch your script or set a function name directly')
+            step.config = ScriptConfig(function=name)
+        else:
+            raise TypeError(f'unsupported type of script {script.__class__.__name__}')
+        for input_df_name in input_df_names:
+            if not isinstance(input_df_name, str):
+                raise TypeError(f'unsupported type of input df name {input_df_name.__class__.__name__}')
+            step.inputs.append({'dataframe': input_df_name})
+        for output_df_name in output_df_names:
+            if not isinstance(output_df_name, str):
+                raise TypeError(f'unsupported type of input df name {output_df_name.__class__.__name__}')
+            step.outputs.append({'dataframe': output_df_name})
+        self.steps.append(step)
+
+    def add_model(self, config:MLModelConfig, input_df: str, output_df: str = None):
+
+        if config is None:
+            raise ValueError('please provide a config.')
+        if input_df is None:
+            raise ValueError('please provide a input_df name.')
+
+        step = PipelineStep()
+        step.step_type = StepType.MODEL
+        step.inputs.append({'dataframe': input_df})
+        if output_df is not None:
+            step.outputs.append({'dataframe': output_df})
+        step.config = config
+        self.steps.append(step)
+
+    def add_writer(self, config: WriteConfig, input_df: str):
+
+        if config is None:
+            raise ValueError('please provide a config.')
+        if input_df is None:
+            raise ValueError('please provide a input_df name.')
+
+        step = PipelineStep()
+        step.step_type = StepType.WRITE
+        step.inputs.append({'dataframe': input_df})
+        step.config = config
+        self.steps.append(step)
+
+    def add_plot(self, script, df_name: str):
+        """
+        add a plot to the pipeline.
+        :param script: name, Script or ScriptConfig.
+        :param df_name: name of the dataframe to plot.
+        """
+
+        if script is None:
+            raise ValueError('please provide a script.')
+
+        if isinstance(script, ScriptConfig):
+            script_name = ScriptConfig(function=script)
+        elif isinstance(script, str):
+            script_name = script
+        elif isinstance(script, Script):
+            script_name = script.name
+            if script_name is None:
+                raise ValueError('please fetch your script or set a function name directly')
+        else:
+            raise TypeError(f'unsupported type of script {script.__class__.__name__}')
+
+        if df_name is None:
+            raise ValueError(f'please provide a dataframe name')
+
+        self.plots.append({'dataframe': df_name, 'script': script_name})
+
+    def check_variables(self):
+        """
+        verify that variables dict is a valid { "name" : "VarType" } dictionary.
+        """
+        if self.variables is None:
+            self.variables = {}
+        elif not isinstance(self.variables, dict):
+            raise TypeError(f'variables must be empty nor a valid dictionary')
+        for key in self.variables:
+            # check if valid type (trigger an error if not)
+            VarType(self.variables[key])
+
+    def api_id(self) -> str:
+        """
+        Id of the pipeline
+
+        :return: string formatted UUID of the Pipeline.
+        """
+        return str(self.pipeline_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate pipeline.
+        :return: Endpoint name.
+        """
+        return "Pipelines"
+
+    def from_json(self, obj):
+        """
+        load from JSON dictionary representation
+        """
+        if "id" in obj.keys():
+            self.pipeline_id = uuid.UUID(obj["id"])
+        if "key" in obj.keys():
+            self.key = str(obj['key'])
+        if "id" not in obj.keys() and "key" not in obj.keys():
+            raise KeyError("at least id or key must be set on a pipeline")
+        if "templateId" in obj.keys() and obj["templateId"] is not None:
+            self.template_id = uuid.UUID(obj["templateId"])
+        if "experimentKey" in obj.keys() and obj["experimentKey"] is not None:
+            self.experiment_id = uuid.UUID(obj["experimentKey"])
+        if "variables" in obj.keys():
+            if isinstance(obj["variables"], str):
+                self.variables = json.loads(obj["variables"])
+            else:
+                self.variables = obj["variables"]
+            if self.variables is not None or not isinstance(self.variables, dict):
+                if isinstance(self.variables, list) and len(self.variables) == 0:
+                    self.variables = {}
+            self.check_variables()
+        if "steps" in obj.keys():
+            if isinstance(obj["steps"], str):
+                steps = json.loads(obj["steps"])
+            else:
+                steps = obj["steps"]
+            for obj_step in steps:
+                step = PipelineStep()
+                step.from_json(obj_step)
+                self.steps.append(step)
+        if "plots" in obj.keys():
+            if isinstance(obj["plots"], str):
+                self.plots = json.loads(obj["plots"])
+            else:
+                self.plots = obj["plots"]
+        if "createdById" in obj.keys() and obj["createdById"] is not None:
+            self.createdById = obj["createdById"]
+        if "createdDate" in obj.keys() and obj["createdDate"] is not None:
+            self.createdDate = obj["createdDate"]
+        if "updatedById" in obj.keys() and obj["updatedById"] is not None:
+            self.updatedById = obj["updatedById"]
+        if "updatedDate" in obj.keys() and obj["updatedDate"] is not None:
+            self.updatedDate = obj["updatedDate"]
+
+    def to_json(self):
+        """
+        Convert to a json version of Execution definition.
+        By default, use DS API format.
+        """
+        obj = {
+            "id": str(self.pipeline_id)
+        }
+        if self.key is not None:
+            obj["key"] = self.key
+        if self.steps is not None:
+            obj_steps = []
+            step: PipelineStep
+            for step in self.steps:
+                obj_steps.append(step.to_json())
+            obj["steps"] = json.dumps(obj_steps)
+        if self.plots is not None:
+            obj["plots"] = json.dumps(self.plots)
+        if self.variables is not None:
+            self.check_variables()
+            obj["variables"] = json.dumps(self.variables)
+        if self.template_id is not None:
+            obj["templateId"] = str(self.template_id)
+        if self.experiment_id is not None:
+            obj["experimentKey"] = str(self.experiment_id)
+        if self.createdById is not None:
+            obj["createdById"] = str(self.createdById)
+        if self.createdDate is not None:
+            obj["createdDate"] = str(self.createdDate)
+        if self.updatedById is not None:
+            obj["updatedById"] = str(self.updatedById)
+        if self.updatedDate is not None:
+            obj["updatedDate"] = str(self.updatedDate)
+        return obj
+
+
+
+
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/plot.py` & `wizata-dsapi-0.3.1/wizata_dsapi/plot.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,69 +1,69 @@
-import uuid
-from .api_dto import ApiDto
-
-
-class Plot(ApiDto):
-    """
-    A plot is a definition of a Plotly figure that can be stored and shared on Wizata.
-
-    :ivar plot_id: The UUID of the plot.
-    :ivar generatedById: The UUID of the Execution from which the plot was created.
-    :ivar name: A simple name helping the user identifying the plot.
-    :ivar figure: Plotly figure defining the plot itself.
-    """
-
-    def __init__(self, plot_id=None, name=None, generated_by_id=None, figure=None):
-        if plot_id is None:
-            self.plot_id = uuid.uuid4()
-        else:
-            self.plot_id = plot_id
-        self.name = name
-        self.generatedById = generated_by_id
-        self.figure = figure
-
-    def api_id(self) -> str:
-        """
-        Id of the plot (plot_id)
-
-        :return: string formatted UUID of the plot.
-        """
-        return str(self.plot_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate plots.
-        :return: Endpoint name.
-        """
-        return "Plots"
-
-    def from_json(self, obj):
-        """
-        Load the Plot entity from a dictionary representation of the Plot.
-
-        :param obj: Dict version of the Plot.
-        """
-        if "id" in obj.keys():
-            self.plot_id = uuid.UUID(obj["id"])
-        if "name" in obj.keys():
-            self.name = obj["name"]
-        if "figure" in obj.keys():
-            self.figure = obj["figure"]
-        if "generatedById" in obj.keys():
-            self.generatedById = obj["generatedById"]
-
-    def to_json(self):
-        """
-        Convert the plot to a dictionary compatible to JSON format.
-
-        :return: dictionary representation of the Plot object.
-        """
-        obj = {
-            "id": str(self.plot_id)
-        }
-        if self.name is not None:
-            obj["name"] = self.name
-        if self.figure is not None:
-            obj["figure"] = self.figure
-        if self.generatedById is not None:
-            obj["generatedById"] = self.generatedById
-        return obj
+import uuid
+from .api_dto import ApiDto
+
+
+class Plot(ApiDto):
+    """
+    A plot is a definition of a Plotly figure that can be stored and shared on Wizata.
+
+    :ivar plot_id: The UUID of the plot.
+    :ivar generatedById: The UUID of the Execution from which the plot was created.
+    :ivar name: A simple name helping the user identifying the plot.
+    :ivar figure: Plotly figure defining the plot itself.
+    """
+
+    def __init__(self, plot_id=None, name=None, generated_by_id=None, figure=None):
+        if plot_id is None:
+            self.plot_id = uuid.uuid4()
+        else:
+            self.plot_id = plot_id
+        self.name = name
+        self.generatedById = generated_by_id
+        self.figure = figure
+
+    def api_id(self) -> str:
+        """
+        Id of the plot (plot_id)
+
+        :return: string formatted UUID of the plot.
+        """
+        return str(self.plot_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate plots.
+        :return: Endpoint name.
+        """
+        return "Plots"
+
+    def from_json(self, obj):
+        """
+        Load the Plot entity from a dictionary representation of the Plot.
+
+        :param obj: Dict version of the Plot.
+        """
+        if "id" in obj.keys():
+            self.plot_id = uuid.UUID(obj["id"])
+        if "name" in obj.keys():
+            self.name = obj["name"]
+        if "figure" in obj.keys():
+            self.figure = obj["figure"]
+        if "generatedById" in obj.keys():
+            self.generatedById = obj["generatedById"]
+
+    def to_json(self):
+        """
+        Convert the plot to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Plot object.
+        """
+        obj = {
+            "id": str(self.plot_id)
+        }
+        if self.name is not None:
+            obj["name"] = self.name
+        if self.figure is not None:
+            obj["figure"] = self.figure
+        if self.generatedById is not None:
+            obj["generatedById"] = self.generatedById
+        return obj
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/request.py` & `wizata-dsapi-0.3.1/wizata_dsapi/request.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,462 +1,462 @@
-import uuid
-from datetime import datetime, timedelta, timezone
-from .dataframe_toolkit import generate_epoch
-
-
-class Request:
-    """
-    A Request to fetch dataframes from Wizata App.
-
-    To execute the request please use a DS API client.
-
-    :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
-
-    :ivar template_id: UUID of the template.
-    :ivar template: str unique id of the template.
-    :ivar twin_id: UUID of the Digital Twin.
-    :ivar twin: str hardware id of the Digital Twin.
-
-    :ivar start: Datetime defining beginning of period.
-    :ivar end: Datetime defining end of period.
-    :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
-    :ivar interval: Interval in seconds between each aggregation.
-    :ivar filters: Filter to apply on the query (not yet fully implemented).
-    :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
-    :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
-    """
-
-    def __init__(self,
-                 datapoints=None,
-                 start=None,
-                 end=None,
-                 agg_method='mean',
-                 interval=None,
-                 null='drop',
-                 template_id=None,
-                 template=None,
-                 twin_id=None,
-                 twin=None,
-                 request_id=None,
-                 filters=None,
-                 options=None):
-        if request_id is None:
-            request_id = uuid.uuid4()
-        self.request_id = request_id
-        self.function = None
-
-        # Equipments & Data Points
-        self.equipments = []
-        if datapoints is not None:
-            self.add_datapoints(datapoints)
-
-        # Template & Registration
-        self.template = None
-        self.select_template(
-             template_id=template_id,
-             template_key=template,
-             twin_id=twin_id,
-             twin_hardware_id=twin
-        )
-
-        self.start = start
-        self.end = end
-
-        self.aggregation = agg_method
-        if interval is not None:
-            self.interval = int(interval) / 1000
-
-        self.filters = filters
-        self.options = options
-
-        self.on_off_sensor = None
-        self.restart_time = None
-        self.sensitivity = None
-        self.dataframe = None
-        self.extra_data = None
-        self.target_feat = None
-        self.connections = None
-        self.name = None
-
-        self.null = null
-
-    def prepare(self):
-        """
-        prepare a dict JSON compatible only for the QUERY part of the request.
-
-        :return: a dict JSON compatible
-        """
-        query = {}
-        if self.request_id is not None:
-            query["id"] = str(self.request_id)
-        if self.equipments is not None:
-            query["equipments_list"] = self.equipments
-        else:
-            raise KeyError("Missing data points inside the query - add_datapoints")
-        if self.start is not None and self.end is not None:
-
-            if isinstance(self.start, str):
-                start = self.start
-            else:
-                start = self.__format_date(self.start)
-
-            if isinstance(self.end, str):
-                end = self.end
-            else:
-                end = self.__format_date(self.end)
-
-            query["timeframe"] = {
-                "start": start,
-                "end": end
-            }
-        else:
-            raise KeyError("Missing start and end date, please use datatime format")
-        if self.aggregation is not None and self.interval:
-            query["aggregations"] = {
-                "agg_method": self.aggregation,
-                "interval": self.interval * 1000
-            }
-        else:
-            raise KeyError("Missing aggregations information inside the request")
-        if self.null is not None and self.null != 'drop':
-            query['null'] = self.null
-        if self.template is not None:
-            query['template'] = self.template
-        if self.filters is not None:
-            query['filters'] = self.filters
-        if self.options is not None:
-            query['options'] = self.options
-        return query
-
-    def __format_date(self, dt_to_format):
-        if isinstance(dt_to_format, datetime):
-            millisec = dt_to_format.timestamp() * 1000
-            return int(millisec)
-        else:
-            raise TypeError("date is not a valid datetime")
-
-    def start_time(self, now=None) -> datetime:
-        """
-        get start time
-        :param now: override now value for relative datetime
-        :return: start datetime
-        """
-        if self.start is None:
-            raise ValueError('missing start datetime')
-        elif isinstance(self.start, str):
-            return datetime.fromtimestamp(generate_epoch(self.start, now=now) / 1000, timezone.utc)
-        elif isinstance(self.start, datetime):
-            return self.start
-        else:
-            raise TypeError(f'unsupported start datetime type {self.start.__class__.__name__}')
-
-    def end_time(self, now=None) -> datetime:
-        """
-        get end time
-        :param now: override now value for relative datetime
-        :return: start datetime
-        """
-        if self.end is None:
-            raise ValueError('missing end datetime')
-        elif isinstance(self.end, str):
-            return datetime.fromtimestamp(generate_epoch(self.end, now=now) / 1000, timezone.utc)
-        elif isinstance(self.end, datetime):
-            return self.end
-        else:
-            raise TypeError(f'unsupported end datetime type {self.end.__class__.__name__}')
-
-    def add_datapoints(self, datapoints, shift: int = 0):
-        """
-        Add datapoints to fetch without defining its equipments.
-        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
-        :param shift: Shift to apply in seconds on timestamp, by default 0.
-        """
-        self.equipments.append({
-            "id": None,
-            "datapoints": list(datapoints),
-            "shift": str(shift) + "s"
-        })
-
-    def get_datapoints(self) -> list:
-        """
-        return list of declared datapoints.
-        """
-        datapoints = []
-
-        if self.equipments is not None:
-            for equipment in self.equipments:
-                if "datapoints" not in equipment.keys():
-                    raise KeyError("No 'data points' have been provided for equipment with id '" +
-                                   str(equipment["id"]) + "'")
-                for datapoint in equipment["datapoints"]:
-                    if isinstance(datapoint, str):
-                        datapoints.append(datapoint)
-                    elif "id" in datapoint.keys():
-                        datapoints.append(datapoint["id"])
-                    else:
-                        raise KeyError("Incorrect datapoint declaration : '" + str(datapoint) + "'")
-
-        return datapoints
-
-    def set_datapoints(self, datapoints: list):
-        """
-        replace current datapoints by provided list
-        """
-        self.equipments = []
-        if datapoints is not None:
-            self.add_datapoints(datapoints)
-
-    def add_equipment(self, equipment_id: uuid.UUID, datapoints, shift=0):
-        """
-        Add datapoints to fetch with a Digital Twin ID identification.
-        :param equipment_id: UUID of the Digital Twin ID to which the datapoints are linked.
-        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
-        :param shift: Shift to apply in seconds on timestamp, by default 0.
-        """
-        if not isinstance(equipment_id, uuid.UUID):
-            raise TypeError("equipment_id must be of type uuid.UUID")
-        for equipment in self.equipments:
-            if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
-                raise ValueError("equipment_id is already in the request please remove it before adding datapoints.")
-        self.equipments.append({
-            "id": str(equipment_id),
-            "datapoints": list(datapoints),
-            "shift": str(shift) + "s"
-        })
-
-    # attempt to remove equipment from the query if exists
-    def remove_equipment(self, equipment_id: uuid.UUID):
-        """
-        Remove an equipment from the list including all its listed datapoints.
-        :param equipment_id: UUID of the Digital Twin item.
-        """
-        if equipment_id is not None and not isinstance(equipment_id, uuid.UUID):
-            raise TypeError("equipment_id must be None or of type uuid.UUID")
-        found = None
-        for equipment in self.equipments:
-            if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
-                found = equipment
-        if found is not None:
-            self.equipments.remove(equipment)
-
-    def set_aggregation(self, method, interval):
-        """
-        Specifies aggregation properties
-        :param method: 'mean' or 'stddev'
-        :param interval: interval in ms (will be stored in seconds)
-        """
-        if method not in self.list_agg_methods():
-            raise KeyError(f'unsupported agg_method {method}.')
-        self.aggregation = method
-        if interval is not None:
-            self.interval = int(interval) / 1000
-
-    def list_agg_methods(self) -> list:
-        """
-        get a list of all authorized methods.
-        :return: list of all authorized methods.
-        """
-        return [
-            "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max", "min"
-        ]
-
-    def select_template(self,
-                        template_id=None,
-                        template_key=None,
-                        twin_id=None,
-                        twin_hardware_id=None):
-        """
-        Select a template and its registration.
-        :param template_id: template UUID
-        :param template_key: template key ( ignored if template_id specified )
-        :param twin_id: Digital Twin UUID
-        :param twin_hardware_id: hardware ID of Digital Twin ( ignored if twin_id specified )
-        """
-        if template_id is None and template_key is None and twin_id is None and twin_hardware_id is None:
-            self.template = None
-            return
-        else:
-            self.template = {}
-
-            if template_id is not None:
-                self.template['template_id'] = uuid.UUID(template_id)
-            elif template_key is not None:
-                self.template['template_key'] = str(template_key)
-            else:
-                raise ValueError('A twin can only be specified with its template')
-
-            if twin_id is not None:
-                self.template['twin_id'] = uuid.UUID(twin_id)
-            elif twin_hardware_id is not None:
-                self.template['twin_hardware_id'] = str(twin_hardware_id)
-            else:
-                raise ValueError('A template can only be specified with its registered twin')
-
-    def get_params(self):
-        """
-        get a list of all parameters.
-        """
-        params = []
-
-        if self.start is not None and isinstance(self.start, str) and self.start.startswith("@"):
-            params.append(self.start[1:])
-
-        if self.end is not None and isinstance(self.end, str) and self.end.startswith("@"):
-            params.append(self.end[1:])
-
-        return list(set(params))
-
-    def set_param(self, name: str, value):
-        """
-        set value of parameter based on his name.
-        """
-        assigned = False
-
-        if value is None:
-            raise ValueError(f'please provide a valid param value for {name}')
-
-        if self.start is not None and isinstance(self.start, str) \
-                and self.start.startswith("@") and self.start[1:] == name:
-            self.start = value
-            assigned = True
-
-        if self.end is not None and isinstance(self.end, str) \
-                and self.end.startswith("@") and self.end[1:] == name:
-            self.end = value
-            assigned = True
-
-        if not assigned:
-            raise KeyError(f'parameter {name} not found in request.')
-
-    def to_json(self):
-        """
-        convert to a dict JSON compatible for all properties. For query only, use prepare().
-
-        :return: a dict JSON compatible
-        """
-
-        # Prepare is 'to_json' without future obsolete properties
-        obj = self.prepare()
-
-        if self.target_feat is not None:
-            obj["target_feat"] = {
-                "sensor": self.target_feat["sensor"],
-                "operator": self.target_feat["operator"],
-                "threshold": self.target_feat["threshold"]
-            }
-        if self.on_off_sensor is not None and self.restart_time is not None:
-            obj["restart_filter"] = {
-                "on_off_sensor": self.on_off_sensor,
-                "stop_restart_time": self.restart_time
-            }
-
-        if self.sensitivity is not None:
-            obj["sensitivity"] = self.sensitivity
-
-        if self.extra_data is not None:
-            obj["extra_data"] = self.extra_data
-
-        return obj
-
-    def from_json(self, json_data):
-        """
-        load a request based on dict from a JSON file.
-
-        :param json_data: JSON formatted dictionnary object representing a query.
-        """
-        if "id" in json_data.keys():
-            self.request_id = uuid.UUID(json_data["id"])
-
-        if "name" in json_data.keys():
-            self.name = json_data["name"]
-
-        found_dps = False
-        if "equipments_list" in json_data.keys():
-            self.equipments = json_data["equipments_list"]
-            for equipment in self.equipments:
-                if "datapoints" not in equipment.keys():
-                    raise KeyError("No 'data points' have been provided for equipment with id '" +
-                                   str(equipment["id"]) + "'")
-                else:
-                    found_dps = True
-        elif "datapoints" in json_data.keys():
-            equipment = {"datapoints": []}
-            for datapoint in json_data["datapoints"]:
-                equipment["datapoints"].append(datapoint)
-            self.equipments.append(equipment)
-            found_dps = True
-
-        if "template" in json_data.keys():
-            self.template = json_data["template"]
-            found_dps = True
-
-        if not found_dps:
-            raise KeyError('no equipments_list datapoints, nor template specified inside the request.')
-
-        if "timeframe" not in json_data.keys():
-            raise KeyError("No 'time range' have been selected, please set it up and re-try.")
-
-        if "start" not in json_data["timeframe"].keys():
-            raise KeyError("No 'start time' have been selected, please set it up and re-try.")
-
-        if isinstance(json_data["timeframe"]["start"], str):
-            self.start = json_data["timeframe"]["start"]
-        else:
-            self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000, timezone.utc)
-
-        if "end" not in json_data["timeframe"].keys():
-            raise KeyError("No 'end time' have been selected, please set it up and re-try.")
-
-        if isinstance(json_data["timeframe"]["end"], str):
-            self.end = json_data["timeframe"]["end"]
-        else:
-            self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000, timezone.utc)
-
-        if "aggregations" not in json_data.keys():
-            raise KeyError("No 'aggregations' have been selected, please set it up and re-try.")
-
-        if "agg_method" not in json_data["aggregations"].keys():
-            raise KeyError("No 'Aggregation Method' have been selected, please set it up and re-try.")
-        if json_data["aggregations"]["agg_method"] not in self.list_agg_methods():
-            raise KeyError(f'unsupported agg_method {json_data["aggregations"]["agg_method"]}.')
-        self.aggregation = json_data["aggregations"]["agg_method"]
-
-        if "interval" not in json_data["aggregations"].keys():
-            raise KeyError("No 'Aggregation Interval' have been selected, please set it up and re-try.")
-        self.interval = int(json_data["aggregations"]["interval"] / 1000)
-
-        if "filters" in json_data.keys():
-            self.filters = json_data["filters"]
-        else:
-            self.filters = {}
-
-        if "options" in json_data.keys():
-            self.options = json_data["options"]
-        else:
-            self.options = {}
-
-        if "connections" in json_data.keys():
-            self.connections = json_data["connections"]
-
-        if "null" in json_data.keys():
-            self.null = json_data["null"]
-
-        if "target_feat" in json_data.keys():
-            self.target_feat = json_data["target_feat"]
-            if "sensor" not in self.target_feat.keys():
-                raise KeyError("No 'sensor' have been declared inside the target feature, this is a technical error.")
-            if "operator" not in self.target_feat.keys():
-                raise KeyError("No 'operator' have been declared inside the target feature, this is a technical error.")
-            if "threshold" not in self.target_feat.keys():
-                raise KeyError("No 'threshold' have been declared inside the target feature, this is a technical error.")
-
-        if "restart_filter" in json_data.keys():
-            self.on_off_sensor = json_data["restart_filter"]["on_off_sensor"]
-            self.restart_time = json_data["restart_filter"]["stop_restart_time"]
-
-        if "sensitivity" in json_data.keys():
-            self.sensitivity = json_data["sensitivity"]
-
-        if "extra_data" in json_data.keys():
-            self.extra_data = json_data["extra_data"]
-
-
+import uuid
+from datetime import datetime, timedelta, timezone
+from .dataframe_toolkit import generate_epoch
+
+
+class Request:
+    """
+    A Request to fetch dataframes from Wizata App.
+
+    To execute the request please use a DS API client.
+
+    :ivar equipments: List of Equipments containing Digital Twin item and datapoints to fetch.
+
+    :ivar template_id: UUID of the template.
+    :ivar template: str unique id of the template.
+    :ivar twin_id: UUID of the Digital Twin.
+    :ivar twin: str hardware id of the Digital Twin.
+
+    :ivar start: Datetime defining beginning of period.
+    :ivar end: Datetime defining end of period.
+    :ivar aggregation: Aggregation method to fetch, accept "mean" and "stddev".
+    :ivar interval: Interval in seconds between each aggregation.
+    :ivar filters: Filter to apply on the query (not yet fully implemented).
+    :ivar connections: Connections rules between equipment to align data in time (not yet fully implemented).
+    :ivar null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
+    """
+
+    def __init__(self,
+                 datapoints=None,
+                 start=None,
+                 end=None,
+                 agg_method='mean',
+                 interval=None,
+                 null='drop',
+                 template_id=None,
+                 template=None,
+                 twin_id=None,
+                 twin=None,
+                 request_id=None,
+                 filters=None,
+                 options=None):
+        if request_id is None:
+            request_id = uuid.uuid4()
+        self.request_id = request_id
+        self.function = None
+
+        # Equipments & Data Points
+        self.equipments = []
+        if datapoints is not None:
+            self.add_datapoints(datapoints)
+
+        # Template & Registration
+        self.template = None
+        self.select_template(
+             template_id=template_id,
+             template_key=template,
+             twin_id=twin_id,
+             twin_hardware_id=twin
+        )
+
+        self.start = start
+        self.end = end
+
+        self.aggregation = agg_method
+        if interval is not None:
+            self.interval = int(interval) / 1000
+
+        self.filters = filters
+        self.options = options
+
+        self.on_off_sensor = None
+        self.restart_time = None
+        self.sensitivity = None
+        self.dataframe = None
+        self.extra_data = None
+        self.target_feat = None
+        self.connections = None
+        self.name = None
+
+        self.null = null
+
+    def prepare(self):
+        """
+        prepare a dict JSON compatible only for the QUERY part of the request.
+
+        :return: a dict JSON compatible
+        """
+        query = {}
+        if self.request_id is not None:
+            query["id"] = str(self.request_id)
+        if self.equipments is not None:
+            query["equipments_list"] = self.equipments
+        else:
+            raise KeyError("Missing data points inside the query - add_datapoints")
+        if self.start is not None and self.end is not None:
+
+            if isinstance(self.start, str):
+                start = self.start
+            else:
+                start = self.__format_date(self.start)
+
+            if isinstance(self.end, str):
+                end = self.end
+            else:
+                end = self.__format_date(self.end)
+
+            query["timeframe"] = {
+                "start": start,
+                "end": end
+            }
+        else:
+            raise KeyError("Missing start and end date, please use datatime format")
+        if self.aggregation is not None and self.interval:
+            query["aggregations"] = {
+                "agg_method": self.aggregation,
+                "interval": self.interval * 1000
+            }
+        else:
+            raise KeyError("Missing aggregations information inside the request")
+        if self.null is not None and self.null != 'drop':
+            query['null'] = self.null
+        if self.template is not None:
+            query['template'] = self.template
+        if self.filters is not None:
+            query['filters'] = self.filters
+        if self.options is not None:
+            query['options'] = self.options
+        return query
+
+    def __format_date(self, dt_to_format):
+        if isinstance(dt_to_format, datetime):
+            millisec = dt_to_format.timestamp() * 1000
+            return int(millisec)
+        else:
+            raise TypeError("date is not a valid datetime")
+
+    def start_time(self, now=None) -> datetime:
+        """
+        get start time
+        :param now: override now value for relative datetime
+        :return: start datetime
+        """
+        if self.start is None:
+            raise ValueError('missing start datetime')
+        elif isinstance(self.start, str):
+            return datetime.fromtimestamp(generate_epoch(self.start, now=now) / 1000, timezone.utc)
+        elif isinstance(self.start, datetime):
+            return self.start
+        else:
+            raise TypeError(f'unsupported start datetime type {self.start.__class__.__name__}')
+
+    def end_time(self, now=None) -> datetime:
+        """
+        get end time
+        :param now: override now value for relative datetime
+        :return: start datetime
+        """
+        if self.end is None:
+            raise ValueError('missing end datetime')
+        elif isinstance(self.end, str):
+            return datetime.fromtimestamp(generate_epoch(self.end, now=now) / 1000, timezone.utc)
+        elif isinstance(self.end, datetime):
+            return self.end
+        else:
+            raise TypeError(f'unsupported end datetime type {self.end.__class__.__name__}')
+
+    def add_datapoints(self, datapoints, shift: int = 0):
+        """
+        Add datapoints to fetch without defining its equipments.
+        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
+        :param shift: Shift to apply in seconds on timestamp, by default 0.
+        """
+        self.equipments.append({
+            "id": None,
+            "datapoints": list(datapoints),
+            "shift": str(shift) + "s"
+        })
+
+    def get_datapoints(self) -> list:
+        """
+        return list of declared datapoints.
+        """
+        datapoints = []
+
+        if self.equipments is not None:
+            for equipment in self.equipments:
+                if "datapoints" not in equipment.keys():
+                    raise KeyError("No 'data points' have been provided for equipment with id '" +
+                                   str(equipment["id"]) + "'")
+                for datapoint in equipment["datapoints"]:
+                    if isinstance(datapoint, str):
+                        datapoints.append(datapoint)
+                    elif "id" in datapoint.keys():
+                        datapoints.append(datapoint["id"])
+                    else:
+                        raise KeyError("Incorrect datapoint declaration : '" + str(datapoint) + "'")
+
+        return datapoints
+
+    def set_datapoints(self, datapoints: list):
+        """
+        replace current datapoints by provided list
+        """
+        self.equipments = []
+        if datapoints is not None:
+            self.add_datapoints(datapoints)
+
+    def add_equipment(self, equipment_id: uuid.UUID, datapoints, shift=0):
+        """
+        Add datapoints to fetch with a Digital Twin ID identification.
+        :param equipment_id: UUID of the Digital Twin ID to which the datapoints are linked.
+        :param datapoints: List(str) of datapoints to fetch identified by Hardware ID.
+        :param shift: Shift to apply in seconds on timestamp, by default 0.
+        """
+        if not isinstance(equipment_id, uuid.UUID):
+            raise TypeError("equipment_id must be of type uuid.UUID")
+        for equipment in self.equipments:
+            if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
+                raise ValueError("equipment_id is already in the request please remove it before adding datapoints.")
+        self.equipments.append({
+            "id": str(equipment_id),
+            "datapoints": list(datapoints),
+            "shift": str(shift) + "s"
+        })
+
+    # attempt to remove equipment from the query if exists
+    def remove_equipment(self, equipment_id: uuid.UUID):
+        """
+        Remove an equipment from the list including all its listed datapoints.
+        :param equipment_id: UUID of the Digital Twin item.
+        """
+        if equipment_id is not None and not isinstance(equipment_id, uuid.UUID):
+            raise TypeError("equipment_id must be None or of type uuid.UUID")
+        found = None
+        for equipment in self.equipments:
+            if "id" in equipment.keys() and equipment["id"] == str(equipment_id):
+                found = equipment
+        if found is not None:
+            self.equipments.remove(equipment)
+
+    def set_aggregation(self, method, interval):
+        """
+        Specifies aggregation properties
+        :param method: 'mean' or 'stddev'
+        :param interval: interval in ms (will be stored in seconds)
+        """
+        if method not in self.list_agg_methods():
+            raise KeyError(f'unsupported agg_method {method}.')
+        self.aggregation = method
+        if interval is not None:
+            self.interval = int(interval) / 1000
+
+    def list_agg_methods(self) -> list:
+        """
+        get a list of all authorized methods.
+        :return: list of all authorized methods.
+        """
+        return [
+            "mean", "stddev", "mode", "median", "count", "sum", "first", "last", "max", "min"
+        ]
+
+    def select_template(self,
+                        template_id=None,
+                        template_key=None,
+                        twin_id=None,
+                        twin_hardware_id=None):
+        """
+        Select a template and its registration.
+        :param template_id: template UUID
+        :param template_key: template key ( ignored if template_id specified )
+        :param twin_id: Digital Twin UUID
+        :param twin_hardware_id: hardware ID of Digital Twin ( ignored if twin_id specified )
+        """
+        if template_id is None and template_key is None and twin_id is None and twin_hardware_id is None:
+            self.template = None
+            return
+        else:
+            self.template = {}
+
+            if template_id is not None:
+                self.template['template_id'] = uuid.UUID(template_id)
+            elif template_key is not None:
+                self.template['template_key'] = str(template_key)
+            else:
+                raise ValueError('A twin can only be specified with its template')
+
+            if twin_id is not None:
+                self.template['twin_id'] = uuid.UUID(twin_id)
+            elif twin_hardware_id is not None:
+                self.template['twin_hardware_id'] = str(twin_hardware_id)
+            else:
+                raise ValueError('A template can only be specified with its registered twin')
+
+    def get_params(self):
+        """
+        get a list of all parameters.
+        """
+        params = []
+
+        if self.start is not None and isinstance(self.start, str) and self.start.startswith("@"):
+            params.append(self.start[1:])
+
+        if self.end is not None and isinstance(self.end, str) and self.end.startswith("@"):
+            params.append(self.end[1:])
+
+        return list(set(params))
+
+    def set_param(self, name: str, value):
+        """
+        set value of parameter based on his name.
+        """
+        assigned = False
+
+        if value is None:
+            raise ValueError(f'please provide a valid param value for {name}')
+
+        if self.start is not None and isinstance(self.start, str) \
+                and self.start.startswith("@") and self.start[1:] == name:
+            self.start = value
+            assigned = True
+
+        if self.end is not None and isinstance(self.end, str) \
+                and self.end.startswith("@") and self.end[1:] == name:
+            self.end = value
+            assigned = True
+
+        if not assigned:
+            raise KeyError(f'parameter {name} not found in request.')
+
+    def to_json(self):
+        """
+        convert to a dict JSON compatible for all properties. For query only, use prepare().
+
+        :return: a dict JSON compatible
+        """
+
+        # Prepare is 'to_json' without future obsolete properties
+        obj = self.prepare()
+
+        if self.target_feat is not None:
+            obj["target_feat"] = {
+                "sensor": self.target_feat["sensor"],
+                "operator": self.target_feat["operator"],
+                "threshold": self.target_feat["threshold"]
+            }
+        if self.on_off_sensor is not None and self.restart_time is not None:
+            obj["restart_filter"] = {
+                "on_off_sensor": self.on_off_sensor,
+                "stop_restart_time": self.restart_time
+            }
+
+        if self.sensitivity is not None:
+            obj["sensitivity"] = self.sensitivity
+
+        if self.extra_data is not None:
+            obj["extra_data"] = self.extra_data
+
+        return obj
+
+    def from_json(self, json_data):
+        """
+        load a request based on dict from a JSON file.
+
+        :param json_data: JSON formatted dictionnary object representing a query.
+        """
+        if "id" in json_data.keys():
+            self.request_id = uuid.UUID(json_data["id"])
+
+        if "name" in json_data.keys():
+            self.name = json_data["name"]
+
+        found_dps = False
+        if "equipments_list" in json_data.keys():
+            self.equipments = json_data["equipments_list"]
+            for equipment in self.equipments:
+                if "datapoints" not in equipment.keys():
+                    raise KeyError("No 'data points' have been provided for equipment with id '" +
+                                   str(equipment["id"]) + "'")
+                else:
+                    found_dps = True
+        elif "datapoints" in json_data.keys():
+            equipment = {"datapoints": []}
+            for datapoint in json_data["datapoints"]:
+                equipment["datapoints"].append(datapoint)
+            self.equipments.append(equipment)
+            found_dps = True
+
+        if "template" in json_data.keys():
+            self.template = json_data["template"]
+            found_dps = True
+
+        if not found_dps:
+            raise KeyError('no equipments_list datapoints, nor template specified inside the request.')
+
+        if "timeframe" not in json_data.keys():
+            raise KeyError("No 'time range' have been selected, please set it up and re-try.")
+
+        if "start" not in json_data["timeframe"].keys():
+            raise KeyError("No 'start time' have been selected, please set it up and re-try.")
+
+        if isinstance(json_data["timeframe"]["start"], str):
+            self.start = json_data["timeframe"]["start"]
+        else:
+            self.start = datetime.fromtimestamp(json_data["timeframe"]["start"] / 1000, timezone.utc)
+
+        if "end" not in json_data["timeframe"].keys():
+            raise KeyError("No 'end time' have been selected, please set it up and re-try.")
+
+        if isinstance(json_data["timeframe"]["end"], str):
+            self.end = json_data["timeframe"]["end"]
+        else:
+            self.end = datetime.fromtimestamp(json_data["timeframe"]["end"] / 1000, timezone.utc)
+
+        if "aggregations" not in json_data.keys():
+            raise KeyError("No 'aggregations' have been selected, please set it up and re-try.")
+
+        if "agg_method" not in json_data["aggregations"].keys():
+            raise KeyError("No 'Aggregation Method' have been selected, please set it up and re-try.")
+        if json_data["aggregations"]["agg_method"] not in self.list_agg_methods():
+            raise KeyError(f'unsupported agg_method {json_data["aggregations"]["agg_method"]}.')
+        self.aggregation = json_data["aggregations"]["agg_method"]
+
+        if "interval" not in json_data["aggregations"].keys():
+            raise KeyError("No 'Aggregation Interval' have been selected, please set it up and re-try.")
+        self.interval = int(json_data["aggregations"]["interval"] / 1000)
+
+        if "filters" in json_data.keys():
+            self.filters = json_data["filters"]
+        else:
+            self.filters = {}
+
+        if "options" in json_data.keys():
+            self.options = json_data["options"]
+        else:
+            self.options = {}
+
+        if "connections" in json_data.keys():
+            self.connections = json_data["connections"]
+
+        if "null" in json_data.keys():
+            self.null = json_data["null"]
+
+        if "target_feat" in json_data.keys():
+            self.target_feat = json_data["target_feat"]
+            if "sensor" not in self.target_feat.keys():
+                raise KeyError("No 'sensor' have been declared inside the target feature, this is a technical error.")
+            if "operator" not in self.target_feat.keys():
+                raise KeyError("No 'operator' have been declared inside the target feature, this is a technical error.")
+            if "threshold" not in self.target_feat.keys():
+                raise KeyError("No 'threshold' have been declared inside the target feature, this is a technical error.")
+
+        if "restart_filter" in json_data.keys():
+            self.on_off_sensor = json_data["restart_filter"]["on_off_sensor"]
+            self.restart_time = json_data["restart_filter"]["stop_restart_time"]
+
+        if "sensitivity" in json_data.keys():
+            self.sensitivity = json_data["sensitivity"]
+
+        if "extra_data" in json_data.keys():
+            self.extra_data = json_data["extra_data"]
+
+
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/script.py` & `wizata-dsapi-0.3.1/wizata_dsapi/script.py`

 * *Ordering differences only*

 * *Files 25% similar despite different names*

```diff
@@ -1,231 +1,231 @@
-import json
-import uuid
-import dill
-import os
-import types
-from .api_dto import ApiDto
-import inspect
-from collections import OrderedDict
-
-
-class ScriptConfig(ApiDto):
-    """
-    a script config defines execution properties for a specific script.
-    usually to define how a pipeline should call your script.
-
-    :ivar function: name of function referencing the script.
-    """
-
-    def __init__(self, function=None):
-        self.function = function
-
-    def from_json(self, obj):
-        if isinstance(obj, str):
-            self.function = obj
-            return
-        else:
-            if "function" in obj:
-                self.function = obj["function"]
-
-    def to_json(self):
-        obj = {
-            "function": self.function
-        }
-        return obj
-
-class Script(ApiDto):
-    """
-    A piece of python code that can either transform data, generate plot or train Machine Learning Models.
-
-    Scripts once validated can be used from Python or directly inside Wizata App by users.
-
-    :ivar script_id: The UUID of the ML Model.
-    :ivar description: Provide an insight-full description of what does your script.
-    :ivar status: 'draft', 'valid' or 'invalid' - to validate your script use client validate method.
-    :ivar needExactColumnNumbers: False by default, define if the model requires exact columns numbers to be executed.
-    :ivar needExactColumnNames: False by default, define if the model requires exact columns names to be executed.
-    :ivar canGeneratePlot: Set during validation, inform if the script generate plotly figures from dataframe.
-    :ivar canGenerateData: Set during validation, inform if the script transform input dataframe into another one.
-    :ivar canGenerateModel: Set during validation, inform if the script trains Machine Learning models from dataframe.
-    :ivar inputColumns: list of all columns used to call the script the model.
-    :ivar outputColumns: list of all columns generated by the script if it generates data.
-    :ivar function: Dill object containing the function code and decorators, please use copy()
-    """
-
-    def __init__(self, script_id=None, description=None, function=None,
-                 exact_names=False, exact_numbers=False):
-
-        # Id
-        if script_id is None:
-            script_id = uuid.uuid4()
-        self.script_id = script_id
-        self._name = None
-
-        # Properties
-        self.description = description
-        self.needExactColumnNumbers = exact_numbers
-        self.needExactColumnNames = exact_names
-
-        # Validation Properties
-        self.canGeneratePlot = False
-        self.canGenerateModel = False
-        self.canGenerateData = False
-        self.status = "draft"
-        self.inputColumns = []
-        self.outputColumns = []
-
-        # Source code property
-        self.source = None
-
-        # Function properties (code)
-        self.function = None
-        if function is not None:
-            self.copy(function)
-
-
-    @property
-    def name(self):
-        """
-        Name of the function
-        :return: name of the function
-        """
-        return self._name
-
-    def api_id(self) -> str:
-        """
-        Id of the script (script_id)
-
-        :return: string formatted UUID of the script.
-        """
-        return str(self.script_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate scripts.
-        :return: Endpoint name.
-        """
-        return "Scripts"
-
-    def to_json(self):
-        """
-        Convert the script to a dictionary compatible to JSON format.
-
-        :return: dictionary representation of the Script object.
-        """
-        obj = {
-            "id": str(self.script_id),
-            "canGeneratePlot": str(self.canGeneratePlot),
-            "canGenerateModel": str(self.canGenerateModel),
-            "canGenerateData": str(self.canGenerateData),
-            "status": str(self.status),
-            "needExactColumnNumbers": str(self.needExactColumnNumbers),
-            "needExactColumnNames": str(self.needExactColumnNames),
-            "inputColumns": json.dumps(list(self.inputColumns)),
-            "outputColumns": json.dumps(list(self.outputColumns))
-        }
-        if self.name is not None:
-            obj["name"] = str(self.name)
-        if self.name is not None:
-            obj["description"] = str(self.description)
-        return obj
-
-    def from_json(self, obj):
-        """
-        Load the Script entity from a dictionary representation of the Script.
-
-        :param obj: Dict version of the Script.
-        """
-        if "id" in obj.keys():
-            self.script_id = uuid.UUID(obj["id"])
-        if "name" in obj.keys():
-            self._name = obj["name"]
-        if "description" in obj.keys():
-            if obj["description"] != "None":
-                self.description = obj["description"]
-        if "canGeneratePlot" in obj.keys():
-            if isinstance(obj["canGeneratePlot"], str) and obj["canGeneratePlot"].lower() == "false":
-                self.canGeneratePlot = False
-            else:
-                self.canGeneratePlot = bool(obj["canGeneratePlot"])
-        if "canGenerateModel" in obj.keys():
-            if isinstance(obj["canGenerateModel"], str) and obj["canGenerateModel"].lower() == "false":
-                self.canGenerateModel = False
-            else:
-                self.canGenerateModel = bool(obj["canGenerateModel"])
-        if "canGenerateData" in obj.keys():
-            if isinstance(obj["canGenerateData"], str) and obj["canGenerateData"].lower() == "false":
-                self.canGenerateData = False
-            else:
-                self.canGenerateData = bool(obj["canGenerateData"])
-        if "status" in obj.keys():
-            self.status = str(obj["status"]).lower()
-        if "needExactColumnNumbers" in obj.keys():
-            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
-                self.needExactColumnNumbers = False
-            else:
-                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
-        if "needExactColumnNames" in obj.keys():
-            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
-                self.needExactColumnNames = False
-            else:
-                self.needExactColumnNames = bool(obj["needExactColumnNames"])
-        if "inputColumns" in obj.keys():
-            if obj["inputColumns"].lower() == "false":
-                self.inputColumns = False
-            else:
-                self.inputColumns = json.loads(obj["inputColumns"])
-        if "outputColumns" in obj.keys():
-            if obj["outputColumns"].lower() == "false":
-                self.outputColumns = False
-            else:
-                self.outputColumns = json.loads(obj["outputColumns"])
-
-    def copy(self, myfunction):
-        """
-        Copy your function code and decorators to a format executable by the Wizata App.
-        :param myfunction: your function - pass the function itself as parameter
-        """
-
-        if myfunction.__code__.co_argcount < 1:
-            raise ValueError('your function must contains at least one parameter')
-
-        self.function = Function()
-
-        self.function.id = myfunction.__name__
-        self.function.params = inspect.signature(myfunction).parameters
-
-        self._name = myfunction.__name__
-
-        self.function.code = myfunction.__code__
-
-        f_globals = myfunction.__globals__
-        self.function.globals = []
-        for k_global in f_globals:
-            if isinstance(myfunction.__globals__[k_global], types.ModuleType):
-                module = f_globals[k_global]
-                self.function.globals.append({
-                    "var": k_global,
-                    "module": str(module.__name__)
-                })
-
-        if myfunction.__code__.co_filename is not None:
-            if os.path.exists(myfunction.__code__.co_filename):
-                with open(myfunction.__code__.co_filename, "r") as f:
-                    source_code = f.read()
-                self.source = source_code
-
-
-class Function:
-    """
-    Python Code Function
-
-    :ivar id: technical name and then id of the function
-    :ivar code: code of the function __code__
-    :ivar globals: modules references __globals__
-    """
-
-    def __init__(self):
-        self.id = None
-        self.code = None
-        self.globals = None
-        self.params = OrderedDict()
+import json
+import uuid
+import dill
+import os
+import types
+from .api_dto import ApiDto
+import inspect
+from collections import OrderedDict
+
+
+class ScriptConfig(ApiDto):
+    """
+    a script config defines execution properties for a specific script.
+    usually to define how a pipeline should call your script.
+
+    :ivar function: name of function referencing the script.
+    """
+
+    def __init__(self, function=None):
+        self.function = function
+
+    def from_json(self, obj):
+        if isinstance(obj, str):
+            self.function = obj
+            return
+        else:
+            if "function" in obj:
+                self.function = obj["function"]
+
+    def to_json(self):
+        obj = {
+            "function": self.function
+        }
+        return obj
+
+class Script(ApiDto):
+    """
+    A piece of python code that can either transform data, generate plot or train Machine Learning Models.
+
+    Scripts once validated can be used from Python or directly inside Wizata App by users.
+
+    :ivar script_id: The UUID of the ML Model.
+    :ivar description: Provide an insight-full description of what does your script.
+    :ivar status: 'draft', 'valid' or 'invalid' - to validate your script use client validate method.
+    :ivar needExactColumnNumbers: False by default, define if the model requires exact columns numbers to be executed.
+    :ivar needExactColumnNames: False by default, define if the model requires exact columns names to be executed.
+    :ivar canGeneratePlot: Set during validation, inform if the script generate plotly figures from dataframe.
+    :ivar canGenerateData: Set during validation, inform if the script transform input dataframe into another one.
+    :ivar canGenerateModel: Set during validation, inform if the script trains Machine Learning models from dataframe.
+    :ivar inputColumns: list of all columns used to call the script the model.
+    :ivar outputColumns: list of all columns generated by the script if it generates data.
+    :ivar function: Dill object containing the function code and decorators, please use copy()
+    """
+
+    def __init__(self, script_id=None, description=None, function=None,
+                 exact_names=False, exact_numbers=False):
+
+        # Id
+        if script_id is None:
+            script_id = uuid.uuid4()
+        self.script_id = script_id
+        self._name = None
+
+        # Properties
+        self.description = description
+        self.needExactColumnNumbers = exact_numbers
+        self.needExactColumnNames = exact_names
+
+        # Validation Properties
+        self.canGeneratePlot = False
+        self.canGenerateModel = False
+        self.canGenerateData = False
+        self.status = "draft"
+        self.inputColumns = []
+        self.outputColumns = []
+
+        # Source code property
+        self.source = None
+
+        # Function properties (code)
+        self.function = None
+        if function is not None:
+            self.copy(function)
+
+
+    @property
+    def name(self):
+        """
+        Name of the function
+        :return: name of the function
+        """
+        return self._name
+
+    def api_id(self) -> str:
+        """
+        Id of the script (script_id)
+
+        :return: string formatted UUID of the script.
+        """
+        return str(self.script_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate scripts.
+        :return: Endpoint name.
+        """
+        return "Scripts"
+
+    def to_json(self):
+        """
+        Convert the script to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Script object.
+        """
+        obj = {
+            "id": str(self.script_id),
+            "canGeneratePlot": str(self.canGeneratePlot),
+            "canGenerateModel": str(self.canGenerateModel),
+            "canGenerateData": str(self.canGenerateData),
+            "status": str(self.status),
+            "needExactColumnNumbers": str(self.needExactColumnNumbers),
+            "needExactColumnNames": str(self.needExactColumnNames),
+            "inputColumns": json.dumps(list(self.inputColumns)),
+            "outputColumns": json.dumps(list(self.outputColumns))
+        }
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.name is not None:
+            obj["description"] = str(self.description)
+        return obj
+
+    def from_json(self, obj):
+        """
+        Load the Script entity from a dictionary representation of the Script.
+
+        :param obj: Dict version of the Script.
+        """
+        if "id" in obj.keys():
+            self.script_id = uuid.UUID(obj["id"])
+        if "name" in obj.keys():
+            self._name = obj["name"]
+        if "description" in obj.keys():
+            if obj["description"] != "None":
+                self.description = obj["description"]
+        if "canGeneratePlot" in obj.keys():
+            if isinstance(obj["canGeneratePlot"], str) and obj["canGeneratePlot"].lower() == "false":
+                self.canGeneratePlot = False
+            else:
+                self.canGeneratePlot = bool(obj["canGeneratePlot"])
+        if "canGenerateModel" in obj.keys():
+            if isinstance(obj["canGenerateModel"], str) and obj["canGenerateModel"].lower() == "false":
+                self.canGenerateModel = False
+            else:
+                self.canGenerateModel = bool(obj["canGenerateModel"])
+        if "canGenerateData" in obj.keys():
+            if isinstance(obj["canGenerateData"], str) and obj["canGenerateData"].lower() == "false":
+                self.canGenerateData = False
+            else:
+                self.canGenerateData = bool(obj["canGenerateData"])
+        if "status" in obj.keys():
+            self.status = str(obj["status"]).lower()
+        if "needExactColumnNumbers" in obj.keys():
+            if isinstance(obj["needExactColumnNumbers"], str) and obj["needExactColumnNumbers"].lower() == "false":
+                self.needExactColumnNumbers = False
+            else:
+                self.needExactColumnNumbers = bool(obj["needExactColumnNumbers"])
+        if "needExactColumnNames" in obj.keys():
+            if isinstance(obj["needExactColumnNames"], str) and obj["needExactColumnNames"].lower() == "false":
+                self.needExactColumnNames = False
+            else:
+                self.needExactColumnNames = bool(obj["needExactColumnNames"])
+        if "inputColumns" in obj.keys():
+            if obj["inputColumns"].lower() == "false":
+                self.inputColumns = False
+            else:
+                self.inputColumns = json.loads(obj["inputColumns"])
+        if "outputColumns" in obj.keys():
+            if obj["outputColumns"].lower() == "false":
+                self.outputColumns = False
+            else:
+                self.outputColumns = json.loads(obj["outputColumns"])
+
+    def copy(self, myfunction):
+        """
+        Copy your function code and decorators to a format executable by the Wizata App.
+        :param myfunction: your function - pass the function itself as parameter
+        """
+
+        if myfunction.__code__.co_argcount < 1:
+            raise ValueError('your function must contains at least one parameter')
+
+        self.function = Function()
+
+        self.function.id = myfunction.__name__
+        self.function.params = inspect.signature(myfunction).parameters
+
+        self._name = myfunction.__name__
+
+        self.function.code = myfunction.__code__
+
+        f_globals = myfunction.__globals__
+        self.function.globals = []
+        for k_global in f_globals:
+            if isinstance(myfunction.__globals__[k_global], types.ModuleType):
+                module = f_globals[k_global]
+                self.function.globals.append({
+                    "var": k_global,
+                    "module": str(module.__name__)
+                })
+
+        if myfunction.__code__.co_filename is not None:
+            if os.path.exists(myfunction.__code__.co_filename):
+                with open(myfunction.__code__.co_filename, "r") as f:
+                    source_code = f.read()
+                self.source = source_code
+
+
+class Function:
+    """
+    Python Code Function
+
+    :ivar id: technical name and then id of the function
+    :ivar code: code of the function __code__
+    :ivar globals: modules references __globals__
+    """
+
+    def __init__(self):
+        self.id = None
+        self.code = None
+        self.globals = None
+        self.params = OrderedDict()
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/twin.py` & `wizata-dsapi-0.3.1/wizata_dsapi/twin.py`

 * *Ordering differences only*

 * *Files 27% similar despite different names*

```diff
@@ -1,82 +1,82 @@
-import uuid
-from .api_dto import ApiDto
-from enum import Enum
-
-
-class TwinBlockType(Enum):
-    AREA = "area"
-    MACHINE = "machine"
-    EQUIPMENT = "equipment"
-    FLOW = "flow"
-
-
-class Twin(ApiDto):
-    """
-    Digital Twin item/asset declared and managed on Wizata.
-
-    :ivar twin_id: UUID of the Digital Twin.
-    :ivar hardware_id: str hardware id identifying the Asset.
-    :ivar name: logical display name of the Asset.
-    :ivar type: type (area, machine, equipment or flow).
-    """
-
-    def __init__(self, twin_id=None, hardware_id=None, name=None, parent_id=None, ttype=TwinBlockType.MACHINE):
-        if twin_id is None:
-            self.twin_id = uuid.uuid4()
-        else:
-            self.twin_id = twin_id
-        self.hardware_id = hardware_id
-        self.name = name
-        self.parent_id = parent_id
-        self.type = ttype
-
-    def api_id(self) -> str:
-        """
-        Id of the experiment (experiment_id)
-
-        :return: string formatted UUID of the Experiment.
-        """
-        return str(self.twin_id).upper()
-
-    def endpoint(self) -> str:
-        """
-        Name of the endpoints used to manipulate execution.
-        :return: Endpoint name.
-        """
-        return "Twins"
-
-    def from_json(self, obj):
-        """
-        Load the Twin entity from a dictionary.
-
-        :param obj: Dict version of the Twin.
-        """
-        if "id" in obj.keys():
-            self.twin_id = uuid.UUID(obj["id"])
-        if "hardwareId" in obj.keys() and obj["hardwareId"] is not None:
-            self.hardware_id = obj["hardwareId"]
-        if "name" in obj.keys() and obj["name"] is not None:
-            self.name = obj["name"]
-        if "parentId" in obj.keys() and obj["parentId"] is not None:
-            self.parent_id = uuid.UUID(obj["parentId"])
-        if "type" in obj.keys():
-            self.type = TwinBlockType(str(obj["type"]))
-
-    def to_json(self):
-        """
-        Convert the twin to a dictionary compatible to JSON format.
-
-        :return: dictionary representation of the Twin object.
-        """
-        obj = {
-            "id": str(self.twin_id)
-        }
-        if self.hardware_id is not None:
-            obj["hardwareId"] = str(self.hardware_id)
-        if self.name is not None:
-            obj["name"] = str(self.name)
-        if self.parent_id is not None:
-            obj["parentId"] = str(self.parent_id)
-        if self.type is not None and isinstance(self.type, TwinBlockType):
-            obj["type"] = self.type.value
-        return obj
+import uuid
+from .api_dto import ApiDto
+from enum import Enum
+
+
+class TwinBlockType(Enum):
+    AREA = "area"
+    MACHINE = "machine"
+    EQUIPMENT = "equipment"
+    FLOW = "flow"
+
+
+class Twin(ApiDto):
+    """
+    Digital Twin item/asset declared and managed on Wizata.
+
+    :ivar twin_id: UUID of the Digital Twin.
+    :ivar hardware_id: str hardware id identifying the Asset.
+    :ivar name: logical display name of the Asset.
+    :ivar type: type (area, machine, equipment or flow).
+    """
+
+    def __init__(self, twin_id=None, hardware_id=None, name=None, parent_id=None, ttype=TwinBlockType.MACHINE):
+        if twin_id is None:
+            self.twin_id = uuid.uuid4()
+        else:
+            self.twin_id = twin_id
+        self.hardware_id = hardware_id
+        self.name = name
+        self.parent_id = parent_id
+        self.type = ttype
+
+    def api_id(self) -> str:
+        """
+        Id of the experiment (experiment_id)
+
+        :return: string formatted UUID of the Experiment.
+        """
+        return str(self.twin_id).upper()
+
+    def endpoint(self) -> str:
+        """
+        Name of the endpoints used to manipulate execution.
+        :return: Endpoint name.
+        """
+        return "Twins"
+
+    def from_json(self, obj):
+        """
+        Load the Twin entity from a dictionary.
+
+        :param obj: Dict version of the Twin.
+        """
+        if "id" in obj.keys():
+            self.twin_id = uuid.UUID(obj["id"])
+        if "hardwareId" in obj.keys() and obj["hardwareId"] is not None:
+            self.hardware_id = obj["hardwareId"]
+        if "name" in obj.keys() and obj["name"] is not None:
+            self.name = obj["name"]
+        if "parentId" in obj.keys() and obj["parentId"] is not None:
+            self.parent_id = uuid.UUID(obj["parentId"])
+        if "type" in obj.keys():
+            self.type = TwinBlockType(str(obj["type"]))
+
+    def to_json(self):
+        """
+        Convert the twin to a dictionary compatible to JSON format.
+
+        :return: dictionary representation of the Twin object.
+        """
+        obj = {
+            "id": str(self.twin_id)
+        }
+        if self.hardware_id is not None:
+            obj["hardwareId"] = str(self.hardware_id)
+        if self.name is not None:
+            obj["name"] = str(self.name)
+        if self.parent_id is not None:
+            obj["parentId"] = str(self.parent_id)
+        if self.type is not None and isinstance(self.type, TwinBlockType):
+            obj["type"] = self.type.value
+        return obj
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi/wizata_dsapi_client.py` & `wizata-dsapi-0.3.1/wizata_dsapi/wizata_dsapi_client.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,1312 +1,1379 @@
-import datetime
-import json
-import uuid
-import sys
-from typing import Tuple
-
-import dill
-import requests
-import pickle
-import pandas
-import plotly
-import msal
-import os
-import types
-import sklearn
-import wizata_dsapi
-from pandas import DataFrame
-from wizata_dsapi import MLModel
-
-import string
-import random
-
-from .plot import Plot
-from .request import Request
-from .mlmodel import MLModel
-from .experiment import Experiment
-from .script import Script
-from .execution import Execution
-from .dsapi_json_encoder import DSAPIEncoder
-from .ds_dataframe import DSDataFrame
-from .model_toolkit import predict
-from .template import Template, TemplateProperty
-from .twinregistration import TwinRegistration
-from .twin import Twin
-from .datapoint import DataPoint, BusinessType, Label, Category
-from .pipeline import Pipeline, PipelineStep, VarType
-
-
-class WizataDSAPIClient:
-
-    def __init__(self,
-                 client_id=None,
-                 scope=None,
-                 tenant_id=None,
-                 username=None,
-                 password=None,
-                 domain="localhost",
-                 protocol="https",
-                 client_secret=None):
-
-        # properties
-        self.domain = domain
-        self.protocol = protocol
-
-        # authentication
-        self.__username = username
-        self.__password = password
-
-        self.__client_id = client_id
-        self.__tenant_id = tenant_id
-        if tenant_id is not None:
-            self.__authority = "https://login.microsoftonline.com/" + tenant_id
-        self.__scopes = [scope]
-
-        self.__interactive_token = None
-        self.__daemon = False
-
-        if client_secret is not None:
-            self.__daemon = True
-            self.__confidential_app = msal.ConfidentialClientApplication(
-                client_id=self.__client_id,
-                client_credential=client_secret,
-                authority=self.__authority
-            )
-
-        self.__app = msal.PublicClientApplication(
-            client_id=self.__client_id,
-            authority=self.__authority
-        )
-
-    def authenticate(self):
-        result = self.__app.acquire_token_interactive(
-            scopes=self.__scopes,
-            success_template="""<html><body>You are authenticated and your code is running, you can close this page.<script>setTimeout(function(){window.close()}, 3000);</script></body></html> """
-        )
-        self.__daemon = False
-        self.__interactive_token = result["access_token"]
-
-    def __url(self):
-        return self.protocol + "://" + self.domain + "/dsapi/"
-
-    def __token(self):
-        # Interactive Authentication
-        if self.__interactive_token is not None:
-            return self.__interactive_token
-
-        if not self.__daemon:
-            # Silent Authentication
-            result = None
-            accounts = self.__app.get_accounts(username=self.__username)
-            if accounts:
-                # If there is an account in the cache, try to get the token silently
-                result = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
-
-            if not result:
-                # If there is no cached token, try to get a new token using the provided username and password
-                result = self.__app.acquire_token_by_username_password(
-                    username=self.__username,
-                    password=self.__password,
-                    scopes=self.__scopes
-                )
-
-            if "error_description" in result.keys():
-                raise RuntimeError(str(result["error_description"]))
-
-            if "access_token" in result.keys():
-                return result["access_token"]
-            else:
-                raise RuntimeError(str(result))
-        else:
-            result = self.__confidential_app.acquire_token_silent(scopes=self.__scopes, account=None)
-
-            if not result:
-                result = self.__confidential_app.acquire_token_for_client(scopes=self.__scopes)
-
-            if "error_description" in result.keys():
-                raise RuntimeError(str(result["error_description"]))
-
-            if "access_token" in result.keys():
-                return result["access_token"]
-
-            return result
-
-    def __header(self):
-        return {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {self.__token()}'
-        }
-
-    def __raise_error(self, response):
-        json_content = response.json()
-        if "errors" in json_content.keys():
-            message = json_content["errors"][0]["message"]
-            return RuntimeError(str(response.status_code) + " - " + message)
-        else:
-            return RuntimeError(str(response.status_code) + " - " + response.reason)
-
-    def lists(self, str_type):
-        """
-        lists all elements of a specific entity.
-
-        :param str_type: plural name of the entity (e.g. scripts, plots, mlmodels, dataframes...)
-        :return: list of all elements with at least the id property.
-        """
-        if str_type == "scripts":
-            response = requests.request("GET",
-                                        self.__url() + "scripts/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                scripts = []
-                for json_model in response.json():
-                    scripts.append(Script(uuid.UUID(json_model["id"])))
-                return scripts
-            else:
-                raise self.__raise_error(response)
-        elif str_type == "plots":
-            response = requests.request("GET",
-                                        self.__url() + "plots/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                plots = []
-                for plot in response.json():
-                    plots.append(Plot(plot["id"]))
-                return plots
-            else:
-                raise self.__raise_error(response)
-        elif str_type == "mlmodels":
-            response = requests.request("GET",
-                                        self.__url() + "mlmodels/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                json_models = response.json()
-                ml_models = []
-                for json_model in json_models:
-                    ml_models.append(MLModel(uuid.UUID(json_model["id"])))
-                return ml_models
-            else:
-                raise self.__raise_error(response)
-        elif str_type == "dataframes":
-            response = requests.request("GET",
-                                        self.__url() + "dataframes/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                json_dfs = response.json()
-                dfs = []
-                for json_model in json_dfs:
-                    dfs.append(DSDataFrame(uuid.UUID(json_model["id"])))
-                return dfs
-            else:
-                raise self.__raise_error(response)
-        elif str_type == "templates":
-            response = requests.request("GET",
-                                        self.__url() + "templates/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                templates_json = response.json()
-                templates = []
-                for template_json in templates_json:
-                    template = Template()
-                    template.from_json(template_json)
-                    templates.append(template)
-                return templates
-            else:
-                raise self.__raise_error(response)
-        elif str_type == "pipelines":
-            response = requests.request("GET",
-                                        self.__url() + "pipelines/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                pipelines_json = response.json()
-                pipelines = []
-                for pipeline_json in pipelines_json:
-                    pipeline = Pipeline()
-                    pipeline.from_json(pipeline_json)
-                    pipelines.append(pipeline)
-                return pipelines
-            else:
-                raise self.__raise_error(response)
-        else:
-            raise TypeError("Type not supported.")
-
-    def get(self,
-            obj=None,
-            script_name=None,
-            experiment_key=None,
-            pipeline_key=None,
-            model_key=None,
-            template_key=None,
-            twin_hardware_id=None):
-        """
-        get full content of an object identified with is id.
-
-        :param obj: object of a supported entity with at list its id
-        :param script_name: alternatively you can use a function name to get a script
-        :param experiment_key: alternatively you can use an experiment key to get an experiment
-        :param pipeline_key: alternatively you can use an pipeline key to get a pipeline
-        :param model_key: model key you want to get.
-        :param template_key: template key you want to get.
-        :param twin_hardware_id: twin hardware id you want to get.
-        :return: object completed with all properties on server (None if not found or raise Error if with id)
-        """
-        if script_name is not None:
-            response = requests.request("GET",
-                                        self.__url() + "scripts/" + str(script_name) + "/",
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                script_bytes = response.content
-                return dill.loads(script_bytes)
-            else:
-                raise self.__raise_error(response)
-        elif experiment_key is not None:
-            response = requests.request("GET",
-                                        self.__url() + "experiments/",
-                                        params={
-                                            'key': experiment_key
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Experiment()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-        elif pipeline_key is not None:
-            response = requests.request("GET",
-                                        self.__url() + "pipelines/",
-                                        params={
-                                            'key': pipeline_key
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Pipeline()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-        elif model_key is not None:
-            response = requests.request("GET",
-                                        self.__url() + "mlmodels/",
-                                        params={
-                                            'key': model_key
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = MLModel()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-
-        elif template_key is not None:
-            response = requests.request("GET",
-                                        self.__url() + "templates/",
-                                        params={
-                                            'key': template_key
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Template()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-
-        elif twin_hardware_id is not None:
-            response = requests.request("GET",
-                                        self.__url() + "twins/",
-                                        params={
-                                            'key': twin_hardware_id
-                                        },
-                                        headers=self.__header()
-                                        )
-            if response.status_code == 200:
-                for obj_json in response.json():
-                    obj = Twin()
-                    obj.from_json(obj_json)
-                    return obj
-                return None
-            else:
-                raise self.__raise_error(response)
-
-        elif obj is not None:
-            if isinstance(obj, Execution):
-                response = requests.request("GET",
-                                            self.__url() + "execute/" + str(obj.execution_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            if isinstance(obj, MLModel):
-                response = requests.request("GET",
-                                            self.__url() + "mlmodels/" + str(obj.model_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    mlmodel_bytes = response.content
-                    return pickle.loads(mlmodel_bytes)
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Script):
-                response = requests.request("GET",
-                                            self.__url() + "scripts/" + str(obj.name) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    script_bytes = response.content
-                    return dill.loads(script_bytes)
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Plot):
-                response = requests.request("GET",
-                                            self.__url() + "plots/" + str(obj.plot_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, DSDataFrame):
-                response = requests.request("GET",
-                                            self.__url() + "dataframes/" + str(obj.df_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    df_bytes = response.content
-                    return pickle.loads(df_bytes)
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Request):
-                response = requests.request("POST", self.__url() + "execute/data",
-                                            headers=self.__header(),
-                                            data=json.dumps(obj.prepare(), cls=DSAPIEncoder))
-                if response.status_code == 200:
-                    return pickle.loads(response.content)
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Experiment):
-                response = requests.request("GET",
-                                            self.__url() + "experiments/" + str(obj.experiment_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Pipeline):
-                response = requests.request("GET",
-                                            self.__url() + "pipelines/" + str(obj.pipeline_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Template):
-                response = requests.request("GET",
-                                            self.__url() + "templates/" + str(obj.template_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, DataPoint):
-                response = requests.request("GET",
-                                            self.__url() + "datapoints/" + str(obj.datapoint_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            elif isinstance(obj, Twin):
-                response = requests.request("GET",
-                                            self.__url() + "twins/" + str(obj.twin_id) + "/",
-                                            headers=self.__header()
-                                            )
-                if response.status_code == 200:
-                    obj.from_json(response.json())
-                    return obj
-                else:
-                    raise self.__raise_error(response)
-            else:
-                raise TypeError("Type not supported.")
-
-    def create(self, obj):
-        """
-        create and save an object on the server
-
-        :param obj: object to save on the server (any id is ignored and replaced)
-        :return: id of created object
-        """
-        if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
-                function=obj
-            )
-        if isinstance(obj, Script):
-            response = requests.post(self.__url() + "scripts/",
-                                     headers=self.__header(),
-                                     data=dill.dumps(obj))
-            if response.status_code == 200:
-                obj.script_id = uuid.UUID(response.json()["id"])
-                return obj.script_id
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Experiment):
-            if len(obj.key) > 16:
-                raise ValueError('experiment key is limited to 16 char.')
-            response = requests.post(self.__url() + "experiments/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Pipeline):
-            response = requests.post(self.__url() + "pipelines/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.post(self.__url() + "templates/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, DataPoint):
-            response = requests.post(self.__url() + "datapoints/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Twin):
-            response = requests.post(self.__url() + "twins/",
-                                     headers=self.__header(),
-                                     data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        else:
-            raise TypeError("Type not supported.")
-
-    def update(self, obj):
-        """
-        update and save an object on the server
-
-        :param obj: object to update on the server
-        :return: None
-        """
-        if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
-                function=obj
-            )
-        if isinstance(obj, Script):
-            response = requests.put(self.__url() + "scripts/" + str(obj.script_id) + "/",
-                                    headers=self.__header(),
-                                    data=dill.dumps(obj))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Experiment):
-            response = requests.put(self.__url() + "experiments/" + str(obj.experiment_id) + "/",
-                                    headers=self.__header(),
-                                    data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.put(self.__url() + "templates/" + str(obj.template_id) + "/",
-                                    headers=self.__header(),
-                                    data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Pipeline):
-            response = requests.put(self.__url() + "pipelines/" + str(obj.pipeline_id) + "/",
-                                    headers=self.__header(),
-                                    data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, DataPoint):
-            response = requests.put(self.__url() + "datapoints/" + str(obj.datapoint_id) + "/",
-                                    headers=self.__header(),
-                                    data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Twin):
-            response = requests.put(self.__url() + "twins/" + str(obj.twin_id) + "/",
-                                    headers=self.__header(),
-                                    data=json.dumps(obj.to_json()))
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        else:
-            raise TypeError("Type not supported.")
-
-    def upsert(self, obj):
-        """
-        upsert on object on the server
-        work with Script, MLModel or directly a function name
-
-        :param obj: object to upsert on the server
-        :return: ID of the object created or updated
-        """
-        if callable(obj) and isinstance(obj, types.FunctionType):
-            obj = Script(
-                function=obj
-            )
-        if isinstance(obj, Script):
-            response = requests.put(self.__url() + "scripts/",
-                                    headers=self.__header(),
-                                    data=dill.dumps(obj))
-            if response.status_code == 200:
-                obj.script_id = uuid.UUID(response.json()['id'])
-                return obj.script_id
-            else:
-                raise self.__raise_error(response)
-        if isinstance(obj, MLModel):
-            response = requests.put(self.__url() + "mlmodels/",
-                                    headers=self.__header(),
-                                    data=pickle.dumps(obj))
-            if response.status_code == 200:
-                obj.model_id = uuid.UUID(response.json()['id'])
-                return obj.model_id
-            else:
-                raise self.__raise_error(response)
-        if isinstance(obj, Template):
-            return self.upsert_template(obj.key, obj.name)
-        if isinstance(obj, Pipeline):
-            return self.upsert_pipeline(pipeline=obj)
-        else:
-            raise TypeError("Type not supported.")
-
-    def delete(self, obj):
-        """
-        delete an object on the server
-
-        :param obj: object to delete including all content
-        :return: None
-        """
-        if isinstance(obj, Pipeline):
-            response = requests.delete(self.__url() + "pipelines" + "/" + str(obj.pipeline_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        if isinstance(obj, Experiment):
-            response = requests.delete(self.__url() + "experiments" + "/" + str(obj.experiment_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        if isinstance(obj, Script):
-            response = requests.delete(self.__url() + "scripts" + "/" + str(obj.script_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Plot):
-            response = requests.delete(self.__url() + "plots" + "/" + str(obj.plot_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, MLModel):
-            response = requests.delete(self.__url() + "mlmodels" + "/" + str(obj.model_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, DSDataFrame):
-            response = requests.delete(self.__url() + "dataframes" + "/" + str(obj.df_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Template):
-            response = requests.delete(self.__url() + "templates" + "/" + str(obj.template_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, DataPoint):
-            response = requests.delete(self.__url() + "datapoints" + "/" + str(obj.datapoint_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        elif isinstance(obj, Twin):
-            response = requests.delete(self.__url() + "twins" + "/" + str(obj.twin_id) + "/",
-                                       headers=self.__header())
-            if response.status_code == 200:
-                return
-            else:
-                raise self.__raise_error(response)
-        else:
-            raise TypeError("Type not supported.")
-
-    def query(self,
-              datapoints: list[str] = None,
-              start: datetime = None,
-              end: datetime = None,
-              interval: int = None,
-              agg_method: str = "mean",
-              template: str = None,
-              twin: str = None,
-              null: str = None,
-              filters: dict = None,
-              options: dict = None) -> pandas.DataFrame:
-        """
-        Query a dataframe from API.
-        :param agg_method:
-        :param datapoints: list of datapoints to fetch.
-        :param start: start datetime of range to fetch
-        :param end: end datetime of range to fetch
-        :param interval: interval in milliseconds.
-        :param template: template to fetch.
-        :param twin: hardware ID of twin to fetch based on template.
-        :param null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
-        :param filters: dict of filters.
-        :param options: dict of options.
-        :return: dataframe
-        """
-        request = Request()
-
-        if datapoints is not None:
-            request.add_datapoints(datapoints)
-
-        if start is not None:
-            request.start = start
-        else:
-            raise ValueError('start datetime is required.')
-
-        if end is not None:
-            request.end = end
-        else:
-            raise ValueError('end datetime is required.')
-
-        if null is not None:
-            request.null = null
-
-        if interval is None:
-            raise ValueError('interval is required.')
-        request.set_aggregation(agg_method, interval)
-
-        if template is not None and twin is not None:
-            request.select_template(
-                template_key=template,
-                twin_hardware_id=twin
-            )
-
-        if filters is not None:
-            request.filters = filters
-
-        if options is not None:
-            request.options = options
-
-        return self.get(request)
-
-    def __execute(self,
-                  execution: Execution = None,
-                  request: Request = None,
-                  dataframe=None,
-                  script=None,
-                  ml_model=None,
-                  isAnomalyDetection=False,
-                  function=None,
-                  experiment=None,
-                  properties: dict = None,
-                  pipeline=None,
-                  twin=None,
-                  mode: str = 'experiment'
-                  ) -> Execution:
-        """
-        internal function - deprecated - please use experiment() or test_run() instead.
-        """
-        # Prepare
-        if execution is None:
-            execution = Execution()
-        if request is not None:
-            execution.request = request
-        if dataframe is not None:
-            if isinstance(dataframe, pandas.DataFrame):
-                execution.dataframe = dataframe
-            elif isinstance(dataframe, DSDataFrame):
-                execution.input_ds_dataframe = dataframe
-        if script is not None:
-            if isinstance(script, uuid.UUID) or (isinstance(script, str) and is_valid_uuid(script)):
-                execution.script = Script(script)
-            elif isinstance(script, str):
-                execution.script = self.get(script_name=script)
-            elif isinstance(script, Script):
-                execution.script = script
-        if ml_model is not None:
-            if isinstance(ml_model, uuid.UUID) or (isinstance(ml_model, str) and is_valid_uuid(ml_model)):
-                execution.ml_model = MLModel(ml_model)
-            elif isinstance(ml_model, str):
-                execution.ml_model = self.get(model_key=ml_model)
-            elif isinstance(ml_model, MLModel):
-                execution.ml_model = ml_model
-
-        if isAnomalyDetection:
-            execution.isAnomalyDetection = True
-        if function is not None:
-            execution.function = function
-        if experiment is not None:
-            if isinstance(experiment, uuid.UUID):
-                execution.experiment_id = experiment
-            elif isinstance(experiment, str):
-                execution.experiment_id = self.get(experiment_key=experiment).experiment_id
-            elif isinstance(experiment, Experiment):
-                execution.experiment_id = experiment.experiment_id
-        if properties is not None and isinstance(properties, dict):
-            execution.properties = properties
-
-        if pipeline is not None:
-            if isinstance(pipeline, uuid.UUID) or (isinstance(pipeline, str) and is_valid_uuid(pipeline)):
-                execution.pipeline = Pipeline(pipeline_id=uuid.UUID(pipeline))
-            elif isinstance(pipeline, str):
-                execution.pipeline = self.get(pipeline_key=pipeline)
-            elif isinstance(pipeline, Pipeline):
-                execution.pipeline = pipeline
-        if twin is not None:
-            if execution.properties is None:
-                execution.properties = {}
-            if isinstance(twin, uuid.UUID) or (isinstance(twin, str) and is_valid_uuid(twin)):
-                execution.properties["twinId"] = str(twin)
-            elif isinstance(twin, str):
-                execution.properties["twinId"] = str(self.get(twin_hardware_id=twin).twin_id)
-            elif isinstance(twin, Twin):
-                execution.properties["twinId"] = str(twin.twin_id)
-
-        # Execute
-        if isinstance(execution, Execution):
-            response = requests.post(f"{self.__url()}execute/?mode={mode}",
-                                     headers=self.__header(),
-                                     data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
-
-            # Parse
-            if response.status_code == 200:
-                obj = response.json()
-                result_execution = Execution()
-                result_execution.from_json(obj)
-                if "plots" in obj.keys():
-                    for plot in obj["plots"]:
-                        result_execution.plots.append(self.get(Plot(plot_id=plot["id"])))
-                if "models" in obj.keys():
-                    for mlmodel in obj["models"]:
-                        result_execution.models.append(self.get(MLModel(model_id=mlmodel["id"])))
-                if "resultDataframe" in obj.keys() and obj["resultDataframe"]["id"] is not None:
-                    result_execution.output_ds_dataframe = self.get(DSDataFrame(df_id=obj["resultDataframe"]["id"]))
-                if "anomaliesList" in obj.keys() and isinstance(obj["anomaliesList"], str):
-                    result_execution.anomalies = json.loads(obj["anomaliesList"])
-                return result_execution
-            else:
-                raise self.__raise_error(response)
-        else:
-            raise TypeError("No execution have been loaded from parameters.")
-
-    def experiment(self, experiment, pipeline, twin=None, properties: dict = None) -> Execution:
-        """
-        experiment and train models with a pipeline.
-
-        - existing experiment is required (use create or upsert_experiment(key, name)).
-        - if your pipeline is templated please provide a twin.
-        - please provide all variables and parameters required through properties.
-        - return an execution
-            - check status with "wizata_dsapi.api().get(execution).status"
-            - see plots with "wizata_dsapi.api().plots(execution)"
-
-        :param experiment: existing experiment identified by its id (uuid or wizata_dsapi.Experiment) or key (str).
-        :param pipeline: pipeline identified by its id (uuid or wizata_dsapi.Pipeline) or key (str) .
-        :param twin: twin identified by its id (uuid or wizata_dsapi.Twin) or hardware ID (str)(optional).
-        :param properties: dictionary containing override for variables or additional parameters for your script.
-        """
-        return self.__execute(
-            experiment=experiment,
-            pipeline=pipeline,
-            twin=twin,
-            properties=properties,
-            mode='experiment'
-        )
-
-    def run(self, pipeline, twin=None, properties: dict = None) -> Execution:
-        """
-        run a pipeline.
-
-        - existing models are used for simulation and prediction.
-        - caution this might affect data inside platform or trigger automation.
-        - if your pipeline is templated please provide a twin.
-        - please provide all variables and parameters required through properties.
-        - return an execution
-            - check status with "wizata_dsapi.api().get(execution).status"
-            - check results in platform (dashboard/explorer) or perform queries.
-
-        :param pipeline: pipeline identified by its id (uuid or wizata_dsapi.Pipeline) or key (str).
-        :param twin: twin identified by its id (uuid or wizata_dsapi.Twin) or hardware ID (str).
-        :param properties: dictionary containing override for variables or additional parameters for your script.
-        """
-        return self.__execute(
-            pipeline=pipeline,
-            twin=twin,
-            properties=properties,
-            mode='production'
-        )
-
-    def plot(self, plot_id: str = None, plot: Plot = None, figure=None,):
-        """
-        Fetch and show plot.
-        :param plot: Wizata Plot Object
-        :param figure: JSON Figure
-        :param plot_id: Plot Id
-        :return: plotly figure
-        """
-        if plot is not None and plot.figure is not None:
-            return plotly.io.from_json(plot.figure)
-        elif plot is not None and plot.figure is None:
-            plot = self.get(plot)
-            if plot.figure is not None:
-                return plotly.io.from_json(plot.figure)
-            else:
-                raise ValueError('No plot has been fetch.')
-        elif figure is not None:
-            return plotly.io.from_json(plot.figure)
-        elif plot_id is not None:
-            plot = self.get(Plot(plot_id=plot_id))
-            if plot.figure is not None:
-                return plotly.io.from_json(plot.figure)
-            else:
-                raise ValueError('No plot has been fetch.')
-        else:
-            raise KeyError('No valid arguments.')
-
-    def plots(self, execution):
-        """
-        get all plot for an execution.
-        :param execution: id or Execution.
-        :return: list of plots.
-        """
-
-        if execution is None:
-            raise ValueError("execution cannot be None to retrieve plot")
-        if isinstance(execution, uuid.UUID):
-            execution_id = execution
-        elif isinstance(execution, str):
-            execution_id = uuid.UUID(execution)
-        elif isinstance(execution, Execution):
-            execution_id = execution.execution_id
-        else:
-            raise Exception(f'unsupported type {execution}')
-
-        response = requests.request("GET",
-                                    self.__url() + f"plots/?generatedById={execution_id}",
-                                    headers=self.__header()
-                                    )
-        if response.status_code == 200:
-            plots = []
-            for plot in response.json():
-                plots.append(self.plot(plot_id=str(plot["id"])))
-            return plots
-        else:
-            raise self.__raise_error(response)
-
-    def register_model(self,
-                       model_key,
-                       train_model,
-                       df: pandas.DataFrame,
-                       scaler=None,
-                       has_anomalies: bool = False,
-                       has_target_feat: bool = False,
-                       experiment_key = None) -> tuple[MLModel, pandas.DataFrame]:
-        """
-        Register a Machine Learning model to Wizata.
-        Model is tested by the API against a sample dataframe.
-        :param model_key: logical string id to identify the model.
-        :param train_model: trained model (must be compatible with pickle library)
-        :param df: sample dataframe.
-        :param scaler: scaler (must be compatible with pickle library)
-        :param has_anomalies: True is model generate Anomalies
-        :param has_target_feat: True if model need a target feature to be selected
-        :param experiment_key: Reference of an experiment to which link the generated ML Model
-        :return: registered ML Model , pandas.DataFrame
-        """
-        if model_key is None and isinstance(model_key, str):
-            raise ValueError('Please provide a str Model Key to identify the model.')
-        if train_model is None:
-            raise ValueError('Trained Machine Learning model should not be null')
-        elif df is None:
-            raise ValueError('A sample dataframe must be provided')
-
-        # Create a ML Model object
-        ml_model = MLModel()
-        ml_model.trained_model = train_model
-        if scaler is not None:
-            ml_model.scaler = scaler
-        ml_model.has_anomalies = has_anomalies
-        ml_model.has_target_feat = has_target_feat
-        ml_model.input_columns = df.columns
-        ml_model.key = model_key
-
-        if experiment_key is not None:
-            ml_model.experimentId = self.get(experiment_key=experiment_key).experiment_id
-
-        try:
-            result_df = predict(df, ml_model)
-            if result_df is not None:
-                ml_model.status = "valid"
-                self.upsert(ml_model)
-                return ml_model, result_df
-            else:
-                raise RuntimeError('no dataframe was generated by your model while testing predict capabilities')
-        except Exception as e:
-            raise RuntimeError('not able to validated the model : ' + str(e))
-
-    def upsert_experiment(self, key: str, name: str):
-        """
-        Upsert an experiment.
-        :param key: unique key identifying the experiment.
-        :param name: display name of the experiment
-        :return: upserted experiment.
-        """
-        experiment = self.get(experiment_key=key)
-        if experiment is not None:
-            found = True
-            experiment.name = name
-        else:
-            experiment = Experiment(
-                key=key,
-                name=name
-            )
-            found = False
-
-        if not found:
-            return self.create(experiment)
-        else:
-            return self.update(experiment)
-
-    def upsert_template(self, key: str, name: str):
-        """
-        Upsert a template.
-        :param key: unique key identifying the template.
-        :param name: display name of the template
-        :return: upserted template.
-        """
-
-        template = self.get(template_key=key)
-        if template is not None:
-            found = True
-            template.name = name
-        else:
-            template = Template(
-                key=key,
-                name=name
-            )
-            found = False
-
-        if not found:
-            return self.create(template)
-        else:
-            return self.update(template)
-
-    def upsert_pipeline(self, pipeline: Pipeline):
-        """
-        Upsert a template (ignore ID, use the key)
-        :return: upserted template.
-        """
-
-        get = self.get(pipeline_key=pipeline.key)
-        if get is not None:
-            pipeline.pipeline_id = get.pipeline_id
-            return self.update(pipeline)
-        else:
-            return self.create(pipeline)
-
-    def add_template_property(self,
-                              template,
-                              property_name: str, property_type: str = "datapoint",
-                              is_required: bool = True):
-
-        if property_type not in ['datapoint', 'float', 'integer', 'string']:
-            raise ValueError('property type must be datapoint, float, integer or string')
-
-        if isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
-
-        if property_name is None:
-            raise ValueError('please provide a valid name for the property')
-
-        property_dict = {
-            "type": property_type,
-            "name": property_name,
-            "required": is_required
-        }
-
-        response = requests.post(self.__url() + "templates/" + str(template.template_id) + '/properties/',
-                                 headers=self.__header(),
-                                 data=json.dumps(property_dict))
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def remove_template_property(self, template, property_name: str):
-
-        if isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
-
-        if property_name is None:
-            raise ValueError('please provide a valid name for the property')
-
-        property_dict = {
-            "name": property_name
-        }
-
-        response = requests.delete(self.__url() + "templates/" + str(template.template_id) + '/properties/',
-                                   headers=self.__header(),
-                                   data=json.dumps(property_dict))
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def get_registrations(self, template) -> list:
-        """
-        retrieve all registrations for
-        :param template: template object, UUID or str key.
-        :return: list of twin registration.
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-        if template is None:
-            raise ValueError('template cannot be found on server')
-
-        response = requests.get(self.__url() + "templates/" + str(template.template_id) + '/registrations/',
-                                headers=self.__header())
-        if response.status_code == 200:
-            registrations_json = response.json()
-            registrations = []
-            for twin_registration_json in registrations_json:
-                registration = TwinRegistration()
-                registration.from_json(twin_registration_json)
-                registrations.append(registration)
-            return registrations
-        else:
-            raise self.__raise_error(response)
-
-    def register_twin(self, template, twin, properties: dict, override=True):
-        """
-        register a twin on a specific template using a map.
-        :param template: template object, UUID or str key.
-        :param twin: twin object, UUID or str key.
-        :param properties: dict where key = template property and value = datapoint name or const value (str, int, float, relative or epoch datetime).
-        :param override: by default at True - allow overriding any existing subscription
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-
-        if template is None:
-            raise ValueError('template cannot be found on server')
-
-        if twin is None:
-            raise ValueError('twin must be specified.')
-        elif isinstance(twin, uuid.UUID):
-            twin_id = twin
-        elif isinstance(twin, str):
-            twin_id = self.get(twin_hardware_id=twin).twin_id
-        elif isinstance(twin, Twin):
-            twin_id = twin.twin_id
-        else:
-            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
-
-        if template.properties is None or len(template.properties) == 0:
-            raise ValueError('template chosen does not contains any properties')
-
-        if properties is None or len(properties.keys()) == 0:
-            raise ValueError('your map dictionary must contains properties matching template')
-
-        twin_properties = {
-            "properties": []
-        }
-        for key in properties.keys():
-            property_type = None
-            for template_property in template.properties:
-                template_property: TemplateProperty
-                if key == template_property.name:
-                    property_type = template_property.p_type
-            if property_type is None:
-                raise ValueError(f'cannot find property {key} in template or cannot determine its type')
-            twin_properties["properties"].append({
-                'name': key,
-                property_type.value: properties[key]
-            })
-
-        # Check if already exist
-        exists = False
-        response_exists = requests.get(self.__url() + "templates/" + str(template.template_id)
-                                       + '/registrations/' + str(twin_id) + '/',
-                                       headers=self.__header())
-        if response_exists.status_code == 200:
-            exists = True
-
-        if exists and not override:
-            raise ValueError("registration already exists and override not allowed.")
-
-        if exists and override:
-            response = requests.put(self.__url() + "templates/" + str(template.template_id)
-                                    + '/registrations/' + str(twin_id) + '/',
-                                    headers=self.__header(),
-                                    data=json.dumps(twin_properties))
-        else:
-            response = requests.post(self.__url() + "templates/" + str(template.template_id)
-                                     + '/registrations/' + str(twin_id) + '/',
-                                     headers=self.__header(),
-                                     data=json.dumps(twin_properties))
-
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-    def unregister_twin(self, template, twin):
-        """
-        un-register a twin from a specific template.
-        :param template: template object, UUID or str key.
-        :param twin: twin object, UUID or str key.
-        """
-
-        if template is None:
-            raise ValueError('template must be specified.')
-        elif isinstance(template, uuid.UUID):
-            template = self.get(wizata_dsapi.Template(template_id=template))
-        elif isinstance(template, str):
-            template = self.get(template_key=template)
-        elif not isinstance(template, Template):
-            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
-
-        if twin is None:
-            raise ValueError('twin must be specified.')
-        elif isinstance(twin, uuid.UUID):
-            twin_id = twin
-        elif isinstance(twin, str):
-            twin_id = self.get(twin_hardware_id=twin).twin_id
-        elif isinstance(twin, Twin):
-            twin_id = twin.twin_id
-        else:
-            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
-
-        response = requests.delete(self.__url() + "templates/" + str(template.template_id)
-                                   + '/registrations/' + str(twin_id) + '/',
-                                   headers=self.__header())
-        if response.status_code == 200:
-            return
-        else:
-            raise self.__raise_error(response)
-
-
-def api() -> WizataDSAPIClient:
-    """
-    Create a WizataDSAPIClient from environment variables.
-    :return: client
-    """
-    protocol = 'https'
-
-    if os.environ.get('WIZATA_PROTOCOL') is not None:
-        protocol = os.environ.get('WIZATA_PROTOCOL')
-
-    if os.environ.get('WIZATA_CLIENT_SECRET') is not None:
-        return WizataDSAPIClient(
-            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
-            client_id=os.environ.get('WIZATA_CLIENT_ID'),
-            client_secret=os.environ.get('WIZATA_CLIENT_SECRET'),
-            scope=os.environ.get('WIZATA_CLIENT_ID') + '/.default',
-            domain=os.environ.get('WIZATA_DOMAIN'),
-            protocol=protocol
-        )
-    else:
-        return WizataDSAPIClient(
-            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
-            client_id=os.environ.get('WIZATA_CLIENT_ID'),
-            scope=os.environ.get('WIZATA_SCOPE'),
-            username=os.environ.get('WIZATA_USERNAME'),
-            password=os.environ.get('WIZATA_PASSWORD'),
-            domain=os.environ.get('WIZATA_DOMAIN'),
-            protocol=protocol
-        )
-
-
-def is_valid_uuid(val):
-    try:
-        uuid.UUID(str(val))
-        return True
-    except ValueError:
-        return False
+import datetime
+import json
+import uuid
+import sys
+from typing import Tuple
+
+import dill
+import requests
+import pickle
+import pandas
+import plotly
+import msal
+import os
+import types
+import sklearn
+import wizata_dsapi
+from pandas import DataFrame
+from wizata_dsapi import MLModel
+
+import string
+import random
+
+from .plot import Plot
+from .request import Request
+from .mlmodel import MLModel
+from .experiment import Experiment
+from .script import Script
+from .execution import Execution
+from .dsapi_json_encoder import DSAPIEncoder
+from .ds_dataframe import DSDataFrame
+from .model_toolkit import predict
+from .template import Template, TemplateProperty
+from .twinregistration import TwinRegistration
+from .twin import Twin
+from .datapoint import DataPoint, BusinessType, Label, Category
+from .pipeline import Pipeline, PipelineStep, VarType
+
+
+class WizataDSAPIClient:
+
+    def __init__(self,
+                 client_id=None,
+                 scope=None,
+                 tenant_id=None,
+                 username=None,
+                 password=None,
+                 domain="localhost",
+                 protocol="https",
+                 client_secret=None):
+
+        # properties
+        self.domain = domain
+        self.protocol = protocol
+
+        # authentication
+        self.__username = username
+        self.__password = password
+
+        self.__client_id = client_id
+        self.__tenant_id = tenant_id
+        if tenant_id is not None:
+            self.__authority = "https://login.microsoftonline.com/" + tenant_id
+        self.__scopes = [scope]
+
+        self.__interactive_token = None
+        self.__daemon = False
+
+        if client_secret is not None:
+            self.__daemon = True
+            self.__confidential_app = msal.ConfidentialClientApplication(
+                client_id=self.__client_id,
+                client_credential=client_secret,
+                authority=self.__authority
+            )
+
+        self.__app = msal.PublicClientApplication(
+            client_id=self.__client_id,
+            authority=self.__authority
+        )
+
+    def authenticate(self):
+        result = self.__app.acquire_token_interactive(
+            scopes=self.__scopes,
+            success_template="""<html><body>You are authenticated and your code is running, you can close this page.<script>setTimeout(function(){window.close()}, 3000);</script></body></html> """
+        )
+        self.__daemon = False
+        self.__interactive_token = result["access_token"]
+
+    def __url(self):
+        return self.protocol + "://" + self.domain + "/dsapi/"
+
+    def __token(self):
+        # Interactive Authentication
+        if self.__interactive_token is not None:
+            return self.__interactive_token
+
+        if not self.__daemon:
+            # Silent Authentication
+            result = None
+            accounts = self.__app.get_accounts(username=self.__username)
+            if accounts:
+                # If there is an account in the cache, try to get the token silently
+                result = self.__app.acquire_token_silent(scopes=self.__scopes, account=accounts[0])
+
+            if not result:
+                # If there is no cached token, try to get a new token using the provided username and password
+                result = self.__app.acquire_token_by_username_password(
+                    username=self.__username,
+                    password=self.__password,
+                    scopes=self.__scopes
+                )
+
+            if "error_description" in result.keys():
+                raise RuntimeError(str(result["error_description"]))
+
+            if "access_token" in result.keys():
+                return result["access_token"]
+            else:
+                raise RuntimeError(str(result))
+        else:
+            result = self.__confidential_app.acquire_token_silent(scopes=self.__scopes, account=None)
+
+            if not result:
+                result = self.__confidential_app.acquire_token_for_client(scopes=self.__scopes)
+
+            if "error_description" in result.keys():
+                raise RuntimeError(str(result["error_description"]))
+
+            if "access_token" in result.keys():
+                return result["access_token"]
+
+            return result
+
+    def __header(self):
+        return {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.__token()}'
+        }
+
+    def __raise_error(self, response):
+        json_content = response.json()
+        if "errors" in json_content.keys():
+            message = json_content["errors"][0]["message"]
+            return RuntimeError(str(response.status_code) + " - " + message)
+        else:
+            return RuntimeError(str(response.status_code) + " - " + response.reason)
+
+    def lists(self, str_type):
+        """
+        lists all elements of a specific entity.
+
+        :param str_type: plural name of the entity (e.g. scripts, plots, mlmodels, dataframes...)
+        :return: list of all elements with at least the id property.
+        """
+        if str_type == "scripts":
+            response = requests.request("GET",
+                                        self.__url() + "scripts/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                scripts = []
+                for json_model in response.json():
+                    scripts.append(Script(uuid.UUID(json_model["id"])))
+                return scripts
+            else:
+                raise self.__raise_error(response)
+        elif str_type == "plots":
+            response = requests.request("GET",
+                                        self.__url() + "plots/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                plots = []
+                for plot in response.json():
+                    plots.append(Plot(plot["id"]))
+                return plots
+            else:
+                raise self.__raise_error(response)
+        elif str_type == "mlmodels":
+            response = requests.request("GET",
+                                        self.__url() + "mlmodels/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                json_models = response.json()
+                ml_models = []
+                for json_model in json_models:
+                    ml_models.append(MLModel(uuid.UUID(json_model["id"])))
+                return ml_models
+            else:
+                raise self.__raise_error(response)
+        elif str_type == "dataframes":
+            response = requests.request("GET",
+                                        self.__url() + "dataframes/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                json_dfs = response.json()
+                dfs = []
+                for json_model in json_dfs:
+                    dfs.append(DSDataFrame(uuid.UUID(json_model["id"])))
+                return dfs
+            else:
+                raise self.__raise_error(response)
+        elif str_type == "templates":
+            response = requests.request("GET",
+                                        self.__url() + "templates/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                templates_json = response.json()
+                templates = []
+                for template_json in templates_json:
+                    template = Template()
+                    template.from_json(template_json)
+                    templates.append(template)
+                return templates
+            else:
+                raise self.__raise_error(response)
+        elif str_type == "pipelines":
+            response = requests.request("GET",
+                                        self.__url() + "pipelines/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                pipelines_json = response.json()
+                pipelines = []
+                for pipeline_json in pipelines_json:
+                    pipeline = Pipeline()
+                    pipeline.from_json(pipeline_json)
+                    pipelines.append(pipeline)
+                return pipelines
+            else:
+                raise self.__raise_error(response)
+        else:
+            raise TypeError("Type not supported.")
+
+    def get(self,
+            obj=None,
+            script_name=None,
+            experiment_key=None,
+            pipeline_key=None,
+            model_key=None,
+            template_key=None,
+            twin_hardware_id=None,
+            datapoint_hardware_id=None):
+        """
+        get full content of an object identified with is id.
+
+        :param obj: object of a supported entity with at list its id
+        :param script_name: alternatively you can use a function name to get a script
+        :param experiment_key: alternatively you can use an experiment key to get an experiment
+        :param pipeline_key: alternatively you can use an pipeline key to get a pipeline
+        :param model_key: model key you want to get.
+        :param template_key: template key you want to get.
+        :param twin_hardware_id: twin hardware id you want to get.
+        :param datapoint_hardware_id: datapoint hardware id you want to get.
+        :return: object completed with all properties on server (None if not found or raise Error if with id)
+        """
+        if script_name is not None:
+            response = requests.request("GET",
+                                        self.__url() + "scripts/" + str(script_name) + "/",
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                script_bytes = response.content
+                return dill.loads(script_bytes)
+            else:
+                raise self.__raise_error(response)
+        elif experiment_key is not None:
+            response = requests.request("GET",
+                                        self.__url() + "experiments/",
+                                        params={
+                                            'key': experiment_key
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = Experiment()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+        elif pipeline_key is not None:
+            response = requests.request("GET",
+                                        self.__url() + "pipelines/",
+                                        params={
+                                            'key': pipeline_key
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = Pipeline()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+        elif model_key is not None:
+            response = requests.request("GET",
+                                        self.__url() + "mlmodels/",
+                                        params={
+                                            'key': model_key
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = MLModel()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+
+        elif template_key is not None:
+            response = requests.request("GET",
+                                        self.__url() + "templates/",
+                                        params={
+                                            'key': template_key
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = Template()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+
+        elif twin_hardware_id is not None:
+            response = requests.request("GET",
+                                        self.__url() + "twins/",
+                                        params={
+                                            'key': twin_hardware_id
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = Twin()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+
+        elif datapoint_hardware_id is not None:
+            response = requests.request("GET",
+                                        self.__url() + "datapoints/",
+                                        params={
+                                            'key': datapoint_hardware_id
+                                        },
+                                        headers=self.__header()
+                                        )
+            if response.status_code == 200:
+                for obj_json in response.json():
+                    obj = DataPoint()
+                    obj.from_json(obj_json)
+                    return obj
+                return None
+            else:
+                raise self.__raise_error(response)
+
+        elif obj is not None:
+            if isinstance(obj, Execution):
+                response = requests.request("GET",
+                                            self.__url() + "execute/" + str(obj.execution_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            if isinstance(obj, MLModel):
+                response = requests.request("GET",
+                                            self.__url() + "mlmodels/" + str(obj.model_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    mlmodel_bytes = response.content
+                    return pickle.loads(mlmodel_bytes)
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Script):
+                response = requests.request("GET",
+                                            self.__url() + "scripts/" + str(obj.name) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    script_bytes = response.content
+                    return dill.loads(script_bytes)
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Plot):
+                response = requests.request("GET",
+                                            self.__url() + "plots/" + str(obj.plot_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, DSDataFrame):
+                response = requests.request("GET",
+                                            self.__url() + "dataframes/" + str(obj.df_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    df_bytes = response.content
+                    return pickle.loads(df_bytes)
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Request):
+                response = requests.request("POST", self.__url() + "execute/data",
+                                            headers=self.__header(),
+                                            data=json.dumps(obj.prepare(), cls=DSAPIEncoder))
+                if response.status_code == 200:
+                    return pickle.loads(response.content)
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Experiment):
+                response = requests.request("GET",
+                                            self.__url() + "experiments/" + str(obj.experiment_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Pipeline):
+                response = requests.request("GET",
+                                            self.__url() + "pipelines/" + str(obj.pipeline_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Template):
+                response = requests.request("GET",
+                                            self.__url() + "templates/" + str(obj.template_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, DataPoint):
+                response = requests.request("GET",
+                                            self.__url() + "datapoints/" + str(obj.datapoint_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            elif isinstance(obj, Twin):
+                response = requests.request("GET",
+                                            self.__url() + "twins/" + str(obj.twin_id) + "/",
+                                            headers=self.__header()
+                                            )
+                if response.status_code == 200:
+                    obj.from_json(response.json())
+                    return obj
+                else:
+                    raise self.__raise_error(response)
+            else:
+                raise TypeError("Type not supported.")
+
+    def get_categories(self) -> dict:
+        """
+        get a name / uuid dictionary with all categories in platform.
+        """
+        response = requests.request("GET",
+                                    self.__url() + "datapoints/categories/",
+                                    headers=self.__header()
+                                    )
+        if response.status_code == 200:
+            categories_json = response.json()
+            categories_dict = {}
+            for category_json in categories_json:
+                categories_dict[category_json["name"]] = category_json["id"]
+            return categories_dict
+        else:
+            raise self.__raise_error(response)
+
+    def create(self, obj):
+        """
+        create and save an object on the server
+
+        :param obj: object to save on the server (any id is ignored and replaced)
+        :return: id of created object
+        """
+        if callable(obj) and isinstance(obj, types.FunctionType):
+            obj = Script(
+                function=obj
+            )
+        if isinstance(obj, Script):
+            response = requests.post(self.__url() + "scripts/",
+                                     headers=self.__header(),
+                                     data=dill.dumps(obj))
+            if response.status_code == 200:
+                obj.script_id = uuid.UUID(response.json()["id"])
+                return obj.script_id
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Experiment):
+            if len(obj.key) > 16:
+                raise ValueError('experiment key is limited to 16 char.')
+            response = requests.post(self.__url() + "experiments/",
+                                     headers=self.__header(),
+                                     data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Pipeline):
+            response = requests.post(self.__url() + "pipelines/",
+                                     headers=self.__header(),
+                                     data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Template):
+            response = requests.post(self.__url() + "templates/",
+                                     headers=self.__header(),
+                                     data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, DataPoint):
+            response = requests.post(self.__url() + "datapoints/",
+                                     headers=self.__header(),
+                                     data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Twin):
+            response = requests.post(self.__url() + "twins/",
+                                     headers=self.__header(),
+                                     data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        else:
+            raise TypeError("Type not supported.")
+
+    def update(self, obj):
+        """
+        update and save an object on the server
+
+        :param obj: object to update on the server
+        :return: None
+        """
+        if callable(obj) and isinstance(obj, types.FunctionType):
+            obj = Script(
+                function=obj
+            )
+        if isinstance(obj, Script):
+            response = requests.put(self.__url() + "scripts/" + str(obj.script_id) + "/",
+                                    headers=self.__header(),
+                                    data=dill.dumps(obj))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Experiment):
+            response = requests.put(self.__url() + "experiments/" + str(obj.experiment_id) + "/",
+                                    headers=self.__header(),
+                                    data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Template):
+            response = requests.put(self.__url() + "templates/" + str(obj.template_id) + "/",
+                                    headers=self.__header(),
+                                    data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Pipeline):
+            response = requests.put(self.__url() + "pipelines/" + str(obj.pipeline_id) + "/",
+                                    headers=self.__header(),
+                                    data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, DataPoint):
+            response = requests.put(self.__url() + "datapoints/" + str(obj.datapoint_id) + "/",
+                                    headers=self.__header(),
+                                    data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Twin):
+            response = requests.put(self.__url() + "twins/" + str(obj.twin_id) + "/",
+                                    headers=self.__header(),
+                                    data=json.dumps(obj.to_json()))
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        else:
+            raise TypeError("Type not supported.")
+
+    def upsert(self, obj):
+        """
+        upsert on object on the server
+        work with Script, MLModel or directly a function name
+
+        :param obj: object to upsert on the server
+        :return: ID of the object created or updated
+        """
+        if callable(obj) and isinstance(obj, types.FunctionType):
+            obj = Script(
+                function=obj
+            )
+        if isinstance(obj, Script):
+            response = requests.put(self.__url() + "scripts/",
+                                    headers=self.__header(),
+                                    data=dill.dumps(obj))
+            if response.status_code == 200:
+                obj.script_id = uuid.UUID(response.json()['id'])
+                return obj.script_id
+            else:
+                raise self.__raise_error(response)
+        if isinstance(obj, MLModel):
+            response = requests.put(self.__url() + "mlmodels/",
+                                    headers=self.__header(),
+                                    data=pickle.dumps(obj))
+            if response.status_code == 200:
+                obj.model_id = uuid.UUID(response.json()['id'])
+                return obj.model_id
+            else:
+                raise self.__raise_error(response)
+        if isinstance(obj, Template):
+            return self.upsert_template(obj.key, obj.name)
+        if isinstance(obj, Pipeline):
+            return self.upsert_pipeline(pipeline=obj)
+        if isinstance(obj, DataPoint):
+            return self.upsert_datapoint(datapoint=obj)
+        if isinstance(obj, Twin):
+            return self.upsert_twin(twin=obj)
+        else:
+            raise TypeError("Type not supported.")
+
+    def delete(self, obj):
+        """
+        delete an object on the server
+
+        :param obj: object to delete including all content
+        :return: None
+        """
+        if isinstance(obj, Pipeline):
+            response = requests.delete(self.__url() + "pipelines" + "/" + str(obj.pipeline_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        if isinstance(obj, Experiment):
+            response = requests.delete(self.__url() + "experiments" + "/" + str(obj.experiment_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        if isinstance(obj, Script):
+            response = requests.delete(self.__url() + "scripts" + "/" + str(obj.script_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Plot):
+            response = requests.delete(self.__url() + "plots" + "/" + str(obj.plot_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, MLModel):
+            response = requests.delete(self.__url() + "mlmodels" + "/" + str(obj.model_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, DSDataFrame):
+            response = requests.delete(self.__url() + "dataframes" + "/" + str(obj.df_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Template):
+            response = requests.delete(self.__url() + "templates" + "/" + str(obj.template_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, DataPoint):
+            response = requests.delete(self.__url() + "datapoints" + "/" + str(obj.datapoint_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        elif isinstance(obj, Twin):
+            response = requests.delete(self.__url() + "twins" + "/" + str(obj.twin_id) + "/",
+                                       headers=self.__header())
+            if response.status_code == 200:
+                return
+            else:
+                raise self.__raise_error(response)
+        else:
+            raise TypeError("Type not supported.")
+
+    def query(self,
+              datapoints: list[str] = None,
+              start: datetime = None,
+              end: datetime = None,
+              interval: int = None,
+              agg_method: str = "mean",
+              template: str = None,
+              twin: str = None,
+              null: str = None,
+              filters: dict = None,
+              options: dict = None) -> pandas.DataFrame:
+        """
+        Query a dataframe from API.
+        :param agg_method:
+        :param datapoints: list of datapoints to fetch.
+        :param start: start datetime of range to fetch
+        :param end: end datetime of range to fetch
+        :param interval: interval in milliseconds.
+        :param template: template to fetch.
+        :param twin: hardware ID of twin to fetch based on template.
+        :param null: By default at 'drop' and dropping NaN values. If not intended behavior please set it to 'ignore' or 'all'.
+        :param filters: dict of filters.
+        :param options: dict of options.
+        :return: dataframe
+        """
+        request = Request()
+
+        if datapoints is not None:
+            request.add_datapoints(datapoints)
+
+        if start is not None:
+            request.start = start
+        else:
+            raise ValueError('start datetime is required.')
+
+        if end is not None:
+            request.end = end
+        else:
+            raise ValueError('end datetime is required.')
+
+        if null is not None:
+            request.null = null
+
+        if interval is None:
+            raise ValueError('interval is required.')
+        request.set_aggregation(agg_method, interval)
+
+        if template is not None and twin is not None:
+            request.select_template(
+                template_key=template,
+                twin_hardware_id=twin
+            )
+
+        if filters is not None:
+            request.filters = filters
+
+        if options is not None:
+            request.options = options
+
+        return self.get(request)
+
+    def __execute(self,
+                  execution: Execution = None,
+                  request: Request = None,
+                  dataframe=None,
+                  script=None,
+                  ml_model=None,
+                  isAnomalyDetection=False,
+                  function=None,
+                  experiment=None,
+                  properties: dict = None,
+                  pipeline=None,
+                  twin=None,
+                  mode: str = 'experiment'
+                  ) -> Execution:
+        """
+        internal function - deprecated - please use experiment() or test_run() instead.
+        """
+        # Prepare
+        if execution is None:
+            execution = Execution()
+        if request is not None:
+            execution.request = request
+        if dataframe is not None:
+            if isinstance(dataframe, pandas.DataFrame):
+                execution.dataframe = dataframe
+            elif isinstance(dataframe, DSDataFrame):
+                execution.input_ds_dataframe = dataframe
+        if script is not None:
+            if isinstance(script, uuid.UUID) or (isinstance(script, str) and is_valid_uuid(script)):
+                execution.script = Script(script)
+            elif isinstance(script, str):
+                execution.script = self.get(script_name=script)
+            elif isinstance(script, Script):
+                execution.script = script
+        if ml_model is not None:
+            if isinstance(ml_model, uuid.UUID) or (isinstance(ml_model, str) and is_valid_uuid(ml_model)):
+                execution.ml_model = MLModel(ml_model)
+            elif isinstance(ml_model, str):
+                execution.ml_model = self.get(model_key=ml_model)
+            elif isinstance(ml_model, MLModel):
+                execution.ml_model = ml_model
+
+        if isAnomalyDetection:
+            execution.isAnomalyDetection = True
+        if function is not None:
+            execution.function = function
+        if experiment is not None:
+            if isinstance(experiment, uuid.UUID):
+                execution.experiment_id = experiment
+            elif isinstance(experiment, str):
+                execution.experiment_id = self.get(experiment_key=experiment).experiment_id
+            elif isinstance(experiment, Experiment):
+                execution.experiment_id = experiment.experiment_id
+        if properties is not None and isinstance(properties, dict):
+            execution.properties = properties
+
+        if pipeline is not None:
+            if isinstance(pipeline, uuid.UUID) or (isinstance(pipeline, str) and is_valid_uuid(pipeline)):
+                execution.pipeline = Pipeline(pipeline_id=uuid.UUID(pipeline))
+            elif isinstance(pipeline, str):
+                execution.pipeline = self.get(pipeline_key=pipeline)
+            elif isinstance(pipeline, Pipeline):
+                execution.pipeline = pipeline
+        if twin is not None:
+            if execution.properties is None:
+                execution.properties = {}
+            if isinstance(twin, uuid.UUID) or (isinstance(twin, str) and is_valid_uuid(twin)):
+                execution.properties["twinId"] = str(twin)
+            elif isinstance(twin, str):
+                execution.properties["twinId"] = str(self.get(twin_hardware_id=twin).twin_id)
+            elif isinstance(twin, Twin):
+                execution.properties["twinId"] = str(twin.twin_id)
+
+        # Execute
+        if isinstance(execution, Execution):
+            response = requests.post(f"{self.__url()}execute/?mode={mode}",
+                                     headers=self.__header(),
+                                     data=json.dumps(execution.to_json(), cls=DSAPIEncoder))
+
+            # Parse
+            if response.status_code == 200:
+                obj = response.json()
+                result_execution = Execution()
+                result_execution.from_json(obj)
+                if "plots" in obj.keys():
+                    for plot in obj["plots"]:
+                        result_execution.plots.append(self.get(Plot(plot_id=plot["id"])))
+                if "models" in obj.keys():
+                    for mlmodel in obj["models"]:
+                        result_execution.models.append(self.get(MLModel(model_id=mlmodel["id"])))
+                if "resultDataframe" in obj.keys() and obj["resultDataframe"]["id"] is not None:
+                    result_execution.output_ds_dataframe = self.get(DSDataFrame(df_id=obj["resultDataframe"]["id"]))
+                if "anomaliesList" in obj.keys() and isinstance(obj["anomaliesList"], str):
+                    result_execution.anomalies = json.loads(obj["anomaliesList"])
+                return result_execution
+            else:
+                raise self.__raise_error(response)
+        else:
+            raise TypeError("No execution have been loaded from parameters.")
+
+    def experiment(self, experiment, pipeline, twin=None, properties: dict = None) -> Execution:
+        """
+        experiment and train models with a pipeline.
+
+        - existing experiment is required (use create or upsert_experiment(key, name)).
+        - if your pipeline is templated please provide a twin.
+        - please provide all variables and parameters required through properties.
+        - return an execution
+            - check status with "wizata_dsapi.api().get(execution).status"
+            - see plots with "wizata_dsapi.api().plots(execution)"
+
+        :param experiment: existing experiment identified by its id (uuid or wizata_dsapi.Experiment) or key (str).
+        :param pipeline: pipeline identified by its id (uuid or wizata_dsapi.Pipeline) or key (str) .
+        :param twin: twin identified by its id (uuid or wizata_dsapi.Twin) or hardware ID (str)(optional).
+        :param properties: dictionary containing override for variables or additional parameters for your script.
+        """
+        return self.__execute(
+            experiment=experiment,
+            pipeline=pipeline,
+            twin=twin,
+            properties=properties,
+            mode='experiment'
+        )
+
+    def run(self, pipeline, twin=None, properties: dict = None) -> Execution:
+        """
+        run a pipeline.
+
+        - existing models are used for simulation and prediction.
+        - caution this might affect data inside platform or trigger automation.
+        - if your pipeline is templated please provide a twin.
+        - please provide all variables and parameters required through properties.
+        - return an execution
+            - check status with "wizata_dsapi.api().get(execution).status"
+            - check results in platform (dashboard/explorer) or perform queries.
+
+        :param pipeline: pipeline identified by its id (uuid or wizata_dsapi.Pipeline) or key (str).
+        :param twin: twin identified by its id (uuid or wizata_dsapi.Twin) or hardware ID (str).
+        :param properties: dictionary containing override for variables or additional parameters for your script.
+        """
+        return self.__execute(
+            pipeline=pipeline,
+            twin=twin,
+            properties=properties,
+            mode='production'
+        )
+
+    def plot(self, plot_id: str = None, plot: Plot = None, figure=None,):
+        """
+        Fetch and show plot.
+        :param plot: Wizata Plot Object
+        :param figure: JSON Figure
+        :param plot_id: Plot Id
+        :return: plotly figure
+        """
+        if plot is not None and plot.figure is not None:
+            return plotly.io.from_json(plot.figure)
+        elif plot is not None and plot.figure is None:
+            plot = self.get(plot)
+            if plot.figure is not None:
+                return plotly.io.from_json(plot.figure)
+            else:
+                raise ValueError('No plot has been fetch.')
+        elif figure is not None:
+            return plotly.io.from_json(plot.figure)
+        elif plot_id is not None:
+            plot = self.get(Plot(plot_id=plot_id))
+            if plot.figure is not None:
+                return plotly.io.from_json(plot.figure)
+            else:
+                raise ValueError('No plot has been fetch.')
+        else:
+            raise KeyError('No valid arguments.')
+
+    def plots(self, execution):
+        """
+        get all plot for an execution.
+        :param execution: id or Execution.
+        :return: list of plots.
+        """
+
+        if execution is None:
+            raise ValueError("execution cannot be None to retrieve plot")
+        if isinstance(execution, uuid.UUID):
+            execution_id = execution
+        elif isinstance(execution, str):
+            execution_id = uuid.UUID(execution)
+        elif isinstance(execution, Execution):
+            execution_id = execution.execution_id
+        else:
+            raise Exception(f'unsupported type {execution}')
+
+        response = requests.request("GET",
+                                    self.__url() + f"plots/?generatedById={execution_id}",
+                                    headers=self.__header()
+                                    )
+        if response.status_code == 200:
+            plots = []
+            for plot in response.json():
+                plots.append(self.plot(plot_id=str(plot["id"])))
+            return plots
+        else:
+            raise self.__raise_error(response)
+
+    def register_model(self,
+                       model_key,
+                       train_model,
+                       df: pandas.DataFrame,
+                       scaler=None,
+                       has_anomalies: bool = False,
+                       has_target_feat: bool = False,
+                       experiment_key = None) -> tuple[MLModel, pandas.DataFrame]:
+        """
+        Register a Machine Learning model to Wizata.
+        Model is tested by the API against a sample dataframe.
+        :param model_key: logical string id to identify the model.
+        :param train_model: trained model (must be compatible with pickle library)
+        :param df: sample dataframe.
+        :param scaler: scaler (must be compatible with pickle library)
+        :param has_anomalies: True is model generate Anomalies
+        :param has_target_feat: True if model need a target feature to be selected
+        :param experiment_key: Reference of an experiment to which link the generated ML Model
+        :return: registered ML Model , pandas.DataFrame
+        """
+        if model_key is None and isinstance(model_key, str):
+            raise ValueError('Please provide a str Model Key to identify the model.')
+        if train_model is None:
+            raise ValueError('Trained Machine Learning model should not be null')
+        elif df is None:
+            raise ValueError('A sample dataframe must be provided')
+
+        # Create a ML Model object
+        ml_model = MLModel()
+        ml_model.trained_model = train_model
+        if scaler is not None:
+            ml_model.scaler = scaler
+        ml_model.has_anomalies = has_anomalies
+        ml_model.has_target_feat = has_target_feat
+        ml_model.input_columns = df.columns
+        ml_model.key = model_key
+
+        if experiment_key is not None:
+            ml_model.experimentId = self.get(experiment_key=experiment_key).experiment_id
+
+        try:
+            result_df = predict(df, ml_model)
+            if result_df is not None:
+                ml_model.status = "valid"
+                self.upsert(ml_model)
+                return ml_model, result_df
+            else:
+                raise RuntimeError('no dataframe was generated by your model while testing predict capabilities')
+        except Exception as e:
+            raise RuntimeError('not able to validated the model : ' + str(e))
+
+    def upsert_experiment(self, key: str, name: str):
+        """
+        Upsert an experiment.
+        :param key: unique key identifying the experiment.
+        :param name: display name of the experiment
+        :return: upserted experiment.
+        """
+        experiment = self.get(experiment_key=key)
+        if experiment is not None:
+            found = True
+            experiment.name = name
+        else:
+            experiment = Experiment(
+                key=key,
+                name=name
+            )
+            found = False
+
+        if not found:
+            return self.create(experiment)
+        else:
+            return self.update(experiment)
+
+    def upsert_template(self, key: str, name: str):
+        """
+        Upsert a template.
+        :param key: unique key identifying the template.
+        :param name: display name of the template
+        :return: upserted template.
+        """
+
+        template = self.get(template_key=key)
+        if template is not None:
+            found = True
+            template.name = name
+        else:
+            template = Template(
+                key=key,
+                name=name
+            )
+            found = False
+
+        if not found:
+            return self.create(template)
+        else:
+            return self.update(template)
+
+    def upsert_pipeline(self, pipeline: Pipeline):
+        """
+        Upsert a template (ignore ID, use the key)
+        :return: upserted template.
+        """
+
+        get = self.get(pipeline_key=pipeline.key)
+        if get is not None:
+            pipeline.pipeline_id = get.pipeline_id
+            return self.update(pipeline)
+        else:
+            return self.create(pipeline)
+
+    def upsert_datapoint(self, datapoint: DataPoint):
+        """
+        Upsert a datapoint (ignore ID, use the key)
+        :return: upsert datapoint.
+        """
+
+        get = self.get(datapoint_hardware_id=datapoint.hardware_id)
+        if get is not None:
+            datapoint.datapoint_id = get.datapoint_id
+            return self.update(datapoint)
+        else:
+            return self.create(datapoint)
+
+
+    def upsert_twin(self, twin: Twin):
+        """
+        Upsert a twin (ignore ID, use the key)
+        :return: upsert twin.
+        """
+
+        get = self.get(twin_hardware_id=twin.hardware_id)
+        if get is not None:
+            twin.twin_id = get.twin_id
+            return self.update(twin)
+        else:
+            return self.create(twin)
+
+    def add_template_property(self,
+                              template,
+                              property_name: str, property_type: str = "datapoint",
+                              is_required: bool = True):
+
+        # check type
+        p_type = VarType(property_type)
+
+        if isinstance(template, str):
+            template = self.get(template_key=template)
+        elif not isinstance(template, Template):
+            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
+
+        if property_name is None:
+            raise ValueError('please provide a valid name for the property')
+
+        property_dict = {
+            "type": p_type.value,
+            "name": property_name,
+            "required": is_required
+        }
+
+        response = requests.post(self.__url() + "templates/" + str(template.template_id) + '/properties/',
+                                 headers=self.__header(),
+                                 data=json.dumps(property_dict))
+        if response.status_code == 200:
+            return
+        else:
+            raise self.__raise_error(response)
+
+    def remove_template_property(self, template, property_name: str):
+
+        if isinstance(template, str):
+            template = self.get(template_key=template)
+        elif not isinstance(template, Template):
+            raise TypeError('template must be a key str referring template or a proper wizata_dsapi Template')
+
+        if property_name is None:
+            raise ValueError('please provide a valid name for the property')
+
+        property_dict = {
+            "name": property_name
+        }
+
+        response = requests.delete(self.__url() + "templates/" + str(template.template_id) + '/properties/',
+                                   headers=self.__header(),
+                                   data=json.dumps(property_dict))
+        if response.status_code == 200:
+            return
+        else:
+            raise self.__raise_error(response)
+
+    def get_registrations(self, template) -> list:
+        """
+        retrieve all registrations for
+        :param template: template object, UUID or str key.
+        :return: list of twin registration.
+        """
+
+        if template is None:
+            raise ValueError('template must be specified.')
+        elif isinstance(template, uuid.UUID):
+            template = self.get(wizata_dsapi.Template(template_id=template))
+        elif isinstance(template, str):
+            template = self.get(template_key=template)
+        elif not isinstance(template, Template):
+            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
+        if template is None:
+            raise ValueError('template cannot be found on server')
+
+        response = requests.get(self.__url() + "templates/" + str(template.template_id) + '/registrations/',
+                                headers=self.__header())
+        if response.status_code == 200:
+            registrations_json = response.json()
+            registrations = []
+            for twin_registration_json in registrations_json:
+                registration = TwinRegistration()
+                registration.from_json(twin_registration_json)
+                registrations.append(registration)
+            return registrations
+        else:
+            raise self.__raise_error(response)
+
+    def register_twin(self, template, twin, properties: dict, override=True):
+        """
+        register a twin on a specific template using a map.
+        :param template: template object, UUID or str key.
+        :param twin: twin object, UUID or str key.
+        :param properties: dict where key = template property and value = datapoint name or const value (str, int, float, relative or epoch datetime).
+        :param override: by default at True - allow overriding any existing subscription
+        """
+
+        if template is None:
+            raise ValueError('template must be specified.')
+        elif isinstance(template, uuid.UUID):
+            template = self.get(wizata_dsapi.Template(template_id=template))
+        elif isinstance(template, str):
+            template = self.get(template_key=template)
+        elif not isinstance(template, Template):
+            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
+
+        if template is None:
+            raise ValueError('template cannot be found on server')
+
+        if twin is None:
+            raise ValueError('twin must be specified.')
+        elif isinstance(twin, uuid.UUID):
+            twin_id = twin
+        elif isinstance(twin, str):
+            twin_id = self.get(twin_hardware_id=twin).twin_id
+        elif isinstance(twin, Twin):
+            twin_id = twin.twin_id
+        else:
+            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
+
+        if template.properties is None or len(template.properties) == 0:
+            raise ValueError('template chosen does not contains any properties')
+
+        if properties is None or len(properties.keys()) == 0:
+            raise ValueError('your map dictionary must contains properties matching template')
+
+        twin_properties = {
+            "properties": []
+        }
+        for key in properties.keys():
+            property_type = None
+            for template_property in template.properties:
+                template_property: TemplateProperty
+                if key == template_property.name:
+                    property_type = template_property.p_type
+            if property_type is None:
+                raise ValueError(f'cannot find property {key} in template or cannot determine its type')
+            twin_properties["properties"].append({
+                'name': key,
+                property_type.value: properties[key]
+            })
+
+        # Check if already exist
+        exists = False
+        response_exists = requests.get(self.__url() + "templates/" + str(template.template_id)
+                                       + '/registrations/' + str(twin_id) + '/',
+                                       headers=self.__header())
+        if response_exists.status_code == 200:
+            exists = True
+
+        if exists and not override:
+            raise ValueError("registration already exists and override not allowed.")
+
+        if exists and override:
+            response = requests.put(self.__url() + "templates/" + str(template.template_id)
+                                    + '/registrations/' + str(twin_id) + '/',
+                                    headers=self.__header(),
+                                    data=json.dumps(twin_properties))
+        else:
+            response = requests.post(self.__url() + "templates/" + str(template.template_id)
+                                     + '/registrations/' + str(twin_id) + '/',
+                                     headers=self.__header(),
+                                     data=json.dumps(twin_properties))
+
+        if response.status_code == 200:
+            return
+        else:
+            raise self.__raise_error(response)
+
+    def unregister_twin(self, template, twin):
+        """
+        un-register a twin from a specific template.
+        :param template: template object, UUID or str key.
+        :param twin: twin object, UUID or str key.
+        """
+
+        if template is None:
+            raise ValueError('template must be specified.')
+        elif isinstance(template, uuid.UUID):
+            template = self.get(wizata_dsapi.Template(template_id=template))
+        elif isinstance(template, str):
+            template = self.get(template_key=template)
+        elif not isinstance(template, Template):
+            raise TypeError('template must be UUID, a key str referring template or a proper wizata_dsapi Template')
+
+        if twin is None:
+            raise ValueError('twin must be specified.')
+        elif isinstance(twin, uuid.UUID):
+            twin_id = twin
+        elif isinstance(twin, str):
+            twin_id = self.get(twin_hardware_id=twin).twin_id
+        elif isinstance(twin, Twin):
+            twin_id = twin.twin_id
+        else:
+            raise TypeError('twin must be UUID, a key str referring hardware ID or a proper wizata_dsapi Twin')
+
+        response = requests.delete(self.__url() + "templates/" + str(template.template_id)
+                                   + '/registrations/' + str(twin_id) + '/',
+                                   headers=self.__header())
+        if response.status_code == 200:
+            return
+        else:
+            raise self.__raise_error(response)
+
+
+def api() -> WizataDSAPIClient:
+    """
+    Create a WizataDSAPIClient from environment variables.
+    :return: client
+    """
+    protocol = 'https'
+
+    if os.environ.get('WIZATA_PROTOCOL') is not None:
+        protocol = os.environ.get('WIZATA_PROTOCOL')
+
+    if os.environ.get('WIZATA_CLIENT_SECRET') is not None:
+        return WizataDSAPIClient(
+            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
+            client_id=os.environ.get('WIZATA_CLIENT_ID'),
+            client_secret=os.environ.get('WIZATA_CLIENT_SECRET'),
+            scope=os.environ.get('WIZATA_CLIENT_ID') + '/.default',
+            domain=os.environ.get('WIZATA_DOMAIN'),
+            protocol=protocol
+        )
+    else:
+        return WizataDSAPIClient(
+            tenant_id=os.environ.get('WIZATA_TENANT_ID'),
+            client_id=os.environ.get('WIZATA_CLIENT_ID'),
+            scope=os.environ.get('WIZATA_SCOPE'),
+            username=os.environ.get('WIZATA_USERNAME'),
+            password=os.environ.get('WIZATA_PASSWORD'),
+            domain=os.environ.get('WIZATA_DOMAIN'),
+            protocol=protocol
+        )
+
+
+def is_valid_uuid(val):
+    try:
+        uuid.UUID(str(val))
+        return True
+    except ValueError:
+        return False
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi.egg-info/SOURCES.txt` & `wizata-dsapi-0.3.1/wizata_dsapi.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 LICENSE.txt
 README.rst
 setup.py
 wizata_dsapi/__init__.py
 wizata_dsapi/api_dto.py
+wizata_dsapi/context.py
 wizata_dsapi/dataframe_toolkit.py
 wizata_dsapi/datapoint.py
 wizata_dsapi/ds_dataframe.py
 wizata_dsapi/dsapi_json_encoder.py
 wizata_dsapi/execution.py
 wizata_dsapi/experiment.py
 wizata_dsapi/mlmodel.py
```

### Comparing `wizata-dsapi-0.2.9/wizata_dsapi.egg-info/requires.txt` & `wizata-dsapi-0.3.1/wizata_dsapi.egg-info/requires.txt`

 * *Files identical despite different names*

