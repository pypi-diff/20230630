# Comparing `tmp/pyjedai-0.0.6.tar.gz` & `tmp/pyjedai-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjedai-0.0.6.tar", last modified: Thu Jun  1 09:49:46 2023, max compression
+gzip compressed data, was "pyjedai-0.0.7.tar", last modified: Fri Jun 30 14:16:07 2023, max compression
```

## Comparing `pyjedai-0.0.6.tar` & `pyjedai-0.0.7.tar`

### file list

```diff
@@ -1,28 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.476420 pyjedai-0.0.6/
--rw-rw-rw-   0        0        0    11684 2022-09-21 14:32:22.000000 pyjedai-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     7197 2023-06-01 09:49:46.474413 pyjedai-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5557 2023-05-17 14:23:07.000000 pyjedai-0.0.6/README.md
--rw-rw-rw-   0        0        0     2425 2023-06-01 09:49:26.000000 pyjedai-0.0.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-01 09:49:46.476420 pyjedai-0.0.6/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.396943 pyjedai-0.0.6/src/
-drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.437252 pyjedai-0.0.6/src/pyjedai/
--rw-rw-rw-   0        0        0        0 2022-07-19 14:45:04.000000 pyjedai-0.0.6/src/pyjedai/__init__.py
--rw-rw-rw-   0        0        0    18483 2023-05-05 17:55:55.000000 pyjedai-0.0.6/src/pyjedai/block_building.py
--rw-rw-rw-   0        0        0     8520 2023-05-05 17:55:55.000000 pyjedai-0.0.6/src/pyjedai/block_cleaning.py
--rw-rw-rw-   0        0        0     8107 2023-05-16 13:45:11.000000 pyjedai-0.0.6/src/pyjedai/clustering.py
--rw-rw-rw-   0        0        0    29695 2023-05-15 12:18:45.000000 pyjedai-0.0.6/src/pyjedai/comparison_cleaning.py
--rw-rw-rw-   0        0        0     9931 2023-05-24 11:14:07.000000 pyjedai-0.0.6/src/pyjedai/datamodel.py
--rw-rw-rw-   0        0        0    18898 2023-05-15 10:36:29.000000 pyjedai-0.0.6/src/pyjedai/evaluation.py
--rw-rw-rw-   0        0        0    14566 2023-05-17 08:37:13.000000 pyjedai-0.0.6/src/pyjedai/joins.py
--rw-rw-rw-   0        0        0      774 2022-08-31 12:44:46.000000 pyjedai-0.0.6/src/pyjedai/logs.py
--rw-rw-rw-   0        0        0    24233 2023-05-16 12:56:27.000000 pyjedai-0.0.6/src/pyjedai/matching.py
--rw-rw-rw-   0        0        0     8156 2023-05-16 12:34:27.000000 pyjedai-0.0.6/src/pyjedai/utils.py
--rw-rw-rw-   0        0        0    27952 2023-06-01 09:32:54.000000 pyjedai-0.0.6/src/pyjedai/vector_based_blocking.py
--rw-rw-rw-   0        0        0      955 2022-07-19 14:45:04.000000 pyjedai-0.0.6/src/pyjedai/visualization.py
--rw-rw-rw-   0        0        0    24786 2023-05-24 13:22:15.000000 pyjedai-0.0.6/src/pyjedai/workflow.py
-drwxrwxrwx   0        0        0        0 2023-06-01 09:49:46.472536 pyjedai-0.0.6/src/pyjedai.egg-info/
--rw-rw-rw-   0        0        0     7197 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      578 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      428 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-01 09:49:46.000000 pyjedai-0.0.6/src/pyjedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11392 2023-06-30 14:15:51.000000 pyjedai-0.0.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-06-30 14:16:07.510203 pyjedai-0.0.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10712 2023-06-30 14:15:51.000000 pyjedai-0.0.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2499 2023-06-30 14:15:51.000000 pyjedai-0.0.7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-30 14:16:07.510203 pyjedai-0.0.7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.506203 pyjedai-0.0.7/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/src/pyjedai/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18191 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7917 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52141 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13881 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/datamodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20949 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14255 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/joins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28190 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/matching.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50691 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/prioritization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23712 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23817 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/vector_based_blocking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/visualization.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24196 2023-06-30 14:15:51.000000 pyjedai-0.0.7/src/pyjedai/workflow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/src/pyjedai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12318 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-30 14:16:07.000000 pyjedai-0.0.7/src/pyjedai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-30 14:16:07.510203 pyjedai-0.0.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_block_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_block_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_clustering.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3858 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_comparison_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-30 14:15:51.000000 pyjedai-0.0.7/tests/test_joins.py
```

### Comparing `pyjedai-0.0.6/LICENSE` & `pyjedai-0.0.7/LICENSE`

 * *Files 12% similar despite different names*

```diff
@@ -1,202 +1,201 @@
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-      Copyright (c) 2022 Konstantinos Nikoletos, George Papadakis & Manolis Koubarakis
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
-   Copyright [2022] [Konstantinos Nikoletos, George Papadakis & Manolis Koubarakis]
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
+   Copyright 2022 Konstantinos Nikoletos & George Papadakis & Manolis Koubarakis
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

### Comparing `pyjedai-0.0.6/pyproject.toml` & `pyjedai-0.0.7/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyjedai"
-version = "0.0.6"
+version = "0.0.7"
 description = "An open-source library that builds powerful end-to-end Entity Resolution workflows."
 readme = "README.md"
 authors = [
     { name = "Konstantinos Nikoletos", email = "nikoletos.kon@gmail.com" },
     { name = "George Papadakis", email = "gpapadis84@gmail.com" },
 ]
 license = {text = "Apache Software License 2.0"}
@@ -55,16 +55,19 @@
     "strsim >= 0.0.3",
     "strsimpy >= 0.2.1",
     "tqdm >= 4.64",
     "transformers >= 4.21",
     "sentence-transformers >= 2.2",
     "faiss-cpu >= 1.7",
     "optuna >= 3.0",
-    'tomli; python_version < "3.11"', 
-    "py-stringmatching >= 0.4"
+    'tomli; python_version < "3.11"',
+    "py-stringmatching >= 0.4",
+    "whoosh >= 2.7",
+    "valentine>=0.1.5",
+    "ordered-set >= 4.0",
 ]
 
 [project.optional-dependencies]
 dev = ["pip-tools", "pytest"]
 
 [project.urls]
 "Homepage" = "http://pyjedai.rtfd.io"
```

### Comparing `pyjedai-0.0.6/src/pyjedai/block_building.py` & `pyjedai-0.0.7/src/pyjedai/block_building.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,447 +1,446 @@
-import itertools
-import logging as log
-import math
-import re
-import time
-from abc import ABC, abstractmethod
-from collections import defaultdict
-from typing import Tuple
-
-import nltk
-import numpy as np
-from tqdm.auto import tqdm
-
-from .datamodel import Block, Data, PYJEDAIFeature
-from .utils import (are_matching, drop_big_blocks_by_size,
-                    drop_single_entity_blocks)
-from .evaluation import Evaluation
-
-class AbstractBlockProcessing(PYJEDAIFeature):
-    """Abstract class for the block building method
-    """
-
-    def __init__(self):
-        super().__init__()
-        self.blocks: dict
-        self.attributes_1: list
-        self.attributes_2: list
-        self.num_of_blocks_dropped: int
-        self.original_num_of_blocks: int
-    
-    def report(self) -> None:
-        """Prints Block Building method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
-            "Attributes from D1:\n\t" + ', '.join(c for c in (self.attributes_1 if self.attributes_1 is not None \
-                else self.data.dataset_1.columns)) +
-            ("\nAttributes from D2:\n\t" + ', '.join(c for c in (self.attributes_2 if self.attributes_2 is not None \
-                else self.data.dataset_2.columns)) if not self.data.is_dirty_er else "") +
-            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-    def evaluate(self,
-                 prediction,
-                 export_to_df: bool = False,
-                 export_to_dict: bool = False,
-                 with_classification_report: bool = False,
-                 verbose: bool = True,
-                 with_stats: bool = False) -> any:
-
-        if prediction is None:
-            if self.blocks is None:
-                raise AttributeError("Can not proceed to evaluation without build_blocks.")
-            else:
-                eval_blocks = self.blocks
-        else:
-            eval_blocks = prediction
-            
-        if self.data is None:
-            raise AttributeError("Can not proceed to evaluation without data object.")
-
-        if self.data.ground_truth is None:
-            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " + 
-                    "Data object has not been initialized with the ground-truth file")
-
-        eval_obj = Evaluation(self.data)
-        true_positives = 0
-        entity_index = eval_obj._create_entity_index_from_blocks(eval_blocks)
-        for _, (id1, id2) in self.data.ground_truth.iterrows():
-            id1 = self.data._ids_mapping_1[id1]
-            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
-            if id1 in entity_index and    \
-                id2 in entity_index and are_matching(entity_index, id1, id2):
-                true_positives += 1
-
-        eval_obj.calculate_scores(true_positives=true_positives)
-        eval_result = eval_obj.report(self.method_configuration(),
-                                export_to_df,
-                                export_to_dict,
-                                with_classification_report,
-                                verbose)
-        if with_stats:
-            self.stats(eval_blocks)
-        return eval_result
-    
-    
-    def stats(self, blocks: dict) -> None:
-        self.list_of_sizes = []
-        self.entities_in_blocks = set()
-        for block in blocks.values():
-            self.sum_of_sizes += block.get_size()
-            self.min_block_size = min(self.min_block_size, block.get_size()) if self.min_block_size else block.get_size()
-            self.max_block_size = max(self.max_block_size, block.get_size()) if self.max_block_size else block.get_size()
-            self.min_block_comparisons = min(self.min_block_comparisons, block.get_cardinality(self.data.is_dirty_er)) if self.min_block_comparisons else block.get_cardinality(self.data.is_dirty_er)
-            self.max_block_comparisons = max(self.max_block_comparisons, block.get_cardinality(self.data.is_dirty_er)) if self.max_block_comparisons else block.get_cardinality(self.data.is_dirty_er)
-            self.list_of_sizes.append(block.get_size())
-            self.entities_in_blocks = self.entities_in_blocks.union(block.entities_D1)
-            if not self.data.is_dirty_er:
-                self.entities_in_blocks = self.entities_in_blocks.union(block.entities_D2)
-            self.total_num_of_comparisons += block.get_cardinality(self.data.is_dirty_er)
-        
-        self.num_of_blocks = len(blocks)
-        self.average_block_size = int(self.sum_of_sizes / self.num_of_blocks)
-        self.list_of_sizes = sorted(self.list_of_sizes)
-        median = self.list_of_sizes[int(len(self.list_of_sizes)/2)]
-        print(
-            "Statistics:" +
-            "\n\tNumber of blocks: " + str(self.num_of_blocks) +
-            "\n\tAverage block size: " + str(self.average_block_size) +
-            "\n\tMedian block size: " + str(median) +
-            "\n\tMax block size: " + str(self.max_block_size) +
-            "\n\tMin block size: " + str(self.min_block_size) +
-            "\n\tNumber of blocks dropped: " + str(self.num_of_blocks_dropped) +
-            "\n\tNumber of comparisons: " + str(self.total_num_of_comparisons) +
-            "\n\tMax comparisons per block: " + str(self.max_block_comparisons) +
-            "\n\tMin comparisons per block: " + str(self.min_block_comparisons) +
-            "\n\tEntities in blocks: " + str(len(self.entities_in_blocks))
-        )
-        print(u'\u2500' * 123)
-
-
-class AbstractBlockBuilding(AbstractBlockProcessing):
-    """Abstract class for the block building method
-    """
-
-    _method_name: str
-    _method_info: str
-    _method_short_name: str
-
-    def __init__(self):
-        super().__init__()
-        self.blocks: dict
-        self._progress_bar: tqdm
-        self.attributes_1: list
-        self.attributes_2: list
-        self.execution_time: float
-        self.data: Data
-        self.sum_of_sizes: int = 0
-        self.list_of_sizes: list = []
-        self.total_num_of_comparisons: int = 0
-        self.min_block_size: int = None
-        self.max_block_size: int = None
-        self.min_block_comparisons: int = None
-        self.max_block_comparisons: int = None
-
-    def build_blocks(
-            self,
-            data: Data,
-            attributes_1: list = None,
-            attributes_2: list = None,
-            tqdm_disable: bool = False
-    ) -> Tuple[dict, dict]:
-        """Main method of Blocking in a dataset
-
-            Args:
-                data (Data): Data module that contaiins the processed dataset
-                attributes_1 (list, optional): Attribute columns of the dataset 1 \
-                    that will be processed. Defaults to None. \
-                    If not provided, all attributes are slected.
-                attributes_2 (list, optional): Attribute columns of the dataset 2. \
-                    Defaults to None. If not provided, all attributes are slected.
-                tqdm_disable (bool, optional): Disables all tqdm at processing. Defaults to False.
-
-            Returns:
-                Tuple[dict, dict]: Dictionary of blocks, Dict of entity index (reversed blocks).
-        """
-
-        _start_time = time.time()
-        self.data, self.attributes_1, self.attributes_2 = data, attributes_1, attributes_2
-        self._progress_bar = tqdm(
-            total=data.num_of_entities, desc=self._method_name, disable=tqdm_disable
-        )
-
-        # TODO Text process function can be applied in this step (.apply)
-        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
-                            .apply(" ".join, axis=1) \
-                            .apply(self._tokenize_entity) \
-                            .values.tolist()
-                        # if attributes_1 else data.entities_d1.apply(self._tokenize_entity)
-
-        self._all_tokens = set(itertools.chain.from_iterable(self._entities_d1))
-
-        if not data.is_dirty_er:
-            self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
-                    .apply(" ".join, axis=1) \
-                    .apply(self._tokenize_entity) \
-                    .values.tolist()
-            self._all_tokens.union(set(itertools.chain.from_iterable(self._entities_d2)))
-
-        entity_id = itertools.count()
-        blocks = {}
-        
-        for entity in self._entities_d1:
-            eid = next(entity_id)
-            for token in entity:
-                blocks.setdefault(token, Block())
-                blocks[token].entities_D1.add(eid)
-            self._progress_bar.update(1)
-
-        if not data.is_dirty_er:
-            for entity in self._entities_d2:
-                eid = next(entity_id)
-                for token in entity:
-                    blocks.setdefault(token, Block())
-                    blocks[token].entities_D2.add(eid)
-                self._progress_bar.update(1)
-
-        self.original_num_of_blocks = len(blocks)
-        self.blocks = self._clean_blocks(blocks)
-        self.num_of_blocks_dropped = len(blocks) - len(self.blocks)
-        self.execution_time = time.time() - _start_time
-        self._progress_bar.close()
-
-        return self.blocks
-
-    def report(self) -> None:
-        """Prints Block Building method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
-            "Attributes from D1:\n\t" + ', '.join(c for c in (self.attributes_1 if self.attributes_1 is not None \
-                else self.data.dataset_1.columns)) +
-            ("\nAttributes from D2:\n\t" + ', '.join(c for c in (self.attributes_2 if self.attributes_2 is not None \
-                else self.data.dataset_2.columns)) if not self.data.is_dirty_er else "") +
-            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-    @abstractmethod
-    def _clean_blocks(self, blocks: dict) -> dict:
-        pass
-
-    @abstractmethod
-    def _configuration(self) -> dict:
-        pass
-    
-class StandardBlocking(AbstractBlockBuilding):
-    """ Creates one block for every token in \
-        the attribute values of at least two entities.
-    """
-
-    _method_name = "Standard Blocking"
-    _method_short_name: str = "SB"
-    _method_info = "Creates one block for every token in " + \
-        "the attribute values of at least two entities."
-
-    def __init__(self) -> any:
-        super().__init__()
-
-    def _tokenize_entity(self, entity: str) -> list:
-        """Produces a list of workds of a given string
-
-        Args:
-            entity (str): String representation  of an entity
-
-        Returns:
-            list: List of words
-        """
-        return list(set(filter(None, re.split('[\\W_]', entity.lower()))))
-
-    def _clean_blocks(self, blocks: dict) -> dict:
-        """No cleaning"""
-        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
-
-    def _configuration(self) -> dict:
-        """No configuration"""
-        return {}
-
-class QGramsBlocking(StandardBlocking):
-    """ Creates one block for every q-gram that is extracted \
-        from any token in the attribute values of any entity. \
-            The q-gram must be shared by at least two entities.
-    """
-
-    _method_name = "Q-Grams Blocking"
-    _method_short_name: str = "QGB"
-    _method_info = "Creates one block for every q-gram that is extracted " + \
-                    "from any token in the attribute values of any entity. " + \
-                    "The q-gram must be shared by at least two entities."
-
-    def __init__(
-            self, qgrams: int = 6
-    ) -> any:
-        super().__init__()
-        self.qgrams = qgrams
-
-    def _tokenize_entity(self, entity) -> set:
-        keys = set()
-        for token in super()._tokenize_entity(entity):
-            if len(token) < self.qgrams:
-                keys.add(token)
-            else:
-                keys.update(''.join(qg) for qg in nltk.ngrams(token, n=self.qgrams))
-        return keys
-
-    def _clean_blocks(self, blocks: dict) -> dict:
-        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
-
-    def _configuration(self) -> dict:
-        return {
-            "Q-Gramms" : self.qgrams
-        }
-
-class SuffixArraysBlocking(StandardBlocking):
-    """ It creates one block for every suffix that appears \
-        in the attribute value tokens of at least two entities.
-    """
-
-    _method_name = "Suffix Arrays Blocking"
-    _method_short_name: str = "SAB"
-    _method_info = "Creates one block for every suffix that appears in the " + \
-        "attribute value tokens of at least two entities."
-
-    def __init__(
-            self,
-            suffix_length: int = 6,
-            max_block_size: int = 53
-    ) -> any:
-        super().__init__()
-        self.suffix_length, self.max_block_size = suffix_length, max_block_size
-
-    def _tokenize_entity(self, entity) -> set:
-        keys = set()
-        for token in super()._tokenize_entity(entity):
-            if len(token) < self.suffix_length:
-                keys.add(token)
-            else:
-                for length in range(0, len(token) - self.suffix_length + 1):
-                    keys.add(token[length:])
-        return keys
-
-    def _clean_blocks(self, blocks: dict) -> dict:
-        return drop_big_blocks_by_size(blocks, self.max_block_size, self.data.is_dirty_er)
-
-    def _configuration(self) -> dict:
-        return {
-            "Suffix length" : self.suffix_length,
-            "Maximum Block Size" : self.max_block_size
-        }
-
-class ExtendedSuffixArraysBlocking(StandardBlocking):
-    """ It creates one block for every substring \
-        (not just suffix) that appears in the tokens of at least two entities.
-    """
-
-    _method_name = "Extended Suffix Arrays Blocking"
-    _method_short_name: str = "ESAB"
-    _method_info = "Creates one block for every substring (not just suffix) " + \
-        "that appears in the tokens of at least two entities."
-
-    def __init__(
-            self,
-            suffix_length: int = 6,
-            max_block_size: int = 39
-    ) -> any:
-        super().__init__()
-        self.suffix_length, self.max_block_size = suffix_length, max_block_size
-
-    def _tokenize_entity(self, entity) -> set:
-        keys = set()
-        for token in super()._tokenize_entity(entity):
-            keys.add(token)
-            if len(token) > self.suffix_length:
-                for current_size in range(self.suffix_length, len(token)): 
-                    for letters in list(nltk.ngrams(token, n=current_size)):
-                        keys.add("".join(letters))
-        return keys
-
-    def _clean_blocks(self, blocks: dict) -> dict:
-        return drop_big_blocks_by_size(blocks, self.max_block_size, self.data.is_dirty_er)
-
-    def _configuration(self) -> dict:
-        return {
-            "Suffix length" : self.suffix_length,
-            "Maximum Block Size" : self.max_block_size
-        }
-
-class ExtendedQGramsBlocking(StandardBlocking):
-    """It creates one block for every combination of q-grams that represents at least two entities.
-    The q-grams are extracted from any token in the attribute values of any entity.
-    """
-
-    _method_name = "Extended QGramsBlocking"
-    _method_short_name: str = "EQGB"
-    _method_info = "Creates one block for every substring (not just suffix) " + \
-        "that appears in the tokens of at least two entities."
-
-    def __init__(
-            self,
-            qgrams: int = 6,
-            threshold: float = 0.95
-    ) -> any:
-        super().__init__()
-        self.threshold: float = threshold
-        self.MAX_QGRAMS: int = 15
-        self.qgrams = qgrams
-
-    def _tokenize_entity(self, entity) -> set:
-        keys = set()
-        for token in super()._tokenize_entity(entity):
-            if len(token) < self.qgrams:
-                keys.add(token)
-            else:   
-                qgrams = [''.join(qgram) for qgram in nltk.ngrams(token, n=self.qgrams)]
-                if len(qgrams) == 1:
-                    keys.update(qgrams)
-                else:
-                    if len(qgrams) > self.MAX_QGRAMS:
-                        qgrams = qgrams[:self.MAX_QGRAMS]
-
-                    minimum_length = max(1, math.floor(len(qgrams) * self.threshold))
-                    for i in range(minimum_length, len(qgrams) + 1):
-                        keys.update(self._qgrams_combinations(qgrams, i))
-
-        return keys
-
-    def _qgrams_combinations(self, sublists: list, sublist_length: int) -> list:
-        if sublist_length == 0 or len(sublists) < sublist_length:
-            return []
-
-        remaining_elements = sublists.copy()
-        last_sublist = remaining_elements.pop(len(sublists)-1)
-
-        combinations_exclusive_x = self._qgrams_combinations(remaining_elements, sublist_length)
-        combinations_inclusive_x = self._qgrams_combinations(remaining_elements, sublist_length-1)
-
-        resulting_combinations = combinations_exclusive_x.copy() if combinations_exclusive_x else []
-
-        if not combinations_inclusive_x: # is empty
-            resulting_combinations.append(last_sublist)
-        else:
-            for combination in combinations_inclusive_x:
-                resulting_combinations.append(combination+last_sublist)
-
-        return resulting_combinations
-
-    def _clean_blocks(self, blocks: dict) -> dict:
-        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
-
-    def _configuration(self) -> dict:
-        return {
-            "Q-Gramms" : self.qgrams,
-            "Threshold" : self.threshold
-        }
+import itertools
+import logging as log
+import math
+import re
+import time
+from abc import ABC, abstractmethod
+from collections import defaultdict
+from typing import Tuple
+
+import nltk
+import numpy as np
+from tqdm.auto import tqdm
+
+from .datamodel import Block, Data, PYJEDAIFeature
+from .utils import (are_matching, drop_big_blocks_by_size,
+                    drop_single_entity_blocks, get_blocks_cardinality)
+from .evaluation import Evaluation
+
+class AbstractBlockProcessing(PYJEDAIFeature):
+    """Abstract class for the block building method
+    """
+
+    def __init__(self):
+        super().__init__()
+        self.blocks: dict
+        self.attributes_1: list
+        self.attributes_2: list
+        self.num_of_blocks_dropped: int
+        self.original_num_of_blocks: int
+        self.sum_of_sizes: int = 0
+        self.total_num_of_comparisons: int = 0
+        self.min_block_size: int = None
+        self.max_block_size: int = None
+        self.min_block_comparisons: int = None
+        self.max_block_comparisons: int = None
+            
+    def report(self) -> None:
+        """Prints Block Building method configuration
+        """
+        print(
+            "Method name: " + self._method_name +
+            "\nMethod info: " + self._method_info +
+            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
+            "Attributes from D1:\n\t" + ', '.join(c for c in (self.attributes_1 if self.attributes_1 is not None \
+                else self.data.dataset_1.columns)) +
+            ("\nAttributes from D2:\n\t" + ', '.join(c for c in (self.attributes_2 if self.attributes_2 is not None \
+                else self.data.dataset_2.columns)) if not self.data.is_dirty_er else "") +
+            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
+        )
+
+    def evaluate(self,
+                 prediction,
+                 export_to_df: bool = False,
+                 export_to_dict: bool = False,
+                 with_classification_report: bool = False,
+                 verbose: bool = True,
+                 with_stats: bool = False) -> any:
+
+        if prediction is None:
+            if self.blocks is None:
+                raise AttributeError("Can not proceed to evaluation without build_blocks.")
+            else:
+                eval_blocks = self.blocks
+        else:
+            eval_blocks = prediction
+            
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " + 
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        entity_index = eval_obj._create_entity_index_from_blocks(eval_blocks)
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
+            if id1 in entity_index and    \
+                id2 in entity_index and are_matching(entity_index, id1, id2):
+                true_positives += 1
+
+        total_matching_pairs = get_blocks_cardinality(eval_blocks, self.data.is_dirty_er)
+        eval_obj.calculate_scores(true_positives=true_positives, total_matching_pairs=total_matching_pairs)
+        eval_result = eval_obj.report(self.method_configuration(),
+                                export_to_df,
+                                export_to_dict,
+                                with_classification_report,
+                                verbose)
+        if with_stats:
+            self.stats(eval_blocks)
+        return eval_result
+
+    def stats(self, blocks: dict) -> None:
+        self.list_of_sizes = []
+        self.entities_in_blocks = set()
+        for block in blocks.values():
+            self.sum_of_sizes += block.get_size()
+            self.min_block_size = min(self.min_block_size, block.get_size()) if self.min_block_size else block.get_size()
+            self.max_block_size = max(self.max_block_size, block.get_size()) if self.max_block_size else block.get_size()
+            self.min_block_comparisons = min(self.min_block_comparisons, block.get_cardinality(self.data.is_dirty_er)) if self.min_block_comparisons else block.get_cardinality(self.data.is_dirty_er)
+            self.max_block_comparisons = max(self.max_block_comparisons, block.get_cardinality(self.data.is_dirty_er)) if self.max_block_comparisons else block.get_cardinality(self.data.is_dirty_er)
+            self.list_of_sizes.append(block.get_size())
+            self.entities_in_blocks = self.entities_in_blocks.union(block.entities_D1)
+            if not self.data.is_dirty_er:
+                self.entities_in_blocks = self.entities_in_blocks.union(block.entities_D2)
+            self.total_num_of_comparisons += block.get_cardinality(self.data.is_dirty_er)
+        
+        self.num_of_blocks = len(blocks)
+        self.average_block_size = int(self.sum_of_sizes / self.num_of_blocks)
+        self.list_of_sizes = sorted(self.list_of_sizes)
+        median = self.list_of_sizes[int(len(self.list_of_sizes)/2)]
+        print(
+            "Statistics:" +
+            "\n\tNumber of blocks: " + str(self.num_of_blocks) +
+            "\n\tAverage block size: " + str(self.average_block_size) +
+            "\n\tMedian block size: " + str(median) +
+            "\n\tMax block size: " + str(self.max_block_size) +
+            "\n\tMin block size: " + str(self.min_block_size) +
+            "\n\tNumber of blocks dropped: " + str(self.num_of_blocks_dropped) +
+            "\n\tNumber of comparisons: " + str(self.total_num_of_comparisons) +
+            "\n\tMax comparisons per block: " + str(self.max_block_comparisons) +
+            "\n\tMin comparisons per block: " + str(self.min_block_comparisons) +
+            "\n\tEntities in blocks: " + str(len(self.entities_in_blocks))
+        )
+        print(u'\u2500' * 123)
+
+class AbstractBlockBuilding(AbstractBlockProcessing):
+    """Abstract class for the block building method
+    """
+
+    _method_name: str
+    _method_info: str
+    _method_short_name: str
+
+    def __init__(self):
+        super().__init__()
+        self.blocks: dict
+        self._progress_bar: tqdm
+        self.attributes_1: list
+        self.attributes_2: list
+        self.execution_time: float
+        self.data: Data
+        self.list_of_sizes: list = []
+
+    def build_blocks(
+            self,
+            data: Data,
+            attributes_1: list = None,
+            attributes_2: list = None,
+            tqdm_disable: bool = False
+    ) -> Tuple[dict, dict]:
+        """Main method of Blocking in a dataset
+
+            Args:
+                data (Data): Data module that contaiins the processed dataset
+                attributes_1 (list, optional): Attribute columns of the dataset 1 \
+                    that will be processed. Defaults to None. \
+                    If not provided, all attributes are slected.
+                attributes_2 (list, optional): Attribute columns of the dataset 2. \
+                    Defaults to None. If not provided, all attributes are slected.
+                tqdm_disable (bool, optional): Disables all tqdm at processing. Defaults to False.
+
+            Returns:
+                Tuple[dict, dict]: Dictionary of blocks, Dict of entity index (reversed blocks).
+        """
+
+        _start_time = time.time()
+        self.data, self.attributes_1, self.attributes_2 = data, attributes_1, attributes_2
+        self._progress_bar = tqdm(
+            total=data.num_of_entities, desc=self._method_name, disable=tqdm_disable
+        )
+
+        # TODO Text process function can be applied in this step (.apply)
+        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
+                            .apply(" ".join, axis=1) \
+                            .apply(self._tokenize_entity) \
+                            .values.tolist()
+                        # if attributes_1 else data.entities_d1.apply(self._tokenize_entity)
+
+        self._all_tokens = set(itertools.chain.from_iterable(self._entities_d1))
+
+        if not data.is_dirty_er:
+            self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
+                    .apply(" ".join, axis=1) \
+                    .apply(self._tokenize_entity) \
+                    .values.tolist()
+            self._all_tokens.union(set(itertools.chain.from_iterable(self._entities_d2)))
+
+        entity_id = itertools.count()
+        blocks = {}
+        
+        for entity in self._entities_d1:
+            eid = next(entity_id)
+            for token in entity:
+                blocks.setdefault(token, Block())
+                blocks[token].entities_D1.add(eid)
+            self._progress_bar.update(1)
+
+        if not data.is_dirty_er:
+            for entity in self._entities_d2:
+                eid = next(entity_id)
+                for token in entity:
+                    blocks.setdefault(token, Block())
+                    blocks[token].entities_D2.add(eid)
+                self._progress_bar.update(1)
+
+        self.original_num_of_blocks = len(blocks)
+        self.blocks = self._clean_blocks(blocks)
+        self.num_of_blocks_dropped = len(blocks) - len(self.blocks)
+        self.execution_time = time.time() - _start_time
+        self._progress_bar.close()
+
+        return self.blocks
+
+    def report(self) -> None:
+        """Prints Block Building method configuration
+        """
+        print(
+            "Method name: " + self._method_name +
+            "\nMethod info: " + self._method_info +
+            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
+            "Attributes from D1:\n\t" + ', '.join(c for c in (self.attributes_1 if self.attributes_1 is not None \
+                else self.data.dataset_1.columns)) +
+            ("\nAttributes from D2:\n\t" + ', '.join(c for c in (self.attributes_2 if self.attributes_2 is not None \
+                else self.data.dataset_2.columns)) if not self.data.is_dirty_er else "") +
+            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
+        )
+
+    @abstractmethod
+    def _clean_blocks(self, blocks: dict) -> dict:
+        pass
+
+    @abstractmethod
+    def _configuration(self) -> dict:
+        pass
+    
+class StandardBlocking(AbstractBlockBuilding):
+    """ Creates one block for every token in \
+        the attribute values of at least two entities.
+    """
+
+    _method_name = "Standard Blocking"
+    _method_short_name: str = "SB"
+    _method_info = "Creates one block for every token in " + \
+        "the attribute values of at least two entities."
+
+    def __init__(self) -> any:
+        super().__init__()
+
+    def _tokenize_entity(self, entity: str) -> list:
+        """Produces a list of workds of a given string
+
+        Args:
+            entity (str): String representation  of an entity
+
+        Returns:
+            list: List of words
+        """
+        return list(set(filter(None, re.split('[\\W_]', entity.lower()))))
+
+    def _clean_blocks(self, blocks: dict) -> dict:
+        """No cleaning"""
+        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
+
+    def _configuration(self) -> dict:
+        """No configuration"""
+        return {}
+
+class QGramsBlocking(StandardBlocking):
+    """ Creates one block for every q-gram that is extracted \
+        from any token in the attribute values of any entity. \
+            The q-gram must be shared by at least two entities.
+    """
+
+    _method_name = "Q-Grams Blocking"
+    _method_short_name: str = "QGB"
+    _method_info = "Creates one block for every q-gram that is extracted " + \
+                    "from any token in the attribute values of any entity. " + \
+                    "The q-gram must be shared by at least two entities."
+
+    def __init__(
+            self, qgrams: int = 6
+    ) -> any:
+        super().__init__()
+        self.qgrams = qgrams
+
+    def _tokenize_entity(self, entity) -> set:
+        keys = set()
+        for token in super()._tokenize_entity(entity):
+            if len(token) < self.qgrams:
+                keys.add(token)
+            else:
+                keys.update(''.join(qg) for qg in nltk.ngrams(token, n=self.qgrams))
+        return keys
+
+    def _clean_blocks(self, blocks: dict) -> dict:
+        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
+
+    def _configuration(self) -> dict:
+        return {
+            "Q-Gramms" : self.qgrams
+        }
+
+class SuffixArraysBlocking(StandardBlocking):
+    """ It creates one block for every suffix that appears \
+        in the attribute value tokens of at least two entities.
+    """
+
+    _method_name = "Suffix Arrays Blocking"
+    _method_short_name: str = "SAB"
+    _method_info = "Creates one block for every suffix that appears in the " + \
+        "attribute value tokens of at least two entities."
+
+    def __init__(
+            self,
+            suffix_length: int = 6,
+            max_block_size: int = 53
+    ) -> any:
+        super().__init__()
+        self.suffix_length, self.max_block_size = suffix_length, max_block_size
+
+    def _tokenize_entity(self, entity) -> set:
+        keys = set()
+        for token in super()._tokenize_entity(entity):
+            if len(token) < self.suffix_length:
+                keys.add(token)
+            else:
+                for length in range(0, len(token) - self.suffix_length + 1):
+                    keys.add(token[length:])
+        return keys
+
+    def _clean_blocks(self, blocks: dict) -> dict:
+        return drop_big_blocks_by_size(blocks, self.max_block_size, self.data.is_dirty_er)
+
+    def _configuration(self) -> dict:
+        return {
+            "Suffix length" : self.suffix_length,
+            "Maximum Block Size" : self.max_block_size
+        }
+
+class ExtendedSuffixArraysBlocking(StandardBlocking):
+    """ It creates one block for every substring \
+        (not just suffix) that appears in the tokens of at least two entities.
+    """
+
+    _method_name = "Extended Suffix Arrays Blocking"
+    _method_short_name: str = "ESAB"
+    _method_info = "Creates one block for every substring (not just suffix) " + \
+        "that appears in the tokens of at least two entities."
+
+    def __init__(
+            self,
+            suffix_length: int = 6,
+            max_block_size: int = 39
+    ) -> any:
+        super().__init__()
+        self.suffix_length, self.max_block_size = suffix_length, max_block_size
+
+    def _tokenize_entity(self, entity) -> set:
+        keys = set()
+        for token in super()._tokenize_entity(entity):
+            keys.add(token)
+            if len(token) > self.suffix_length:
+                for current_size in range(self.suffix_length, len(token)): 
+                    for letters in list(nltk.ngrams(token, n=current_size)):
+                        keys.add("".join(letters))
+        return keys
+
+    def _clean_blocks(self, blocks: dict) -> dict:
+        return drop_big_blocks_by_size(blocks, self.max_block_size, self.data.is_dirty_er)
+
+    def _configuration(self) -> dict:
+        return {
+            "Suffix length" : self.suffix_length,
+            "Maximum Block Size" : self.max_block_size
+        }
+
+class ExtendedQGramsBlocking(StandardBlocking):
+    """It creates one block for every combination of q-grams that represents at least two entities.
+    The q-grams are extracted from any token in the attribute values of any entity.
+    """
+
+    _method_name = "Extended QGramsBlocking"
+    _method_short_name: str = "EQGB"
+    _method_info = "Creates one block for every substring (not just suffix) " + \
+        "that appears in the tokens of at least two entities."
+
+    def __init__(
+            self,
+            qgrams: int = 6,
+            threshold: float = 0.95
+    ) -> any:
+        super().__init__()
+        self.threshold: float = threshold
+        self.MAX_QGRAMS: int = 15
+        self.qgrams = qgrams
+
+    def _tokenize_entity(self, entity) -> set:
+        keys = set()
+        for token in super()._tokenize_entity(entity):
+            if len(token) < self.qgrams:
+                keys.add(token)
+            else:   
+                qgrams = [''.join(qgram) for qgram in nltk.ngrams(token, n=self.qgrams)]
+                if len(qgrams) == 1:
+                    keys.update(qgrams)
+                else:
+                    if len(qgrams) > self.MAX_QGRAMS:
+                        qgrams = qgrams[:self.MAX_QGRAMS]
+
+                    minimum_length = max(1, math.floor(len(qgrams) * self.threshold))
+                    for i in range(minimum_length, len(qgrams) + 1):
+                        keys.update(self._qgrams_combinations(qgrams, i))
+
+        return keys
+
+    def _qgrams_combinations(self, sublists: list, sublist_length: int) -> list:
+        if sublist_length == 0 or len(sublists) < sublist_length:
+            return []
+
+        remaining_elements = sublists.copy()
+        last_sublist = remaining_elements.pop(len(sublists)-1)
+
+        combinations_exclusive_x = self._qgrams_combinations(remaining_elements, sublist_length)
+        combinations_inclusive_x = self._qgrams_combinations(remaining_elements, sublist_length-1)
+
+        resulting_combinations = combinations_exclusive_x.copy() if combinations_exclusive_x else []
+
+        if not combinations_inclusive_x: # is empty
+            resulting_combinations.append(last_sublist)
+        else:
+            for combination in combinations_inclusive_x:
+                resulting_combinations.append(combination+last_sublist)
+
+        return resulting_combinations
+
+    def _clean_blocks(self, blocks: dict) -> dict:
+        return drop_single_entity_blocks(blocks, self.data.is_dirty_er)
+
+    def _configuration(self) -> dict:
+        return {
+            "Q-Gramms" : self.qgrams,
+            "Threshold" : self.threshold
+        }
```

### Comparing `pyjedai-0.0.6/src/pyjedai/block_cleaning.py` & `pyjedai-0.0.7/src/pyjedai/block_cleaning.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,210 +1,209 @@
-"""Block Cleaning Module
-Contains:
- - BlockFiltering
- - BlockPurging
-"""
-from abc import ABC
-from collections import defaultdict
-from time import time
-from typing import Tuple
-
-import numpy as np
-from tqdm.autonotebook import tqdm
-
-from .block_building import AbstractBlockProcessing
-from .datamodel import Block, Data
-from .utils import create_entity_index, drop_single_entity_blocks
-
-class AbstractBlockCleaning(AbstractBlockProcessing):
-
-    def __init__(self) -> None:
-        super().__init__()
-
-    def report(self) -> None:
-        """Prints Block Building method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            "\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) +
-            "Runtime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-class BlockFiltering(AbstractBlockCleaning):
-    """Retains every entity in a subset of its smallest blocks.
-
-        Filtering consists of 3 steps:
-        - Blocks sort in ascending cardinality
-        - Creation of Entity Index: inversed block dictionary
-        - Retain every entity in ratio % of its smallest blocks
-        - Blocks reconstruction
-    """
-
-    _method_name = "Block Filtering"
-    _method_short_name: str = "BF"
-    _method_info = "Retains every entity in a subset of its smallest blocks."
-
-    def __init__(self, ratio: float = 0.8) -> None:
-        super().__init__()
-        if ratio > 1.0 or ratio < 0.0:
-            raise AttributeError("Ratio is a number between 0.0 and 1.0")
-        else:
-            self.ratio = ratio
-        self.entity_index: dict
-
-    def __str__(self) -> str:
-        print(self._method_name + self._method_info)
-        print("Ratio: ", self.ratio)
-        return super().__str__()
-
-    def process(
-            self,
-            blocks: dict,
-            data: Data,
-            tqdm_disable: bool = False
-    ) -> Tuple[dict, dict]:
-        """Main method of Block Filtering.
-
-        Args:
-            blocks (dict): dict of keys to Blocks.
-            data (Data): input dataset.
-            tqdm_disable (bool, optional): disable progress bars. Defaults to False.
-
-        Returns:
-            Tuple[dict, dict]: dict of keys to Blocks, entity index (reversed blocks)
-        """
-        start_time, self.tqdm_disable, self.data = time(), tqdm_disable, data
-        self._progress_bar = tqdm(
-            total=3,
-            desc=self._method_name,
-            disable=self.tqdm_disable
-        )
-        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
-        self._progress_bar.update(1)
-        entity_index = create_entity_index(sorted_blocks, self.data.is_dirty_er)
-        self._progress_bar.update(1)
-        filtered_blocks = {}
-        for entity_id, block_keys in entity_index.items():
-            # Create new blocks from the entity index
-            # print(list(block_keys[:int(round(self.ratio*len(block_keys)))]))
-            block_keys = list(block_keys)
-            for key in list(block_keys[:int(round(self.ratio*len(block_keys)))]):
-                filtered_blocks.setdefault(key, Block())
-                # Entities ids start to 0 ... n-1 for 1st dataset
-                # and n ... m for 2nd dataset
-                _ = filtered_blocks[key].entities_D1.add(entity_id) if entity_id < self.data.dataset_limit \
-                    else filtered_blocks[key].entities_D2.add(entity_id)
-        self._progress_bar.update(1)
-        new_blocks = drop_single_entity_blocks(filtered_blocks, self.data.is_dirty_er)
-        self._progress_bar.close()
-        self.execution_time = time() - start_time
-        self.blocks = new_blocks
-        
-        return new_blocks
-
-    def _configuration(self) -> dict:
-        return {
-            "Ratio" : self.ratio
-        }
-
-
-class BlockPurging(AbstractBlockCleaning):
-    """Discards the blocks exceeding a certain number of comparisons.
-    """
-
-    _method_name = "Block Purging"
-    _method_short_name: str = "BP"
-    _method_info = "Discards the blocks exceeding a certain number of comparisons."
-
-    def __init__(self, smoothing_factor: float = 1.025) -> any:
-        super().__init__()
-        self.smoothing_factor: float = smoothing_factor
-        self.max_comparisons_per_block: float
-
-    def process(
-            self,
-            blocks: dict,
-            data: Data,
-            tqdm_disable: bool = False
-    ) -> dict:
-        """Main method of Block Purging.
-
-        Args:
-            blocks (dict): Blocks of entities.
-            data (Data): Data module. Contains all the information about the dataset.
-            tqdm_disable (bool, optional): Disable progress bar. Defaults to False.
-
-        Returns:
-            dict: Purged blocks.
-        """
-        self.tqdm_disable, self.data, start_time = tqdm_disable, data, time()
-        if not blocks:
-            raise AttributeError("Empty dict of blocks was given as input!")
-        else:
-            new_blocks = blocks.copy()
-        self._progress_bar = tqdm(total=2*len(new_blocks), desc=self._method_name, disable=self.tqdm_disable)            
-        self._set_threshold(new_blocks)
-        new_blocks = dict(filter(self._cardinality_threshold, blocks.items()))
-        self._progress_bar.close()
-        self.execution_time = time() - start_time
-        self.blocks = new_blocks
-
-        return new_blocks
-
-    def _cardinality_threshold(self, id_block_tuple) -> bool:
-        self._progress_bar.update(1)
-        return id_block_tuple[1].get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
-
-    def _set_threshold(self, blocks: dict) -> None:
-        """Calculates the maximum number of comparisons per block, so in the next step to be purged.
-
-        Args:
-            blocks (dict): _description_
-        """
-        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
-        distinct_comparisons_level = set(b.get_cardinality(self.data.is_dirty_er) \
-                                        for _, b in sorted_blocks.items())
-        block_assignments = np.empty([len(distinct_comparisons_level)])
-        comparisons_level = np.empty([len(distinct_comparisons_level)])
-        total_comparisons_per_level = np.empty([len(distinct_comparisons_level)])
-        index = -1
-        for _, block in sorted_blocks.items():
-            if index == -1:
-                index += 1
-                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
-                block_assignments[index] = 0
-                total_comparisons_per_level[index] = 0
-            elif block.get_cardinality(self.data.is_dirty_er) != comparisons_level[index]:
-                index += 1
-                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
-                block_assignments[index] = block_assignments[index-1]
-                total_comparisons_per_level[index] = total_comparisons_per_level[index-1]
-
-            block_assignments[index] += block.get_size()
-            total_comparisons_per_level[index] += block.get_cardinality(self.data.is_dirty_er)
-            self._progress_bar.update(1)
-
-        current_bc = current_cc = current_size = \
-            previous_bc = previous_cc = previous_size = 0
-        for i in range(len(block_assignments)-1, 0, -1):
-            previous_size = current_size
-            previous_bc = current_bc
-            previous_cc = current_cc
-            current_size = comparisons_level[i]
-            current_bc = block_assignments[i]
-            current_cc = total_comparisons_per_level[i]
-            if current_bc * previous_cc < self.smoothing_factor * current_cc * previous_bc:
-                break
-        self.max_comparisons_per_block = previous_size
-
-    def _satisfies_threshold(self, block: Block) -> bool:
-        return block.get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
-
-    def _configuration(self) -> dict:
-        return {
-            "Smoothing factor" : self.smoothing_factor,
-            "Max Comparisons per Block" : self.max_comparisons_per_block
-        }
-
-def _sort_blocks_cardinality(blocks: dict, is_dirty_er: bool) -> dict:
-    return dict(sorted(blocks.items(), key=lambda x: x[1].get_cardinality(is_dirty_er)))
+"""Block Cleaning Module
+Contains:
+ - BlockFiltering
+ - BlockPurging
+"""
+from abc import ABC
+from collections import defaultdict
+from time import time
+from typing import Tuple
+
+import numpy as np
+from tqdm.autonotebook import tqdm
+
+from .block_building import AbstractBlockProcessing
+from .datamodel import Block, Data
+from .utils import create_entity_index, drop_single_entity_blocks, java_math_round
+
+class AbstractBlockCleaning(AbstractBlockProcessing):
+
+    def __init__(self) -> None:
+        super().__init__()
+
+    def report(self) -> None:
+        """Prints Block Building method configuration
+        """
+        print(
+            "Method name: " + self._method_name +
+            "\nMethod info: " + self._method_info +
+            "\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) +
+            "Runtime: {:2.4f} seconds".format(self.execution_time)
+        )
+
+class BlockFiltering(AbstractBlockCleaning):
+    """Retains every entity in a subset of its smallest blocks.
+
+        Filtering consists of 3 steps:
+        - Blocks sort in ascending cardinality
+        - Creation of Entity Index: inversed block dictionary
+        - Retain every entity in ratio % of its smallest blocks
+        - Blocks reconstruction
+    """
+
+    _method_name = "Block Filtering"
+    _method_short_name: str = "BF"
+    _method_info = "Retains every entity in a subset of its smallest blocks."
+
+    def __init__(self, ratio: float = 0.8) -> None:
+        super().__init__()
+        if ratio > 1.0 or ratio < 0.0:
+            raise AttributeError("Ratio is a number between 0.0 and 1.0")
+        else:
+            self.ratio = ratio
+        self.entity_index: dict
+
+    def __str__(self) -> str:
+        print(self._method_name + self._method_info)
+        print("Ratio: ", self.ratio)
+        return super().__str__()
+
+    def process(
+            self,
+            blocks: dict,
+            data: Data,
+            tqdm_disable: bool = False
+    ) -> Tuple[dict, dict]:
+        """Main method of Block Filtering.
+
+        Args:
+            blocks (dict): dict of keys to Blocks.
+            data (Data): input dataset.
+            tqdm_disable (bool, optional): disable progress bars. Defaults to False.
+
+        Returns:
+            Tuple[dict, dict]: dict of keys to Blocks, entity index (reversed blocks)
+        """
+        start_time, self.tqdm_disable, self.data = time(), tqdm_disable, data
+        self._progress_bar = tqdm(
+            total=3,
+            desc=self._method_name,
+            disable=self.tqdm_disable
+        )
+        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
+        self._progress_bar.update(1)
+        self.entity_index = create_entity_index(sorted_blocks, self.data.is_dirty_er)
+        self._progress_bar.update(1)
+        filtered_blocks = {}
+        for entity_id, block_keys in self.entity_index.items():
+            # Create new blocks from the entity index
+            block_keys = list(block_keys)
+            for key in list(block_keys[:java_math_round(self.ratio*float(len(block_keys)))]):
+                filtered_blocks.setdefault(key, Block())
+                # Entities ids start to 0 ... n-1 for 1st dataset
+                # and n ... m for 2nd dataset
+                _ = filtered_blocks[key].entities_D1.add(entity_id) if entity_id < self.data.dataset_limit \
+                    else filtered_blocks[key].entities_D2.add(entity_id)
+        self._progress_bar.update(1)
+        new_blocks = drop_single_entity_blocks(filtered_blocks, self.data.is_dirty_er)
+        self._progress_bar.close()
+        self.num_of_blocks_dropped = len(blocks) - len(new_blocks)
+        self.execution_time = time() - start_time
+        self.blocks = new_blocks
+
+        return self.blocks
+
+    def _configuration(self) -> dict:
+        return {
+            "Ratio" : self.ratio
+        }
+
+class BlockPurging(AbstractBlockCleaning):
+    """Discards the blocks exceeding a certain number of comparisons.
+    """
+
+    _method_name = "Block Purging"
+    _method_short_name: str = "BP"
+    _method_info = "Discards the blocks exceeding a certain number of comparisons."
+
+    def __init__(self, smoothing_factor: float = 1.025) -> any:
+        super().__init__()
+        self.smoothing_factor: float = smoothing_factor
+        self.max_comparisons_per_block: float
+
+    def process(
+            self,
+            blocks: dict,
+            data: Data,
+            tqdm_disable: bool = False
+    ) -> dict:
+        """Main method of Block Purging.
+
+        Args:
+            blocks (dict): Blocks of entities.
+            data (Data): Data module. Contains all the information about the dataset.
+            tqdm_disable (bool, optional): Disable progress bar. Defaults to False.
+
+        Returns:
+            dict: Purged blocks.
+        """
+        self.tqdm_disable, self.data, start_time = tqdm_disable, data, time()
+        if not blocks:
+            raise AttributeError("Empty dict of blocks was given as input!")
+        else:
+            new_blocks = blocks.copy()
+        self._progress_bar = tqdm(total=2*len(new_blocks), desc=self._method_name, disable=self.tqdm_disable)            
+        self._set_threshold(new_blocks)
+        new_blocks = dict(filter(self._cardinality_threshold, blocks.items()))
+        self._progress_bar.close()
+        self.execution_time = time() - start_time
+        self.blocks = new_blocks
+
+        return new_blocks
+
+    def _cardinality_threshold(self, id_block_tuple) -> bool:
+        self._progress_bar.update(1)
+        return id_block_tuple[1].get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
+
+    def _set_threshold(self, blocks: dict) -> None:
+        """Calculates the maximum number of comparisons per block, so in the next step to be purged.
+
+        Args:
+            blocks (dict): _description_
+        """
+        sorted_blocks = _sort_blocks_cardinality(blocks, self.data.is_dirty_er)
+        distinct_comparisons_level = set(b.get_cardinality(self.data.is_dirty_er) \
+                                        for _, b in sorted_blocks.items())
+        block_assignments = np.empty([len(distinct_comparisons_level)])
+        comparisons_level = np.empty([len(distinct_comparisons_level)])
+        total_comparisons_per_level = np.empty([len(distinct_comparisons_level)])
+        index = -1
+        for _, block in sorted_blocks.items():
+            if index == -1:
+                index += 1
+                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
+                block_assignments[index] = 0
+                total_comparisons_per_level[index] = 0
+            elif block.get_cardinality(self.data.is_dirty_er) != comparisons_level[index]:
+                index += 1
+                comparisons_level[index] = block.get_cardinality(self.data.is_dirty_er)
+                block_assignments[index] = block_assignments[index-1]
+                total_comparisons_per_level[index] = total_comparisons_per_level[index-1]
+
+            block_assignments[index] += block.get_size()
+            total_comparisons_per_level[index] += block.get_cardinality(self.data.is_dirty_er)
+            self._progress_bar.update(1)
+
+        current_bc = current_cc = current_size = \
+            previous_bc = previous_cc = previous_size = 0
+        for i in range(len(block_assignments)-1, 0, -1):
+            previous_size = current_size
+            previous_bc = current_bc
+            previous_cc = current_cc
+            current_size = comparisons_level[i]
+            current_bc = block_assignments[i]
+            current_cc = total_comparisons_per_level[i]
+            if current_bc * previous_cc < self.smoothing_factor * current_cc * previous_bc:
+                break
+        self.max_comparisons_per_block = previous_size
+
+    def _satisfies_threshold(self, block: Block) -> bool:
+        return block.get_cardinality(self.data.is_dirty_er) <= self.max_comparisons_per_block
+
+    def _configuration(self) -> dict:
+        return {
+            "Smoothing factor" : self.smoothing_factor,
+            "Max Comparisons per Block" : self.max_comparisons_per_block
+        }
+
+def _sort_blocks_cardinality(blocks: dict, is_dirty_er: bool) -> dict:
+    return dict(sorted(blocks.items(), key=lambda x: x[1].get_cardinality(is_dirty_er)))
```

### Comparing `pyjedai-0.0.6/src/pyjedai/clustering.py` & `pyjedai-0.0.7/src/pyjedai/clustering.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,190 +1,190 @@
-from queue import PriorityQueue
-from time import time
-
-from networkx import Graph, connected_components
-from tqdm.autonotebook import tqdm
-
-from .datamodel import Data, PYJEDAIFeature
-from .evaluation import Evaluation
-from .utils import are_matching
-
-
-class AbstractClustering(PYJEDAIFeature):
-    
-    def __init__(self) -> None:
-        super().__init__()
-        self.data: Data
-        self.similarity_threshold: float = 0.1
-        
-    def evaluate(self,
-                 prediction,
-                 export_to_df: bool = False,
-                 export_to_dict: bool = False,
-                 with_classification_report: bool = False,
-                 verbose: bool = True) -> any:
-
-        if prediction is None:
-            if self.blocks is None:
-                raise AttributeError("Can not proceed to evaluation without build_blocks.")
-            else:
-                eval_blocks = self.blocks
-        else:
-            eval_blocks = prediction
-            
-        if self.data is None:
-            raise AttributeError("Can not proceed to evaluation without data object.")
-
-        if self.data.ground_truth is None:
-            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " + 
-                    "Data object has not been initialized with the ground-truth file")
-
-        eval_obj = Evaluation(self.data)
-        true_positives = 0
-        entity_index = eval_obj._create_entity_index_from_clusters(eval_blocks)
-        for _, (id1, id2) in self.data.ground_truth.iterrows():
-            id1 = self.data._ids_mapping_1[id1]
-            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
-            if id1 in entity_index and    \
-                id2 in entity_index and are_matching(entity_index, id1, id2):
-                true_positives += 1
-        # print(entity_index)
-        eval_obj.calculate_scores(true_positives=true_positives)
-        return eval_obj.report(self.method_configuration(),
-                                export_to_df,
-                                export_to_dict,
-                                with_classification_report,
-                                verbose)
-    
-    def stats(self) -> None:
-        pass
-
-class ConnectedComponentsClustering(AbstractClustering):
-    """Creates the connected components of the graph. \
-        Applied to graph created from entity matching. \
-        Input graph consists of the entity ids (nodes) and the similarity scores (edges).
-    """
-
-    _method_name: str = "Connected Components Clustering"
-    _method_short_name: str = "CCC"
-    _method_info: str = "Gets equivalence clusters from the " + \
-                    "transitive closure of the similarity graph."
-
-    def __init__(self) -> None:
-        super().__init__()
-        self.similarity_threshold: float
-
-    def process(self, graph: Graph, data: Data, similarity_threshold: float = None) -> list:
-        """NetworkX Connected Components Algorithm in the produced graph.
-
-        Args:
-            graph (Graph): Consists of the entity ids (nodes) and the similarity scores (edges).
-
-        Returns:
-            list: list of clusters
-        """
-        start_time = time()
-        self.data = data
-        self.similarity_threshold: float = similarity_threshold
-        graph_copy = graph.copy()
-        if self.similarity_threshold is not None:
-            for x in graph.edges(data=True):
-                if x[2]['weight'] < self.similarity_threshold:
-                    graph_copy.remove_edge(x[0], x[1])
-        clusters = list(connected_components(graph_copy))
-        # print(clusters)
-        # print("Number of clusters: ", len(clusters))
-        resulting_clusters = list(filter(lambda x: len(x) == 2, clusters)) \
-                                if not data.is_dirty_er else clusters
-        # print("Number of clusters after filtering: ", len(resulting_clusters))
-        self.execution_time = time() - start_time
-        return resulting_clusters
-
-    def _configuration(self) -> dict:
-        return {}
-
-class UniqueMappingClustering(AbstractClustering):
-    """Prunes all edges with a weight lower than t, sorts the remaining ones in
-        decreasing weight/similarity and iteratively forms a partition for
-        the top-weighted pair as long as none of its entities has already
-        been matched to some other.
-    """
-
-    _method_name: str = "Unique Mapping Clustering"
-    _method_short_name: str = "UMC"
-    _method_info: str = "Prunes all edges with a weight lower than t, sorts the remaining ones in" + \
-                        "decreasing weight/similarity and iteratively forms a partition for" + \
-                        "the top-weighted pair as long as none of its entities has already" + \
-                        "been matched to some other."
-
-    def __init__(self) -> None:
-        """Unique Mapping Clustering Constructor
-
-        Args:
-            similarity_threshold (float, optional): Prunes all edges with a weight
-                lower than this. Defaults to 0.1.
-            data (Data): Dataset module.
-        """
-        super().__init__()
-        self.similarity_threshold: float
-
-    def process(self, graph: Graph, data: Data, similarity_threshold: float = 0.1) -> list:
-        """NetworkX Connected Components Algorithm in the produced graph.
-
-        Args:
-            graph (Graph): Consists of the entity ids (nodes) and the similarity scores (edges).
-
-        Returns:
-            list: list of clusters
-        """
-        if data.is_dirty_er:
-            raise AttributeError("Unique Mapping Clustering can only be performed in Clean-Clean Entity Resolution.")
-        self.similarity_threshold: float = similarity_threshold
-        
-        start_time = time()
-        matched_entities = set()
-        self.data = data
-        new_graph = Graph()
-        priority_queue = PriorityQueue(maxsize = graph.number_of_edges()*2)
-        for x in graph.edges(data=True):
-            if x[2]['weight'] > self.similarity_threshold:
-                priority_queue.put_nowait((1- x[2]['weight'], x[0], x[1]))
-
-        while not priority_queue.empty():
-            sim, entity_1, entity_2 = priority_queue.get()
-            if entity_1 in matched_entities or entity_2 in matched_entities:
-                continue
-            new_graph.add_edge(entity_1, entity_2, weight=sim)
-            matched_entities.add(entity_1)
-            matched_entities.add(entity_2)
-
-        clusters = ConnectedComponentsClustering().process(new_graph, data, similarity_threshold=None)
-        self.execution_time = time() - start_time
-        return clusters
-
-    def _configuration(self) -> dict:
-        return {}
-
-class ExactClustering(AbstractClustering):
-    """Implements an adapted, simplified version of the Exact THRESHOLD algorithm,
-        introduced in "Similarity Flooding: A Versatile Graph Matching Algorithm and Its Application to Schema Matching",
-        also referred in "BIGMAT: A Distributed Affinity-Preserving Random Walk Strategy for Instance Matching on Knowledge Graphs".
-        In essence, it keeps the top-1 candidate per entity, as long as the candidate also considers this node as its top candidate.
-    """
-
-    _method_name: str = "Exact Clustering"
-    _method_short_name: str = "EC"
-    _method_info: str = "Ιmplements an adapted, simplified version of the Exact THRESHOLD algorithm," + \
-        "In essence, it keeps the top-1 candidate per entity, as long as the candidate also considers this node as its top candidate."
-
-    def __init__(self, similarity_threshold: float = 0.1) -> None:
-        """"""
-        super().__init__()
-        self.similarity_threshold = similarity_threshold
-
-    def process(self, graph: Graph, data: Data) -> list:
-        """
-        """
-        raise NotImplementedError("Exact Clustering is not implemented yet.")
-
-    def _configuration(self) -> dict:
-        return {}
+from queue import PriorityQueue
+from time import time
+
+from networkx import Graph, connected_components
+from tqdm.autonotebook import tqdm
+
+from .datamodel import Data, PYJEDAIFeature
+from .evaluation import Evaluation
+from .utils import are_matching
+
+
+class AbstractClustering(PYJEDAIFeature):
+    
+    def __init__(self) -> None:
+        super().__init__()
+        self.data: Data
+        self.similarity_threshold: float = 0.1
+        
+    def evaluate(self,
+                 prediction,
+                 export_to_df: bool = False,
+                 export_to_dict: bool = False,
+                 with_classification_report: bool = False,
+                 verbose: bool = True) -> any:
+
+        if prediction is None:
+            if self.blocks is None:
+                raise AttributeError("Can not proceed to evaluation without build_blocks.")
+            else:
+                eval_blocks = self.blocks
+        else:
+            eval_blocks = prediction
+            
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " + 
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        entity_index = eval_obj._create_entity_index_from_clusters(eval_blocks)
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
+            if id1 in entity_index and    \
+                id2 in entity_index and are_matching(entity_index, id1, id2):
+                true_positives += 1
+        # print(entity_index)
+        eval_obj.calculate_scores(true_positives=true_positives)
+        return eval_obj.report(self.method_configuration(),
+                                export_to_df,
+                                export_to_dict,
+                                with_classification_report,
+                                verbose)
+    
+    def stats(self) -> None:
+        pass
+
+class ConnectedComponentsClustering(AbstractClustering):
+    """Creates the connected components of the graph. \
+        Applied to graph created from entity matching. \
+        Input graph consists of the entity ids (nodes) and the similarity scores (edges).
+    """
+
+    _method_name: str = "Connected Components Clustering"
+    _method_short_name: str = "CCC"
+    _method_info: str = "Gets equivalence clusters from the " + \
+                    "transitive closure of the similarity graph."
+
+    def __init__(self) -> None:
+        super().__init__()
+        self.similarity_threshold: float
+
+    def process(self, graph: Graph, data: Data, similarity_threshold: float = None) -> list:
+        """NetworkX Connected Components Algorithm in the produced graph.
+
+        Args:
+            graph (Graph): Consists of the entity ids (nodes) and the similarity scores (edges).
+
+        Returns:
+            list: list of clusters
+        """
+        start_time = time()
+        self.data = data
+        self.similarity_threshold: float = similarity_threshold
+        graph_copy = graph.copy()
+        if self.similarity_threshold is not None:
+            for x in graph.edges(data=True):
+                if x[2]['weight'] < self.similarity_threshold:
+                    graph_copy.remove_edge(x[0], x[1])
+        clusters = list(connected_components(graph_copy))
+        # print(clusters)
+        # print("Number of clusters: ", len(clusters))
+        resulting_clusters = list(filter(lambda x: len(x) == 2, clusters)) \
+                                if not data.is_dirty_er else clusters
+        # print("Number of clusters after filtering: ", len(resulting_clusters))
+        self.execution_time = time() - start_time
+        return resulting_clusters
+
+    def _configuration(self) -> dict:
+        return {}
+
+class UniqueMappingClustering(AbstractClustering):
+    """Prunes all edges with a weight lower than t, sorts the remaining ones in
+        decreasing weight/similarity and iteratively forms a partition for
+        the top-weighted pair as long as none of its entities has already
+        been matched to some other.
+    """
+
+    _method_name: str = "Unique Mapping Clustering"
+    _method_short_name: str = "UMC"
+    _method_info: str = "Prunes all edges with a weight lower than t, sorts the remaining ones in" + \
+                        "decreasing weight/similarity and iteratively forms a partition for" + \
+                        "the top-weighted pair as long as none of its entities has already" + \
+                        "been matched to some other."
+
+    def __init__(self) -> None:
+        """Unique Mapping Clustering Constructor
+
+        Args:
+            similarity_threshold (float, optional): Prunes all edges with a weight
+                lower than this. Defaults to 0.1.
+            data (Data): Dataset module.
+        """
+        super().__init__()
+        self.similarity_threshold: float
+
+    def process(self, graph: Graph, data: Data, similarity_threshold: float = 0.1) -> list:
+        """NetworkX Connected Components Algorithm in the produced graph.
+
+        Args:
+            graph (Graph): Consists of the entity ids (nodes) and the similarity scores (edges).
+
+        Returns:
+            list: list of clusters
+        """
+        if data.is_dirty_er:
+            raise AttributeError("Unique Mapping Clustering can only be performed in Clean-Clean Entity Resolution.")
+        self.similarity_threshold: float = similarity_threshold
+        
+        start_time = time()
+        matched_entities = set()
+        self.data = data
+        new_graph = Graph()
+        priority_queue = PriorityQueue(maxsize = graph.number_of_edges()*2)
+        for x in graph.edges(data=True):
+            if x[2]['weight'] > self.similarity_threshold:
+                priority_queue.put_nowait((1- x[2]['weight'], x[0], x[1]))
+
+        while not priority_queue.empty():
+            sim, entity_1, entity_2 = priority_queue.get()
+            if entity_1 in matched_entities or entity_2 in matched_entities:
+                continue
+            new_graph.add_edge(entity_1, entity_2, weight=sim)
+            matched_entities.add(entity_1)
+            matched_entities.add(entity_2)
+
+        clusters = ConnectedComponentsClustering().process(new_graph, data, similarity_threshold=None)
+        self.execution_time = time() - start_time
+        return clusters
+
+    def _configuration(self) -> dict:
+        return {}
+
+class ExactClustering(AbstractClustering):
+    """Implements an adapted, simplified version of the Exact THRESHOLD algorithm,
+        introduced in "Similarity Flooding: A Versatile Graph Matching Algorithm and Its Application to Schema Matching",
+        also referred in "BIGMAT: A Distributed Affinity-Preserving Random Walk Strategy for Instance Matching on Knowledge Graphs".
+        In essence, it keeps the top-1 candidate per entity, as long as the candidate also considers this node as its top candidate.
+    """
+
+    _method_name: str = "Exact Clustering"
+    _method_short_name: str = "EC"
+    _method_info: str = "Ιmplements an adapted, simplified version of the Exact THRESHOLD algorithm," + \
+        "In essence, it keeps the top-1 candidate per entity, as long as the candidate also considers this node as its top candidate."
+
+    def __init__(self, similarity_threshold: float = 0.1) -> None:
+        """"""
+        super().__init__()
+        self.similarity_threshold = similarity_threshold
+
+    def process(self, graph: Graph, data: Data) -> list:
+        """
+        """
+        raise NotImplementedError("Exact Clustering is not implemented yet.")
+
+    def _configuration(self) -> dict:
+        return {}
```

### Comparing `pyjedai-0.0.6/src/pyjedai/joins.py` & `pyjedai-0.0.7/src/pyjedai/joins.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,359 +1,362 @@
-import itertools
-import math
-import re
-from collections import defaultdict
-from queue import PriorityQueue
-from time import time
-
-import networkx
-import nltk
-import numpy as np
-import pandas as pd
-import tqdm
-from tqdm.autonotebook import tqdm
-
-from .datamodel import Data, PYJEDAIFeature
-from .evaluation import Evaluation
-
-class AbstractJoin(PYJEDAIFeature):
-    """Abstract class of Joins module
-    """
-
-    def __init__(
-            self,
-            metric: str,
-            tokenization: str,
-            qgrams: int = 2,
-            similarity_threshold: float = None
-    ) -> None:
-        """AbstractJoin Constructor
-
-        Args:
-            metric (str): String similarity metric
-            tokenization (str): Tokenizer
-            qgrams (int, optional): For Jaccard metric. Defaults to 2.
-            similarity_threshold (float, optional): Threshold for preserving pair. Defaults to None.
-        """
-        self.metric = metric
-        self.qgrams = qgrams
-        self.tokenization = tokenization
-        self._source_frequency: np.array
-        self.similarity_threshold: float = similarity_threshold
-        self.reverse_order: bool
-        self.attributes_1: list
-        self.attributes_2: list
-        self._flags: np.array
-        self.pairs: networkx.Graph
-
-    def fit(self,
-            data: Data,
-            reverse_order: bool = False,
-            attributes_1: list = None,
-            attributes_2: list = None,
-            tqdm_disable: bool = False
-    ) -> networkx.Graph:
-        """Joins main method
-
-            Args:
-                data (Data): dataset module
-                reverse_order (bool, optional): _description_. Defaults to False.
-                attributes_1 (list, optional): _description_. Defaults to None.
-                attributes_2 (list, optional): _description_. Defaults to None.
-                tqdm_disable (bool, optional): _description_. Defaults to False.
-
-            Returns:
-                networkx.Graph: graph containg nodes as entities and edges as similarity score
-        """
-        if reverse_order and data.is_dirty_er:
-            raise ValueError("Can't have reverse order in Dirty Entity Resolution")
-
-        start_time = time()
-        self.tqdm_disable, self.reverse_order, self.attributes_1, self.attributes_2, self.data = \
-            tqdm_disable, reverse_order, attributes_1, attributes_2, data
-
-        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
-                            .apply(" ".join, axis=1) \
-                            .apply(self._tokenize_entity) \
-                            .values.tolist()
-
-        if not data.is_dirty_er:
-            self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
-                    .apply(" ".join, axis=1) \
-                    .apply(self._tokenize_entity) \
-                    .values.tolist()
-
-        num_of_entities = self.data.num_of_entities_2 if reverse_order else self.data.num_of_entities_1
-
-        self._progress_bar = tqdm(
-            total=self.data.num_of_entities if not self.data.is_dirty_er else num_of_entities*2,
-            desc=self._method_name+" ("+self.metric+")", disable=self.tqdm_disable
-        )
-
-        self._flags, \
-        self._counters, \
-        self._sims, \
-        self._source_frequency, \
-        self.pairs = np.empty([num_of_entities]), \
-                    np.zeros([num_of_entities]), \
-                    np.empty([self.data.num_of_entities_1*self.data.num_of_entities_2]), \
-                    np.empty([num_of_entities]), \
-                    networkx.Graph()
-        self._flags[:] = -1
-        entity_index = self._create_entity_index(
-                self._entities_d2 if reverse_order else self._entities_d1
-            )
-
-        if self.data.is_dirty_er:
-            eid = 0
-            for entity in self._entities_d1:
-                candidates = set()
-                for token in entity:
-                    if token in entity_index:
-                        current_candidates = entity_index[token]
-                        for candidate_id in current_candidates:
-                            if self._flags[candidate_id] != eid:
-                                self._counters[candidate_id] = 0
-                                self._flags[candidate_id] = eid
-                            self._counters[candidate_id] += 1
-                            candidates.add(candidate_id)
-                self._process_candidates(candidates, eid, len(entity))
-                self._progress_bar.update(1)
-                eid += 1
-        else:
-            if reverse_order:
-                entities = self._entities_d1
-                num_of_entities = self.data.num_of_entities_1
-            else:
-                entities = self._entities_d2
-                num_of_entities = self.data.num_of_entities_2
-
-            for i in range(0, num_of_entities):
-                candidates = set()
-                record = entities[i]
-                entity_id = i if reverse_order else i+self.data.dataset_limit
-                for token in record:
-                    if token in entity_index:
-                        current_candidates = entity_index[token]
-                        for candidate_id in current_candidates:
-                            if self._flags[candidate_id] != entity_id:
-                                self._counters[candidate_id] = 0
-                                self._flags[candidate_id] = entity_id
-                            self._counters[candidate_id] += 1
-                            candidates.add(candidate_id)
-                if 0 < len(candidates):
-                    self._process_candidates(candidates, entity_id, len(record))
-                self._progress_bar.update(1)
-        self._progress_bar.close()
-        self.execution_time = time() - start_time
-
-        return self.pairs
-
-    def _tokenize_entity(self, entity: str) -> set:
-        if self.tokenization == 'qgrams':
-            return set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)])
-        elif self.tokenization == 'standard':
-            return set(filter(None, re.split('[\\W_]', entity.lower())))
-        elif self.tokenization == 'standard_multiset':
-            tok_ids_index = {}
-            multiset = set()
-            for tok in set(filter(None, re.split('[\\W_]', entity.lower()))):
-                tok_id =  tok_ids_index[tok] if tok in tok_ids_index else 0
-                multiset.add(tok+str(tok_id))
-                tok_ids_index[tok] = tok_id+1
-            return multiset
-        elif self.tokenization == 'qgrams_multiset':
-            grams_ids_index = {}
-            qgrams = set()
-            for gram in set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)]):
-                gram_id =  grams_ids_index[gram] if gram in grams_ids_index else 0
-                qgrams.add(gram+str(gram_id))
-                grams_ids_index[gram] = gram_id+1
-            return qgrams
-        else:
-            raise AttributeError("Tokenization not found")
-
-    def _calc_similarity(
-            self,
-            common_tokens: int,
-            source_frequency: int,
-            tokens_size: int
-        ) -> float:
-        """Similarity score
-
-        Args:
-            common_tokens (int): number of common tokens
-            source_frequency (int): frequency
-            tokens_size (int): size of tokens
-
-        Returns:
-            float: similarity
-        """
-        if self.metric == 'cosine':
-            return common_tokens / math.sqrt(source_frequency*tokens_size)
-        elif self.metric == 'dice':
-            return 2 * common_tokens / (source_frequency+tokens_size)
-        elif self.metric == 'jaccard':
-            return common_tokens / (source_frequency+tokens_size-common_tokens)
-
-    def _create_entity_index(self, entities: list) -> dict:
-        entity_index = defaultdict(set)
-        entity_id = itertools.count()
-        for entity in entities:
-            eid = next(entity_id)
-            for token in entity:
-                entity_index[token].add(eid)
-            self._source_frequency[eid] = len(entity)
-            self._progress_bar.update(1)
-
-        return entity_index
-
-#     def _similarity(self, entity_id1: int, entity_id2: int, attributes: any=None) -> float:
-#         similarity: float = 0.0
-#         if isinstance(attributes, dict):
-#             for attribute, weight in self.attributes.items():
-#                 similarity += weight*self._metric(
-#                     self.data.entities.iloc[entity_id1][attribute],
-#                     self.data.entities.iloc[entity_id2][attribute]
-#                 )
-#         if isinstance(attributes, list):
-#             for attribute in self.attributes:
-#                 similarity += self._metric(
-#                     self.data.entities.iloc[entity_id1][attribute],
-#                     self.data.entities.iloc[entity_id2][attribute]
-#                 )
-#                 similarity /= len(self.attributes)
-#         else:
-#             # print(self.data.entities.iloc[entity_id1].str.cat(sep=' '),
-#                 # self.data.entities.iloc[entity_id2].str.cat(sep=' '))
-#             # concatenated row string
-#             similarity = self._metric(
-#                 self.data.entities.iloc[entity_id1].str.cat(sep=' '),
-#                 self.data.entities.iloc[entity_id2].str.cat(sep=' ')
-#             )
-#         return similarity
-
-    def _insert_to_graph(self, entity_id1, entity_id2, similarity):
-        if self.similarity_threshold <= similarity:
-            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
-
-    def evaluate(self, prediction=None, export_to_df: bool = False,
-                 export_to_dict: bool = False, with_classification_report: bool = False,
-                 verbose: bool = True) -> any:
-        if self.data is None:
-            raise AttributeError("Can not proceed to evaluation without data object.")
-
-        if self.data.ground_truth is None:
-            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
-                    "Data object has not been initialized with the ground-truth file")
-
-        eval_obj = Evaluation(self.data)
-        true_positives = 0
-        total_matching_pairs = prediction.number_of_edges()
-        for _, (id1, id2) in self.data.ground_truth.iterrows():
-            id1 = self.data._ids_mapping_1[id1]
-            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
-                                                else self.data._ids_mapping_2[id2]
-            if (id1 in prediction and id2 in prediction[id1]) or   \
-                 (id2 in prediction and id1 in prediction[id2]):
-                true_positives += 1
-
-        eval_obj.calculate_scores(true_positives=true_positives, 
-                                  total_matching_pairs=total_matching_pairs)
-        return eval_obj.report(self.method_configuration(),
-                        export_to_df,
-                        export_to_dict,
-                        with_classification_report,
-                        verbose)
-
-    def stats(self) -> None:
-        pass
-
-    def _configuration(self) -> dict:
-        return {
-            "similarity_threshold" : self.similarity_threshold,
-            "metric" : self.metric,
-            "tokenization" : self.tokenization,
-            "qgrams": self.qgrams
-        }    
-
-class ΕJoin(AbstractJoin):
-    """
-     Ε Join algorithm
-    """
-    _method_name = "EJoin"
-    _method_info = " ΕJoin algorithm"
-    _method_short_name = "EJ"
-
-    def __init__(
-        self,
-        similarity_threshold: float = 0.82,
-        metric: str = 'cosine',
-        tokenization: str = 'qgrams',
-        qgrams: int = 2
-    ) -> None:
-        super().__init__(metric, tokenization, qgrams, similarity_threshold)
-
-    def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
-        for candidate_id in candidates:
-            self._insert_to_graph(
-                candidate_id+self.data.dataset_limit if self.reverse_order \
-                                                        and not self.data.is_dirty_er \
-                                                    else candidate_id,
-                entity_id,
-                self._calc_similarity(
-                    self._counters[candidate_id],
-                    self._source_frequency[candidate_id],
-                    tokens_size
-                )
-            )
-
-class TopKJoin(AbstractJoin):
-    """Top-K Join algorithm
-    """
-
-    _method_name = "Top-K Join"
-    _method_info = "Top-K Join algorithm"
-    _method_short_name = "TopKJ"
-
-    def __init__(self,
-                 K: int,
-                 metric: str,
-                 tokenization: str,
-                 qgrams: int = 2
-        ) -> None:
-        super().__init__(metric, tokenization, qgrams)
-        self.K = K
-
-    def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
-        minimum_weight=0
-        pq = PriorityQueue()
-        for candidate_id in candidates:
-            sim = self._calc_similarity(
-                self._counters[candidate_id], self._source_frequency[candidate_id], tokens_size
-            )
-            if minimum_weight < sim:
-                pq.put(sim)
-                if self.K < pq.qsize():
-                    minimum_weight = pq.get()
-
-        minimum_weight = pq.get()
-        for candidate_id in candidates:
-            self.similarity_threshold = minimum_weight
-            self._insert_to_graph(
-                candidate_id + self.data.dataset_limit if self.reverse_order else candidate_id,
-                entity_id,
-                self._calc_similarity(
-                    self._counters[candidate_id], 
-                    self._source_frequency[candidate_id],
-                    tokens_size
-                )
-            )
-
-    def _configuration(self) -> dict:
-        return {
-            "similarity_threshold" : self.similarity_threshold,
-            "K" : self.K,
-            "metric" : self.metric,
-            "tokenization" : self.tokenization,
-            "qgrams": self.qgrams
-        }
+import itertools
+import math
+import re
+from collections import defaultdict
+from queue import PriorityQueue
+from time import time
+
+import networkx
+import nltk
+import numpy as np
+import pandas as pd
+import tqdm
+from tqdm.autonotebook import tqdm
+
+from .datamodel import Data, PYJEDAIFeature
+from .evaluation import Evaluation
+
+class AbstractJoin(PYJEDAIFeature):
+    """Abstract class of Joins module
+    """
+
+    def __init__(
+            self,
+            metric: str,
+            tokenization: str,
+            qgrams: int = 2,
+            similarity_threshold: float = None
+    ) -> None:
+        """AbstractJoin Constructor
+
+        Args:
+            metric (str): String similarity metric
+            tokenization (str): Tokenizer
+            qgrams (int, optional): For Jaccard metric. Defaults to 2.
+            similarity_threshold (float, optional): Threshold for preserving pair. Defaults to None.
+        """
+        self.metric = metric
+        self.qgrams = qgrams
+        self.tokenization = tokenization
+        self._source_frequency: np.array
+        self.similarity_threshold: float = similarity_threshold
+        self.reverse_order: bool
+        self.attributes_1: list
+        self.attributes_2: list
+        self._flags: np.array
+        self.pairs: networkx.Graph
+
+    def fit(self,
+            data: Data,
+            reverse_order: bool = False,
+            attributes_1: list = None,
+            attributes_2: list = None,
+            tqdm_disable: bool = False
+    ) -> networkx.Graph:
+        """Joins main method
+
+            Args:
+                data (Data): dataset module
+                reverse_order (bool, optional): _description_. Defaults to False.
+                attributes_1 (list, optional): _description_. Defaults to None.
+                attributes_2 (list, optional): _description_. Defaults to None.
+                tqdm_disable (bool, optional): _description_. Defaults to False.
+
+            Returns:
+                networkx.Graph: graph containg nodes as entities and edges as similarity score
+        """
+        if reverse_order and data.is_dirty_er:
+            raise ValueError("Can't have reverse order in Dirty Entity Resolution")
+
+        start_time = time()
+        self.tqdm_disable, self.reverse_order, self.attributes_1, self.attributes_2, self.data = \
+            tqdm_disable, reverse_order, attributes_1, attributes_2, data
+
+        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
+                            .apply(" ".join, axis=1) \
+                            .apply(self._tokenize_entity) \
+                            .values.tolist()
+
+        if not data.is_dirty_er:
+            self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
+                    .apply(" ".join, axis=1) \
+                    .apply(self._tokenize_entity) \
+                    .values.tolist()
+
+        num_of_entities = self.data.num_of_entities_2 if reverse_order else self.data.num_of_entities_1
+
+        self._progress_bar = tqdm(
+            total=self.data.num_of_entities if not self.data.is_dirty_er else num_of_entities*2,
+            desc=self._method_name+" ("+self.metric+")", disable=self.tqdm_disable
+        )
+
+        self._flags, \
+        self._counters, \
+        self._sims, \
+        self._source_frequency, \
+        self.pairs = np.empty([num_of_entities]), \
+                    np.zeros([num_of_entities]), \
+                    np.empty([self.data.num_of_entities_1*self.data.num_of_entities_2]), \
+                    np.empty([num_of_entities]), \
+                    networkx.Graph()
+        self._flags[:] = -1
+        entity_index = self._create_entity_index(
+                self._entities_d2 if reverse_order else self._entities_d1
+            )
+
+        if self.data.is_dirty_er:
+            eid = 0
+            for entity in self._entities_d1:
+                candidates = set()
+                for token in entity:
+                    if token in entity_index:
+                        current_candidates = entity_index[token]
+                        for candidate_id in current_candidates:
+                            if self._flags[candidate_id] != eid:
+                                self._counters[candidate_id] = 0
+                                self._flags[candidate_id] = eid
+                            self._counters[candidate_id] += 1
+                            candidates.add(candidate_id)
+                self._process_candidates(candidates, eid, len(entity))
+                self._progress_bar.update(1)
+                eid += 1
+        else:
+            if reverse_order:
+                entities = self._entities_d1
+                num_of_entities = self.data.num_of_entities_1
+            else:
+                entities = self._entities_d2
+                num_of_entities = self.data.num_of_entities_2
+
+            for i in range(0, num_of_entities):
+                candidates = set()
+                record = entities[i]
+                entity_id = i if reverse_order else i+self.data.dataset_limit
+                for token in record:
+                    if token in entity_index:
+                        current_candidates = entity_index[token]
+                        for candidate_id in current_candidates:
+                            if self._flags[candidate_id] != entity_id:
+                                self._counters[candidate_id] = 0
+                                self._flags[candidate_id] = entity_id
+                            self._counters[candidate_id] += 1
+                            candidates.add(candidate_id)
+                if 0 < len(candidates):
+                    self._process_candidates(candidates, entity_id, len(record))
+                self._progress_bar.update(1)
+        self._progress_bar.close()
+        self.execution_time = time() - start_time
+
+        return self.pairs
+
+    def _tokenize_entity(self, entity: str) -> set:
+        if self.tokenization == 'qgrams':
+            return set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)])
+        elif self.tokenization == 'standard':
+            return set(filter(None, re.split('[\\W_]', entity.lower())))
+        elif self.tokenization == 'standard_multiset':
+            tok_ids_index = {}
+            multiset = set()
+            for tok in set(filter(None, re.split('[\\W_]', entity.lower()))):
+                tok_id =  tok_ids_index[tok] if tok in tok_ids_index else 0
+                multiset.add(tok+str(tok_id))
+                tok_ids_index[tok] = tok_id+1
+            return multiset
+        elif self.tokenization == 'qgrams_multiset':
+            grams_ids_index = {}
+            qgrams = set()
+            for gram in set([' '.join(grams) for grams in nltk.ngrams(entity.lower(), n=self.qgrams)]):
+                gram_id =  grams_ids_index[gram] if gram in grams_ids_index else 0
+                qgrams.add(gram+str(gram_id))
+                grams_ids_index[gram] = gram_id+1
+            return qgrams
+        else:
+            raise AttributeError("Tokenization not found")
+
+    def _calc_similarity(
+            self,
+            common_tokens: int,
+            source_frequency: int,
+            tokens_size: int
+        ) -> float:
+        """Similarity score
+
+        Args:
+            common_tokens (int): number of common tokens
+            source_frequency (int): frequency
+            tokens_size (int): size of tokens
+
+        Returns:
+            float: similarity
+        """
+        if self.metric == 'cosine':
+            return common_tokens / math.sqrt(source_frequency*tokens_size)
+        elif self.metric == 'dice':
+            return 2 * common_tokens / (source_frequency+tokens_size)
+        elif self.metric == 'jaccard':
+            return common_tokens / (source_frequency+tokens_size-common_tokens)
+
+    def _create_entity_index(self, entities: list) -> dict:
+        entity_index = defaultdict(set)
+        entity_id = itertools.count()
+        for entity in entities:
+            eid = next(entity_id)
+            for token in entity:
+                entity_index[token].add(eid)
+            self._source_frequency[eid] = len(entity)
+            self._progress_bar.update(1)
+
+        return entity_index
+
+#     def _similarity(self, entity_id1: int, entity_id2: int, attributes: any=None) -> float:
+#         similarity: float = 0.0
+#         if isinstance(attributes, dict):
+#             for attribute, weight in self.attributes.items():
+#                 similarity += weight*self._metric(
+#                     self.data.entities.iloc[entity_id1][attribute],
+#                     self.data.entities.iloc[entity_id2][attribute]
+#                 )
+#         if isinstance(attributes, list):
+#             for attribute in self.attributes:
+#                 similarity += self._metric(
+#                     self.data.entities.iloc[entity_id1][attribute],
+#                     self.data.entities.iloc[entity_id2][attribute]
+#                 )
+#                 similarity /= len(self.attributes)
+#         else:
+#             # print(self.data.entities.iloc[entity_id1].str.cat(sep=' '),
+#                 # self.data.entities.iloc[entity_id2].str.cat(sep=' '))
+#             # concatenated row string
+#             similarity = self._metric(
+#                 self.data.entities.iloc[entity_id1].str.cat(sep=' '),
+#                 self.data.entities.iloc[entity_id2].str.cat(sep=' ')
+#             )
+#         return similarity
+
+    def _insert_to_graph(self, entity_id1, entity_id2, similarity):
+        if self.similarity_threshold <= similarity:
+            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
+
+    def evaluate(self, prediction=None, export_to_df: bool = False,
+                 export_to_dict: bool = False, with_classification_report: bool = False,
+                 verbose: bool = True) -> any:
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        total_matching_pairs = prediction.number_of_edges()
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
+                                                else self.data._ids_mapping_2[id2]
+            if (id1 in prediction and id2 in prediction[id1]) or   \
+                 (id2 in prediction and id1 in prediction[id2]):
+                true_positives += 1
+
+        eval_obj.calculate_scores(true_positives=true_positives, 
+                                  total_matching_pairs=total_matching_pairs)
+        return eval_obj.report(self.method_configuration(),
+                        export_to_df,
+                        export_to_dict,
+                        with_classification_report,
+                        verbose)
+        
+    def stats(self) -> None:
+        pass
+
+    def stats(self) -> None:
+        pass
+
+    def _configuration(self) -> dict:
+        return {
+            "similarity_threshold" : self.similarity_threshold,
+            "metric" : self.metric,
+            "tokenization" : self.tokenization,
+            "qgrams": self.qgrams
+        }    
+
+class EJoin(AbstractJoin):
+    """
+     E Join algorithm
+    """
+    _method_name = "EJoin"
+    _method_info = " EJoin algorithm"
+    _method_short_name = "EJ"
+
+    def __init__(
+        self,
+        similarity_threshold: float = 0.82,
+        metric: str = 'cosine',
+        tokenization: str = 'qgrams',
+        qgrams: int = 2
+    ) -> None:
+        super().__init__(metric, tokenization, qgrams, similarity_threshold)
+
+    def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
+        for candidate_id in candidates:
+            self._insert_to_graph(
+                candidate_id+self.data.dataset_limit if self.reverse_order \
+                                                        and not self.data.is_dirty_er \
+                                                    else candidate_id,
+                entity_id,
+                self._calc_similarity(
+                    self._counters[candidate_id],
+                    self._source_frequency[candidate_id],
+                    tokens_size
+                )
+            )
+
+class TopKJoin(AbstractJoin):
+    """Top-K Join algorithm
+    """
+
+    _method_name = "Top-K Join"
+    _method_info = "Top-K Join algorithm"
+    _method_short_name = "TopKJ"
+
+    def __init__(self,
+                 K: int,
+                 metric: str,
+                 tokenization: str,
+                 qgrams: int = 2
+        ) -> None:
+        super().__init__(metric, tokenization, qgrams)
+        self.K = K
+
+    def _process_candidates(self, candidates: set, entity_id: int, tokens_size: int) -> None:
+        minimum_weight=0
+        pq = PriorityQueue()
+        for candidate_id in candidates:
+            sim = self._calc_similarity(
+                self._counters[candidate_id], self._source_frequency[candidate_id], tokens_size
+            )
+            if minimum_weight < sim:
+                pq.put(sim)
+                if self.K < pq.qsize():
+                    minimum_weight = pq.get()
+
+        minimum_weight = pq.get()
+        for candidate_id in candidates:
+            self.similarity_threshold = minimum_weight
+            self._insert_to_graph(
+                candidate_id + self.data.dataset_limit if self.reverse_order else candidate_id,
+                entity_id,
+                self._calc_similarity(
+                    self._counters[candidate_id], 
+                    self._source_frequency[candidate_id],
+                    tokens_size
+                )
+            )
+
+    def _configuration(self) -> dict:
+        return {
+            "similarity_threshold" : self.similarity_threshold,
+            "K" : self.K,
+            "metric" : self.metric,
+            "tokenization" : self.tokenization,
+            "qgrams": self.qgrams
+        }
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pyjedai-0.0.6/src/pyjedai/matching.py` & `pyjedai-0.0.7/src/pyjedai/matching.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,528 +1,612 @@
-"""Entity Matching Module
-"""
-import statistics
-from time import time
-
-import matplotlib.pyplot as plt
-import numpy as np
-from networkx import Graph
-from py_stringmatching.similarity_measure.affine import Affine
-from py_stringmatching.similarity_measure.bag_distance import BagDistance
-from py_stringmatching.similarity_measure.cosine import Cosine
-from py_stringmatching.similarity_measure.dice import Dice
-from py_stringmatching.similarity_measure.editex import Editex
-from py_stringmatching.similarity_measure.generalized_jaccard import \
-    GeneralizedJaccard
-from py_stringmatching.similarity_measure.hamming_distance import \
-    HammingDistance
-from py_stringmatching.similarity_measure.jaccard import Jaccard
-from py_stringmatching.similarity_measure.jaro import Jaro
-from py_stringmatching.similarity_measure.jaro_winkler import JaroWinkler
-from py_stringmatching.similarity_measure.levenshtein import Levenshtein
-from py_stringmatching.similarity_measure.monge_elkan import MongeElkan
-from py_stringmatching.similarity_measure.needleman_wunsch import \
-    NeedlemanWunsch
-from py_stringmatching.similarity_measure.overlap_coefficient import \
-    OverlapCoefficient
-from py_stringmatching.similarity_measure.partial_ratio import PartialRatio
-from py_stringmatching.similarity_measure.partial_token_sort import \
-    PartialTokenSort
-from py_stringmatching.similarity_measure.ratio import Ratio
-from py_stringmatching.similarity_measure.smith_waterman import SmithWaterman
-from py_stringmatching.similarity_measure.soundex import Soundex
-from py_stringmatching.similarity_measure.tfidf import TfIdf
-from py_stringmatching.similarity_measure.token_sort import TokenSort
-from py_stringmatching.similarity_measure.tversky_index import TverskyIndex
-from py_stringmatching.tokenizer.alphabetic_tokenizer import \
-    AlphabeticTokenizer
-from py_stringmatching.tokenizer.alphanumeric_tokenizer import \
-    AlphanumericTokenizer
-from py_stringmatching.tokenizer.delimiter_tokenizer import DelimiterTokenizer
-from py_stringmatching.tokenizer.qgram_tokenizer import QgramTokenizer
-from py_stringmatching.tokenizer.whitespace_tokenizer import \
-    WhitespaceTokenizer
-from sklearn.feature_extraction.text import TfidfVectorizer
-# from scipy.spatial.distance import cosine
-from sklearn.metrics.pairwise import cosine_similarity
-from tqdm.autonotebook import tqdm
-
-from .datamodel import Data, PYJEDAIFeature
-from .evaluation import Evaluation
-from .utils import WordQgrammsTokenizer
-
-# Package import from https://anhaidgroup.github.io/py_stringmatching/v0.4.2/index.html
-
-def cosine(x, y):
-    """Cosine similarity between two vectors
-    """
-    return cosine_similarity(x.reshape(1, -1), y.reshape(1, -1))[0][0]
-
-available_tokenizers = [
-    'white_space_tokenizer', 'qgram_tokenizer', 'delimiter_tokenizer',
-    'alphabetic_tokenizer', 'alphanumeric_tokenizer'
-]
-
-metrics_mapping = {
-    'levenshtein' : Levenshtein(),
-    'edit_distance': Levenshtein(),
-    'jaro_winkler' : JaroWinkler(),
-    'bag_distance' : BagDistance(),
-    'editex' : Editex(),
-    'cosine' : Cosine(),
-    'jaro' : Jaro(),
-    'soundex' : Soundex(),
-    'tfidf' : TfIdf(),
-    'tversky_index':TverskyIndex(),
-    'ratio' : Ratio(),
-    'partial_token_sort' : PartialTokenSort(),
-    'partial_ratio' : PartialRatio(),
-    'hamming_distance' : HammingDistance(),
-    'jaccard' : Jaccard(),
-    'generalized_jaccard' : GeneralizedJaccard(),
-    'dice': Dice(),
-    'overlap_coefficient' : OverlapCoefficient(),
-    'token_sort': TokenSort(),
-    'cosine_vector_similarity': cosine
-}
-
-string_metrics = [
-    'bag_distance', 'editex', 'hamming_distance', 'jaro', 'jaro_winkler', 'levenshtein',
-    'edit_distance', 'partial_ratio', 'partial_token_sort', 'ratio', 'soundex', 'token_sort'
-]
-
-set_metrics = [
-    'cosine', 'dice', 'generalized_jaccard', 'jaccard', 'overlap_coefficient', 'tversky_index'
-]
-
-bag_metrics = [
-    'tf-idf'
-]
-
-vector_metrics = [
-    'cosine_vector_similarity'
-]
-
-available_metrics = string_metrics + set_metrics + bag_metrics + vector_metrics
-
-
-class EntityMatching(PYJEDAIFeature):
-    """Calculates similarity from 0.0 to 1.0 for all blocks
-    """
-
-    _method_name: str = "Entity Matching"
-    _method_info: str = "Calculates similarity from 0. to 1. for all blocks"
-
-    def __init__(
-            self,
-            metric: str = 'dice',
-            tokenizer: str = 'white_space_tokenizer',
-            similarity_threshold: float = 0.5,
-            qgram: int = 2, # for jaccard
-            tokenizer_return_set = False, # unique values or not,
-            attributes: any = None,
-            delim_set: list = None, # DelimiterTokenizer
-            padding: bool = True, # QgramTokenizer
-            prefix_pad: str = '#', # QgramTokenizer (if padding=True)
-            suffix_pad: str = '$' # QgramTokenizer (if padding=True)
-        ) -> None:
-        self.pairs: Graph
-        self.metric = metric
-        self.qgram: int = qgram
-        self.attributes: list = attributes
-        self.similarity_threshold = similarity_threshold
-        self.vectors_d1 = None
-        self.vectors_d2 = None
-        self.tokenizer = tokenizer
-        self.execution_time = 0
-        #
-        # Selecting tokenizer
-        #
-        if metric not in available_metrics:
-            raise AttributeError(
-                'Metric ({}) does not exist. Please select one of the available. ({})'.format(
-                    metric, available_metrics
-                )
-            )
-        else:
-            self._metric = metric
-
-        if metric in set_metrics:
-            self.tokenizer_return_set = True
-        else:
-            self.tokenizer_return_set = tokenizer_return_set
-
-        if tokenizer == 'white_space_tokenizer':
-            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'char_qgram_tokenizer':
-            self._tokenizer = QgramTokenizer(qval=self.qgram,
-                                             return_set=self.tokenizer_return_set,
-                                             padding=padding,
-                                             suffix_pad=suffix_pad,
-                                             prefix_pad=prefix_pad)
-        elif tokenizer == 'word_qgram_tokenizer':
-            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'delimiter_tokenizer':
-            self._tokenizer = DelimiterTokenizer(return_set=self.tokenizer_return_set,
-                                                 delim_set=delim_set)
-        elif tokenizer == 'alphabetic_tokenizer':
-            self._tokenizer = AlphabeticTokenizer(return_set=self.tokenizer_return_set)
-        elif tokenizer == 'alphanumeric_tokenizer':
-            self._tokenizer = AlphanumericTokenizer(return_set=self.tokenizer_return_set)
-        else:
-            raise AttributeError(
-                'Tokenizer ({}) does not exist. Please select one of the available. ({})'.format(
-                    tokenizer, available_tokenizers
-                )
-            )
-        
-    def predict(self,
-                blocks: dict,
-                data: Data,
-                tqdm_disable: bool = False,
-                vectors_d1: np.array = None,
-                vectors_d2: np.array = None) -> Graph:
-        """Main method of entity matching. Inputs a set of blocks and outputs a graph \
-            that contains of the entity ids (nodes) and the similarity scores between them (edges).
-
-            Args:
-                blocks (dict): blocks of entities
-                data (Data): dataset module
-                tqdm_disable (bool, optional): Disables progress bar. Defaults to False.
-
-            Returns:
-                networkx.Graph: entity ids (nodes) and similarity scores between them (edges)
-        """
-        start_time = time()
-        self.tqdm_disable = tqdm_disable
-        self.vectors_d1 = vectors_d1
-        self.vectors_d2 = vectors_d2
-        
-        if self.metric in vector_metrics:
-            if(vectors_d2 is not None and vectors_d1 is None):
-                raise ValueError("Embeddings of the first dataset not given")
-
-            if(vectors_d1 is not None):
-                self.vectors = vectors_d1
-                if(not data.is_dirty_er):
-                    if(vectors_d2 is None):
-                        raise ValueError("Embeddings of the second dataset not given")
-                    self.vectors = np.concatenate((vectors_d1,vectors_d2), axis=0)
-
-        if not blocks:
-            raise ValueError("Empty blocks structure")
-        self.data = data
-        self.pairs = Graph()
-        all_blocks = list(blocks.values())
-        self._progress_bar = tqdm(total=len(blocks),
-                                  desc=self._method_name+" ("+self.metric+")",
-                                  disable=self.tqdm_disable)
-        
-        if self.metric == 'tf-idf':
-            self._calculate_tfidf()
-        
-        if 'Block' in str(type(all_blocks[0])):
-            self._predict_raw_blocks(blocks)
-        elif isinstance(all_blocks[0], set):
-            self._predict_prunned_blocks(blocks)
-        else:
-            raise AttributeError("Wrong type of Blocks")
-        self.execution_time = time() - start_time
-        self._progress_bar.close()
-
-        return self.pairs
-
-    def _predict_raw_blocks(self, blocks: dict) -> None:
-        """Method for similarity evaluation blocks after Block building
-
-        Args:
-            blocks (dict): Block building blocks
-        """
-        if self.data.is_dirty_er:
-            for _, block in blocks.items():
-                entities_array = list(block.entities_D1)
-                for index_1 in range(0, len(entities_array), 1):
-                    for index_2 in range(index_1+1, len(entities_array), 1):
-                        similarity = self._similarity(entities_array[index_1],
-                                                      entities_array[index_2])
-                        self._insert_to_graph(entities_array[index_1],
-                                              entities_array[index_2],
-                                              similarity)
-                self._progress_bar.update(1)
-        else:
-            for _, block in blocks.items():
-                for entity_id1 in block.entities_D1:
-                    for entity_id2 in block.entities_D2:
-                        similarity = self._similarity(entity_id1, entity_id2)
-                        self._insert_to_graph(entity_id1, entity_id2, similarity)
-                self._progress_bar.update(1)
-
-    def _predict_prunned_blocks(self, blocks: dict) -> None:
-        """Similarity evaluation after comparison cleaning.
-
-        Args:
-            blocks (dict): Comparison cleaning blocks.
-        """
-        for entity_id, candidates in blocks.items():
-            for candidate_id in candidates:
-                similarity = self._similarity(entity_id, candidate_id)
-                self._insert_to_graph(entity_id, candidate_id, similarity)
-            self._progress_bar.update(1)
-
-    def _insert_to_graph(self, entity_id1, entity_id2, similarity):
-        if self.similarity_threshold is None or \
-            (self.similarity_threshold is not None and similarity > self.similarity_threshold):
-            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
-
-    def _calculate_vector_similarity(self, entity_id1: int, entity_id2: int) -> float:
-        if self.metric in vector_metrics:
-            return metrics_mapping[self._metric](self.vectors[entity_id1],
-                                                 self.vectors[entity_id2])
-        else:
-            raise AttributeError("Please select one vector similarity metric from the given: " + ','.join(vector_metrics))
-
-    def _calculate_tfidf(self) -> None:
-        
-        analyzer = 'char' if self.tokenizer == 'char_qgram_tokenizer' else 'word'
-        vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
-        
-        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
-        self._entities_d1 = d1 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist()
-        
-        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
-        self._entities_d2 = d2 \
-                    .apply(" ".join, axis=1) \
-                    .apply(lambda x: x.lower()) \
-                    .values.tolist() if not self.data.is_dirty_er else None
-                    
-        if self.data.is_dirty_er:
-            pass
-        else:
-            self.corpus = self._entities_d1 + self._entities_d2
-            self.tfidf_vectorizer = vectorizer.fit(self.corpus)
-            self.tfidf_matrix = vectorizer.transform(self.corpus)
-            self.tfidf_similarity_matrix = cosine_similarity(self.tfidf_matrix)
-            # feature_names = self.tfidf_vectorizer.get_feature_names()
-            # tfidf_df = pd.DataFrame(self.tfidf_matrix.toarray(), columns=feature_names)
-            # self.tfidf_df = tfidf_df
-
-    def _calculate_tfidf_similarity(self, entity_id1: int, entity_id2: int) -> float:
-        return self.tfidf_similarity_matrix[entity_id1][entity_id2]
-
-    def _similarity(self, entity_id1: int, entity_id2: int) -> float:
-
-        similarity: float = 0.0
-        if self.vectors_d1 is not None and self.metric in vector_metrics:
-            return self._calculate_vector_similarity(entity_id1, entity_id2)
-        elif self.metric == 'tf-idf':
-            return self._calculate_tfidf_similarity(entity_id1, entity_id2)
-
-        if isinstance(self.attributes, dict):
-            for attribute, weight in self.attributes.items():
-                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
-                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
-
-                similarity += weight*metrics_mapping[self._metric].get_sim_score(
-                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
-                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-                )
-        if isinstance(self.attributes, list):
-            for attribute in self.attributes:
-                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
-                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
-                similarity += metrics_mapping[self._metric].get_sim_score(
-                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
-                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-                )
-                similarity /= len(self.attributes)
-        else:
-            # concatenated row string
-            e1 = self.data.entities.iloc[entity_id1].str.cat(sep=' ').lower()
-            e2 = self.data.entities.iloc[entity_id2].str.cat(sep=' ').lower()
-            te1 = self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1
-            te2 = self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
-            similarity = metrics_mapping[self._metric].get_sim_score(te1, te2)
-
-        return similarity        
-
-    def report(self) -> None:
-        """Prints Block Building method configuration
-        """
-        print(
-            "Method name: " + self._method_name +
-            "\nMethod info: " + self._method_info +
-            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
-            "Attributes:\n\t" + ', '.join(c for c in (self.attributes if self.attributes is not None \
-                else self.data.dataset_1.columns)) +
-            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
-        )
-
-    def _configuration(self) -> dict:
-        return {
-            "Metric" : self.metric,
-            "Attributes" : self.attributes,
-            "Similarity threshold" : self.similarity_threshold
-        }
-
-    def get_weights_avg(self) -> float:
-        return sum([w for _, _, w in self.pairs.edges(data='weight')])/len(self.pairs.edges(data='weight'))
-
-    def get_weights_median(self) -> float:
-        return [w for _, _, w in sorted(self.pairs.edges(data='weight'))][int(len(self.pairs.edges(data='weight'))/2)]    
-    
-    def get_weights_standard_deviation(self) -> float:
-        return statistics.stdev([w for _, _, w in self.pairs.edges(data='weight')])
-    
-    def plot_distribution_of_all_weights(self) -> None:
-        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
-        plt.figure(figsize=(10, 6))
-        all_weights = [w for _, _, w in self.pairs.edges(data='weight')]
-        sorted_weights = sorted(all_weights, reverse=True)
-        
-        plt.hist(sorted_weights)
-        plt.xlim(0, 1)
-        # only one line may be specified; full height
-        plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
-        plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
-        plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
-        plt.legend()
-        plt.show()
-
-    
-    def plot_distribution_of_all_weights_2d(self) -> None:
-        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
-        plt.figure(figsize=(10, 6))
-        all_weights = [w for _, _, w in self.pairs.edges(data='weight')]
-        sorted_weights = sorted(all_weights, reverse=True)
-        
-        fig, ax = plt.subplots(tight_layout=True)
-        hist = ax.hist2d(sorted_weights, sorted_weights)
-        # plt.hist(sorted_weights)
-        # plt.xlim(0, 1)
-        # only one line may be specified; full height
-        plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
-        plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
-        plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
-        plt.legend()
-        plt.show()
-
-    def plot_distribution_of_scores(self) -> None:
-        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
-        def weight_distribution(G):
-            bins = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
-            distribution = [0] * (len(bins)-1)
-            for u, v, w in G.edges(data='weight'):
-                for i in range(len(bins) - 1):
-                    if bins[i] <= w < bins[i + 1]:
-                        distribution[i] += 1
-                        break
-            return distribution, len(G.edges(data='weight'))
-
-        labels = [f'{(i)/10:.1f} - {(i+1)/10:.1f}' for i in range(0, 10)]
-
-        distribution, num_of_pairs = weight_distribution(self.pairs)
-        width = 0.5
-        x = np.arange(len(labels))  # the label locations
-        distribution = list(map(lambda x: (x/num_of_pairs)*100, distribution))
-        print("Distribution-% of predicted scores: ", distribution)
-
-        fig, ax = plt.subplots(figsize=(10,6))
-        r1 = ax.bar(x, distribution, width, align='center', color='red')
-        ax.set_xticks(x)
-        ax.set_xticklabels(labels)
-    
-        
-        # Add some text for labels, title and custom x-axis tick labels, etc.
-        ax.set_ylabel('Percentage of pairs in each range to all (%)')
-        ax.set_title(title)
-        ax.set_xlabel('Similarity score range')
-        fig.tight_layout()
-        
-        # only one line may be specified; full height
-        plt.axvline(x = self.get_weights_avg()*10, color = 'blue', label = 'Average weight')
-        plt.axvline(x = self.get_weights_median()*10, color = 'black', label = 'Median weight')
-        plt.axvline(x = self.get_weights_avg()*10+self.get_weights_standard_deviation()*10, color = 'green', label = 'Average + SD weight')
-        plt.legend()
-        plt.show()
-
-    def plot_gt_distribution_of_scores(self) -> None:
-        title = "Distribution of scores with " + self.metric + " metric on ground truth pairs"
-        def weight_distribution():
-            bins = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
-            distribution = [0] * (len(bins)-1)
-            for _, (id1, id2) in self.data.ground_truth.iterrows():
-                id1 = self.data._ids_mapping_1[id1]
-                id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
-                w = self._calculate_vector_similarity(id1, id2)
-
-                for i in range(len(bins) - 1):
-                    if bins[i] <= w < bins[i + 1]:
-                        distribution[i] += 1
-                        break
-            return distribution, len(self.data.ground_truth)
-
-        labels = [f'{(i)/10:.1f} - {(i+1)/10:.1f}' for i in range(0, 10)]
-
-        distribution, num_of_pairs = weight_distribution()
-        width = 0.5
-        x = np.arange(len(labels))  # the label locations
-        distribution = list(map(lambda x: (x/num_of_pairs)*100, distribution))
-        print("Distribution-% of predicted scores: ", distribution)
-
-        fig, ax = plt.subplots(figsize=(10,6))
-        r1 = ax.bar(x, distribution, width, align='center', color='blue')
-        ax.set_xticks(x)
-        ax.set_xticklabels(labels)
-
-        # Add some text for labels, title and custom x-axis tick labels, etc.
-        ax.set_ylabel('Percentage of pairs in each range to all (%)')
-        ax.set_title(title)
-        ax.set_xlabel('Similarity score range')
-        fig.tight_layout()
-        plt.show()
-
-
-    def evaluate(self,
-                 prediction,
-                 export_to_df: bool = False,
-                 export_to_dict: bool = False,
-                 with_classification_report: bool = False,
-                 verbose: bool = True) -> any:
-
-        if self.data is None:
-            raise AttributeError("Can not proceed to evaluation without data object.")
-
-        if self.data.ground_truth is None:
-            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
-                    "Data object has not been initialized with the ground-truth file")
-
-        eval_obj = Evaluation(self.data)
-        true_positives = 0
-        total_matching_pairs = prediction.number_of_edges()
-        for _, (id1, id2) in self.data.ground_truth.iterrows():
-            id1 = self.data._ids_mapping_1[id1]
-            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
-                                                else self.data._ids_mapping_2[id2]
-            if (id1 in prediction and id2 in prediction[id1]) or   \
-                 (id2 in prediction and id1 in prediction[id2]):
-                true_positives += 1
-
-        eval_obj.calculate_scores(true_positives=true_positives,
-                                  total_matching_pairs=total_matching_pairs)
-        return eval_obj.report(self.method_configuration(),
-                                export_to_df,
-                                export_to_dict,
-                                with_classification_report,
-                                verbose)
-
-    def _configuration(self) -> dict:
-        return {
-            "Tokenizer" : self.tokenizer,
-            "Metric" : self.metric,
-            "Similarity Threshold" : self.similarity_threshold
-        }
-        
-    def stats(self) -> None:
-        pass
+"""Entity Matching Module
+"""
+import statistics
+from time import time
+
+import matplotlib.pyplot as plt
+import numpy as np
+from networkx import Graph
+from py_stringmatching.similarity_measure.affine import Affine
+from py_stringmatching.similarity_measure.bag_distance import BagDistance
+from py_stringmatching.similarity_measure.cosine import Cosine
+from py_stringmatching.similarity_measure.dice import Dice
+from py_stringmatching.similarity_measure.editex import Editex
+from py_stringmatching.similarity_measure.generalized_jaccard import \
+    GeneralizedJaccard
+from py_stringmatching.similarity_measure.hamming_distance import \
+    HammingDistance
+from py_stringmatching.similarity_measure.jaccard import Jaccard
+from py_stringmatching.similarity_measure.jaro import Jaro
+from py_stringmatching.similarity_measure.jaro_winkler import JaroWinkler
+from py_stringmatching.similarity_measure.levenshtein import Levenshtein
+from py_stringmatching.similarity_measure.monge_elkan import MongeElkan
+from py_stringmatching.similarity_measure.needleman_wunsch import \
+    NeedlemanWunsch
+from py_stringmatching.similarity_measure.overlap_coefficient import \
+    OverlapCoefficient
+from py_stringmatching.similarity_measure.partial_ratio import PartialRatio
+from py_stringmatching.similarity_measure.partial_token_sort import \
+    PartialTokenSort
+from py_stringmatching.similarity_measure.ratio import Ratio
+from py_stringmatching.similarity_measure.smith_waterman import SmithWaterman
+from py_stringmatching.similarity_measure.soundex import Soundex
+from py_stringmatching.similarity_measure.tfidf import TfIdf
+from py_stringmatching.similarity_measure.token_sort import TokenSort
+from py_stringmatching.similarity_measure.tversky_index import TverskyIndex
+from py_stringmatching.tokenizer.alphabetic_tokenizer import \
+    AlphabeticTokenizer
+from py_stringmatching.tokenizer.alphanumeric_tokenizer import \
+    AlphanumericTokenizer
+from py_stringmatching.tokenizer.delimiter_tokenizer import DelimiterTokenizer
+from py_stringmatching.tokenizer.qgram_tokenizer import QgramTokenizer
+from py_stringmatching.tokenizer.whitespace_tokenizer import \
+    WhitespaceTokenizer
+from sklearn.feature_extraction.text import TfidfVectorizer
+# from scipy.spatial.distance import cosine
+from sklearn.metrics.pairwise import cosine_similarity, pairwise_distances
+from tqdm.autonotebook import tqdm
+from sklearn.metrics import jaccard_score
+from scipy.spatial.distance import dice, jaccard
+
+from .datamodel import Data, PYJEDAIFeature
+from .evaluation import Evaluation
+from .utils import WordQgrammsTokenizer
+from whoosh.scoring import TF_IDF, Frequency, PL2, BM25F
+
+# Package import from https://anhaidgroup.github.io/py_stringmatching/v0.4.2/index.html
+
+def cosine(x, y):
+    """Cosine similarity between two vectors
+    """
+    return cosine_similarity(x.reshape(1, -1), y.reshape(1, -1))[0][0]
+
+available_tokenizers = [
+    'white_space_tokenizer', 'qgram_tokenizer', 'delimiter_tokenizer',
+    'alphabetic_tokenizer', 'alphanumeric_tokenizer'
+]
+
+metrics_mapping = {
+    'levenshtein' : Levenshtein(),
+    'edit_distance': Levenshtein(),
+    'jaro_winkler' : JaroWinkler(),
+    'bag_distance' : BagDistance(),
+    'editex' : Editex(),
+    'cosine' : Cosine(),
+    'jaro' : Jaro(),
+    'soundex' : Soundex(),
+    'tfidf' : TfIdf(),
+    'tversky_index':TverskyIndex(),
+    'ratio' : Ratio(),
+    'partial_token_sort' : PartialTokenSort(),
+    'partial_ratio' : PartialRatio(),
+    'hamming_distance' : HammingDistance(),
+    'jaccard' : Jaccard(),
+    'generalized_jaccard' : GeneralizedJaccard(),
+    'dice': Dice(),
+    'overlap_coefficient' : OverlapCoefficient(),
+    'token_sort': TokenSort(),
+    'cosine_vector_similarity': cosine,
+    'TF-IDF' : TF_IDF(),
+    'Frequency' : Frequency(),
+    'PL2' : PL2(),
+    'BM25F' : BM25F()
+}
+
+string_metrics = [
+    'bag_distance', 'editex', 'hamming_distance', 'jaro', 'jaro_winkler', 'levenshtein',
+    'edit_distance', 'partial_ratio', 'partial_token_sort', 'ratio', 'soundex', 'token_sort'
+]
+
+set_metrics = [
+    'cosine', 'dice', 'generalized_jaccard', 'jaccard', 'overlap_coefficient', 'tversky_index'
+]
+
+bag_metrics = [
+    'tf-idf'
+]
+
+vector_metrics = [
+    'cosine_vector_similarity'
+]
+
+index_metrics = [
+    'TF-IDF', 'Frequency', 'PL2', 'BM25F'
+] 
+
+available_metrics = string_metrics + set_metrics + bag_metrics + vector_metrics + index_metrics
+
+
+class EntityMatching(PYJEDAIFeature):
+    """Calculates similarity from 0.0 to 1.0 for all blocks
+    """
+
+    _method_name: str = "Entity Matching"
+    _method_info: str = "Calculates similarity from 0. to 1. for all blocks"
+
+    def __init__(
+            self,
+            metric: str = 'dice',
+            tokenizer: str = 'white_space_tokenizer',
+            similarity_threshold: float = 0.5,
+            qgram: int = 2, # for jaccard
+            tokenizer_return_set = False, # unique values or not,
+            attributes: any = None,
+            tfidf_similarity_metric: str = 'cosine',
+            delim_set: list = None, # DelimiterTokenizer
+            padding: bool = True, # QgramTokenizer
+            prefix_pad: str = '#', # QgramTokenizer (if padding=True)
+            suffix_pad: str = '$' # QgramTokenizer (if padding=True)
+        ) -> None:
+        self.pairs: Graph
+        self.metric = metric
+        self.qgram: int = qgram
+        self.attributes: list = attributes
+        self.similarity_threshold = similarity_threshold
+        self.vectors_d1 = None
+        self.vectors_d2 = None
+        self.tokenizer = tokenizer
+        self.execution_time = 0
+        self.tfidf_similarity_metric = tfidf_similarity_metric
+        #
+        # Selecting tokenizer
+        #
+        if metric not in available_metrics:
+            raise AttributeError(
+                'Metric ({}) does not exist. Please select one of the available. ({})'.format(
+                    metric, available_metrics
+                )
+            )
+        else:
+            self._metric = metric
+
+        if metric in set_metrics:
+            self.tokenizer_return_set = True
+        else:
+            self.tokenizer_return_set = tokenizer_return_set
+
+        if tokenizer == 'white_space_tokenizer':
+            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
+        elif tokenizer == 'char_qgram_tokenizer':
+            self._tokenizer = QgramTokenizer(qval=self.qgram,
+                                             return_set=self.tokenizer_return_set,
+                                             padding=padding,
+                                             suffix_pad=suffix_pad,
+                                             prefix_pad=prefix_pad)
+        elif tokenizer == 'word_qgram_tokenizer':
+            self._tokenizer = WhitespaceTokenizer(return_set=self.tokenizer_return_set)
+        elif tokenizer == 'delimiter_tokenizer':
+            self._tokenizer = DelimiterTokenizer(return_set=self.tokenizer_return_set,
+                                                 delim_set=delim_set)
+        elif tokenizer == 'alphabetic_tokenizer':
+            self._tokenizer = AlphabeticTokenizer(return_set=self.tokenizer_return_set)
+        elif tokenizer == 'alphanumeric_tokenizer':
+            self._tokenizer = AlphanumericTokenizer(return_set=self.tokenizer_return_set)
+        else:
+            raise AttributeError(
+                'Tokenizer ({}) does not exist. Please select one of the available. ({})'.format(
+                    tokenizer, available_tokenizers
+                )
+            )
+        
+    def predict(self,
+                blocks: dict,
+                data: Data,
+                tqdm_disable: bool = False,
+                vectors_d1: np.array = None,
+                vectors_d2: np.array = None) -> Graph:
+        """Main method of entity matching. Inputs a set of blocks and outputs a graph \
+            that contains of the entity ids (nodes) and the similarity scores between them (edges).
+
+            Args:
+                blocks (dict): blocks of entities
+                data (Data): dataset module
+                tqdm_disable (bool, optional): Disables progress bar. Defaults to False.
+
+            Returns:
+                networkx.Graph: entity ids (nodes) and similarity scores between them (edges)
+        """
+        start_time = time()
+        self.tqdm_disable = tqdm_disable
+        self.vectors_d1 = vectors_d1
+        self.vectors_d2 = vectors_d2
+        
+        if self.metric in vector_metrics:
+            if(vectors_d1 is None):
+                raise ValueError("Embeddings of the first dataset not given")
+            else:
+                self.vectors = vectors_d1
+                if(not data.is_dirty_er):
+                    if(vectors_d2 is None):
+                        raise ValueError("Embeddings of the second dataset not given")
+                    self.vectors = np.concatenate((vectors_d1,vectors_d2), axis=0)
+
+        if not blocks:
+            raise ValueError("Empty blocks structure")
+        self.data = data
+        self.pairs = Graph()
+        all_blocks = list(blocks.values())
+        self._progress_bar = tqdm(total=len(blocks),
+                                  desc=self._method_name+" ("+self.metric+ ", " + str(self.tokenizer) + ")",
+                                  disable=self.tqdm_disable)
+                
+        if self.metric == 'tf-idf':
+            self._calculate_tfidf()
+        
+        if 'Block' in str(type(all_blocks[0])):
+            self._predict_raw_blocks(blocks)
+        elif isinstance(all_blocks[0], set):
+            self._predict_prunned_blocks(blocks)
+        else:
+            raise AttributeError("Wrong type of Blocks")
+        self.execution_time = time() - start_time
+        self._progress_bar.close()
+
+        return self.pairs
+
+    def _predict_raw_blocks(self, blocks: dict) -> None:
+        """Method for similarity evaluation blocks after Block building
+
+        Args:
+            blocks (dict): Block building blocks
+        """
+        if self.data.is_dirty_er:
+            for _, block in blocks.items():
+                entities_array = list(block.entities_D1)
+                for index_1 in range(0, len(entities_array), 1):
+                    for index_2 in range(index_1+1, len(entities_array), 1):
+                        similarity = self._similarity(entities_array[index_1],
+                                                      entities_array[index_2])
+                        self._insert_to_graph(entities_array[index_1],
+                                              entities_array[index_2],
+                                              similarity)
+                self._progress_bar.update(1)
+        else:
+            for _, block in blocks.items():
+                for entity_id1 in block.entities_D1:
+                    for entity_id2 in block.entities_D2:
+                        similarity = self._similarity(entity_id1, entity_id2)
+                        self._insert_to_graph(entity_id1, entity_id2, similarity)
+                self._progress_bar.update(1)
+
+    def _predict_prunned_blocks(self, blocks: dict) -> None:
+        """Similarity evaluation after comparison cleaning.
+
+        Args:
+            blocks (dict): Comparison cleaning blocks.
+        """
+        for entity_id, candidates in blocks.items():
+            for candidate_id in candidates:
+                similarity = self._similarity(entity_id, candidate_id)
+                self._insert_to_graph(entity_id, candidate_id, similarity)
+            self._progress_bar.update(1)
+
+    def _insert_to_graph(self, entity_id1, entity_id2, similarity):
+        if self.similarity_threshold is None or \
+            (self.similarity_threshold is not None and similarity > self.similarity_threshold):
+            self.pairs.add_edge(entity_id1, entity_id2, weight=similarity)
+
+    def _calculate_vector_similarity(self, entity_id1: int, entity_id2: int) -> float:
+        if self.metric in vector_metrics:
+            return metrics_mapping[self._metric](self.vectors[entity_id1],
+                                                 self.vectors[entity_id2])
+        else:
+            raise AttributeError("Please select one vector similarity metric from the given: " + ','.join(vector_metrics))
+        
+    def _calculate_tfidf(self) -> None:
+        
+        analyzer = 'char' if self.tokenizer == 'char_qgram_tokenizer' else 'word'
+        vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
+        
+        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
+        self._entities_d1 = d1 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist()
+        
+        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
+        self._entities_d2 = d2 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist() if not self.data.is_dirty_er else None
+                    
+        if self.data.is_dirty_er:
+            pass
+        else:
+            self.corpus = self._entities_d1 + self._entities_d2
+            self.tfidf_vectorizer = vectorizer.fit(self.corpus)
+            
+            if self.tfidf_similarity_metric == 'cosine':
+                self.tfidf_matrix = vectorizer.transform(self.corpus)
+                self.tfidf_similarity_matrix = cosine_similarity(self.tfidf_matrix)
+            elif self.tfidf_similarity_metric == 'jaccard':
+                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus)
+                self.tfidf_similarity_matrix = 1 - pairwise_distances( self.tfidf_matrix.toarray(), metric="jaccard")
+            elif self.tfidf_similarity_metric == 'dice':
+                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus).toarray()
+
+    def _calculate_tfidf_similarity(self, entity_id1: int, entity_id2: int) -> float:
+
+        if self.tfidf_similarity_metric == 'cosine':
+            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
+        elif self.tfidf_similarity_metric == 'jaccard':
+            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
+        elif self.tfidf_similarity_metric == 'dice':
+            return 1-dice(self.tfidf_matrix[entity_id1], self.tfidf_matrix[entity_id2])
+        else:
+            raise AttributeError("Please select one tf-idf similarity metric from the given: cosine, jaccard, dice")
+
+    def _calculate_tfidf(self) -> None:
+        
+        analyzer = 'char' if self.tokenizer == 'char_qgram_tokenizer' else 'word'
+        vectorizer = TfidfVectorizer(analyzer='') if self.qgram is None else TfidfVectorizer(analyzer=analyzer, ngram_range=(self.qgram, self.qgram))
+        
+        d1 = self.data.dataset_1[self.attributes] if self.attributes else self.data.dataset_1
+        self._entities_d1 = d1 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist()
+        
+        d2 = self.data.dataset_2[self.attributes] if self.attributes and not self.data.is_dirty_er else self.data.dataset_2
+        self._entities_d2 = d2 \
+                    .apply(" ".join, axis=1) \
+                    .apply(lambda x: x.lower()) \
+                    .values.tolist() if not self.data.is_dirty_er else None
+                    
+        if self.data.is_dirty_er:
+            pass
+        else:
+            self.corpus = self._entities_d1 + self._entities_d2
+            self.tfidf_vectorizer = vectorizer.fit(self.corpus)
+            
+            if self.tfidf_similarity_metric == 'cosine':
+                self.tfidf_matrix = vectorizer.transform(self.corpus)
+                self.tfidf_similarity_matrix = cosine_similarity(self.tfidf_matrix)
+            elif self.tfidf_similarity_metric == 'jaccard':
+                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus)
+                self.tfidf_similarity_matrix = 1 - pairwise_distances( self.tfidf_matrix.toarray(), metric="jaccard")
+            elif self.tfidf_similarity_metric == 'dice':
+                self.tfidf_matrix = self.tfidf_vectorizer.fit_transform(self.corpus).toarray()
+
+    def _calculate_tfidf_similarity(self, entity_id1: int, entity_id2: int) -> float:
+
+        if self.tfidf_similarity_metric == 'cosine':
+            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
+        elif self.tfidf_similarity_metric == 'jaccard':
+            return self.tfidf_similarity_matrix[entity_id1][entity_id2]
+        elif self.tfidf_similarity_metric == 'dice':
+            return 1-dice(self.tfidf_matrix[entity_id1], self.tfidf_matrix[entity_id2])
+        else:
+            raise AttributeError("Please select one tf-idf similarity metric from the given: cosine, jaccard, dice")
+
+    def _similarity(self, entity_id1: int, entity_id2: int) -> float:
+
+        similarity: float = 0.0
+        if self.vectors_d1 is not None and self.metric in vector_metrics:
+            return self._calculate_vector_similarity(entity_id1, entity_id2)
+        elif self.metric == 'tf-idf':
+            return self._calculate_tfidf_similarity(entity_id1, entity_id2)
+
+        if isinstance(self.attributes, dict):
+            for attribute, weight in self.attributes.items():
+                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
+                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
+
+                similarity += weight*metrics_mapping[self._metric].get_sim_score(
+                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
+                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+                )
+        if isinstance(self.attributes, list):
+            for attribute in self.attributes:
+                e1 = self.data.entities.iloc[entity_id1][attribute].lower()
+                e2 = self.data.entities.iloc[entity_id2][attribute].lower()
+                similarity += metrics_mapping[self._metric].get_sim_score(
+                    self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1,
+                    self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+                )
+                similarity /= len(self.attributes)
+        else:
+            # concatenated row string
+            e1 = self.data.entities.iloc[entity_id1].str.cat(sep=' ').lower()
+            e2 = self.data.entities.iloc[entity_id2].str.cat(sep=' ').lower()
+            te1 = self._tokenizer.tokenize(e1) if self._metric in set_metrics else e1
+            te2 = self._tokenizer.tokenize(e2) if self._metric in set_metrics else e2
+            similarity = metrics_mapping[self._metric].get_sim_score(te1, te2)
+
+        return similarity        
+
+    def report(self) -> None:
+        """Prints Block Building method configuration
+        """
+        print(
+            "Method name: " + self._method_name +
+            "\nMethod info: " + self._method_info +
+            ("\nParameters: \n" + ''.join(['\t{0}: {1}\n'.format(k, v) for k, v in self._configuration().items()]) if self._configuration().items() else "\nParameters: Parameter-Free method\n") +
+            "Attributes:\n\t" + ', '.join(c for c in (self.attributes if self.attributes is not None \
+                else self.data.dataset_1.columns)) +
+            "\nRuntime: {:2.4f} seconds".format(self.execution_time)
+        )
+
+    def _configuration(self) -> dict:
+        conf =  {
+            "Metric" : self.metric,
+            "Attributes" : self.attributes,
+            "Similarity threshold" : self.similarity_threshold,
+            "Tokenizer" : self.tokenizer
+        }
+
+        if self.metric == 'tf-idf':
+            conf["Similarity metric"] = self.tfidf_similarity_metric
+            if self.tokenizer == 'word_qgram_tokenizer' or self.tokenizer == 'char_qgram_tokenizer':
+                conf["QGram size"] = self.qgram
+
+        return conf
+        
+    def get_weights_avg(self) -> float:
+        return sum([w for _, _, w in self.pairs.edges(data='weight')])/len(self.pairs.edges(data='weight'))
+
+    def get_weights_median(self) -> float:
+        return [w for _, _, w in sorted(self.pairs.edges(data='weight'))][int(len(self.pairs.edges(data='weight'))/2)]    
+    
+    def get_weights_standard_deviation(self) -> float:
+        return statistics.stdev([w for _, _, w in self.pairs.edges(data='weight')])
+    
+    def plot_distribution_of_all_weights(self) -> None:
+        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
+        plt.figure(figsize=(10, 6))
+        all_weights = [w for _, _, w in self.pairs.edges(data='weight')]
+        sorted_weights = sorted(all_weights, reverse=True)
+        
+        plt.hist(sorted_weights)
+        plt.xlim(0, 1)
+        # only one line may be specified; full height
+        plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
+        plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
+        plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
+        plt.legend()
+        plt.show()
+
+    
+    def plot_distribution_of_all_weights_2d(self) -> None:
+        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
+        plt.figure(figsize=(10, 6))
+        all_weights = [w for _, _, w in self.pairs.edges(data='weight')]
+        sorted_weights = sorted(all_weights, reverse=True)
+        
+        fig, ax = plt.subplots(tight_layout=True)
+        hist = ax.hist2d(sorted_weights, sorted_weights)
+        # plt.hist(sorted_weights)
+        # plt.xlim(0, 1)
+        # only one line may be specified; full height
+        plt.axvline(x = self.get_weights_avg(), color = 'blue', label = 'Average weight')
+        plt.axvline(x = self.get_weights_median(), color = 'black', label = 'Median weight')
+        plt.axvline(x = self.get_weights_avg()+self.get_weights_standard_deviation(), color = 'green', label = 'Average + SD weight')
+        plt.legend()
+        plt.show()
+
+    def plot_distribution_of_scores(self) -> None:
+        title = "Distribution of scores with " + self.metric + " metric in graph from entity matching"
+        def weight_distribution(G):
+            bins = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
+            distribution = [0] * (len(bins)-1)
+            for u, v, w in G.edges(data='weight'):
+                for i in range(len(bins) - 1):
+                    if bins[i] <= w < bins[i + 1]:
+                        distribution[i] += 1
+                        break
+            return distribution, len(G.edges(data='weight'))
+
+        labels = [f'{(i)/10:.1f} - {(i+1)/10:.1f}' for i in range(0, 10)]
+
+        distribution, num_of_pairs = weight_distribution(self.pairs)
+        width = 0.5
+        x = np.arange(len(labels))  # the label locations
+        distribution = list(map(lambda x: (x/num_of_pairs)*100, distribution))
+        print("Distribution-% of predicted scores: ", distribution)
+
+        fig, ax = plt.subplots(figsize=(10,6))
+        r1 = ax.bar(x, distribution, width, align='center', color='red')
+        ax.set_xticks(x)
+        ax.set_xticklabels(labels)
+    
+        
+        # Add some text for labels, title and custom x-axis tick labels, etc.
+        ax.set_ylabel('Percentage of pairs in each range to all (%)')
+        ax.set_title(title)
+        ax.set_xlabel('Similarity score range')
+        fig.tight_layout()
+        
+        # only one line may be specified; full height
+        plt.axvline(x = self.get_weights_avg()*10, color = 'blue', label = 'Average weight')
+        plt.axvline(x = self.get_weights_median()*10, color = 'black', label = 'Median weight')
+        plt.axvline(x = self.get_weights_avg()*10+self.get_weights_standard_deviation()*10, color = 'green', label = 'Average + SD weight')
+        plt.legend()
+        plt.show()
+
+    def plot_gt_distribution_of_scores(self) -> None:
+        title = "Distribution of scores with " + self.metric + " metric on ground truth pairs"
+        def weight_distribution():
+            bins = [0.0, 0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9, 1.0]
+            distribution = [0] * (len(bins)-1)
+            for _, (id1, id2) in self.data.ground_truth.iterrows():
+                id1 = self.data._ids_mapping_1[id1]
+                id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er else self.data._ids_mapping_2[id2]
+                w = self._calculate_vector_similarity(id1, id2)
+
+                for i in range(len(bins) - 1):
+                    if bins[i] <= w < bins[i + 1]:
+                        distribution[i] += 1
+                        break
+            return distribution, len(self.data.ground_truth)
+
+        labels = [f'{(i)/10:.1f} - {(i+1)/10:.1f}' for i in range(0, 10)]
+
+        distribution, num_of_pairs = weight_distribution()
+        width = 0.5
+        x = np.arange(len(labels))  # the label locations
+        distribution = list(map(lambda x: (x/num_of_pairs)*100, distribution))
+        print("Distribution-% of predicted scores: ", distribution)
+
+        fig, ax = plt.subplots(figsize=(10,6))
+        r1 = ax.bar(x, distribution, width, align='center', color='blue')
+        ax.set_xticks(x)
+        ax.set_xticklabels(labels)
+
+        # Add some text for labels, title and custom x-axis tick labels, etc.
+        ax.set_ylabel('Percentage of pairs in each range to all (%)')
+        ax.set_title(title)
+        ax.set_xlabel('Similarity score range')
+        fig.tight_layout()
+        plt.show()
+
+
+    def evaluate(self,
+                 prediction,
+                 export_to_df: bool = False,
+                 export_to_dict: bool = False,
+                 with_classification_report: bool = False,
+                 verbose: bool = True) -> any:
+
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        total_matching_pairs = prediction.number_of_edges()
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
+                                                else self.data._ids_mapping_2[id2]
+            if (id1 in prediction and id2 in prediction[id1]) or   \
+                 (id2 in prediction and id1 in prediction[id2]):
+                true_positives += 1
+
+        eval_obj.calculate_scores(true_positives=true_positives,
+                                  total_matching_pairs=total_matching_pairs)
+        return eval_obj.report(self.method_configuration(),
+                                export_to_df,
+                                export_to_dict,
+                                with_classification_report,
+                                verbose)
+        
+    def stats(self) -> None:
+        pass
+    
+    def export_pairs(self, filename: str, with_similarity: bool = True) -> None:
+        if self.pairs is None:
+            raise AttributeError("Pairs have not been initialized yet. " +
+                                 "Please run the method `run` first.")
+
+        with open(filename, 'w') as f:
+            for e1, e2, similarity in self.pairs.edges(data='weight'):
+                e1 = self.data._ids_mapping_1[e1] if e1 < self.data.dataset_limit else self.data._ids_mapping_2[e1]
+                e2 = self.data._ids_mapping_1[e2] if e2 < self.data.dataset_limit else self.data._ids_mapping_2[e2]
+                if with_similarity:
+                    f.write(f"{e1}, {e2}, {similarity}\n")
+                else:
+                    f.write(f"{e1}, {e2}\n")
+            f.close()
+
```

### Comparing `pyjedai-0.0.6/src/pyjedai/vector_based_blocking.py` & `pyjedai-0.0.7/src/pyjedai/vector_based_blocking.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,612 +1,527 @@
-'''
-Contains all methods for creating embeddings from text 
-and then performing NNs methods for cluster formation.
-'''
-import os
-import pickle
-import re
-import sys
-import warnings
-from time import time
-from typing import List, Tuple
-
-import faiss
-import gensim.downloader as api
-import networkx as nx
-import numpy as np
-import torch
-import transformers
-from sentence_transformers import SentenceTransformer
-from tqdm.autonotebook import tqdm
-from transformers import (AlbertModel, AlbertTokenizer, BertModel,
-                          BertTokenizer, DistilBertModel, DistilBertTokenizer,
-                          RobertaModel, RobertaTokenizer, XLNetModel,
-                          XLNetTokenizer)
-
-transformers.logging.set_verbosity_error()
-
-from .datamodel import Data, PYJEDAIFeature
-from .evaluation import Evaluation
-from .utils import SubsetIndexer
-
-EMBEDDINGS_DIR = '.embeddings'
-if not os.path.exists(EMBEDDINGS_DIR):
-    os.makedirs(EMBEDDINGS_DIR)
-    EMBEDDINGS_DIR = os.path.abspath(EMBEDDINGS_DIR)
-    print('Created embeddings directory at: ' + EMBEDDINGS_DIR)
-    
-LINUX_ENV=False
-# try:
-#     if 'linux' in sys.platform:
-#         import falconn
-#         import scann
-#         LINUX_ENV=True
-# except:
-#     warnings.warn(ImportWarning, "Can't use FALCONN/SCANN in windows environment")
-
-class EmbeddingsNNBlockBuilding(PYJEDAIFeature):
-    """Block building via creation of embeddings and a Nearest Neighbor Approach.
-    """
-
-    _method_name = "Embeddings-NN Block Building"
-    _method_info = "Creates a set of candidate pais for every entity id " + \
-        "based on Embeddings creariot and Similarity search among the vectors."
-
-    _gensim_mapping_download = {
-        'fasttext' : 'fasttext-wiki-news-subwords-300',
-        'glove' : 'glove-wiki-gigaword-300',
-        'word2vec' : 'word2vec-google-news-300'
-    }
-    _sentence_transformer_mapping = {
-        'smpnet' : 'all-mpnet-base-v2',
-        'st5' : 'gtr-t5-large',
-        'sdistilroberta' : 'all-distilroberta-v1',
-        'sminilm' : 'all-MiniLM-L12-v2',
-        'sent_glove' : 'average_word_embeddings_glove.6B.300d'
-    }
-
-    def __init__(
-            self,
-            vectorizer: str,
-            similarity_search: str
-    ) -> None:
-        super().__init__()
-        self.vectorizer, self.similarity_search = vectorizer, similarity_search
-        self.embeddings: np.array
-        self.vectors_1: np.array
-        self.vectors_2: np.array = None
-        self.vector_size: int
-        self.num_of_clusters: int
-        self.top_k: int
-        self._faiss_metric_type = None
-
-    def _tokenize_entity(self, entity: str) -> str:
-        """Produces a list of workds of a given string
-
-        Args:
-            entity (str): String representation  of an entity
-
-        Returns:
-            str: entity string
-        """
-        return entity.strip().lower()#' '.join(list(filter(None, re.split('[\\W_]', entity.lower()))))
-
-    def build_blocks(self,
-                     data: Data,
-                     vector_size: int = 300,
-                     num_of_clusters: int = 5,
-                     top_k: int = 30,
-                     max_word_embeddings_size: int = 256,
-                     attributes_1: list = None,
-                     attributes_2: list = None,
-                     return_vectors: bool = False,
-                     tqdm_disable: bool = False,
-                     save_embeddings: bool = True,
-                     load_embeddings_if_exist: bool = False,
-                     with_entity_matching: bool = False
-    ) -> any:
-        """Main method of the vector based approach. Contains two steps. First an embedding method. \
-            And afterwards a similarity search upon the vectors created in the previous step.
-            Pre-trained schemes are used for the embedding process.
-
-        Args:
-            data (Data): dataset from datamodel
-            vector_size (int, optional): For the Gensim vectorizers. Defaults to 300. \
-                Qaution for the hugging face embeddings has no effect.
-            num_of_clusters (int, optional): Number of clusters for FAISS. Defaults to 5.
-            top_k (int, optional): Top K similar candidates. Defaults to 30.
-            attributes_1 (list, optional): Vectorization of specific attributes for D1. \
-                                            Defaults to None.
-            attributes_2 (list, optional): Vectorization of specific attributes for D2. \
-                                            Defaults to None.
-            return_vectors (bool, optional): If true, returns the vectors created from the pretrained \
-                                            embeddings instead of the blocks. Defaults to False.
-            tqdm_disable (bool, optional): Disable progress bar. For experiment purposes. \
-                                            Defaults to False.
-
-        Raises:
-            AttributeError: Vectorizer check
-            AttributeError: Similarity Search method check.
-
-        Returns:
-            dict: Entity ids to sets of top-K candidate ids. OR
-            Tuple(np.array, np.array): vectors from d1 and vectors from d2
-        """
-        _start_time = time()
-        self.blocks = dict()
-        self.with_entity_matching = with_entity_matching
-        self.save_embeddings, self.load_embeddings_if_exist = save_embeddings, load_embeddings_if_exist
-        self.max_word_embeddings_size = max_word_embeddings_size
-        self.data, self.attributes_1, self.attributes_2, self.vector_size, self.num_of_clusters, self.top_k \
-            = data, attributes_1, attributes_2, vector_size, num_of_clusters, top_k
-        self._progress_bar = tqdm(total=data.num_of_entities,
-                                  desc=(self._method_name + ' [' + self.vectorizer + ', ' + self.similarity_search + ']'),
-                                  disable=tqdm_disable)
-
-        self._si = SubsetIndexer(None, self.data)
-        
-        # print(data.attributes_1, data.attributes_2)
-        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
-                            .apply(" ".join, axis=1) \
-                            .apply(self._tokenize_entity) \
-                            .values.tolist()
-        
-        self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
-                    .apply(" ".join, axis=1) \
-                    .apply(self._tokenize_entity) \
-                    .values.tolist() if not data.is_dirty_er else None
-
-        vectors_1 = []
-        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        print("Device selected: ", self.device)
-
-        if self.with_entity_matching:
-            self.graph = nx.Graph()
-        
-        if load_embeddings_if_exist:
-            try:
-                print("Loading embeddings from file...")
-                
-                p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + self.data.dataset_name_1 \
-                                                    if self.data.dataset_name_1 is not None else "d1" +'_1.npy')
-                print("Loading file: ", p1)
-                self.vectors_1 = vectors_1 = np.load(p1)
-                self._progress_bar.update(data.num_of_entities_1)
-
-                p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + self.data.dataset_name_2 \
-                                                    if self.data.dataset_name_2 is not None else "d2" +'_2.npy')
-                print("Loading file: ", p2)
-                self.vectors_2 = vectors_2 = np.load(p2)
-                self._progress_bar.update(data.num_of_entities_2)
-                
-                print("Loading embeddings from file finished")
-            except:
-                print("Embeddings not found. Creating new ones.")
-                raise ValueError("Embeddings not found.")
-        else:
-            if self.vectorizer in ['word2vec', 'fasttext', 'doc2vec', 'glove']:
-                vectors_1, vectors_2 = self._create_gensim_embeddings()
-            elif self.vectorizer in ['bert', 'distilbert', 'roberta', 'xlnet', 'albert']:
-                vectors_1, vectors_2 = self._create_pretrained_word_embeddings()
-            elif self.vectorizer in ['smpnet', 'st5', 'sent_glove', 'sdistilroberta', 'sminilm']:
-                vectors_1, vectors_2 = self._create_pretrained_sentence_embeddings()
-            else:
-                raise AttributeError("Not available vectorizer")
-
-        if save_embeddings:
-            print("Saving embeddings...")
-            
-            p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + self.data.dataset_name_1 \
-                                                    if self.data.dataset_name_1 is not None else "d1" +'_1.npy')
-            print("Saving file: ", p1)
-            np.save(p1, self.vectors_1)
-            
-            p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + self.data.dataset_name_2 \
-                                                    if self.data.dataset_name_2 is not None else "d2" +'_2.npy')
-            print("Saving file: ", p2)
-            np.save(p2, self.vectors_2)
-
-        if return_vectors:
-            return (vectors_1, _) if data.is_dirty_er else (vectors_1, vectors_2)
-
-        if self.similarity_search == 'faiss':
-            self._faiss_metric_type = faiss.METRIC_L2
-            self._similarity_search_with_FAISS()
-        elif self.similarity_search == 'falconn':
-            raise NotImplementedError("FALCONN")
-        elif self.similarity_search == 'scann'  and LINUX_ENV:
-            self._similarity_search_with_SCANN()
-        else:
-            raise AttributeError("Not available method")
-        self._progress_bar.close()        
-        self.execution_time = time() - _start_time
-
-        if self.with_entity_matching:
-            return self.blocks, self.graph
-        
-        return self.blocks
-
-    def _create_gensim_embeddings(self) -> Tuple[np.array, np.array]:
-        """Embeddings with Gensim. More on https://github.com/RaRe-Technologies/gensim-data
-
-        Args:
-            entities_d1 (list): Entities from D1
-            entities_d2 (list, optional): Entities from D2 (CCER). Defaults to None.
-
-        Returns:
-            Tuple[np.array, np.array]: Embeddings from D1 and D2
-        """
-        vectors_1 = []
-        vocabulary = api.load(self._gensim_mapping_download[self.vectorizer])
-        for e1 in self._entities_d1:
-            vectors_1.append(self._create_vector(e1, vocabulary))
-            self._progress_bar.update(1)
-        self.vectors_1 = np.array(vectors_1).astype('float32')
-
-        vectors_2 = []
-        if not self.data.is_dirty_er:
-            for e2 in self._entities_d2:
-                vectors_2.append(self._create_vector(e2, vocabulary))
-                self._progress_bar.update(1)
-            self.vectors_2 = np.array(vectors_2).astype('float32')
-
-        return vectors_1, vectors_2
-
-    def _create_pretrained_word_embeddings(self) -> Tuple[np.array, np.array]:
-        if self.vectorizer == 'bert':
-            tokenizer = BertTokenizer.from_pretrained('bert-base-uncased')
-            model = BertModel.from_pretrained("bert-base-uncased")
-        elif self.vectorizer == 'distilbert':
-            tokenizer = DistilBertTokenizer.from_pretrained('distilbert-base-uncased')
-            model = DistilBertModel.from_pretrained("distilbert-base-uncased")
-        elif self.vectorizer == 'roberta':
-            tokenizer = RobertaTokenizer.from_pretrained('roberta-base')
-            model = RobertaModel.from_pretrained('roberta-base')
-        elif self.vectorizer == 'xlnet':
-            tokenizer = XLNetTokenizer.from_pretrained('xlnet-base-cased')
-            model = XLNetModel.from_pretrained('xlnet-base-cased')
-        elif self.vectorizer == 'albert':
-            tokenizer = AlbertTokenizer.from_pretrained('albert-base-v2')
-            model = AlbertModel.from_pretrained("albert-base-v2")
-
-        model = model.to(self.device)
-        self.vectors_1 = self._transform_entities_to_word_embeddings(self._entities_d1,
-                                                                     model,
-                                                                     tokenizer)
-        self.vector_size = self.vectors_1[0].shape[0]
-        print("Vector size: ", self.vectors_1.shape)
-        self.vectors_2 = self._transform_entities_to_word_embeddings(self._entities_d2,
-                                                                     model,
-                                                                     tokenizer) if not self.data.is_dirty_er else None
-        return self.vectors_1, self.vectors_2
-
-
-    def _transform_entities_to_word_embeddings(self, entities, model, tokenizer) -> np.array:
-    
-        model = model.to(self.device)
-        embeddings = []
-        
-        for entity in entities:
-            encoded_input = tokenizer(entity,
-                                        return_tensors='pt',
-                                        truncation=True,
-                                        return_attention_mask = True,
-                                        max_length=self.max_word_embeddings_size,
-                                        padding='max_length')
-
-            encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
-
-            with torch.no_grad():
-                encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
-                output = model(**encoded_input)
-                vector = output.last_hidden_state[:, 0, :]
-                
-            vector = vector.cpu().numpy()
-            embeddings.append(vector.reshape(-1))
-            self._progress_bar.update(1)
-        
-        self.vector_size = embeddings[0].shape[0]
-        return np.array(embeddings).astype('float32')
-
-    def _create_pretrained_sentence_embeddings(self):
-        model = SentenceTransformer(self._sentence_transformer_mapping[self.vectorizer],
-                                    device=self.device)
-        vectors_1 = []
-        for e1 in self._entities_d1:
-            vector = model.encode(e1)
-            vectors_1.append(vector)
-            self._progress_bar.update(1)
-        self.vector_size = len(vectors_1[0])
-        self.vectors_1 = np.array(vectors_1).astype('float32')
-        vectors_2 = []
-        if not self.data.is_dirty_er:
-            for e2 in self._entities_d2:
-                vector = model.encode(e2)
-                vectors_2.append(vector)
-                self._progress_bar.update(1)
-            self.vector_size = len(vectors_2[0])
-            self.vectors_2 = np.array(vectors_2).astype('float32')
-
-        return vectors_1, vectors_2
-
-    def _similarity_search_with_FAISS(self):
-        index = faiss.IndexFlatL2(self.vectors_1.shape[1])
-        index.metric_type = faiss.METRIC_INNER_PRODUCT
-        index.train(self.vectors_1)  # train on the vectors of dataset 1
-        index.add(self.vectors_1)   # add the vectors and update the index
-
-        self.distances, self.neighbors = index.search(self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
-                                                      self.top_k)
-        
-        self.blocks = dict()
-        
-        for i in range(0, self.neighbors.shape[0]):
-            if self.data.is_dirty_er:
-                entity_id_d2 = i
-            else:
-                entity_id_d2 = i + self.data.dataset_limit
-            
-            if entity_id_d2 not in self.blocks.keys():
-                self.blocks[entity_id_d2] = set()            
-            
-            j = 0
-            for entity_id_d1 in self.neighbors[i]:
-
-                if entity_id_d1 == -1:
-                    continue
-                
-                if entity_id_d1 not in self.blocks.keys():
-                    self.blocks[entity_id_d1] = set()
-
-                self.blocks[entity_id_d1].add(entity_id_d2)
-                self.blocks[entity_id_d2].add(entity_id_d1)
-                
-                if self.with_entity_matching:
-                    self.graph.add_edge(entity_id_d2, entity_id_d1, weight=self.distances[i][j])
-
-                j += 1
-
-
-    def _similarity_search_with_FALCONN(self):
-        pass
-
-    def _similarity_search_with_SCANN(self):
-        if not LINUX_ENV:
-            raise ImportError("Can't use SCANN in windows environment. Use FAISS instead.")
-
-        searcher = scann.scann_ops_pybind.builder(self.vectors_1,
-                                                    num_neighbors=self.top_k, 
-                                                    distance_measure="dot_product") \
-                                        .tree(num_leaves=2000, num_leaves_to_search=100, training_sample_size=250000) \
-                                        .score_ah(2, anisotropic_quantization_threshold=0.2) \
-                                        .reorder(100) \
-                                        .build()
-
-        self.neighbors, self.distances = searcher.search_batched(
-            self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
-            final_num_neighbors=self.top_k
-        )
-        if self.data.is_dirty_er:
-            self.blocks = {
-                self._si.d1_retained_ids[i] : set(x for x in self.neighbors[i] if x not in [-1, i]) \
-                        for i in range(0, self.neighbors.shape[0])
-            }
-        else:
-            self.blocks = {
-                self._si.d2_retained_ids[i] : set(x for x in self.neighbors[i] if x != -1) \
-                        for i in range(0, self.neighbors.shape[0])
-            }
-
-    def _create_vector(self, tokens: List[str], vocabulary) -> np.array:
-        num_of_tokens = 0
-        vector = np.zeros(self.vector_size)
-        for token in tokens.split():
-            if token in vocabulary:
-                vector += vocabulary[token]
-                num_of_tokens += 1
-        if num_of_tokens > 0:
-            vector /= num_of_tokens
-
-        return vector
-
-    def evaluate(self,
-                 prediction,
-                 export_to_df: bool = False,
-                 export_to_dict: bool = False,
-                 with_classification_report: bool = False,
-                 verbose: bool = True,
-                 with_stats: bool = False) -> any:
-
-        if self.data is None:
-            raise AttributeError("Can not proceed to evaluation without data object.")
-
-        if self.data.ground_truth is None:
-            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
-                    "Data object has not been initialized with the ground-truth file")
-
-        eval_obj = Evaluation(self.data)
-        true_positives = 0
-        total_matching_pairs = sum([len(block) for block in prediction.values()])
-        for _, (id1, id2) in self.data.ground_truth.iterrows():
-            id1 = self.data._ids_mapping_1[id1]
-            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
-                                                else self.data._ids_mapping_2[id2]
-            if (id1 in prediction and id2 in prediction[id1]) or   \
-                (id2 in prediction and id1 in prediction[id2]):
-                true_positives += 1
-
-        eval_obj.calculate_scores(true_positives=true_positives, 
-                                  total_matching_pairs=total_matching_pairs)
-        evaluation = eval_obj.report(self.method_configuration(),
-                                export_to_df,
-                                export_to_dict,
-                                with_classification_report,
-                                verbose)
-
-        if with_stats:
-            self.stats()
-
-        return evaluation
-
-    def _configuration(self) -> dict:
-        return {
-            "Vectorizer" : self.vectorizer,
-            "Similarity-Search" : self.similarity_search,
-            "Top-K" : self.top_k,
-            "Vector size": self.vector_size
-        }
-    
-    def stats(self) -> None:
-        print("Statistics:")
-        if self.similarity_search == 'faiss':
-            print(" FAISS:" +
-                # "\n\tNumber of entries in each list:  " + str(self._faiss_num_lists) + 
-                "\n\tIndices shape returned after search: " + str(self.neighbors.shape)
-            )
-        elif self.similarity_search == 'falconn':           
-            pass
-        elif self.similarity_search == 'scann'  and LINUX_ENV:
-            pass
-        
-        print(u'\u2500' * 123)
-        
-class PREmbeddingsNNBlockBuilding(EmbeddingsNNBlockBuilding):
-    """Block building via creation of embeddings and a Nearest Neighbor Approach with specified budget
-    """
-
-    _method_name = "Progressive Embeddings-NN Block Building"
-    _method_info = "Creates a set of candidate pairs for every entity id " + \
-        "based on Progresssive Similarity Search over the entity embeddings neighborhood"
-
-    def __init__(
-            self,
-            vectorizer: str,
-            similarity_search: str,
-            budget: int
-    ) -> None:
-        super().__init__(vectorizer, similarity_search)
-        self._budget = budget
-        self.vectorizer, self.similarity_search = vectorizer, similarity_search
-        self.embeddings: np.array
-        self.vectors_1: np.array
-        self.vectors_2: np.array = None
-        self.vector_size: int
-        self.num_of_clusters: int
-        self.top_k: int
-
-    def precomputed_vectors(self,
-                    data: Data,
-                    vectors_1: np.array = None,
-                    vectors_2: np.array = None
-    ) -> bool:
-
-        if(not vectors_1):
-            return False
-
-        if(not data.is_dirty_er):
-            return vectors_2 is not None
-
-        return True
-
-    def build_blocks(self,
-                     data: Data,
-                     cc_blocks: dict = None,
-                     vectors_1: np.array = None,
-                     vectors_2: np.array = None, 
-                     vector_size: int = 300,
-                     num_of_clusters: int = 5,
-                     top_k: int = 30,
-                     max_word_embeddings_size: int = 256,
-                     attributes_1: list = None,
-                     attributes_2: list = None,
-                     return_vectors: bool = False,
-                     tqdm_disable: bool = True
-    ) -> any:
-        """Retrieves the entities retained after the last step, produces/retrieves their embeddings and applies popular NN neighbor techniques
-           to produce pair candidates
-        Args:
-            data (Data): Data Module
-            cc_blocks (dict, optional): Blocks, subset of the initial dataset retrieved from the last CC step. Defaults to None.
-            vectors_1 (np.array, optional): Precalculated embeddings of entities of dataset 1. Defaults to None.
-            vectors_2 (np.array, optional): Precalculated embeddings of entities of dataset 2. Defaults to None.
-            vector_size (int, optional): The size of the embeddings. Defaults to 300.
-            num_of_clusters (int, optional): The number of clusters. Defaults to 5.
-            top_k (int, optional): The number of candidates that will be produced per entity. Defaults to 30.
-            attributes_1 (list, optional): Attributes of entities in dataset 1 that we want to take into consideration. Defaults to None.
-            attributes_2 (list, optional): Attributes of entities in dataset 2 that we want to take into consideration. Defaults to None.
-            return_vectors (bool, optional): If true, returns the entities vector embeddings. Defaults to True.
-            tqdm_disable (bool, optional): Disable progress bar. For experiment purposes. Defaults to False.
-        Returns:
-            any: Blocks produced by Vector Based BB, vector distances and entity embeddings
-        """
-        _start_time = time()
-        self.blocks = dict()
-        self.max_word_embeddings_size = max_word_embeddings_size
-        self.data, self.attributes_1, self.attributes_2, self.vector_size, self.num_of_clusters, self.top_k \
-            = data, attributes_1, attributes_2, vector_size, num_of_clusters, top_k
-        self._progress_bar = tqdm(total=data.num_of_entities,
-                                  desc=self._method_name,
-                                  disable=tqdm_disable)
-
-        self._si = SubsetIndexer(cc_blocks, self.data)
-        self._d1_valid_indices: list[int] = self._si.d1_retained_ids
-        self._d2_valid_indices: list[int] = [x - self.data.dataset_limit for x in self._si.d2_retained_ids]       
-
-
-        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
-                            .apply(" ".join, axis=1) \
-                            .apply(self._tokenize_entity) \
-                            .values.tolist()
-        self._entities_d1 = [self._entities_d1[x] for x in self._d1_valid_indices]
-                            
-                            
-        self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
-                            .apply(" ".join, axis=1) \
-                            .apply(self._tokenize_entity) \
-                            .values.tolist() if not data.is_dirty_er else None
-        self._entities_d2 = [self._entities_d2[x] for x in self._d2_valid_indices] if not data.is_dirty_er else None
-                                               
-
-        self.vectors_1 = vectors_1
-        self.vectors_2 = vectors_2
-        self.create_vectors()
-        if(return_vectors): return self.vectors_1, self.vectors_2       
-        self.blocks = self.create_blocks()
-        self._progress_bar.close()
-        self.execution_time = time() - _start_time
-
-        return self.blocks
-
-    def create_vectors(self):      
-
-        if(self.precomputed_vectors(data = self.data)):
-            self.vectors_1 = self.vectors_1[self._d1_valid_indices]
-
-            if(not self.data.is_dirty_er):
-                self.vectors_2 = self.vectors_2[self._d2_valid_indices]
-        else:
-            self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-            print("Device selected: ", self.device)
-            
-            if self.vectorizer in ['word2vec', 'fasttext', 'doc2vec', 'glove']:
-                vectors_1, vectors_2 = self._create_gensim_embeddings()
-            elif self.vectorizer in ['bert', 'distilbert', 'roberta', 'xlnet', 'albert']:
-                vectors_1, vectors_2 = self._create_pretrained_word_embeddings()
-            elif self.vectorizer in ['smpnet', 'st5', 'glove', 'sdistilroberta', 'sminilm']:
-                vectors_1, vectors_2 = self._create_pretrained_sentence_embeddings()
-            else:
-                raise AttributeError("Not available vectorizer")
-        
-        self.vectors_1 = vectors_1
-        self.vectors_2 = vectors_2
-
-    def create_blocks(self):
-        if self.similarity_search == 'faiss':
-            self._similarity_search_with_FAISS()
-        elif self.similarity_search == 'falconn':
-            raise NotImplementedError("FALCONN")
-        elif self.similarity_search == 'scann'  and LINUX_ENV:
-            self._similarity_search_with_SCANN()
-        else:
-            raise AttributeError("Not available method")
-        return self.blocks
+'''
+Contains all methods for creating embeddings from text 
+and then performing NNs methods for cluster formation.
+'''
+import os
+import pickle
+import re
+import sys
+import warnings
+from time import time
+from typing import List, Tuple
+
+import faiss
+import gensim.downloader as api
+import networkx as nx
+import numpy as np
+import torch
+import transformers
+from sentence_transformers import SentenceTransformer
+from tqdm.autonotebook import tqdm
+from transformers import (AlbertModel, AlbertTokenizer, BertModel,
+                          BertTokenizer, DistilBertModel, DistilBertTokenizer,
+                          RobertaModel, RobertaTokenizer, XLNetModel,
+                          XLNetTokenizer)
+
+transformers.logging.set_verbosity_error()
+from faiss import normalize_L2
+
+from .datamodel import Data, PYJEDAIFeature
+from .evaluation import Evaluation
+from .utils import SubsetIndexer
+
+EMBEDDINGS_DIR = '.embeddings'
+if not os.path.exists(EMBEDDINGS_DIR):
+    os.makedirs(EMBEDDINGS_DIR)
+    EMBEDDINGS_DIR = os.path.abspath(EMBEDDINGS_DIR)
+    print('Created embeddings directory at: ' + EMBEDDINGS_DIR)
+
+LINUX_ENV=False
+# try:
+#     if 'linux' in sys.platform:
+#         import falconn
+#         import scann
+#         LINUX_ENV=True
+# except:
+#     warnings.warn(ImportWarning, "Can't use FALCONN/SCANN in windows environment")
+
+class EmbeddingsNNBlockBuilding(PYJEDAIFeature):
+    """Block building via creation of embeddings and a Nearest Neighbor Approach.
+    """
+
+    _method_name = "Embeddings-NN Block Building"
+    _method_info = "Creates a set of candidate pais for every entity id " + \
+        "based on Embeddings creariot and Similarity search among the vectors."
+
+    _gensim_mapping_download = {
+        'fasttext' : 'fasttext-wiki-news-subwords-300',
+        'glove' : 'glove-wiki-gigaword-300',
+        'word2vec' : 'word2vec-google-news-300'
+    }
+    _sentence_transformer_mapping = {
+        'smpnet' : 'all-mpnet-base-v2',
+        'st5' : 'gtr-t5-large',
+        'sdistilroberta' : 'all-distilroberta-v1',
+        'sminilm' : 'all-MiniLM-L12-v2',
+        'sent_glove' : 'average_word_embeddings_glove.6B.300d'
+    }
+
+    def __init__(
+            self,
+            vectorizer: str,
+            similarity_search: str
+    ) -> None:
+        super().__init__()
+        self.vectorizer, self.similarity_search = vectorizer, similarity_search
+        self.embeddings: np.array
+        self.vectors_1: np.array
+        self.vectors_2: np.array = None
+        self.vector_size: int
+        self.num_of_clusters: int
+        self.top_k: int
+        self._faiss_metric_type = None
+
+    def _tokenize_entity(self, entity: str) -> str:
+        """Produces a list of workds of a given string
+
+        Args:
+            entity (str): String representation  of an entity
+
+        Returns:
+            str: entity string
+        """
+        return entity.strip().lower()#' '.join(list(filter(None, re.split('[\\W_]', entity.lower()))))
+
+    def build_blocks(self,
+                     data: Data,
+                     vector_size: int = 300,
+                     num_of_clusters: int = 5,
+                     top_k: int = 30,
+                     max_word_embeddings_size: int = 256,
+                     attributes_1: list = None,
+                     attributes_2: list = None,
+                     return_vectors: bool = False,
+                     tqdm_disable: bool = False,
+                     save_embeddings: bool = True,
+                     load_embeddings_if_exist: bool = False,
+                     with_entity_matching: bool = False,
+                     input_cleaned_blocks: dict = None,
+                     similarity_distance: str = 'cosine'
+    ) -> any:
+        """Main method of the vector based approach. Contains two steps. First an embedding method. \
+            And afterwards a similarity search upon the vectors created in the previous step.
+            Pre-trained schemes are used for the embedding process.
+
+        Args:
+            data (Data): dataset from datamodel
+            vector_size (int, optional): For the Gensim vectorizers. Defaults to 300. \
+                Qaution for the hugging face embeddings has no effect.
+            num_of_clusters (int, optional): Number of clusters for FAISS. Defaults to 5.
+            top_k (int, optional): Top K similar candidates. Defaults to 30.
+            attributes_1 (list, optional): Vectorization of specific attributes for D1. \
+                                            Defaults to None.
+            attributes_2 (list, optional): Vectorization of specific attributes for D2. \
+                                            Defaults to None.
+            return_vectors (bool, optional): If true, returns the vectors created from the pretrained \
+                                            embeddings instead of the blocks. Defaults to False.
+            tqdm_disable (bool, optional): Disable progress bar. For experiment purposes. \
+                                            Defaults to False.
+
+        Raises:
+            AttributeError: Vectorizer check
+            AttributeError: Similarity Search method check.
+
+        Returns:
+            dict: Entity ids to sets of top-K candidate ids. OR
+            Tuple(np.array, np.array): vectors from d1 and vectors from d2
+        """
+        print('Building blocks via Embeddings-NN Block Building [' + self.vectorizer + ', ' + self.similarity_search + ']')
+        _start_time = time()
+        self.blocks = dict()
+        self.with_entity_matching = with_entity_matching
+        self.save_embeddings, self.load_embeddings_if_exist = save_embeddings, load_embeddings_if_exist
+        self.max_word_embeddings_size = max_word_embeddings_size
+        self.simiarity_distance = similarity_distance
+        self.data, self.attributes_1, self.attributes_2, self.vector_size, self.num_of_clusters, self.top_k, self.input_cleaned_blocks \
+            = data, attributes_1, attributes_2, vector_size, num_of_clusters, top_k, input_cleaned_blocks
+        self._progress_bar = tqdm(total=data.num_of_entities,
+                                  desc=(self._method_name + ' [' + self.vectorizer + ', ' + self.similarity_search + ']'),
+                                  disable=tqdm_disable)
+
+            
+        if(input_cleaned_blocks == None):
+            self._applied_to_subset = False
+        else:
+            _all_blocks = list(input_cleaned_blocks.values())
+            if 'Block' in str(type(_all_blocks[0])):
+                self._applied_to_subset = False
+            elif isinstance(_all_blocks[0], set):
+                self._applied_to_subset = True
+            else:
+                raise AttributeError("Wrong type of blocks given")
+
+        self._si = SubsetIndexer(self.input_cleaned_blocks, self.data, self._applied_to_subset)
+        self._d1_valid_indices: list[int] = self._si.d1_retained_ids
+        self._d2_valid_indices: list[int] = [x - self.data.dataset_limit for x in self._si.d2_retained_ids]   
+
+        self._entities_d1 = data.dataset_1[attributes_1 if attributes_1 else data.attributes_1] \
+                            .apply(" ".join, axis=1) \
+                            .apply(self._tokenize_entity) \
+                            .values.tolist()
+        self._entities_d1 = [self._entities_d1[x] for x in self._d1_valid_indices]
+        self._entities_d2 = data.dataset_2[attributes_2 if attributes_2 else data.attributes_2] \
+                    .apply(" ".join, axis=1) \
+                    .apply(self._tokenize_entity) \
+                    .values.tolist() if not data.is_dirty_er else None
+        self._entities_d2 = [self._entities_d2[x] for x in self._d2_valid_indices] if not data.is_dirty_er else None
+
+        self.vectors_1 = None
+        self.vectors_2 = None
+        self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        print("Device selected: ", self.device)
+        
+        if self.with_entity_matching:
+            self.graph = nx.Graph()
+        
+        self._d1_loaded : bool = False
+        self._d2_loaded : bool = False
+        if load_embeddings_if_exist:
+                print("Loading embeddings from file...")
+                
+                p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_1 \
+                                                    if self.data.dataset_name_1 is not None else "d1") +'.npy')
+                print("Loading file: ", p1)
+                if os.path.exists(p1):
+                    self.vectors_1 = vectors_1 = np.load(p1)
+                    self.vectors_1 = vectors_1 = vectors_1[self._d1_valid_indices]
+                    self._progress_bar.update(data.num_of_entities_1)
+                    self._d1_loaded = True
+                else:
+                    print("Embeddings not found. Creating new ones.")
+                
+                p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_2 \
+                                                    if self.data.dataset_name_2 is not None else "d2") +'.npy')    
+                print("Loading file: ", p2)
+                if os.path.exists(p2):
+                    self.vectors_2 = vectors_2 = np.load(p2)
+                    self.vectors_2 = vectors_2 = vectors_2[self._d2_valid_indices]
+                    self._progress_bar.update(data.num_of_entities_2)
+                    self._d2_loaded = True
+                else:
+                    print("Embeddings not found. Creating new ones.")
+                print("Loading embeddings from file finished")
+        if not self._d1_loaded or not self._d2_loaded:
+            if self.vectorizer in ['word2vec', 'fasttext', 'doc2vec', 'glove']:
+                self.vectors_1, self.vectors_2 = self._create_gensim_embeddings()
+            elif self.vectorizer in ['bert', 'distilbert', 'roberta', 'xlnet', 'albert']:
+                self.vectors_1, self.vectors_2 = self._create_pretrained_word_embeddings()
+            elif self.vectorizer in ['smpnet', 'st5', 'sent_glove', 'sdistilroberta', 'sminilm']:
+                self.vectors_1, self.vectors_2 = self._create_pretrained_sentence_embeddings()
+            else:
+                raise AttributeError("Not available vectorizer")
+            
+        if save_embeddings:
+            print("Saving embeddings...")
+            
+            if self._applied_to_subset:
+                print("Cannot save embeddings, subset embeddings storing not supported.")
+            else:
+                if not self._d1_loaded:
+                    p1 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_1 \
+                                                            if self.data.dataset_name_1 is not None else "d1") +'.npy')
+                    print("Saving file: ", p1)
+                    np.save(p1, self.vectors_1)
+                
+                if not self._d2_loaded:
+                    p2 = os.path.join(EMBEDDINGS_DIR, self.vectorizer + '_' + (self.data.dataset_name_2 \
+                                                            if self.data.dataset_name_2 is not None else "d2") +'.npy')
+                    print("Saving file: ", p2)
+                    np.save(p2, self.vectors_2)
+
+        if return_vectors:
+            return (self.vectors_1, _) if data.is_dirty_er else (self.vectors_1, self.vectors_2)
+
+        if self.similarity_search == 'faiss':
+            self._faiss_metric_type = faiss.METRIC_L2
+            self._similarity_search_with_FAISS()
+        elif self.similarity_search == 'falconn':
+            raise NotImplementedError("FALCONN")
+        elif self.similarity_search == 'scann'  and LINUX_ENV:
+            self._similarity_search_with_SCANN()
+        else:
+            raise AttributeError("Not available method")
+        self._progress_bar.close()        
+        self.execution_time = time() - _start_time
+        
+        if self.with_entity_matching:
+            return self.blocks, self.graph
+        else:
+            return self.blocks
+
+    def _create_gensim_embeddings(self) -> Tuple[np.array, np.array]:
+        """Embeddings with Gensim. More on https://github.com/RaRe-Technologies/gensim-data
+
+        Args:
+            entities_d1 (list): Entities from D1
+            entities_d2 (list, optional): Entities from D2 (CCER). Defaults to None.
+
+        Returns:
+            Tuple[np.array, np.array]: Embeddings from D1 and D2
+        """
+        vectors_1 = []
+        vocabulary = api.load(self._gensim_mapping_download[self.vectorizer])
+        
+        if not self._d1_loaded:
+            for e1 in self._entities_d1:
+                vectors_1.append(self._create_vector(e1, vocabulary))
+                self._progress_bar.update(1)
+            vectors_1 = np.vstack(vectors_1).astype('float32')
+
+        vectors_2 = []
+        if not self.data.is_dirty_er and not self._d2_loaded:
+            for e2 in self._entities_d2:
+                vectors_2.append(self._create_vector(e2, vocabulary))
+                self._progress_bar.update(1)
+            vectors_2 = np.vstack(vectors_2).astype('float32')
+
+        return vectors_1, vectors_2
+
+    def _create_pretrained_word_embeddings(self) -> Tuple[np.array, np.array]:
+        if self.vectorizer == 'bert':
+            tokenizer = BertTokenizer.from_pretrained('bert-base-uncased')
+            model = BertModel.from_pretrained("bert-base-uncased")
+        elif self.vectorizer == 'distilbert':
+            tokenizer = DistilBertTokenizer.from_pretrained('distilbert-base-uncased')
+            model = DistilBertModel.from_pretrained("distilbert-base-uncased")
+        elif self.vectorizer == 'roberta':
+            tokenizer = RobertaTokenizer.from_pretrained('roberta-base')
+            model = RobertaModel.from_pretrained('roberta-base')
+        elif self.vectorizer == 'xlnet':
+            tokenizer = XLNetTokenizer.from_pretrained('xlnet-base-cased')
+            model = XLNetModel.from_pretrained('xlnet-base-cased')
+        elif self.vectorizer == 'albert':
+            tokenizer = AlbertTokenizer.from_pretrained('albert-base-v2')
+            model = AlbertModel.from_pretrained("albert-base-v2")
+
+        model = model.to(self.device)
+        self.vectors_1 = self._transform_entities_to_word_embeddings(self._entities_d1,
+                                                                     model,
+                                                                     tokenizer) if not self._d1_loaded else self.vectors_1
+        self.vector_size = self.vectors_1[0].shape[0]
+        print("Vector size: ", self.vectors_1.shape)
+        self.vectors_2 = self._transform_entities_to_word_embeddings(self._entities_d2,
+                                                                     model,
+                                                                     tokenizer) if not self.data.is_dirty_er and not self._d2_loaded else self.vectors_2
+        return self.vectors_1, self.vectors_2
+
+    def _transform_entities_to_word_embeddings(self, entities, model, tokenizer) -> np.array:
+    
+        model = model.to(self.device)
+        embeddings = []
+        
+        for entity in entities:
+            encoded_input = tokenizer(entity,
+                                        return_tensors='pt',
+                                        truncation=True,
+                                        return_attention_mask = True,
+                                        max_length=self.max_word_embeddings_size,
+                                        padding='max_length')
+
+            encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
+
+            with torch.no_grad():
+                encoded_input = {key: value.to(self.device) for key, value in encoded_input.items()}  # Move input tensors to GPU
+                output = model(**encoded_input)
+                vector = output.last_hidden_state[:, 0, :]
+                
+            vector = vector.cpu().numpy()
+            embeddings.append(vector.reshape(-1))
+            self._progress_bar.update(1)
+        
+        self.vector_size = embeddings[0].shape[0]
+        return np.array(embeddings).astype('float32')
+
+    def _create_pretrained_sentence_embeddings(self):
+        model = SentenceTransformer(self._sentence_transformer_mapping[self.vectorizer],
+                                    device=self.device)
+        vectors_1 = []
+        if not self._d1_loaded:
+            for e1 in self._entities_d1:
+                vector = model.encode(e1)
+                vectors_1.append(vector)
+                self._progress_bar.update(1)
+            self.vector_size = len(vectors_1[0])
+            vectors_1 = np.vstack(vectors_1).astype('float32')
+        vectors_2 = []
+        if not self.data.is_dirty_er and not self._d2_loaded:            
+            for e2 in self._entities_d2:
+                # print("e2: ", e2)
+                vector = model.encode(e2)
+                vectors_2.append(vector)
+                self._progress_bar.update(1)
+            self.vector_size = len(vectors_2[0])
+            vectors_2 = np.vstack(vectors_2).astype('float32')
+            
+        return vectors_1, vectors_2 
+
+    def _similarity_search_with_FAISS(self):
+        index = faiss.IndexFlatL2(self.vectors_1.shape[1])
+        
+        if self.simiarity_distance == 'cosine' or self.simiarity_distance == 'cosine_without_normalization':
+            index.metric_type = faiss.METRIC_INNER_PRODUCT
+        elif self.simiarity_distance == 'euclidean':
+            index.metric_type = faiss.METRIC_L2
+        else:
+            raise ValueError("Invalid similarity distance: ", self.simiarity_distance)
+
+        if self.simiarity_distance == 'cosine':
+            faiss.normalize_L2(self.vectors_1)
+            faiss.normalize_L2(self.vectors_2)
+            
+        index.train(self.vectors_1)  # train on the vectors of dataset 1
+
+        if self.simiarity_distance == 'cosine':
+            faiss.normalize_L2(self.vectors_1)
+            faiss.normalize_L2(self.vectors_2)
+
+        index.add(self.vectors_1)   # add the vectors and update the index
+
+        if self.simiarity_distance == 'cosine':
+            faiss.normalize_L2(self.vectors_1)
+            faiss.normalize_L2(self.vectors_2)
+        
+        self.distances, self.neighbors = index.search(self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
+                                    self.top_k)
+        
+        self.blocks = dict()
+        
+        for _entity in range(0, self.neighbors.shape[0]):
+            
+            _entity_id = self._si.d1_retained_ids[_entity] if self.data.is_dirty_er else self._si.d2_retained_ids[_entity]
+            
+            if _entity_id not in self.blocks:
+                self.blocks[_entity_id] = set()            
+            
+            for _neighbor_index, _neighbor in enumerate(self.neighbors[_entity]):
+
+                if _neighbor == -1:
+                    continue
+                
+                _neighbor_id = self._si.d1_retained_ids[_neighbor]
+                
+                if _neighbor_id not in self.blocks:
+                    self.blocks[_neighbor_id] = set()
+
+                self.blocks[_neighbor_id].add(_entity_id)
+                self.blocks[_entity_id].add(_neighbor_id)
+                
+                if self.with_entity_matching:
+                    self.graph.add_edge(_entity_id, _neighbor_id, weight=self.distances[_entity][_neighbor_index])
+
+    def _similarity_search_with_FALCONN(self):
+        pass
+
+    def _similarity_search_with_SCANN(self):
+        if not LINUX_ENV:
+            raise ImportError("Can't use SCANN in windows environment. Use FAISS instead.")
+
+        searcher = scann.scann_ops_pybind.builder(self.vectors_1,
+                                                    num_neighbors=self.top_k, 
+                                                    distance_measure="dot_product") \
+                                        .tree(num_leaves=2000, num_leaves_to_search=100, training_sample_size=250000) \
+                                        .score_ah(2, anisotropic_quantization_threshold=0.2) \
+                                        .reorder(100) \
+                                        .build()
+
+        self.neighbors, self.distances = searcher.search_batched(
+            self.vectors_1 if self.data.is_dirty_er else self.vectors_2,
+            final_num_neighbors=self.top_k
+        )
+        if self.data.is_dirty_er:
+            self.blocks = {
+                self._si.d1_retained_ids[i] : set(x for x in self.neighbors[i] if x not in [-1, i]) \
+                        for i in range(0, self.neighbors.shape[0])
+            }
+        else:
+            self.blocks = {
+                self._si.d2_retained_ids[i] : set(x for x in self.neighbors[i] if x != -1) \
+                        for i in range(0, self.neighbors.shape[0])
+            }
+
+    def _create_vector(self, tokens: List[str], vocabulary) -> np.array:
+        num_of_tokens = 0
+        vector = np.zeros(self.vector_size)
+        for token in tokens.split():
+            if token in vocabulary:
+                vector += vocabulary[token]
+                num_of_tokens += 1
+        if num_of_tokens > 0:
+            vector /= num_of_tokens
+
+        return vector
+
+    def evaluate(self,
+                 prediction,
+                 export_to_df: bool = False,
+                 export_to_dict: bool = False,
+                 with_classification_report: bool = False,
+                 verbose: bool = True,
+                 with_stats: bool = False) -> any:
+
+        if self.data is None:
+            raise AttributeError("Can not proceed to evaluation without data object.")
+
+        if self.data.ground_truth is None:
+            raise AttributeError("Can not proceed to evaluation without a ground-truth file. " +
+                    "Data object has not been initialized with the ground-truth file")
+
+        eval_obj = Evaluation(self.data)
+        true_positives = 0
+        total_matching_pairs = sum([len(block) for block in prediction.values()])
+        for _, (id1, id2) in self.data.ground_truth.iterrows():
+            id1 = self.data._ids_mapping_1[id1]
+            id2 = self.data._ids_mapping_1[id2] if self.data.is_dirty_er \
+                                                else self.data._ids_mapping_2[id2]
+            if (id1 in prediction and id2 in prediction[id1]) or   \
+                (id2 in prediction and id1 in prediction[id2]):
+                true_positives += 1
+
+        eval_obj.calculate_scores(true_positives=true_positives, 
+                                  total_matching_pairs=total_matching_pairs)
+        evaluation = eval_obj.report(self.method_configuration(),
+                                export_to_df,
+                                export_to_dict,
+                                with_classification_report,
+                                verbose)
+        
+        if with_stats:
+            self.stats()
+
+        return evaluation
+
+        if with_stats:
+            self.stats()
+
+        return evaluation
+
+    def _configuration(self) -> dict:
+        return {
+            "Vectorizer" : self.vectorizer,
+            "Similarity-Search" : self.similarity_search,
+            "Top-K" : self.top_k,
+            "Vector size": self.vector_size
+        }
+    
+    def stats(self) -> None:
+        print("Statistics:")
+        if self.similarity_search == 'faiss':
+            print(" FAISS:" +
+                # "\n\tNumber of entries in each list:  " + str(self._faiss_num_lists) + 
+                "\n\tIndices shape returned after search: " + str(self.neighbors.shape)
+            )
+        elif self.similarity_search == 'falconn':           
+            pass
+        elif self.similarity_search == 'scann'  and LINUX_ENV:
+            pass
+        
+        print(u'\u2500' * 123)
```

### Comparing `pyjedai-0.0.6/src/pyjedai/visualization.py` & `pyjedai-0.0.7/src/pyjedai/visualization.py`

 * *Files identical despite different names*

### Comparing `pyjedai-0.0.6/src/pyjedai/workflow.py` & `pyjedai-0.0.7/src/pyjedai/workflow.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,590 +1,590 @@
-from abc import ABC
-from itertools import count
-from time import time
-from typing import Callable, List, Tuple
-
-import matplotlib.pyplot as plt
-import optuna
-import pandas as pd
-from networkx import Graph
-# import plotly.express as px
-from tqdm.autonotebook import tqdm
-
-from .datamodel import Data
-from .evaluation import Evaluation, write
-from .block_building import StandardBlocking
-from .block_cleaning import BlockFiltering, BlockPurging
-from .comparison_cleaning import CardinalityNodePruning
-from .matching import EntityMatching
-from .clustering import ConnectedComponentsClustering, UniqueMappingClustering
-
-plt.style.use('seaborn-whitegrid')
-
-class WorkFlow(ABC):
-    """Main module of the pyjedAI and the simplest way to create an end-to-end ER workflow.
-    """
-
-    _id = count()
-
-    def __init__(
-            self,
-            block_building: dict = None,
-            entity_matching: dict = None,
-            block_cleaning: dict = None,
-            comparison_cleaning: dict = None,
-            clustering: dict = None,
-            joins: dict = None,
-            name: str = None
-    ) -> None:
-        self.block_cleaning, self.block_building, self.comparison_cleaning, \
-            self.clustering, self.joins, self.entity_matching = \
-            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
-        self.f1: list = []
-        self.recall: list = []
-        self.precision: list = []
-        self.runtime: list = []
-        self.configurations: list = []
-        self.workflow_exec_time: float
-        self._id: int = next(self._id)
-        self.name: str = name if name else "Workflow-" + str(self._id)
-        self._workflow_bar: tqdm
-        self.final_pairs = None
-
-    def run(self,
-            data: Data,
-            verbose: bool = False,
-            with_classification_report: bool = False,
-            workflow_step_tqdm_disable: bool = True,
-            workflow_tqdm_enable: bool = False
-        ) -> None:
-        """Main function for creating an Entity resolution workflow.
-
-        Args:
-            data (Data): Dataset module.
-            verbose (bool, optional): Print detailed report for each step. Defaults to False.
-            with_classification_report (bool, optional): Print pairs counts. Defaults to False.
-            workflow_step_tqdm_disable (bool, optional):  Tqdm progress bar in each step. Defaults to True.
-            workflow_tqdm_enable (bool, optional): Overall progress bar. Defaults to False.
-        """
-        steps = [self.block_building, self.entity_matching, self.clustering, self.joins, self.block_cleaning, self.comparison_cleaning]
-        num_of_steps = sum(x is not None for x in steps)
-        self._workflow_bar = tqdm(total=num_of_steps,
-                                  desc=self.name,
-                                  disable=not workflow_tqdm_enable)
-        self.data = data
-        self._init_experiment()
-        start_time = time()
-        #
-        # Block building step: Only one algorithm can be performed
-        #
-        block_building_method = self.block_building['method'](**self.block_building["params"]) \
-                                                    if "params" in self.block_building \
-                                                    else self.block_building['method']()
-
-        block_building_blocks = \
-            block_building_method.build_blocks(data,
-                                               attributes_1=self.block_building["attributes_1"] \
-                                                                if "attributes_1" in self.block_building else None,
-                                                attributes_2=self.block_building["attributes_2"] \
-                                                                if "attributes_2" in self.block_building else None,
-                                                tqdm_disable=workflow_step_tqdm_disable)
-        self.final_pairs = block_building_blocks
-        res = block_building_method.evaluate(block_building_blocks,
-                                            export_to_dict=True,
-                                            with_classification_report=with_classification_report,
-                                            verbose=verbose)
-        self._save_step(res, block_building_method.method_configuration())
-        self._workflow_bar.update(1)
-        #
-        # Block cleaning step [optional]: Multiple algorithms
-        #
-        block_cleaning_blocks = None
-        if self.block_cleaning:
-            if isinstance(self.block_cleaning, dict):
-                self.block_cleaning = list(self.block_cleaning)
-            bblocks = block_building_blocks
-            for block_cleaning in self.block_cleaning:
-                block_cleaning_method = block_cleaning['method'](**block_cleaning["params"]) \
-                                                    if "params" in block_cleaning \
-                                                    else block_cleaning['method']()
-                block_cleaning_blocks = block_cleaning_method.process(bblocks,
-                                                                      data,
-                                                                      tqdm_disable=workflow_step_tqdm_disable)
-                
-                self.final_pairs = bblocks = block_cleaning_blocks
-                res = block_cleaning_method.evaluate(bblocks,
-                                                    export_to_dict=True,
-                                                    with_classification_report=with_classification_report,
-                                                    verbose=verbose)
-                self._save_step(res, block_cleaning_method.method_configuration())
-                self._workflow_bar.update(1)
-        #
-        # Comparison cleaning step [optional]
-        #
-        comparison_cleaning_blocks = None
-        if self.comparison_cleaning:
-            comparison_cleaning_method = self.comparison_cleaning['method'](**self.comparison_cleaning["params"]) \
-                                            if "params" in self.comparison_cleaning \
-                                            else self.comparison_cleaning['method']()
-            self.final_pairs = \
-            comparison_cleaning_blocks = \
-            comparison_cleaning_method.process(block_cleaning_blocks if block_cleaning_blocks is not None \
-                                                    else block_building_blocks,
-                                                data,
-                                                tqdm_disable=workflow_step_tqdm_disable)
-            res = comparison_cleaning_method.evaluate(comparison_cleaning_blocks,
-                                                      export_to_dict=True,
-                                                      with_classification_report=with_classification_report,
-                                                      verbose=verbose)
-            self._save_step(res, comparison_cleaning_method.method_configuration())
-            self._workflow_bar.update(1)
-        #
-        # Entity Matching step
-        #
-        entity_matching_method = self.entity_matching['method'](**self.entity_matching["params"]) \
-                                        if "params" in self.entity_matching \
-                                        else self.entity_matching['method']()
-        self.final_pairs = em_graph = entity_matching_method.predict(
-            comparison_cleaning_blocks if comparison_cleaning_blocks is not None \
-                else block_building_blocks,
-            data,
-            tqdm_disable=workflow_step_tqdm_disable
-        )
-        res = entity_matching_method.evaluate(em_graph,
-                                                export_to_dict=True,
-                                                with_classification_report=with_classification_report,
-                                                verbose=verbose)
-        self._save_step(res, entity_matching_method.method_configuration())
-        self._workflow_bar.update(1)
-        #
-        # Clustering step [optional]
-        #
-        if self.clustering:
-            clustering_method = self.clustering['method'](**self.clustering["params"]) \
-                                            if "params" in self.clustering \
-                                            else self.clustering['method']()
-            self.final_pairs = components = clustering_method.process(em_graph, data)
-            res = clustering_method.evaluate(components,
-                                            export_to_dict=True,
-                                            with_classification_report=False,
-                                            verbose=verbose)
-            self._save_step(res, clustering_method.method_configuration())
-            self.workflow_exec_time = time() - start_time
-            self._workflow_bar.update(1)
-        # self.runtime.append(self.workflow_exec_time)
-
-    def _init_experiment(self) -> None:
-        self.f1: list = []
-        self.recall: list = []
-        self.precision: list = []
-        self.runtime: list = []
-        self.configurations: list = []
-        self.workflow_exec_time: float
-
-    def visualize(
-            self,
-            f1: bool = True,
-            recall: bool = True,
-            precision: bool = True,
-            separate: bool = False
-    ) -> None:
-        """Performance Visualization of the workflow.
-
-        Args:
-            f1 (bool, optional): F-Measure. Defaults to True.
-            recall (bool, optional): Recall. Defaults to True.
-            precision (bool, optional): Precision. Defaults to True.
-            separate (bool, optional): Separate plots. Defaults to False.
-        """
-        method_names = [conf['name'] for conf in self.configurations]
-        exec_time = []
-        prev = 0
-
-        for i, _ in enumerate(self.runtime):
-            exec_time.append(prev + self.runtime[i])
-            prev = exec_time[i]
-
-        if separate:
-            fig, axs = plt.subplots(nrows=2, ncols=2, figsize=(10, 8))
-            fig.suptitle(self.name + " Visualization", fontweight='bold', fontsize=14)
-            fig.subplots_adjust(top=0.88)
-            axs[0, 0].plot(method_names,
-                           self.precision,
-                           linewidth=2.0,
-                           label="Precision",
-                           marker='o',
-                           markersize=10)
-            axs[0, 0].set_ylabel("Scores %", fontsize=12)
-            axs[0, 0].set_title("Precision", fontsize=12)
-            axs[0, 1].plot(method_names,
-                           self.recall,
-                           linewidth=2.0,
-                           label="Recall",
-                           marker='*',
-                           markersize=10)
-            axs[0, 1].set_ylabel("Scores %", fontsize=12)
-            axs[0, 1].set_title("Recall", fontsize=12)            
-            axs[1, 0].plot(method_names,
-                           self.f1,
-                           linewidth=2.0,
-                           label="F1-Score",
-                           marker='x',
-                           markersize=10)
-            axs[1, 0].set_ylabel("Scores %", fontsize=12)
-            axs[1, 0].set_title("F1-Score", fontsize=12)
-            # axs[0, 0].legend(loc='lower right')
-            axs[1, 1].plot(method_names,
-                           exec_time,
-                           linewidth=2.0,
-                           label="Time",
-                           marker='.',
-                           markersize=10,
-                           color='r')
-            axs[1, 1].set_ylabel("Time (sec)", fontsize=12)
-            axs[1, 1].set_title("Execution time", fontsize=12)
-            fig.autofmt_xdate()
-        else:
-            fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 8))
-            fig.suptitle(self.name + " Visualization", fontweight='bold', fontsize=14)
-            fig.subplots_adjust(top=0.88)
-            if precision:
-                axs[0].plot(method_names,
-                            self.precision,
-                            linewidth=2.0,
-                            label="Precision",
-                            marker='o',
-                            markersize=10)
-            if recall:
-                axs[0].plot(method_names,
-                            self.recall,
-                            linewidth=2.0,
-                            label="Recall",
-                            marker='*',
-                            markersize=10)
-            if f1:
-                axs[0].plot(method_names,
-                            self.f1, linewidth=2.0,
-                            label="F1-Score",
-                            marker='x',
-                            markersize=10)
-            axs[0].set_xlabel("Models", fontsize=12)
-            axs[0].set_ylabel("Scores %", fontsize=12)
-            axs[0].set_title("Performance per step", fontsize=12)
-            axs[0].legend(loc='lower right')
-            exec_time = []
-            prev = 0
-            for i, _ in enumerate(self.runtime):
-                exec_time.append(prev + self.runtime[i])
-                prev = exec_time[i]
-            axs[1].plot(method_names,
-                        exec_time,
-                        linewidth=2.0,
-                        label="F1-Score",
-                        marker='.',
-                        markersize=10,
-                        color='r')
-            axs[1].set_ylabel("Time (sec)", fontsize=12)
-            axs[1].set_title("Execution time", fontsize=12)
-            fig.autofmt_xdate()
-        plt.show()
-
-    def to_df(self) -> pd.DataFrame:
-        """Transform results into a pandas.DataFrame
-
-        Returns:
-            pd.DataFrame: Results
-        """
-        workflow_df = pd.DataFrame(
-            columns=['Algorithm', 'F1', 'Recall', 'Precision', 'Runtime (sec)', 'Params'])
-        workflow_df['F1'], workflow_df['Recall'], \
-        workflow_df['Precision'], workflow_df['Runtime (sec)'] = \
-            self.f1, self.recall, self.precision, self.runtime
-        workflow_df['Algorithm'] = [c['name'] for c in self.configurations]
-        workflow_df['Params'] = [c['parameters'] for c in self.configurations]
-
-        return workflow_df
-
-    def export_pairs(self) -> pd.DataFrame:
-        """Export pairs to file.
-
-        Returns:
-            pd.DataFrame: pairs as a DataFrame
-        """
-        return write(self.final_pairs, self.data)
-
-    def _save_step(self, results: dict, configuration: dict) -> None:
-        self.f1.append(results['F1 %'])
-        self.recall.append(results['Recall %'])
-        self.precision.append(results['Precision %'])
-        self.configurations.append(configuration)
-        self.runtime.append(configuration['runtime'])
-
-    def get_final_scores(self) -> Tuple[float, float, float]:
-        """Final scores in the last step of the workflow.
-
-        Returns:
-            Tuple[float, float, float]: F-Measure, Precision, Recall.
-        """
-        return self.f1[-1], self.precision[-1], self.recall[-1]
-
-def compare_workflows(workflows: List[WorkFlow], with_visualization=True) -> pd.DataFrame:
-    """Compares workflows by creating multiple plots and tables with results.
-
-    Args:
-        workflows (List[WorkFlow]): Different workflows
-        with_visualization (bool, optional): Diagram generation. Defaults to True.
-
-    Returns:
-        pd.DataFrame: Results
-    """
-    workflow_df = pd.DataFrame(columns=['Name', 'F1', 'Recall', 'Precision', 'Runtime (sec)'])
-    if with_visualization:
-        fig, axs = plt.subplots(nrows=2, ncols=2, figsize=(10, 8))
-        fig.suptitle("Workflows Performance Visualization", fontweight='bold', fontsize=14)
-        fig.subplots_adjust(top=0.88)
-        axs[0, 0].set_ylabel("Scores %", fontsize=12)
-        axs[0, 0].set_title("Precision", fontsize=12)
-        axs[0, 0].set_ylim([0, 100])
-        axs[0, 1].set_ylabel("Scores %", fontsize=12)
-        axs[0, 1].set_title("Recall", fontsize=12)
-        axs[0, 1].set_ylim([0, 100])
-        axs[1, 0].set_ylabel("Scores %", fontsize=12)
-        axs[1, 0].set_title("F1-Score", fontsize=12)
-        axs[1, 0].set_ylim([0, 100])
-        axs[1, 1].set_ylabel("Time (sec)", fontsize=12)
-        axs[1, 1].set_title("Execution time", fontsize=12)
-
-    for w in workflows:
-        workflow_df.loc[len(workflow_df)] = \
-            [w.name, w.f1[-1], w.recall[-1], w.precision[-1], w.workflow_exec_time]
-
-    if with_visualization:
-        axs[0, 0].bar(workflow_df['Name'],
-                      workflow_df['Precision'],
-                      label=workflow_df['Name'],
-                      color='b')
-        axs[0, 1].bar(workflow_df['Name'],
-                      workflow_df['Recall'],
-                      label=workflow_df['Name'],
-                      color='g')
-        axs[1, 0].bar(workflow_df['Name'], workflow_df['F1'], color='orange')
-        axs[1, 1].bar(workflow_df['Name'], workflow_df['Runtime (sec)'], color='r')
-    fig.autofmt_xdate()
-    plt.show()
-
-    return workflow_df
-
-
-############################################
-#  Pre-defined workflows same as JedAI     #
-############################################
-
-def get_best_blocking_workflow_ccer() -> WorkFlow:
-    """Best CC-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(
-                method=BlockPurging,
-                params=dict(smoothing_factor=1.0)
-            ),
-            dict(
-                method=BlockFiltering
-            )
-
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning),
-        entity_matching = dict(
-            method=EntityMatching,
-            metric='cosine',
-            similarity_threshold=0.55
-        ),
-        clustering = dict(
-            method=ConnectedComponentsClustering
-        ),
-        name="best-ccer-workflow"
-    )
-
-def get_best_blocking_workflow_der():
-    """Best D-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
-            dict(method=BlockFiltering)
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning,
-                                   params=dict(weighting_scheme='JS')),
-        entity_matching = dict(method=EntityMatching, 
-                               params=dict(metric='cosine',
-                                           similarity_threshold=0.55)),
-        clustering = dict(method=ConnectedComponentsClustering),
-        name="best-der-workflow"
-    )
-
-def get_default_blocking_workflow_ccer():
-    """Default CC-ER workflow.
-
-    Returns:
-        WorkFlow: Default workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(
-                method=BlockPurging,
-                params=dict(smoothing_factor=1.0)
-            ),
-            dict(
-                method=BlockFiltering
-            )
-
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning),
-        entity_matching = dict(
-            method=EntityMatching,
-            metric='cosine',
-            similarity_threshold=0.55
-        ),
-        clustering = dict(
-            method=UniqueMappingClustering
-        ),
-        name="default-ccer-workflow"
-    )
-
-def get_default_blocking_workflow_der():
-    """Default D-ER workflow.
-
-    Returns:
-        WorkFlow: Best workflow
-    """
-    return WorkFlow(
-        block_building = dict(
-            method=StandardBlocking
-        ),
-        block_cleaning = [
-            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
-            dict(method=BlockFiltering)
-        ],
-        comparison_cleaning = dict(method=CardinalityNodePruning, 
-                                   params=dict(weighting_scheme='JS')),
-        entity_matching = dict(method=EntityMatching,
-                               params=dict(metric='cosine',
-                                           similarity_threshold=0.55)),
-        name="default-der-workflow"
-    )
-
-
-class OptimizeWorkflow:
-    """Optuna Framework for GridSearch/RandomSearch/Prunning in a given pyjedai workflow.
-    """
-
-    _id = count()
-
-    def __init__(
-            self,
-            block_building: Callable, # Mandatory: one method
-            entity_matching: Callable, # Mandatory: one method
-            block_cleaning: List[Callable] = None, # Optional: multiple methods
-            comparison_cleaning: List[Callable] = None, # Optional: multiple methods
-            clustering: Callable = None, # Optional: One method
-            joins: Callable = None, # Optional: One method
-            name: str = None
-    ) -> None:
-        self.block_cleaning, self.block_building, self.comparison_cleaning, \
-            self.clustering, self.joins, self.entity_matching = \
-            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
-        self.f1: float
-        self.recall: float
-        self.precision: float
-        self.runtime: float
-        self.configurations: float
-        self.workflow_exec_time: float
-        self._id: int = next(self._id)
-        self.name: str = name if name else "OptWorkflow-" + str(self._id)
-        self._workflow_bar: tqdm
-
-    def objective(self, target_score: str = 'f1') -> any:
-        """Optuna objective function
-
-            Returns:
-                 One or more from F1,Recall,Precision
-        """
-        pass
-        # if target_score  == 'f1':
-        #     return f1
-        # elif target_score  == 'recall':
-        #     return recall
-        # else:
-        #     return precision
-
-    def run(
-            self,
-            data: Data,
-            num_of_trials = 30,
-            pruner: optuna.pruners = optuna.pruners.NopPruner,
-            sampler: optuna.samplers = optuna.samplers.BaseSampler,
-            study_name = "pyjedai_study",
-            storage_name = "pyjedai_storage_trials",
-            target_score = "f1",
-            load_if_exists=True,
-            verbose=False,
-            tqdm_disable=False,
-            workflow_tqdm_enable=False,
-            optuna_tqdm_enable=True
-    ) -> pd.DataFrame:
-        """Executes the experiments based on a workflow
-
-        Args:
-            data (Data): _description_
-            num_of_trials (int, optional): _description_. Defaults to 30.
-            pruner (optuna.pruners, optional): _description_. Defaults to optuna.pruners.NopPruner.
-            sampler (optuna.samplers, optional): _description_. Defaults to optuna.samplers.BaseSampler.
-            study_name (str, optional): _description_. Defaults to "pyjedai_study".
-            storage_name (str, optional): _description_. Defaults to "pyjedai_storage_trials".
-            target_score (str, optional): _description_. Defaults to "f1".
-            load_if_exists (bool, optional): _description_. Defaults to True.
-            verbose (bool, optional): _description_. Defaults to False.
-            tqdm_disable (bool, optional): _description_. Defaults to False.
-            workflow_tqdm_enable (bool, optional): _description_. Defaults to False.
-            optuna_tqdm_enable (bool, optional): _description_. Defaults to True.
-
-        Returns:
-            pd.DataFrame: _description_
-        """
-        study = optuna.create_study(
-            directions=["maximize"],
-            study_name=study_name,
-            storage=storage_name,
-            load_if_exists=load_if_exists
-        )
-        print("Optuna trials starting")
-        study.optimize(
-            self.objective, 
-            n_trials=num_of_trials, 
-            show_progress_bar=optuna_tqdm_enable
-        )
-        print("Optuna trials finished")
-
-    def visualize(self, with_plotly=True):
-        pass
-    
-    def get_best_trial(self):
-        pass
-    
-    def to_df():
-        pass
+from abc import ABC
+from itertools import count
+from time import time
+from typing import Callable, List, Tuple
+
+import matplotlib.pyplot as plt
+import optuna
+import pandas as pd
+from networkx import Graph
+# import plotly.express as px
+from tqdm.autonotebook import tqdm
+
+from .datamodel import Data
+from .evaluation import Evaluation, write
+from .block_building import StandardBlocking
+from .block_cleaning import BlockFiltering, BlockPurging
+from .comparison_cleaning import CardinalityNodePruning
+from .matching import EntityMatching
+from .clustering import ConnectedComponentsClustering, UniqueMappingClustering
+
+plt.style.use('seaborn-whitegrid')
+
+class WorkFlow(ABC):
+    """Main module of the pyjedAI and the simplest way to create an end-to-end ER workflow.
+    """
+
+    _id = count()
+
+    def __init__(
+            self,
+            block_building: dict = None,
+            entity_matching: dict = None,
+            block_cleaning: dict = None,
+            comparison_cleaning: dict = None,
+            clustering: dict = None,
+            joins: dict = None,
+            name: str = None
+    ) -> None:
+        self.block_cleaning, self.block_building, self.comparison_cleaning, \
+            self.clustering, self.joins, self.entity_matching = \
+            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
+        self.f1: list = []
+        self.recall: list = []
+        self.precision: list = []
+        self.runtime: list = []
+        self.configurations: list = []
+        self.workflow_exec_time: float
+        self._id: int = next(self._id)
+        self.name: str = name if name else "Workflow-" + str(self._id)
+        self._workflow_bar: tqdm
+        self.final_pairs = None
+
+    def run(self,
+            data: Data,
+            verbose: bool = False,
+            with_classification_report: bool = False,
+            workflow_step_tqdm_disable: bool = True,
+            workflow_tqdm_enable: bool = False
+        ) -> None:
+        """Main function for creating an Entity resolution workflow.
+
+        Args:
+            data (Data): Dataset module.
+            verbose (bool, optional): Print detailed report for each step. Defaults to False.
+            with_classification_report (bool, optional): Print pairs counts. Defaults to False.
+            workflow_step_tqdm_disable (bool, optional):  Tqdm progress bar in each step. Defaults to True.
+            workflow_tqdm_enable (bool, optional): Overall progress bar. Defaults to False.
+        """
+        steps = [self.block_building, self.entity_matching, self.clustering, self.joins, self.block_cleaning, self.comparison_cleaning]
+        num_of_steps = sum(x is not None for x in steps)
+        self._workflow_bar = tqdm(total=num_of_steps,
+                                  desc=self.name,
+                                  disable=not workflow_tqdm_enable)
+        self.data = data
+        self._init_experiment()
+        start_time = time()
+        #
+        # Block building step: Only one algorithm can be performed
+        #
+        block_building_method = self.block_building['method'](**self.block_building["params"]) \
+                                                    if "params" in self.block_building \
+                                                    else self.block_building['method']()
+
+        block_building_blocks = \
+            block_building_method.build_blocks(data,
+                                               attributes_1=self.block_building["attributes_1"] \
+                                                                if "attributes_1" in self.block_building else None,
+                                                attributes_2=self.block_building["attributes_2"] \
+                                                                if "attributes_2" in self.block_building else None,
+                                                tqdm_disable=workflow_step_tqdm_disable)
+        self.final_pairs = block_building_blocks
+        res = block_building_method.evaluate(block_building_blocks,
+                                            export_to_dict=True,
+                                            with_classification_report=with_classification_report,
+                                            verbose=verbose)
+        self._save_step(res, block_building_method.method_configuration())
+        self._workflow_bar.update(1)
+        #
+        # Block cleaning step [optional]: Multiple algorithms
+        #
+        block_cleaning_blocks = None
+        if self.block_cleaning:
+            if isinstance(self.block_cleaning, dict):
+                self.block_cleaning = list(self.block_cleaning)
+            bblocks = block_building_blocks
+            for block_cleaning in self.block_cleaning:
+                block_cleaning_method = block_cleaning['method'](**block_cleaning["params"]) \
+                                                    if "params" in block_cleaning \
+                                                    else block_cleaning['method']()
+                block_cleaning_blocks = block_cleaning_method.process(bblocks,
+                                                                      data,
+                                                                      tqdm_disable=workflow_step_tqdm_disable)
+                
+                self.final_pairs = bblocks = block_cleaning_blocks
+                res = block_cleaning_method.evaluate(bblocks,
+                                                    export_to_dict=True,
+                                                    with_classification_report=with_classification_report,
+                                                    verbose=verbose)
+                self._save_step(res, block_cleaning_method.method_configuration())
+                self._workflow_bar.update(1)
+        #
+        # Comparison cleaning step [optional]
+        #
+        comparison_cleaning_blocks = None
+        if self.comparison_cleaning:
+            comparison_cleaning_method = self.comparison_cleaning['method'](**self.comparison_cleaning["params"]) \
+                                            if "params" in self.comparison_cleaning \
+                                            else self.comparison_cleaning['method']()
+            self.final_pairs = \
+            comparison_cleaning_blocks = \
+            comparison_cleaning_method.process(block_cleaning_blocks if block_cleaning_blocks is not None \
+                                                    else block_building_blocks,
+                                                data,
+                                                tqdm_disable=workflow_step_tqdm_disable)
+            res = comparison_cleaning_method.evaluate(comparison_cleaning_blocks,
+                                                      export_to_dict=True,
+                                                      with_classification_report=with_classification_report,
+                                                      verbose=verbose)
+            self._save_step(res, comparison_cleaning_method.method_configuration())
+            self._workflow_bar.update(1)
+        #
+        # Entity Matching step
+        #
+        entity_matching_method = self.entity_matching['method'](**self.entity_matching["params"]) \
+                                        if "params" in self.entity_matching \
+                                        else self.entity_matching['method']()
+        self.final_pairs = em_graph = entity_matching_method.predict(
+            comparison_cleaning_blocks if comparison_cleaning_blocks is not None \
+                else block_building_blocks,
+            data,
+            tqdm_disable=workflow_step_tqdm_disable
+        )
+        res = entity_matching_method.evaluate(em_graph,
+                                                export_to_dict=True,
+                                                with_classification_report=with_classification_report,
+                                                verbose=verbose)
+        self._save_step(res, entity_matching_method.method_configuration())
+        self._workflow_bar.update(1)
+        #
+        # Clustering step [optional]
+        #
+        if self.clustering:
+            clustering_method = self.clustering['method'](**self.clustering["params"]) \
+                                            if "params" in self.clustering \
+                                            else self.clustering['method']()
+            self.final_pairs = components = clustering_method.process(em_graph, data)
+            res = clustering_method.evaluate(components,
+                                            export_to_dict=True,
+                                            with_classification_report=False,
+                                            verbose=verbose)
+            self._save_step(res, clustering_method.method_configuration())
+            self.workflow_exec_time = time() - start_time
+            self._workflow_bar.update(1)
+        # self.runtime.append(self.workflow_exec_time)
+
+    def _init_experiment(self) -> None:
+        self.f1: list = []
+        self.recall: list = []
+        self.precision: list = []
+        self.runtime: list = []
+        self.configurations: list = []
+        self.workflow_exec_time: float
+
+    def visualize(
+            self,
+            f1: bool = True,
+            recall: bool = True,
+            precision: bool = True,
+            separate: bool = False
+    ) -> None:
+        """Performance Visualization of the workflow.
+
+        Args:
+            f1 (bool, optional): F-Measure. Defaults to True.
+            recall (bool, optional): Recall. Defaults to True.
+            precision (bool, optional): Precision. Defaults to True.
+            separate (bool, optional): Separate plots. Defaults to False.
+        """
+        method_names = [conf['name'] for conf in self.configurations]
+        exec_time = []
+        prev = 0
+
+        for i, _ in enumerate(self.runtime):
+            exec_time.append(prev + self.runtime[i])
+            prev = exec_time[i]
+
+        if separate:
+            fig, axs = plt.subplots(nrows=2, ncols=2, figsize=(10, 8))
+            fig.suptitle(self.name + " Visualization", fontweight='bold', fontsize=14)
+            fig.subplots_adjust(top=0.88)
+            axs[0, 0].plot(method_names,
+                           self.precision,
+                           linewidth=2.0,
+                           label="Precision",
+                           marker='o',
+                           markersize=10)
+            axs[0, 0].set_ylabel("Scores %", fontsize=12)
+            axs[0, 0].set_title("Precision", fontsize=12)
+            axs[0, 1].plot(method_names,
+                           self.recall,
+                           linewidth=2.0,
+                           label="Recall",
+                           marker='*',
+                           markersize=10)
+            axs[0, 1].set_ylabel("Scores %", fontsize=12)
+            axs[0, 1].set_title("Recall", fontsize=12)            
+            axs[1, 0].plot(method_names,
+                           self.f1,
+                           linewidth=2.0,
+                           label="F1-Score",
+                           marker='x',
+                           markersize=10)
+            axs[1, 0].set_ylabel("Scores %", fontsize=12)
+            axs[1, 0].set_title("F1-Score", fontsize=12)
+            # axs[0, 0].legend(loc='lower right')
+            axs[1, 1].plot(method_names,
+                           exec_time,
+                           linewidth=2.0,
+                           label="Time",
+                           marker='.',
+                           markersize=10,
+                           color='r')
+            axs[1, 1].set_ylabel("Time (sec)", fontsize=12)
+            axs[1, 1].set_title("Execution time", fontsize=12)
+            fig.autofmt_xdate()
+        else:
+            fig, axs = plt.subplots(nrows=2, ncols=1, figsize=(10, 8))
+            fig.suptitle(self.name + " Visualization", fontweight='bold', fontsize=14)
+            fig.subplots_adjust(top=0.88)
+            if precision:
+                axs[0].plot(method_names,
+                            self.precision,
+                            linewidth=2.0,
+                            label="Precision",
+                            marker='o',
+                            markersize=10)
+            if recall:
+                axs[0].plot(method_names,
+                            self.recall,
+                            linewidth=2.0,
+                            label="Recall",
+                            marker='*',
+                            markersize=10)
+            if f1:
+                axs[0].plot(method_names,
+                            self.f1, linewidth=2.0,
+                            label="F1-Score",
+                            marker='x',
+                            markersize=10)
+            axs[0].set_xlabel("Models", fontsize=12)
+            axs[0].set_ylabel("Scores %", fontsize=12)
+            axs[0].set_title("Performance per step", fontsize=12)
+            axs[0].legend(loc='lower right')
+            exec_time = []
+            prev = 0
+            for i, _ in enumerate(self.runtime):
+                exec_time.append(prev + self.runtime[i])
+                prev = exec_time[i]
+            axs[1].plot(method_names,
+                        exec_time,
+                        linewidth=2.0,
+                        label="F1-Score",
+                        marker='.',
+                        markersize=10,
+                        color='r')
+            axs[1].set_ylabel("Time (sec)", fontsize=12)
+            axs[1].set_title("Execution time", fontsize=12)
+            fig.autofmt_xdate()
+        plt.show()
+
+    def to_df(self) -> pd.DataFrame:
+        """Transform results into a pandas.DataFrame
+
+        Returns:
+            pd.DataFrame: Results
+        """
+        workflow_df = pd.DataFrame(
+            columns=['Algorithm', 'F1', 'Recall', 'Precision', 'Runtime (sec)', 'Params'])
+        workflow_df['F1'], workflow_df['Recall'], \
+        workflow_df['Precision'], workflow_df['Runtime (sec)'] = \
+            self.f1, self.recall, self.precision, self.runtime
+        workflow_df['Algorithm'] = [c['name'] for c in self.configurations]
+        workflow_df['Params'] = [c['parameters'] for c in self.configurations]
+
+        return workflow_df
+
+    def export_pairs(self) -> pd.DataFrame:
+        """Export pairs to file.
+
+        Returns:
+            pd.DataFrame: pairs as a DataFrame
+        """
+        return write(self.final_pairs, self.data)
+
+    def _save_step(self, results: dict, configuration: dict) -> None:
+        self.f1.append(results['F1 %'])
+        self.recall.append(results['Recall %'])
+        self.precision.append(results['Precision %'])
+        self.configurations.append(configuration)
+        self.runtime.append(configuration['runtime'])
+
+    def get_final_scores(self) -> Tuple[float, float, float]:
+        """Final scores in the last step of the workflow.
+
+        Returns:
+            Tuple[float, float, float]: F-Measure, Precision, Recall.
+        """
+        return self.f1[-1], self.precision[-1], self.recall[-1]
+
+def compare_workflows(workflows: List[WorkFlow], with_visualization=True) -> pd.DataFrame:
+    """Compares workflows by creating multiple plots and tables with results.
+
+    Args:
+        workflows (List[WorkFlow]): Different workflows
+        with_visualization (bool, optional): Diagram generation. Defaults to True.
+
+    Returns:
+        pd.DataFrame: Results
+    """
+    workflow_df = pd.DataFrame(columns=['Name', 'F1', 'Recall', 'Precision', 'Runtime (sec)'])
+    if with_visualization:
+        fig, axs = plt.subplots(nrows=2, ncols=2, figsize=(10, 8))
+        fig.suptitle("Workflows Performance Visualization", fontweight='bold', fontsize=14)
+        fig.subplots_adjust(top=0.88)
+        axs[0, 0].set_ylabel("Scores %", fontsize=12)
+        axs[0, 0].set_title("Precision", fontsize=12)
+        axs[0, 0].set_ylim([0, 100])
+        axs[0, 1].set_ylabel("Scores %", fontsize=12)
+        axs[0, 1].set_title("Recall", fontsize=12)
+        axs[0, 1].set_ylim([0, 100])
+        axs[1, 0].set_ylabel("Scores %", fontsize=12)
+        axs[1, 0].set_title("F1-Score", fontsize=12)
+        axs[1, 0].set_ylim([0, 100])
+        axs[1, 1].set_ylabel("Time (sec)", fontsize=12)
+        axs[1, 1].set_title("Execution time", fontsize=12)
+
+    for w in workflows:
+        workflow_df.loc[len(workflow_df)] = \
+            [w.name, w.f1[-1], w.recall[-1], w.precision[-1], w.workflow_exec_time]
+
+    if with_visualization:
+        axs[0, 0].bar(workflow_df['Name'],
+                      workflow_df['Precision'],
+                      label=workflow_df['Name'],
+                      color='b')
+        axs[0, 1].bar(workflow_df['Name'],
+                      workflow_df['Recall'],
+                      label=workflow_df['Name'],
+                      color='g')
+        axs[1, 0].bar(workflow_df['Name'], workflow_df['F1'], color='orange')
+        axs[1, 1].bar(workflow_df['Name'], workflow_df['Runtime (sec)'], color='r')
+    fig.autofmt_xdate()
+    plt.show()
+
+    return workflow_df
+
+
+############################################
+#  Pre-defined workflows same as JedAI     #
+############################################
+
+def get_best_blocking_workflow_ccer() -> WorkFlow:
+    """Best CC-ER workflow.
+
+    Returns:
+        WorkFlow: Best workflow
+    """
+    return WorkFlow(
+        block_building = dict(
+            method=StandardBlocking
+        ),
+        block_cleaning = [
+            dict(
+                method=BlockPurging,
+                params=dict(smoothing_factor=1.0)
+            ),
+            dict(
+                method=BlockFiltering
+            )
+
+        ],
+        comparison_cleaning = dict(method=CardinalityNodePruning),
+        entity_matching = dict(
+            method=EntityMatching,
+            metric='cosine',
+            similarity_threshold=0.55
+        ),
+        clustering = dict(
+            method=ConnectedComponentsClustering
+        ),
+        name="best-ccer-workflow"
+    )
+
+def get_best_blocking_workflow_der():
+    """Best D-ER workflow.
+
+    Returns:
+        WorkFlow: Best workflow
+    """
+    return WorkFlow(
+        block_building = dict(
+            method=StandardBlocking
+        ),
+        block_cleaning = [
+            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
+            dict(method=BlockFiltering)
+        ],
+        comparison_cleaning = dict(method=CardinalityNodePruning,
+                                   params=dict(weighting_scheme='JS')),
+        entity_matching = dict(method=EntityMatching, 
+                               params=dict(metric='cosine',
+                                           similarity_threshold=0.55)),
+        clustering = dict(method=ConnectedComponentsClustering),
+        name="best-der-workflow"
+    )
+
+def get_default_blocking_workflow_ccer():
+    """Default CC-ER workflow.
+
+    Returns:
+        WorkFlow: Default workflow
+    """
+    return WorkFlow(
+        block_building = dict(
+            method=StandardBlocking
+        ),
+        block_cleaning = [
+            dict(
+                method=BlockPurging,
+                params=dict(smoothing_factor=1.0)
+            ),
+            dict(
+                method=BlockFiltering
+            )
+
+        ],
+        comparison_cleaning = dict(method=CardinalityNodePruning),
+        entity_matching = dict(
+            method=EntityMatching,
+            metric='cosine',
+            similarity_threshold=0.55
+        ),
+        clustering = dict(
+            method=UniqueMappingClustering
+        ),
+        name="default-ccer-workflow"
+    )
+
+def get_default_blocking_workflow_der():
+    """Default D-ER workflow.
+
+    Returns:
+        WorkFlow: Best workflow
+    """
+    return WorkFlow(
+        block_building = dict(
+            method=StandardBlocking
+        ),
+        block_cleaning = [
+            dict(method=BlockPurging, params=dict(smoothing_factor=1.0)),
+            dict(method=BlockFiltering)
+        ],
+        comparison_cleaning = dict(method=CardinalityNodePruning, 
+                                   params=dict(weighting_scheme='JS')),
+        entity_matching = dict(method=EntityMatching,
+                               params=dict(metric='cosine',
+                                           similarity_threshold=0.55)),
+        name="default-der-workflow"
+    )
+
+
+class OptimizeWorkflow:
+    """Optuna Framework for GridSearch/RandomSearch/Prunning in a given pyjedai workflow.
+    """
+
+    _id = count()
+
+    def __init__(
+            self,
+            block_building: Callable, # Mandatory: one method
+            entity_matching: Callable, # Mandatory: one method
+            block_cleaning: List[Callable] = None, # Optional: multiple methods
+            comparison_cleaning: List[Callable] = None, # Optional: multiple methods
+            clustering: Callable = None, # Optional: One method
+            joins: Callable = None, # Optional: One method
+            name: str = None
+    ) -> None:
+        self.block_cleaning, self.block_building, self.comparison_cleaning, \
+            self.clustering, self.joins, self.entity_matching = \
+            block_cleaning, block_building, comparison_cleaning, clustering, joins, entity_matching
+        self.f1: float
+        self.recall: float
+        self.precision: float
+        self.runtime: float
+        self.configurations: float
+        self.workflow_exec_time: float
+        self._id: int = next(self._id)
+        self.name: str = name if name else "OptWorkflow-" + str(self._id)
+        self._workflow_bar: tqdm
+
+    def objective(self, target_score: str = 'f1') -> any:
+        """Optuna objective function
+
+            Returns:
+                 One or more from F1,Recall,Precision
+        """
+        pass
+        # if target_score  == 'f1':
+        #     return f1
+        # elif target_score  == 'recall':
+        #     return recall
+        # else:
+        #     return precision
+
+    def run(
+            self,
+            data: Data,
+            num_of_trials = 30,
+            pruner: optuna.pruners = optuna.pruners.NopPruner,
+            sampler: optuna.samplers = optuna.samplers.BaseSampler,
+            study_name = "pyjedai_study",
+            storage_name = "pyjedai_storage_trials",
+            target_score = "f1",
+            load_if_exists=True,
+            verbose=False,
+            tqdm_disable=False,
+            workflow_tqdm_enable=False,
+            optuna_tqdm_enable=True
+    ) -> pd.DataFrame:
+        """Executes the experiments based on a workflow
+
+        Args:
+            data (Data): _description_
+            num_of_trials (int, optional): _description_. Defaults to 30.
+            pruner (optuna.pruners, optional): _description_. Defaults to optuna.pruners.NopPruner.
+            sampler (optuna.samplers, optional): _description_. Defaults to optuna.samplers.BaseSampler.
+            study_name (str, optional): _description_. Defaults to "pyjedai_study".
+            storage_name (str, optional): _description_. Defaults to "pyjedai_storage_trials".
+            target_score (str, optional): _description_. Defaults to "f1".
+            load_if_exists (bool, optional): _description_. Defaults to True.
+            verbose (bool, optional): _description_. Defaults to False.
+            tqdm_disable (bool, optional): _description_. Defaults to False.
+            workflow_tqdm_enable (bool, optional): _description_. Defaults to False.
+            optuna_tqdm_enable (bool, optional): _description_. Defaults to True.
+
+        Returns:
+            pd.DataFrame: _description_
+        """
+        study = optuna.create_study(
+            directions=["maximize"],
+            study_name=study_name,
+            storage=storage_name,
+            load_if_exists=load_if_exists
+        )
+        print("Optuna trials starting")
+        study.optimize(
+            self.objective, 
+            n_trials=num_of_trials, 
+            show_progress_bar=optuna_tqdm_enable
+        )
+        print("Optuna trials finished")
+
+    def visualize(self, with_plotly=True):
+        pass
+    
+    def get_best_trial(self):
+        pass
+    
+    def to_df():
+        pass
```

### Comparing `pyjedai-0.0.6/src/pyjedai.egg-info/SOURCES.txt` & `pyjedai-0.0.7/src/pyjedai.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 LICENSE
 README.md
 pyproject.toml
 src/pyjedai/__init__.py
+src/pyjedai/_version.py
 src/pyjedai/block_building.py
 src/pyjedai/block_cleaning.py
 src/pyjedai/clustering.py
 src/pyjedai/comparison_cleaning.py
 src/pyjedai/datamodel.py
 src/pyjedai/evaluation.py
 src/pyjedai/joins.py
 src/pyjedai/logs.py
 src/pyjedai/matching.py
+src/pyjedai/prioritization.py
 src/pyjedai/utils.py
 src/pyjedai/vector_based_blocking.py
 src/pyjedai/visualization.py
 src/pyjedai/workflow.py
 src/pyjedai.egg-info/PKG-INFO
 src/pyjedai.egg-info/SOURCES.txt
 src/pyjedai.egg-info/dependency_links.txt
 src/pyjedai.egg-info/requires.txt
-src/pyjedai.egg-info/top_level.txt
+src/pyjedai.egg-info/top_level.txt
+tests/test_block_building.py
+tests/test_block_cleaning.py
+tests/test_clustering.py
+tests/test_comparison_cleaning.py
+tests/test_joins.py
```

