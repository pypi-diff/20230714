# Comparing `tmp/pygmid-1.0.tar.gz` & `tmp/pygmid-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pygmid-1.0.tar", last modified: Thu Jan 26 17:40:29 2023, max compression
+gzip compressed data, was "pygmid-1.0.1.tar", last modified: Fri Jul 14 12:25:22 2023, max compression
```

## Comparing `pygmid-1.0.tar` & `pygmid-1.0.1.tar`

### file list

```diff
@@ -1,25 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-01-26 17:40:29.879375 pygmid-1.0/
--rw-rw-rw-   0        0        0    11558 2022-07-06 16:03:41.000000 pygmid-1.0/LICENSE
--rw-rw-rw-   0        0        0    15837 2023-01-26 17:40:29.879375 pygmid-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3736 2023-01-26 17:38:15.000000 pygmid-1.0/README.md
--rw-rw-rw-   0        0        0       86 2022-07-05 10:39:08.000000 pygmid-1.0/pyproject.toml
--rw-rw-rw-   0        0        0      778 2023-01-26 17:40:29.882364 pygmid-1.0/setup.cfg
--rw-rw-rw-   0        0        0       37 2022-07-05 10:39:08.000000 pygmid-1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-01-26 17:40:29.820631 pygmid-1.0/src/
-drwxrwxrwx   0        0        0        0 2023-01-26 17:40:29.847034 pygmid-1.0/src/pygmid/
--rw-rw-rw-   0        0        0    14417 2023-01-09 10:26:21.000000 pygmid-1.0/src/pygmid/Lookup.py
--rw-rw-rw-   0        0        0      531 2023-01-06 19:55:24.000000 pygmid-1.0/src/pygmid/Spectre.py
--rw-rw-rw-   0        0        0      222 2023-01-06 19:55:24.000000 pygmid-1.0/src/pygmid/Sweep.py
--rw-rw-rw-   0        0        0      245 2023-01-08 22:15:09.000000 pygmid-1.0/src/pygmid/__init__.py
--rw-rw-rw-   0        0        0     1154 2022-07-05 10:39:08.000000 pygmid-1.0/src/pygmid/__main__.py
--rw-rw-rw-   0        0        0       47 2023-01-06 19:55:24.000000 pygmid-1.0/src/pygmid/constants.py
--rw-rw-rw-   0        0        0     1109 2023-01-26 17:30:33.000000 pygmid-1.0/src/pygmid/numerical.py
--rw-rw-rw-   0        0        0       46 2022-07-05 10:39:08.000000 pygmid-1.0/src/pygmid/pygmid.py
--rw-rw-rw-   0        0        0     5321 2023-01-26 17:30:33.000000 pygmid-1.0/src/pygmid/utility.py
--rw-rw-rw-   0        0        0       21 2023-01-26 17:30:33.000000 pygmid-1.0/src/pygmid/version.py
-drwxrwxrwx   0        0        0        0 2023-01-26 17:40:29.877381 pygmid-1.0/src/pygmid.egg-info/
--rw-rw-rw-   0        0        0    15837 2023-01-26 17:40:28.000000 pygmid-1.0/src/pygmid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      442 2023-01-26 17:40:29.000000 pygmid-1.0/src/pygmid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-26 17:40:29.000000 pygmid-1.0/src/pygmid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-01-26 17:40:29.000000 pygmid-1.0/src/pygmid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-01-26 17:40:29.000000 pygmid-1.0/src/pygmid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:22.163874 pygmid-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-07-14 12:24:53.000000 pygmid-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-14 12:25:22.163874 pygmid-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-07-14 12:24:53.000000 pygmid-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-07-14 12:24:53.000000 pygmid-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-07-14 12:25:22.163874 pygmid-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-07-14 12:24:53.000000 pygmid-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:22.159874 pygmid-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:22.163874 pygmid-1.0.1/src/pygmid/
+-rw-r--r--   0 runner    (1001) docker     (123)    14222 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/Lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/Spectre.py
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/Sweep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1117 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/numerical.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/pygmid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5172 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-07-14 12:24:53.000000 pygmid-1.0.1/src/pygmid/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:22.163874 pygmid-1.0.1/src/pygmid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15267 2023-07-14 12:25:22.000000 pygmid-1.0.1/src/pygmid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      509 2023-07-14 12:25:22.000000 pygmid-1.0.1/src/pygmid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-14 12:25:22.000000 pygmid-1.0.1/src/pygmid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-07-14 12:25:22.000000 pygmid-1.0.1/src/pygmid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-07-14 12:25:22.000000 pygmid-1.0.1/src/pygmid.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-14 12:25:22.163874 pygmid-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-07-14 12:24:53.000000 pygmid-1.0.1/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-07-14 12:24:53.000000 pygmid-1.0.1/tests/test_lookupVGS.py
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-07-14 12:24:53.000000 pygmid-1.0.1/tests/test_utility.py
```

### Comparing `pygmid-1.0/LICENSE` & `pygmid-1.0.1/LICENSE`

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

### Comparing `pygmid-1.0/PKG-INFO` & `pygmid-1.0.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,361 +1,349 @@
-Metadata-Version: 2.1
-Name: pygmid
-Version: 1.0
-Summary: A python 3 implementation of the gm/ID starter kit
-Home-page: https://github.com/madrasalach/pygmid
-Author: Cian O`Donnell, Danylo Galach
-Author-email: cian.odonnell@tyndall.ie
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <a>
-    <img src="docs/img/icon.png" width="80">
-  </a>
-
-  <h3 align="center">pygmid</h3>
-
-  <p align="center">
-    A python3 implementation of the gm/ID starter kit
-    <br>
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
-    ·
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
-  </p>
-</p>
-
-## Table of contents
-
-- [About](#about)
-- [Installation](#installation)
-- [Usage](#usage)
-- [TODO](#todo)
-- [Authors](#authors)
-
-## About
-
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
-of Stanford University. The package also offers some scripts from the Paul Jesper's book.
-
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
-
-## Installation
-
-To install pygmid from source, download from Github and run pip:
-
-`pip install .`
-
- in the root directory.
-
- pygmid can also be installed from PyPI:
-
-`pip install pygmid`
-
-## Usage
-
-### Scripting with the Lookup Class
-A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
-
-You can create a lookup object as follows:
-
-```python
-from pygmid import Lookup as lk
-
-NCH = lk('180nch.mat')
-```
-### Access MOS Data
-The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
-
-```python
-# get VGS data as array from NCH
-VGS_array = NCH['VGS']
-```
-
-Data is returned as a deep copy of the array contained in the `Lookup` object.
-
-### Lookup functionality 
-
-Lookup of interpolated data occurs as follows:
-
-```python
-VDSs = NCH['VDS'] 
-VGSs = np.arange(0.4, 0.6, 0.05)
-# Plot ID versus VDS
-ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
-# alias function lookup can also be used
-ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
-# check bias
-VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
-print(f'VGS is: {VGS}')
-
-plt.plot(VDSs, np.transpose(ID))
-```
-
-~~Currently only lookup modes 1 and 2 are implemented.~~
-Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
-
-### Technology Extraction Functions
-
-The EKV extraction function can be used as follows:
-
-```python
-from pygmid import EKV_param_extraction, XTRACT
-
-(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
-        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
-
-```
-
-Sample usage of this and other utility functions can be found in `test_utility.py` .
-
-### Examples
-
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
-
-Sample outputs are given below:
-
-![image](docs/img/IDvVDS.png)
-
-![image](docs/img/vtvsL.png)
-
-![image](docs/img/gm_gds.png)
-
-![image](docs/img/ft.png)
-
-![image](docs/img/idwVDS.png)
-
-![image](docs/img/IDWvsgmID.png)
-
-### Command Line Interface (CLI)
-
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
-
-## !TODO
-- ~~look_up MODE 3 (ratio vs ratio)~~
-- ~~look_upVGS and lookupVGS~~
-- ~~pchip interpolation~~
-- SPECTRE techsweep
-- Support for non .mat data structures
-- Improved logging for error generation
-
-## Authors
-
-- Cian O'Donnell : cian.odonnell@tyndall.ie
-- Danylo Galach
-
-## Contributors
-
-- José Rui Custódio
-
-A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
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
-
-
+Metadata-Version: 2.1
+Name: pygmid
+Version: 1.0.1
+Summary: A python 3 implementation of the gm/ID starter kit
+Home-page: https://github.com/madrasalach/pygmid
+Author: Cian O`Donnell, Danylo Galach
+Author-email: cian.odonnell@tyndall.ie
+Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <a>
+    <img src="docs/img/icon.png" width="80">
+  </a>
+
+  <h3 align="center">pygmid</h3>
+
+  <p align="center">
+    A python3 implementation of the gm/ID starter kit
+    <br>
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
+    ·
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
+  </p>
+</p>
+
+## Table of contents
+
+- [About](#about)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Authors](#authors)
+
+## About
+
+pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+of Stanford University. The package also offers some scripts from the Paul Jesper's book.
+
+For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
+section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
+
+## Installation
+
+To install pygmid from source, download from Github and run pip:
+
+`pip install .`
+
+ in the root directory.
+
+ pygmid can also be installed from PyPI:
+
+`pip install pygmid`
+
+## Usage
+
+### Scripting with the Lookup Class
+A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
+
+You can create a lookup object as follows:
+
+```python
+from pygmid import Lookup as lk
+
+NCH = lk('180nch.mat')
+```
+### Access MOS Data
+The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
+
+```python
+# get VGS data as array from NCH
+VGS_array = NCH['VGS']
+```
+
+Data is returned as a deep copy of the array contained in the `Lookup` object.
+
+### Lookup functionality 
+
+Lookup of interpolated data occurs as follows:
+
+```python
+VDSs = NCH['VDS'] 
+VGSs = np.arange(0.4, 0.6, 0.05)
+# Plot ID versus VDS
+ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
+# alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
+# check bias
+VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
+print(f'VGS is: {VGS}')
+
+plt.plot(VDSs, np.transpose(ID))
+```
+
+~~Currently only lookup modes 1 and 2 are implemented.~~
+Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
+
+### Technology Extraction Functions
+
+The EKV extraction function can be used as follows:
+
+```python
+from pygmid import EKV_param_extraction, XTRACT
+
+(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
+        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
+
+```
+
+Sample usage of this and other utility functions can be found in `test_utility.py` .
+
+### Examples
+
+Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+
+Sample outputs are given below:
+
+![image](docs/img/IDvVDS.png)
+
+![image](docs/img/vtvsL.png)
+
+![image](docs/img/gm_gds.png)
+
+![image](docs/img/ft.png)
+
+![image](docs/img/idwVDS.png)
+
+![image](docs/img/IDWvsgmID.png)
+
+### Command Line Interface (CLI)
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+
+## Authors
+
+- Cian O'Donnell : cian.odonnell@mcci.ie
+- Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
+- Danylo Galach
+
+## Contributors
+
+- José Rui Custódio
+
+A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
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

#### html2text {}

```diff
@@ -1,58 +1,55 @@
-Metadata-Version: 2.1 Name: pygmid Version: 1.0 Summary: A python 3
+Metadata-Version: 2.1 Name: pygmid Version: 1.0.1 Summary: A python 3
 implementation of the gm/ID starter kit Home-page: https://github.com/
 madrasalach/pygmid Author: Cian O`Donnell, Danylo Galach Author-email:
-cian.odonnell@tyndall.ie License: UNKNOWN Project-URL: Bug Tracker, https://
-github.com/madrasalach/pygmid/issues Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4 Description-Content-Type: text/markdown License-File:
-LICENSE
+cian.odonnell@tyndall.ie Project-URL: Bug Tracker, https://github.com/
+madrasalach/pygmid/issues Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent Requires-Python: >=3.4
+Description-Content-Type: text/markdown License-File: LICENSE
                               [docs/img/icon.png]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [TODO](#todo) - [Authors](#authors) ## About pygmid is a
-Python 3 port of the gm/ID starter kit by Prof. Boris Murmann of Stanford
-University. The package also offers some scripts from the Paul Jesper's book.
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann. ##
-Installation To install pygmid from source, download from Github and run pip:
-`pip install .` in the root directory. pygmid can also be installed from PyPI:
-`pip install pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID
-lookup object can be generated with the `Lookup` class. The lookup object
-requires lookup data for initialisation. Currently, only `.mat` files are
-supported. You can create a lookup object as follows: ```python from pygmid
-import Lookup as lk NCH = lk('180nch.mat') ``` ### Access MOS Data The `Lookup`
-class allows for pseudo array access of the MOS matrix data. You can access
-data as follows: ```python # get VGS data as array from NCH VGS_array = NCH
-['VGS'] ``` Data is returned as a deep copy of the array contained in the
-`Lookup` object. ### Lookup functionality Lookup of interpolated data occurs as
-follows: ```python VDSs = NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID
-versus VDS ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup
-can also be used ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS =
-NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is:
-{VGS}') plt.plot(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1
-and 2 are implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary
-ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The
-companion lookupVGS function is also included. ### Technology Extraction
-Functions The EKV extraction function can be used as follows: ```python from
-pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
-d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
-0.0) ``` Sample usage of this and other utility functions can be found in
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
+gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
+also offers some scripts from the Paul Jesper's book. For the gm/ID starter
+kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
+website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
+from source, download from Github and run pip: `pip install .` in the root
+directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
+Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
+generated with the `Lookup` class. The lookup object requires lookup data for
+initialisation. Currently, only `.mat` files are supported. You can create a
+lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
+array access of the MOS matrix data. You can access data as follows: ```python
+# get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
+a deep copy of the array contained in the `Lookup` object. ### Lookup
+functionality Lookup of interpolated data occurs as follows: ```python VDSs =
+NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
+NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
+(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
+(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
+implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
+lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
+lookupVGS function is also included. ### Technology Extraction Functions The
+EKV extraction function can be used as follows: ```python from pygmid import
+EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
+d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
+Sample usage of this and other utility functions can be found in
 `test_utility.py` . ### Examples Usage of lookup scripts are given in
 `test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
 [image](docs/img/IDvVDS.png) ![image](docs/img/vtvsL.png) ![image](docs/img/
 gm_gds.png) ![image](docs/img/ft.png) ![image](docs/img/idwVDS.png) ![image]
 (docs/img/IDWvsgmID.png) ### Command Line Interface (CLI) `pygmid` also
 features a CLI which can be used to run techweeps to generate transistor data
-## !TODO - ~~look_up MODE 3 (ratio vs ratio)~~ - ~~look_upVGS and lookupVGS~~ -
-~~pchip interpolation~~ - SPECTRE techsweep - Support for non .mat data
-structures - Improved logging for error generation ## Authors - Cian O'Donnell
-: cian.odonnell@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
+## Authors - Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License. Apache License
 Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS
 FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean
 the terms and conditions for use, reproduction, and distribution as defined by
 Sections 1 through 9 of this document. "Licensor" shall mean the copyright
 owner or entity authorized by the copyright owner that is granting the License.
```

### Comparing `pygmid-1.0/README.md` & `pygmid-1.0.1/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,141 +1,133 @@
-<p align="center">
-  <a>
-    <img src="docs/img/icon.png" width="80">
-  </a>
-
-  <h3 align="center">pygmid</h3>
-
-  <p align="center">
-    A python3 implementation of the gm/ID starter kit
-    <br>
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
-    ·
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
-  </p>
-</p>
-
-## Table of contents
-
-- [About](#about)
-- [Installation](#installation)
-- [Usage](#usage)
-- [TODO](#todo)
-- [Authors](#authors)
-
-## About
-
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
-of Stanford University. The package also offers some scripts from the Paul Jesper's book.
-
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
-
-## Installation
-
-To install pygmid from source, download from Github and run pip:
-
-`pip install .`
-
- in the root directory.
-
- pygmid can also be installed from PyPI:
-
-`pip install pygmid`
-
-## Usage
-
-### Scripting with the Lookup Class
-A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
-
-You can create a lookup object as follows:
-
-```python
-from pygmid import Lookup as lk
-
-NCH = lk('180nch.mat')
-```
-### Access MOS Data
-The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
-
-```python
-# get VGS data as array from NCH
-VGS_array = NCH['VGS']
-```
-
-Data is returned as a deep copy of the array contained in the `Lookup` object.
-
-### Lookup functionality 
-
-Lookup of interpolated data occurs as follows:
-
-```python
-VDSs = NCH['VDS'] 
-VGSs = np.arange(0.4, 0.6, 0.05)
-# Plot ID versus VDS
-ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
-# alias function lookup can also be used
-ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
-# check bias
-VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
-print(f'VGS is: {VGS}')
-
-plt.plot(VDSs, np.transpose(ID))
-```
-
-~~Currently only lookup modes 1 and 2 are implemented.~~
-Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
-
-### Technology Extraction Functions
-
-The EKV extraction function can be used as follows:
-
-```python
-from pygmid import EKV_param_extraction, XTRACT
-
-(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
-        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
-
-```
-
-Sample usage of this and other utility functions can be found in `test_utility.py` .
-
-### Examples
-
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
-
-Sample outputs are given below:
-
-![image](docs/img/IDvVDS.png)
-
-![image](docs/img/vtvsL.png)
-
-![image](docs/img/gm_gds.png)
-
-![image](docs/img/ft.png)
-
-![image](docs/img/idwVDS.png)
-
-![image](docs/img/IDWvsgmID.png)
-
-### Command Line Interface (CLI)
-
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
-
-## !TODO
-- ~~look_up MODE 3 (ratio vs ratio)~~
-- ~~look_upVGS and lookupVGS~~
-- ~~pchip interpolation~~
-- SPECTRE techsweep
-- Support for non .mat data structures
-- Improved logging for error generation
-
-## Authors
-
-- Cian O'Donnell : cian.odonnell@tyndall.ie
-- Danylo Galach
-
-## Contributors
-
-- José Rui Custódio
-
-A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
+<p align="center">
+  <a>
+    <img src="docs/img/icon.png" width="80">
+  </a>
+
+  <h3 align="center">pygmid</h3>
+
+  <p align="center">
+    A python3 implementation of the gm/ID starter kit
+    <br>
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
+    ·
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
+  </p>
+</p>
+
+## Table of contents
+
+- [About](#about)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Authors](#authors)
+
+## About
+
+pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+of Stanford University. The package also offers some scripts from the Paul Jesper's book.
+
+For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
+section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
+
+## Installation
+
+To install pygmid from source, download from Github and run pip:
+
+`pip install .`
+
+ in the root directory.
+
+ pygmid can also be installed from PyPI:
+
+`pip install pygmid`
+
+## Usage
+
+### Scripting with the Lookup Class
+A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
+
+You can create a lookup object as follows:
+
+```python
+from pygmid import Lookup as lk
+
+NCH = lk('180nch.mat')
+```
+### Access MOS Data
+The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
+
+```python
+# get VGS data as array from NCH
+VGS_array = NCH['VGS']
+```
+
+Data is returned as a deep copy of the array contained in the `Lookup` object.
+
+### Lookup functionality 
+
+Lookup of interpolated data occurs as follows:
+
+```python
+VDSs = NCH['VDS'] 
+VGSs = np.arange(0.4, 0.6, 0.05)
+# Plot ID versus VDS
+ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
+# alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
+# check bias
+VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
+print(f'VGS is: {VGS}')
+
+plt.plot(VDSs, np.transpose(ID))
+```
+
+~~Currently only lookup modes 1 and 2 are implemented.~~
+Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
+
+### Technology Extraction Functions
+
+The EKV extraction function can be used as follows:
+
+```python
+from pygmid import EKV_param_extraction, XTRACT
+
+(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
+        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
+
+```
+
+Sample usage of this and other utility functions can be found in `test_utility.py` .
+
+### Examples
+
+Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+
+Sample outputs are given below:
+
+![image](docs/img/IDvVDS.png)
+
+![image](docs/img/vtvsL.png)
+
+![image](docs/img/gm_gds.png)
+
+![image](docs/img/ft.png)
+
+![image](docs/img/idwVDS.png)
+
+![image](docs/img/IDWvsgmID.png)
+
+### Command Line Interface (CLI)
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+
+## Authors
+
+- Cian O'Donnell : cian.odonnell@mcci.ie
+- Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
+- Danylo Galach
+
+## Contributors
+
+- José Rui Custódio
+
+A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
```

#### html2text {}

```diff
@@ -1,45 +1,43 @@
                               [docs/img/icon.png]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [TODO](#todo) - [Authors](#authors) ## About pygmid is a
-Python 3 port of the gm/ID starter kit by Prof. Boris Murmann of Stanford
-University. The package also offers some scripts from the Paul Jesper's book.
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann. ##
-Installation To install pygmid from source, download from Github and run pip:
-`pip install .` in the root directory. pygmid can also be installed from PyPI:
-`pip install pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID
-lookup object can be generated with the `Lookup` class. The lookup object
-requires lookup data for initialisation. Currently, only `.mat` files are
-supported. You can create a lookup object as follows: ```python from pygmid
-import Lookup as lk NCH = lk('180nch.mat') ``` ### Access MOS Data The `Lookup`
-class allows for pseudo array access of the MOS matrix data. You can access
-data as follows: ```python # get VGS data as array from NCH VGS_array = NCH
-['VGS'] ``` Data is returned as a deep copy of the array contained in the
-`Lookup` object. ### Lookup functionality Lookup of interpolated data occurs as
-follows: ```python VDSs = NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID
-versus VDS ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup
-can also be used ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS =
-NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is:
-{VGS}') plt.plot(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1
-and 2 are implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary
-ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The
-companion lookupVGS function is also included. ### Technology Extraction
-Functions The EKV extraction function can be used as follows: ```python from
-pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
-d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
-0.0) ``` Sample usage of this and other utility functions can be found in
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
+gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
+also offers some scripts from the Paul Jesper's book. For the gm/ID starter
+kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
+website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
+from source, download from Github and run pip: `pip install .` in the root
+directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
+Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
+generated with the `Lookup` class. The lookup object requires lookup data for
+initialisation. Currently, only `.mat` files are supported. You can create a
+lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
+array access of the MOS matrix data. You can access data as follows: ```python
+# get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
+a deep copy of the array contained in the `Lookup` object. ### Lookup
+functionality Lookup of interpolated data occurs as follows: ```python VDSs =
+NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
+NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
+(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
+(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
+implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
+lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
+lookupVGS function is also included. ### Technology Extraction Functions The
+EKV extraction function can be used as follows: ```python from pygmid import
+EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
+d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
+Sample usage of this and other utility functions can be found in
 `test_utility.py` . ### Examples Usage of lookup scripts are given in
 `test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
 [image](docs/img/IDvVDS.png) ![image](docs/img/vtvsL.png) ![image](docs/img/
 gm_gds.png) ![image](docs/img/ft.png) ![image](docs/img/idwVDS.png) ![image]
 (docs/img/IDWvsgmID.png) ### Command Line Interface (CLI) `pygmid` also
 features a CLI which can be used to run techweeps to generate transistor data
-## !TODO - ~~look_up MODE 3 (ratio vs ratio)~~ - ~~look_upVGS and lookupVGS~~ -
-~~pchip interpolation~~ - SPECTRE techsweep - Support for non .mat data
-structures - Improved logging for error generation ## Authors - Cian O'Donnell
-: cian.odonnell@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
+## Authors - Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License.
```

### Comparing `pygmid-1.0/src/pygmid/Lookup.py` & `pygmid-1.0.1/src/pygmid/Lookup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,369 +1,376 @@
-import copy
-
-import numpy as np
-import scipy.io
-from scipy.interpolate import interpn
-
-from .constants import eps
-from .numerical import interp1
-
-class Lookup:
-    def __init__(self, filename="MOS.mat", **kwargs):
-        self.__setup(filename, **kwargs)
-        self.__modefuncmap = {1 : self._SimpleLK,
-                              2 : self._SimpleLK,  
-                              3 : self._RatioVRatioLK}
-
-    def __setup(self, filename, **kwargs):
-        """
-        Setup the Lookup object
-
-        Assigns loaded data and defaults
-        to the DATA member variable
-
-        Args:
-            filename
-        Kwargs:
-            Keyword arguments can be used to
-            set default values for the lookup
-            function. METHOD sets the method
-            used for interpolation at the end of lookup
-            mode 3. pchip by default
-        """
-        data = self.__load(filename)
-        if data is not None:
-            self.__DATA = data
-        else:
-            raise Exception(f"Data could not be loaded from {filename}")
-
-        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
-        self.__default = {
-            'L'     :   kwargs.get('L', min(self.__DATA['L'])),
-            'VGS'   :   kwargs.get('VGS', self.__DATA['VGS']),
-            'VDS'   :   kwargs.get('VDS', max(self.__DATA['VDS'])/2),
-            'VSB'   :   kwargs.get('VSB', 0.0),
-            'METHOD':   kwargs.get('METHOD', 'pchip'),
-            'VGB'   :   kwargs.get('VGB', None),
-            'GM_ID' :   kwargs.get('GM_ID', None),
-            'ID_W'  :   kwargs.get('ID_W', None),
-            'VDB'   :   kwargs.get('VDB', None)
-        }
-
-    def __load(self, filename):
-        """
-        Function to load data from file
-
-        Loads array data from file. Currently supports .mat files only.
-        .mat is parsed to convert MATLAB cell data into a dictionary of
-        arrays. Data is loaded from value with first non-header key. 
-        Python interprets MATLAB cell structures as 1-D nests. Nested 
-        data is accessed and deep copied to member DATA variable
-
-        Args:
-            filename
-
-        Returns:
-            First MATLAB variable encountered in file as data
-        """
-        if filename.endswith('.mat'):
-            # parse .mat file into dict object
-            mat = scipy.io.loadmat(filename, matlab_compatible=True)
-
-            for k in mat.keys():
-                if not( k.startswith('__') and k.endswith('__') ):
-                    mat = mat[k]
-                    data = {k.upper():copy.deepcopy(np.squeeze(mat[k][0][0])) for k in mat.dtype.names}
-                    return data   
-        # !TODO add functionality to load other data structures
-        return None
-
-    def __getitem__(self, key):
-        """
-        __getitem__ dunder method overwritten to allow convenient
-        pseudo array access to member data. Returns a copy of the
-        member array.
-        """
-        if key not in self.__DATA.keys():
-            raise ValueError(f"Lookup table does not contain this data")
-
-        return np.copy(self.__DATA[key])
-
-    def _modeset(self, outkey, varkey):
-        """
-        Function to set lookup mode
-            MODE1: output is single variable, variable arg is single
-            MODE2: output is ratio, variable arg is single
-            MODE3: output is ratio, variable arg is ratio
-
-        Args:
-            outkey: keywords (list) of output argument
-            varkey: keywords (list) of variable argument
-
-        Returns:
-            mode (integer). Error if invalid mode selected
-        """
-        out_ratio = isinstance(outkey, list) and len(outkey) > 1
-        var_ratio = isinstance(varkey, list) and len(varkey) > 1
-        if out_ratio and var_ratio:
-            mode = 3
-        elif out_ratio and (not var_ratio):
-            mode = 2
-        elif (not out_ratio) and (not var_ratio):
-            mode = 1
-        else:
-            raise Exception("Invalid syntax or usage mode! Please check documentation.")
-        
-        return mode
-
-    def lookup(self, out, **kwargs):
-        """
-        Alias for look_up() function
-        """
-        return self.look_up(out, **kwargs)
-
-    def look_up(self, out, **kwargs):
-        """
-        Entry method for lookup functionality
-
-        Sanitises input. Extracts the variable key as first key value pair
-        in kwargs dict. Both the outkey and varkey are converted to lists.
-        String is split based on _ character.
-
-        Mode is determined and appropriate lookup function is called from
-        modefuncmap dict
-
-        Args:
-            out: desired variable to be interpolated 'GM', 'ID' etc
-            kwargs: keyword arguments (dict). First key-value pair is
-                    variable argument
-
-        Returns:
-            y: interpolated data, [] if erroneous mode selected
-        """
-        outkeys = out.upper().split('_')
-        varkeys, vararg = next(iter((kwargs.items()))) if kwargs else (None, None)
-        varkeys = str(varkeys).upper().split('_')
-
-        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
-        defaultdict = {k:self.__default.get(k) for k in ['L', 'VGS', 'VDS', 'VSB', 'METHOD']}
-        pars = {k:kwargs.get(k, v) for k, v in defaultdict.items()} # extracts parameters from kwargs
-        
-        # common kwargs for interpolating functions
-        ipkwargs = {'bounds_error': False,
-                    'fill_value' : None}
-
-        try:
-            mode = self._modeset(outkeys, varkeys)
-        except:
-            return []
-        # appropriate lookup function is called with modefuncmap dict
-        y = self.__modefuncmap.get(mode) (outkeys, varkeys, vararg, pars, **ipkwargs)
-        
-        return y
-
-    def _SimpleLK(self, outkeys, varkeys, vararg, pars, **ipkwargs):
-        """
-        Lookup for Modes 1 and 2
-
-        Args:
-            outkeys: list of keys for desired output e.g ['GM', 'ID'] for 'GM_ID'
-            varkeys: unused
-            pars: dict containing L, VGS, VDS and VSB data
-        Output:
-            output: interpolated data specified by outkeys Squeezed to remove extra
-                    dimensions
-        """
-
-        if len(outkeys) > 1:
-            num, den = outkeys
-            with np.errstate(divide='ignore',invalid='ignore'):
-                ydata =  self.__DATA[num]/self.__DATA[den]
-                # nan causing issues with interpn extrapolation
-                ydata[np.isnan(ydata)] = 0.0
-        else:
-            outkey = outkeys[0]
-            ydata = self.__DATA[outkey]
-
-        points = (self.__DATA['L'], self.__DATA['VGS'], self.__DATA['VDS'],\
-            self.__DATA['VSB'])
-        xi_mesh = np.array(np.meshgrid(pars['L'], pars['VGS'], pars['VDS'], pars['VSB'], indexing='ij'))
-        xi = np.rollaxis(xi_mesh, 0, 5)
-        xi = xi.reshape(int(xi_mesh.size/4), 4)
-
-        output = interpn(points, ydata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
-            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
-                 len(np.atleast_1d(pars['VSB'])) )
-        
-        # remove extra dimensions
-        output = np.squeeze(output)
-
-        return output
-
-    def _RatioVRatioLK(self, outkeys, varkeys, vararg, pars, **ipkwargs):
-        """
-        Lookup for Mode 3
-
-        Args:
-            outkeys: list of keys for desired output e.g ['GM', 'ID'] for 'GM_ID'
-            varkeys: list of keys for ratio input e.g ['GM', 'ID'] for 'GM_ID'
-            pars: dict containing L, VGS, VDS and VSB data
-        Output:
-            output: interpolated data specified by outkeys. Squeezed to remove extra
-                    dimensions
-        """
-        with np.errstate(divide='ignore',invalid='ignore'):    
-            # unpack outkeys and ydata
-            num, den = outkeys
-            ydata =  self.__DATA[num]/self.__DATA[den]
-            ydata[np.isnan(ydata)] = 0.0
-            # unpack varkeys and xdata
-            num, den = varkeys
-            xdata = self.__DATA[num]/self.__DATA[den]
-            xdata[np.isnan(xdata)] = 0.0
-
-        xdesired = np.atleast_1d(vararg)
-        
-        points = (self.__DATA['L'], self.__DATA['VGS'], self.__DATA['VDS'],\
-            self.__DATA['VSB'])
-        xi_mesh = np.array(np.meshgrid(pars['L'], pars['VGS'], pars['VDS'], pars['VSB'], indexing='ij'))
-        xi = np.rollaxis(xi_mesh, 0, 5)
-        xi = xi.reshape(int(xi_mesh.size/4), 4)
-        #ipnkwargs = {'bounds_error' : False,
-        #            'fill_value'   : None}
-
-        x = interpn(points, xdata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
-            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
-                 len(np.atleast_1d(pars['VSB'])))
-        
-        y = interpn(points, ydata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
-            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
-                 len(np.atleast_1d(pars['VSB'])))
-        
-        x = np.array(np.squeeze(np.transpose(x, (1, 0, 2, 3))))
-        y = np.array(np.squeeze(np.transpose(y, (1, 0, 2, 3))))
-        
-        if x.ndim == 1:
-            x.shape += (1,)
-            y.shape += (1,)
-
-        dim = x.shape
-        output = np.zeros((dim[1], len(xdesired)))
-        ipkwargs['kind'] = pars['METHOD']
-        
-        for i in range(0, dim[1]):
-            for j in range(0, len(xdesired)):
-                m = max(x[:, i])
-                idx = np.argmax(x[:, i])
-                if (xdesired[j] > m):
-                    print(f'Look up warning: {num}_{den} input larger than maximum! Output is NaN')
-                if (num.upper() == 'GM') and (den.upper() == 'ID'):
-                    x_right = x[idx:-1, i]
-                    y_right = y[idx:-1, i]
-                    output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
-                elif (num.upper() == 'GM') and (den.upper() == 'CGG') or (den.upper() == 'CGG'):
-                    x_left = x[1:idx, i]
-                    y_left = y[1:idx, i]
-                    output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
-                else:
-                    crossings = len(np.argwhere(np.diff(np.sign(x[:,i]-xdesired[j]+eps))))
-                    if crossings > 1:
-                        print('Crossing warning')
-                        return []
-                output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
-
-        output = np.squeeze(output)
-
-        return output
-
-    def lookupVGS(self, **kwargs):
-        return self.look_upVGS(**kwargs)
-
-    def look_upVGS(self, **kwargs):
-        """
-        Companion function to "look_up." Finds transistor VGS for a given inversion level (GM_ID)
-        or current density (ID/W) and given terminal voltages. 
-        The function interpolates (linear only) when the requested points lie off the simulation grid
-        
-        There are two basic usage scenarios:
-        (1) Lookup VGS with known voltage at the source terminal
-        (2) Lookup VGS with unknown source voltage, e.g. when the source of the
-        transistor is the tail node of a differential pair
-        
-        At most one of the input arguments can be a vector; the other must be
-        scalars.
-        
-        Examples of usage modes are given in test_lookupVGS.py
-        
-        Args:
-            pars: dict containing L, VGB, GM_ID and ID_W, VDS, VSB and METHOD
-        Output:
-            output: 1-d numpy array
-        """
-        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
-        defaultdict = {k:self.__default.get(k) for k in ['L', 'VDS', 'VDB', 'VGB', 'GM_ID', 'ID_W', 'VSB', 'METHOD']}
-        pars = {k:kwargs.get(k, v) for k,v in defaultdict.items()}
-
-        #Check whether GM_ID or ID_W was passed to function
-        ratio_string = 'None'
-        ratio_data = None
-
-        if pars['ID_W'] is not None:
-            ratio_string = 'ID_W'
-            ratio_data = pars['ID_W']
-
-        elif pars['GM_ID'] is not None:
-            ratio_string = 'GM_ID'
-            ratio_data = pars['GM_ID']
-        
-        # determining the mode 
-        # In usage mode (1), the inputs to the function are GM_ID (or ID/W), L, 
-        # VDS and VSB
-        if (pars['VGB'] and pars['VDB']) == None:
-            mode = 1
-        # In usage mode (2), VDB and VGB must be supplied to the function
-        elif (pars['VGB'] and pars['VDB']) != None:
-            mode = 2
-        else:
-            print("Invalid syntax or usage mode!")
-        
-        if mode == 1:
-            VGS = self['VGS']
-            ratio = self.look_up(ratio_string, VGS = VGS, VDS=pars['VDS'], VSB=pars['VSB'], L=pars['L'])
-        
-        elif mode == 2:
-            step = self['VGS'][0] - self['VGS'][1]
-            VSB = np.arange(max(self['VSB']), min(self['VSB']) + step, step)
-            VGS = pars['VGB'] - VSB
-            VDS = pars['VDB'] - VSB
-            ratio = np.array([self.look_up(ratio_string, VGS=VGS[i], VDS=VDS[i], VSB=VSB[i], L=pars['L']).item() for i in range(len(VGS))])
-            idx = ~np.isnan(ratio)
-            ratio = ratio[idx]
-            VGS = VGS[idx]
-  
-        if (np.size(pars['L']) == 1):
-            ratio.shape += (1,)
-        else:
-            ratio = np.swapaxes(ratio, 0, 1)
-
-        s = ratio.shape
-        
-        output = np.empty((s[1], len(np.atleast_1d(ratio_data))))
-        output[:] = np.NaN
-         
-        for j in range(s[1]):
-            ratio_range = ratio[:,j]
-            VGS_range = VGS
-
-            if ratio_string == 'GM_ID':
-                m = max(ratio)
-                idx = np.argmax(ratio)
-                VGS_range = VGS_range[idx:]
-                ratio_range = ratio_range[idx:]
-
-                if max(np.atleast_1d(ratio_data)) > m:
-                    print('look_upVGS: GM_ID input larger than maximum!')
-            
-            output[j,:] = interp1(ratio_range, VGS_range)(ratio_data)
-            output = output[:]
-        
-        return np.squeeze(output)
+import copy
+
+import numpy as np
+import scipy.io
+from scipy.interpolate import interpn
+import pickle
+
+from .constants import eps
+from .numerical import interp1
+
+class Lookup:
+    def __init__(self, filename="MOS.mat", **kwargs):
+        self.__setup(filename, **kwargs)
+        self.__modefuncmap = {1 : self._SimpleLK,
+                              2 : self._SimpleLK,  
+                              3 : self._RatioVRatioLK}
+
+    def __setup(self, filename, **kwargs):
+        """
+        Setup the Lookup object
+
+        Assigns loaded data and defaults
+        to the DATA member variable
+
+        Args:
+            filename
+        Kwargs:
+            Keyword arguments can be used to
+            set default values for the lookup
+            function. METHOD sets the method
+            used for interpolation at the end of lookup
+            mode 3. pchip by default
+        """
+        data = self.__load(filename)
+        if data is not None:
+            self.__DATA = data
+        else:
+            raise Exception(f"Data could not be loaded from {filename}")
+
+        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
+        self.__default = {
+            'L'     :   kwargs.get('L', min(self.__DATA['L'])),
+            'VGS'   :   kwargs.get('VGS', self.__DATA['VGS']),
+            'VDS'   :   kwargs.get('VDS', max(self.__DATA['VDS'])/2),
+            'VSB'   :   kwargs.get('VSB', 0.0),
+            'METHOD':   kwargs.get('METHOD', 'pchip'),
+            'VGB'   :   kwargs.get('VGB', None),
+            'GM_ID' :   kwargs.get('GM_ID', None),
+            'ID_W'  :   kwargs.get('ID_W', None),
+            'VDB'   :   kwargs.get('VDB', None)
+        }
+
+    def __load(self, filename):
+        """
+        Function to load data from file
+
+        Loads array data from file. Currently supports .mat files only.
+        .mat is parsed to convert MATLAB cell data into a dictionary of
+        arrays. Data is loaded from value with first non-header key. 
+        Python interprets MATLAB cell structures as 1-D nests. Nested 
+        data is accessed and deep copied to member DATA variable
+
+        Args:
+            filename
+
+        Returns:
+            First MATLAB variable encountered in file as data
+        """
+        if filename.endswith('.mat'):
+            # parse .mat file into dict object
+            mat = scipy.io.loadmat(filename, matlab_compatible=True)
+
+            for k in mat.keys():
+                if not( k.startswith('__') and k.endswith('__') ):
+                    mat = mat[k]
+                    data = {k.upper():copy.deepcopy(np.squeeze(mat[k][0][0])) for k in mat.dtype.names}
+                    return data   
+        
+        elif filename.endswith('.pkl'):
+            with open(filename, 'rb') as f:
+                data = pickle.load(f)
+                return data
+
+        # !TODO add functionality to load other data structures
+        return None
+
+    def __getitem__(self, key):
+        """
+        __getitem__ dunder method overwritten to allow convenient
+        pseudo array access to member data. Returns a copy of the
+        member array.
+        """
+        if key not in self.__DATA.keys():
+            raise ValueError(f"Lookup table does not contain this data")
+
+        return np.copy(self.__DATA[key])
+
+    def _modeset(self, outkey, varkey):
+        """
+        Function to set lookup mode
+            MODE1: output is single variable, variable arg is single
+            MODE2: output is ratio, variable arg is single
+            MODE3: output is ratio, variable arg is ratio
+
+        Args:
+            outkey: keywords (list) of output argument
+            varkey: keywords (list) of variable argument
+
+        Returns:
+            mode (integer). Error if invalid mode selected
+        """
+        out_ratio = isinstance(outkey, list) and len(outkey) > 1
+        var_ratio = isinstance(varkey, list) and len(varkey) > 1
+        if out_ratio and var_ratio:
+            mode = 3
+        elif out_ratio and (not var_ratio):
+            mode = 2
+        elif (not out_ratio) and (not var_ratio):
+            mode = 1
+        else:
+            raise Exception("Invalid syntax or usage mode! Please check documentation.")
+        
+        return mode
+
+    def lookup(self, out, **kwargs):
+        """
+        Alias for look_up() function
+        """
+        return self.look_up(out, **kwargs)
+
+    def look_up(self, out, **kwargs):
+        """
+        Entry method for lookup functionality
+
+        Sanitises input. Extracts the variable key as first key value pair
+        in kwargs dict. Both the outkey and varkey are converted to lists.
+        String is split based on _ character.
+
+        Mode is determined and appropriate lookup function is called from
+        modefuncmap dict
+
+        Args:
+            out: desired variable to be interpolated 'GM', 'ID' etc
+            kwargs: keyword arguments (dict). First key-value pair is
+                    variable argument
+
+        Returns:
+            y: interpolated data, [] if erroneous mode selected
+        """
+        outkeys = out.upper().split('_')
+        varkeys, vararg = next(iter((kwargs.items()))) if kwargs else (None, None)
+        varkeys = str(varkeys).upper().split('_')
+
+        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
+        defaultdict = {k:self.__default.get(k) for k in ['L', 'VGS', 'VDS', 'VSB', 'METHOD']}
+        pars = {k:kwargs.get(k, v) for k, v in defaultdict.items()} # extracts parameters from kwargs
+        
+        # common kwargs for interpolating functions
+        ipkwargs = {'bounds_error': False,
+                    'fill_value' : None}
+
+        try:
+            mode = self._modeset(outkeys, varkeys)
+        except:
+            return []
+        # appropriate lookup function is called with modefuncmap dict
+        y = self.__modefuncmap.get(mode) (outkeys, varkeys, vararg, pars, **ipkwargs)
+        
+        return y
+
+    def _SimpleLK(self, outkeys, varkeys, vararg, pars, **ipkwargs):
+        """
+        Lookup for Modes 1 and 2
+
+        Args:
+            outkeys: list of keys for desired output e.g ['GM', 'ID'] for 'GM_ID'
+            varkeys: unused
+            pars: dict containing L, VGS, VDS and VSB data
+        Output:
+            output: interpolated data specified by outkeys Squeezed to remove extra
+                    dimensions
+        """
+
+        if len(outkeys) > 1:
+            num, den = outkeys
+            with np.errstate(divide='ignore',invalid='ignore'):
+                ydata =  self.__DATA[num]/self.__DATA[den]
+                # nan causing issues with interpn extrapolation
+                ydata[np.isnan(ydata)] = 0.0
+        else:
+            outkey = outkeys[0]
+            ydata = self.__DATA[outkey]
+
+        points = (self.__DATA['L'], self.__DATA['VGS'], self.__DATA['VDS'],\
+            self.__DATA['VSB'])
+        xi_mesh = np.array(np.meshgrid(pars['L'], pars['VGS'], pars['VDS'], pars['VSB'], indexing='ij'))
+        xi = np.rollaxis(xi_mesh, 0, 5)
+        xi = xi.reshape(int(xi_mesh.size/4), 4)
+
+        output = interpn(points, ydata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
+            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
+                 len(np.atleast_1d(pars['VSB'])) )
+        
+        # remove extra dimensions
+        output = np.squeeze(output)
+
+        return output
+
+    def _RatioVRatioLK(self, outkeys, varkeys, vararg, pars, **ipkwargs):
+        """
+        Lookup for Mode 3
+
+        Args:
+            outkeys: list of keys for desired output e.g ['GM', 'ID'] for 'GM_ID'
+            varkeys: list of keys for ratio input e.g ['GM', 'ID'] for 'GM_ID'
+            pars: dict containing L, VGS, VDS and VSB data
+        Output:
+            output: interpolated data specified by outkeys. Squeezed to remove extra
+                    dimensions
+        """
+        with np.errstate(divide='ignore',invalid='ignore'):    
+            # unpack outkeys and ydata
+            num, den = outkeys
+            ydata =  self.__DATA[num]/self.__DATA[den]
+            ydata[np.isnan(ydata)] = 0.0
+            # unpack varkeys and xdata
+            num, den = varkeys
+            xdata = self.__DATA[num]/self.__DATA[den]
+            xdata[np.isnan(xdata)] = 0.0
+
+        xdesired = np.atleast_1d(vararg)
+        
+        points = (self.__DATA['L'], self.__DATA['VGS'], self.__DATA['VDS'],\
+            self.__DATA['VSB'])
+        xi_mesh = np.array(np.meshgrid(pars['L'], pars['VGS'], pars['VDS'], pars['VSB'], indexing='ij'))
+        xi = np.rollaxis(xi_mesh, 0, 5)
+        xi = xi.reshape(int(xi_mesh.size/4), 4)
+        #ipnkwargs = {'bounds_error' : False,
+        #            'fill_value'   : None}
+
+        x = interpn(points, xdata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
+            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
+                 len(np.atleast_1d(pars['VSB'])))
+        
+        y = interpn(points, ydata, xi, **ipkwargs).reshape(len(np.atleast_1d(pars['L'])), \
+            len(np.atleast_1d(pars['VGS'])), len(np.atleast_1d(pars['VDS'])),\
+                 len(np.atleast_1d(pars['VSB'])))
+        
+        x = np.array(np.squeeze(np.transpose(x, (1, 0, 2, 3))))
+        y = np.array(np.squeeze(np.transpose(y, (1, 0, 2, 3))))
+        
+        if x.ndim == 1:
+            x.shape += (1,)
+            y.shape += (1,)
+
+        dim = x.shape
+        output = np.zeros((dim[1], len(xdesired)))
+        ipkwargs['kind'] = pars['METHOD']
+        
+        for i in range(0, dim[1]):
+            for j in range(0, len(xdesired)):
+                m = max(x[:, i])
+                idx = np.argmax(x[:, i])
+                if (xdesired[j] > m):
+                    print(f'Look up warning: {num}_{den} input larger than maximum! Output is NaN')
+                if (num.upper() == 'GM') and (den.upper() == 'ID'):
+                    x_right = x[idx:-1, i]
+                    y_right = y[idx:-1, i]
+                    output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
+                elif (num.upper() == 'GM') and (den.upper() == 'CGG') or (den.upper() == 'CGG'):
+                    x_left = x[1:idx, i]
+                    y_left = y[1:idx, i]
+                    output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
+                else:
+                    crossings = len(np.argwhere(np.diff(np.sign(x[:,i]-xdesired[j]+eps))))
+                    if crossings > 1:
+                        print('Crossing warning')
+                        return []
+                output[i, j] = interp1(x_right, y_right, **ipkwargs)(xdesired[j])
+
+        output = np.squeeze(output)
+
+        return output
+
+    def lookupVGS(self, **kwargs):
+        return self.look_upVGS(**kwargs)
+
+    def look_upVGS(self, **kwargs):
+        """
+        Companion function to "look_up." Finds transistor VGS for a given inversion level (GM_ID)
+        or current density (ID/W) and given terminal voltages. 
+        The function interpolates (linear only) when the requested points lie off the simulation grid
+        
+        There are two basic usage scenarios:
+        (1) Lookup VGS with known voltage at the source terminal
+        (2) Lookup VGS with unknown source voltage, e.g. when the source of the
+        transistor is the tail node of a differential pair
+        
+        At most one of the input arguments can be a vector; the other must be
+        scalars.
+        
+        Examples of usage modes are given in test_lookupVGS.py
+        
+        Args:
+            pars: dict containing L, VGB, GM_ID and ID_W, VDS, VSB and METHOD
+        Output:
+            output: 1-d numpy array
+        """
+        kwargs = {k.upper(): v for k, v in kwargs.items()} # convert kwargs to upper
+        defaultdict = {k:self.__default.get(k) for k in ['L', 'VDS', 'VDB', 'VGB', 'GM_ID', 'ID_W', 'VSB', 'METHOD']}
+        pars = {k:kwargs.get(k, v) for k,v in defaultdict.items()}
+
+        #Check whether GM_ID or ID_W was passed to function
+        ratio_string = 'None'
+        ratio_data = None
+
+        if pars['ID_W'] is not None:
+            ratio_string = 'ID_W'
+            ratio_data = pars['ID_W']
+
+        elif pars['GM_ID'] is not None:
+            ratio_string = 'GM_ID'
+            ratio_data = pars['GM_ID']
+        
+        # determining the mode 
+        # In usage mode (1), the inputs to the function are GM_ID (or ID/W), L, 
+        # VDS and VSB
+        if (pars['VGB'] and pars['VDB']) == None:
+            mode = 1
+        # In usage mode (2), VDB and VGB must be supplied to the function
+        elif (pars['VGB'] and pars['VDB']) != None:
+            mode = 2
+        else:
+            print("Invalid syntax or usage mode!")
+        
+        if mode == 1:
+            VGS = self['VGS']
+            ratio = self.look_up(ratio_string, VGS = VGS, VDS=pars['VDS'], VSB=pars['VSB'], L=pars['L'])
+        
+        elif mode == 2:
+            step = self['VGS'][0] - self['VGS'][1]
+            VSB = np.arange(max(self['VSB']), min(self['VSB']) + step, step)
+            VGS = pars['VGB'] - VSB
+            VDS = pars['VDB'] - VSB
+            ratio = np.array([self.look_up(ratio_string, VGS=VGS[i], VDS=VDS[i], VSB=VSB[i], L=pars['L']).item() for i in range(len(VGS))])
+            idx = ~np.isnan(ratio)
+            ratio = ratio[idx]
+            VGS = VGS[idx]
+  
+        if (np.size(pars['L']) == 1):
+            ratio.shape += (1,)
+        else:
+            ratio = np.swapaxes(ratio, 0, 1)
+
+        s = ratio.shape
+        
+        output = np.empty((s[1], len(np.atleast_1d(ratio_data))))
+        output[:] = np.NaN
+         
+        for j in range(s[1]):
+            ratio_range = ratio[:,j]
+            VGS_range = VGS
+
+            if ratio_string == 'GM_ID':
+                m = max(ratio)
+                idx = np.argmax(ratio)
+                VGS_range = VGS_range[idx:]
+                ratio_range = ratio_range[idx:]
+
+                if max(np.atleast_1d(ratio_data)) > m:
+                    print('look_upVGS: GM_ID input larger than maximum!')
+            
+            output[j,:] = interp1(ratio_range, VGS_range)(ratio_data)
+            output = output[:]
+        
+        return np.squeeze(output)
```

### Comparing `pygmid-1.0/src/pygmid/Spectre.py` & `pygmid-1.0.1/src/pygmid/Spectre.py`

 * *Ordering differences only*

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-import logging
-import subprocess
-import os.path
-
-from subprocess import CalledProcessError
-
-class Spectre:
-    def __init__(self, *args):
-        self.__args = ['spectre', *args]
-
-    def run(self, filename):
-        infile = filename
-        try:
-            cp = subprocess.run(self.__args + [infile], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
-        except CalledProcessError as e:
-            logging.info(f"Error executing process\n\n{e}")
-            return
+import logging
+import subprocess
+import os.path
+
+from subprocess import CalledProcessError
+
+class Spectre:
+    def __init__(self, *args):
+        self.__args = ['spectre', *args]
+
+    def run(self, filename):
+        infile = filename
+        try:
+            cp = subprocess.run(self.__args + [infile], check=True, stdout=subprocess.PIPE, stderr=subprocess.PIPE)
+        except CalledProcessError as e:
+            logging.info(f"Error executing process\n\n{e}")
+            return
         logging.info(cp.stdout)
```

### Comparing `pygmid-1.0/src/pygmid/__main__.py` & `pygmid-1.0.1/src/pygmid/__main__.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,37 +1,37 @@
-import logging
-import sys
-
-from .version import __version__
-from . import pygmid
-
-def _cli():
-    from argparse import ArgumentParser
-    description = "CLI for pygmid. Run techsweeps"
-    parser = ArgumentParser(description=description)
-    parser.add_argument('--version', action='version', version=f"%prog {__version__}")
-    parser.add_argument('-c', action='store_const', dest='constant_value',
-                        const='value-to-store',
-                        help='Store a constant value')
-
-    results = parser.parse_args()
-    # assign values from results here
-    # val = results.constant_value
-
-    #if opt.backend is not None:
-    #    zookeeper.backend = opt.backend
-    #if opt.configfile is not None:
-    #    zookeeper.configfile = opt.configfile
-
-    #if len(remaining_args) != 0:
-    #    print("Usage: python -m zookeeper [settings] \npython -m zookeeper -h for help")
-    #    sys.exit(1)
-    
-    # setup logger    
-    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
-    
-    pygmid.main()
-    sys.exit(0)
-        
-if __name__ == '__main__':
-    # setup logger here
-    _cli()
+import logging
+import sys
+
+from .version import __version__
+from . import pygmid
+
+def _cli():
+    from argparse import ArgumentParser
+    description = "CLI for pygmid. Run techsweeps"
+    parser = ArgumentParser(description=description)
+    parser.add_argument('--version', action='version', version=f"%prog {__version__}")
+    parser.add_argument('-c', action='store_const', dest='constant_value',
+                        const='value-to-store',
+                        help='Store a constant value')
+
+    results = parser.parse_args()
+    # assign values from results here
+    # val = results.constant_value
+
+    #if opt.backend is not None:
+    #    zookeeper.backend = opt.backend
+    #if opt.configfile is not None:
+    #    zookeeper.configfile = opt.configfile
+
+    #if len(remaining_args) != 0:
+    #    print("Usage: python -m zookeeper [settings] \npython -m zookeeper -h for help")
+    #    sys.exit(1)
+    
+    # setup logger    
+    logging.basicConfig(stream=sys.stdout, level=logging.DEBUG)
+    
+    pygmid.main()
+    sys.exit(0)
+        
+if __name__ == '__main__':
+    # setup logger here
+    _cli()
```

### Comparing `pygmid-1.0/src/pygmid/numerical.py` & `pygmid-1.0.1/src/pygmid/numerical.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,41 +1,41 @@
-import numpy as np
-from scipy.interpolate import interp1d, PchipInterpolator
-
-def monotonic_interp1(x, y, **ipkwargs):
-    # check for maximum monotonic subarray here
-    # ...
-    # placeholder
-    xsub = x
-    ysub = y
-    # ...
-
-    return interp1(xsub, ysub, **ipkwargs)
-
-def interp1(x, y, **ipkwargs):
-    """
-    Wrapper function for python 1d interpolation
-    Combines the functionality of interp1d and PchipInterpolator.
-
-    Reorders x and y for increasing monotonicity in x
-
-    Args:
-        x, y
-    Kwargs:
-        Interpolation keywords - see interp1d
-    """
-
-    METHOD = ipkwargs.get('kind', 'pchip')
-    if METHOD == 'pchip':
-        # need to convert ipkwargs
-        pchipkwargs = {
-            'axis'          :   ipkwargs.get('axis', 0),
-            'extrapolate'   :   ipkwargs.get('extrapolate', True)
-        }
-        # enforce increasing monotonicity
-        ind = np.argsort(x)
-        x = x[ind]
-        y = np.take(y, ind, axis=-1)
-
-        return PchipInterpolator(x, y, **pchipkwargs)
-    else:
+import numpy as np
+from scipy.interpolate import interp1d, PchipInterpolator
+
+def monotonic_interp1(x, y, **ipkwargs):
+    # check for maximum monotonic subarray here
+    # ...
+    # placeholder
+    xsub = x
+    ysub = y
+    # ...
+
+    return interp1(xsub, ysub, **ipkwargs)
+
+def interp1(x, y, **ipkwargs):
+    """
+    Wrapper function for python 1d interpolation
+    Combines the functionality of interp1d and PchipInterpolator.
+
+    Reorders x and y for increasing monotonicity in x
+
+    Args:
+        x, y
+    Kwargs:
+        Interpolation keywords - see interp1d
+    """
+
+    METHOD = ipkwargs.get('kind', 'pchip')
+    if METHOD == 'pchip':
+        # need to convert ipkwargs
+        pchipkwargs = {
+            'axis'          :   ipkwargs.get('axis', 0),
+            'extrapolate'   :   ipkwargs.get('extrapolate', True)
+        }
+        # enforce increasing monotonicity
+        ind = np.argsort(x)
+        x = x[ind]
+        y = np.take(y, ind, axis=-1)
+
+        return PchipInterpolator(x, y, **pchipkwargs)
+    else:
         return interp1d(x, y, **ipkwargs)
```

### Comparing `pygmid-1.0/src/pygmid/utility.py` & `pygmid-1.0.1/src/pygmid/utility.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,150 +1,150 @@
-import numpy as np
-
-from .numerical import interp1
-
-
-def EKV_param_extraction(lk, mode, **kwargs):
-    return XTRACT(lk, mode, **kwargs)
-
-def XTRACT(lk, mode, **kwargs):
-    """
-    EKV param extraction algorithm.
-
-    Two modes of operation:
-    1)  L, VSB are scalars. VDS scalar or column vector.
-        rho is an optional scalar
-
-    2)
-    """
-    plot = kwargs.get('plot', False)
-
-    if mode == 1:
-        L   =   kwargs.get('L', min(lk['L']))
-        VDS =   kwargs.get('VDS', lk['VDS'])
-        VSB =   kwargs.get('VSB', 0.0)
-        rho =   kwargs.get('rho', 0.6)
-        UDS =   kwargs.get('UDS', np.arange(0.025, 1.2+0.025, 0.025))
-
-        UT  =   0.0259 * np.asscalar(lk['TEMP'])/300
-
-        # find n(UDS)
-        gm_ID = lk.look_up('GM_ID', VDS=UDS.T, VSB=VSB, L=L)
-        # get max value from each column
-        M = np.amax(gm_ID.T, axis=1)
-        nn = 1/(M*UT)
-        # find VT(UDS)
-        q = 1/rho -1
-        i = q**2 + q
-        VP = UT * (2 * (q-1) + np.log(q))
-        gm_IDref = rho * M
-        # have to use linear interpolation here. gm_ID is not monotonic
-        VGS = [float(interp1(gm_ID[:,k], lk['VGS'], kind='pchip')(gm_IDref[k])) for k in range(len(UDS))]
-        
-        Vth = VGS - nn*VP
-        #find JS(UDS) ===============
-        Js = lk.lookup('ID_W',GM_ID=gm_IDref, VDS=UDS, VSB=VSB, L=L).diagonal()/i 
-        
-        # DERIVATIVES ===============
-        UDS1 = .5*(UDS[:-1] + UDS[1:])
-        UDS2 = .5*(UDS1[:-1] + UDS1[1:])
-        
-        diffUDS = np.diff(UDS)
-        diffUDS1 = np.diff(UDS1)
-
-        # subthreshold slope ============
-        diff1n = np.diff(nn)/diffUDS
-        diff2n = np.diff(diff1n)/diffUDS1
-
-        # threshold voltage =============
-        diff1Vth = np.diff(Vth)/diffUDS
-        diff2Vth = np.diff(diff1Vth)/diffUDS1
-
-        # log specific current ============
-        diff1logJs = np.diff(np.log(Js))/diffUDS
-        diff2logJs = np.diff(diff1logJs)/diffUDS1
-
-        # n(VDS), VT(VDS) , JS(VDS) ===========
-        n  = interp1(UDS, nn, kind='pchip')(VDS) 
-        VT = interp1(UDS, Vth, kind='pchip')(VDS)
-        JS = interp1(UDS, Js, kind='pchip')(VDS)
-
-        d1n = interp1(UDS1, diff1n, kind='pchip')(VDS)
-        d2n = interp1(UDS2, diff2n, kind='pchip')(VDS)
-
-        d1VT = interp1(UDS1, diff1Vth, kind='pchip')(VDS)
-        d2VT = interp1(UDS2, diff2Vth, kind='pchip')(VDS)
-
-        d1logJS = interp1(UDS1, diff1logJs, kind='pchip')(VDS)
-        d2logJS = interp1(UDS2, diff2logJs, kind='pchip')(VDS)
-
-        if plot:
-            #% FIGURE =============
-            # setup mpl
-            import matplotlib as mpl
-            import matplotlib.pyplot as plt
-            mpl.rcParams['axes.spines.right'] = False
-            mpl.rcParams['axes.spines.top'] = False
-            mpl.rcParams.update({"axes.grid" : True})
-            
-            plt.figure(1); plt.plot(UDS, nn, VDS, n, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(2); plt.plot(UDS1, diff1Vth, VDS, d1VT, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(3); plt.plot(UDS2, diff2Vth, VDS, d2VT, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.show()
-            print("Press enter to continue...")
-            input()
-
-            plt.figure(1); plt.plot(UDS, nn, VDS, n, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(2); plt.plot(UDS1, diff1n, VDS, d1n, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(3); plt.plot(UDS2, diff2n, VDS, d2n, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.show()
-            print("Press enter to continue...")
-            input()
-
-            plt.figure(1); plt.plot(UDS, Js, VDS, JS, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(2); plt.plot(UDS1, diff1logJs, VDS, d1logJS, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.figure(3); plt.plot(UDS2, diff2logJs, VDS, d2logJS, '*')
-            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
-            plt.show()
-            print("Press enter to continue...")
-            input()
-
-        return (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS) 
-    elif mode ==2:
-        print("Mode 2 not implemented")
-        return
-        #VGS =   kwargs.get('VGS', lk['VGS'])
-        #ID =   kwargs.get('ID', lk['ID'])
-        #rho =   kwargs.get('rho', 0.6)
-
-        #qFo = 1/rho - 1
-        #i = qFo * qFo + qFo
-
-        #UT = .026
-        #ID = np.atleast_2d(ID)
-        #m1, m2 = ID.shape
-        #gm_Id = np.diff(np.log(ID))/np.diff(VGS[])
-        #z1, b = max(gm_Id)
-
-        # compute VGSo and IDo -------
-        #UGS     = .5*(VGS(1:m1-1) + VGS(2:m1));
-        #for k = 1:m2,
-        #    VGSo(k,1) = interp1(gm_Id(:,k),UGS,z1(k)*rho,'cubic');
-        #    IDo(k,1)  = interp1(VGS,ID(:,k),VGSo(k,1),'cubic');
-        #end
-
-        #n  = 1./(UT*z1');
-        #VT  = VGSo - UT*n.*(2*(qFo-1)+log(qFo));
-        #IS = IDo/i;
-
-        #return n, VT, IS 
-    else:
-        print("Invalid mode")
+import numpy as np
+
+from .numerical import interp1
+
+
+def EKV_param_extraction(lk, mode, **kwargs):
+    return XTRACT(lk, mode, **kwargs)
+
+def XTRACT(lk, mode, **kwargs):
+    """
+    EKV param extraction algorithm.
+
+    Two modes of operation:
+    1)  L, VSB are scalars. VDS scalar or column vector.
+        rho is an optional scalar
+
+    2)
+    """
+    plot = kwargs.get('plot', False)
+
+    if mode == 1:
+        L   =   kwargs.get('L', min(lk['L']))
+        VDS =   kwargs.get('VDS', lk['VDS'])
+        VSB =   kwargs.get('VSB', 0.0)
+        rho =   kwargs.get('rho', 0.6)
+        UDS =   kwargs.get('UDS', np.arange(0.025, 1.2+0.025, 0.025))
+
+        UT  =   0.0259 * np.asscalar(lk['TEMP'])/300
+
+        # find n(UDS)
+        gm_ID = lk.look_up('GM_ID', VDS=UDS.T, VSB=VSB, L=L)
+        # get max value from each column
+        M = np.amax(gm_ID.T, axis=1)
+        nn = 1/(M*UT)
+        # find VT(UDS)
+        q = 1/rho -1
+        i = q**2 + q
+        VP = UT * (2 * (q-1) + np.log(q))
+        gm_IDref = rho * M
+        # have to use linear interpolation here. gm_ID is not monotonic
+        VGS = [float(interp1(gm_ID[:,k], lk['VGS'], kind='pchip')(gm_IDref[k])) for k in range(len(UDS))]
+        
+        Vth = VGS - nn*VP
+        #find JS(UDS) ===============
+        Js = lk.lookup('ID_W',GM_ID=gm_IDref, VDS=UDS, VSB=VSB, L=L).diagonal()/i 
+        
+        # DERIVATIVES ===============
+        UDS1 = .5*(UDS[:-1] + UDS[1:])
+        UDS2 = .5*(UDS1[:-1] + UDS1[1:])
+        
+        diffUDS = np.diff(UDS)
+        diffUDS1 = np.diff(UDS1)
+
+        # subthreshold slope ============
+        diff1n = np.diff(nn)/diffUDS
+        diff2n = np.diff(diff1n)/diffUDS1
+
+        # threshold voltage =============
+        diff1Vth = np.diff(Vth)/diffUDS
+        diff2Vth = np.diff(diff1Vth)/diffUDS1
+
+        # log specific current ============
+        diff1logJs = np.diff(np.log(Js))/diffUDS
+        diff2logJs = np.diff(diff1logJs)/diffUDS1
+
+        # n(VDS), VT(VDS) , JS(VDS) ===========
+        n  = interp1(UDS, nn, kind='pchip')(VDS) 
+        VT = interp1(UDS, Vth, kind='pchip')(VDS)
+        JS = interp1(UDS, Js, kind='pchip')(VDS)
+
+        d1n = interp1(UDS1, diff1n, kind='pchip')(VDS)
+        d2n = interp1(UDS2, diff2n, kind='pchip')(VDS)
+
+        d1VT = interp1(UDS1, diff1Vth, kind='pchip')(VDS)
+        d2VT = interp1(UDS2, diff2Vth, kind='pchip')(VDS)
+
+        d1logJS = interp1(UDS1, diff1logJs, kind='pchip')(VDS)
+        d2logJS = interp1(UDS2, diff2logJs, kind='pchip')(VDS)
+
+        if plot:
+            #% FIGURE =============
+            # setup mpl
+            import matplotlib as mpl
+            import matplotlib.pyplot as plt
+            mpl.rcParams['axes.spines.right'] = False
+            mpl.rcParams['axes.spines.top'] = False
+            mpl.rcParams.update({"axes.grid" : True})
+            
+            plt.figure(1); plt.plot(UDS, nn, VDS, n, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(2); plt.plot(UDS1, diff1Vth, VDS, d1VT, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(3); plt.plot(UDS2, diff2Vth, VDS, d2VT, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.show()
+            print("Press enter to continue...")
+            input()
+
+            plt.figure(1); plt.plot(UDS, nn, VDS, n, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(2); plt.plot(UDS1, diff1n, VDS, d1n, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(3); plt.plot(UDS2, diff2n, VDS, d2n, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.show()
+            print("Press enter to continue...")
+            input()
+
+            plt.figure(1); plt.plot(UDS, Js, VDS, JS, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(2); plt.plot(UDS1, diff1logJs, VDS, d1logJS, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.figure(3); plt.plot(UDS2, diff2logJs, VDS, d2logJS, '*')
+            #plt.ylabel(r"$n$"); plt.xlabel(r"$V_{DS}$ [V]")
+            plt.show()
+            print("Press enter to continue...")
+            input()
+
+        return (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS) 
+    elif mode ==2:
+        print("Mode 2 not implemented")
+        return
+        #VGS =   kwargs.get('VGS', lk['VGS'])
+        #ID =   kwargs.get('ID', lk['ID'])
+        #rho =   kwargs.get('rho', 0.6)
+
+        #qFo = 1/rho - 1
+        #i = qFo * qFo + qFo
+
+        #UT = .026
+        #ID = np.atleast_2d(ID)
+        #m1, m2 = ID.shape
+        #gm_Id = np.diff(np.log(ID))/np.diff(VGS[])
+        #z1, b = max(gm_Id)
+
+        # compute VGSo and IDo -------
+        #UGS     = .5*(VGS(1:m1-1) + VGS(2:m1));
+        #for k = 1:m2,
+        #    VGSo(k,1) = interp1(gm_Id(:,k),UGS,z1(k)*rho,'cubic');
+        #    IDo(k,1)  = interp1(VGS,ID(:,k),VGSo(k,1),'cubic');
+        #end
+
+        #n  = 1./(UT*z1');
+        #VT  = VGSo - UT*n.*(2*(qFo-1)+log(qFo));
+        #IS = IDo/i;
+
+        #return n, VT, IS 
+    else:
+        print("Invalid mode")
         return
```

### Comparing `pygmid-1.0/src/pygmid.egg-info/PKG-INFO` & `pygmid-1.0.1/src/pygmid.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,361 +1,349 @@
-Metadata-Version: 2.1
-Name: pygmid
-Version: 1.0
-Summary: A python 3 implementation of the gm/ID starter kit
-Home-page: https://github.com/madrasalach/pygmid
-Author: Cian O`Donnell, Danylo Galach
-Author-email: cian.odonnell@tyndall.ie
-License: UNKNOWN
-Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-<p align="center">
-  <a>
-    <img src="docs/img/icon.png" width="80">
-  </a>
-
-  <h3 align="center">pygmid</h3>
-
-  <p align="center">
-    A python3 implementation of the gm/ID starter kit
-    <br>
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
-    ·
-    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
-  </p>
-</p>
-
-## Table of contents
-
-- [About](#about)
-- [Installation](#installation)
-- [Usage](#usage)
-- [TODO](#todo)
-- [Authors](#authors)
-
-## About
-
-pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
-of Stanford University. The package also offers some scripts from the Paul Jesper's book.
-
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
-
-## Installation
-
-To install pygmid from source, download from Github and run pip:
-
-`pip install .`
-
- in the root directory.
-
- pygmid can also be installed from PyPI:
-
-`pip install pygmid`
-
-## Usage
-
-### Scripting with the Lookup Class
-A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
-
-You can create a lookup object as follows:
-
-```python
-from pygmid import Lookup as lk
-
-NCH = lk('180nch.mat')
-```
-### Access MOS Data
-The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
-
-```python
-# get VGS data as array from NCH
-VGS_array = NCH['VGS']
-```
-
-Data is returned as a deep copy of the array contained in the `Lookup` object.
-
-### Lookup functionality 
-
-Lookup of interpolated data occurs as follows:
-
-```python
-VDSs = NCH['VDS'] 
-VGSs = np.arange(0.4, 0.6, 0.05)
-# Plot ID versus VDS
-ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
-# alias function lookup can also be used
-ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
-# check bias
-VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
-print(f'VGS is: {VGS}')
-
-plt.plot(VDSs, np.transpose(ID))
-```
-
-~~Currently only lookup modes 1 and 2 are implemented.~~
-Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
-
-### Technology Extraction Functions
-
-The EKV extraction function can be used as follows:
-
-```python
-from pygmid import EKV_param_extraction, XTRACT
-
-(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
-        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
-
-```
-
-Sample usage of this and other utility functions can be found in `test_utility.py` .
-
-### Examples
-
-Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
-
-Sample outputs are given below:
-
-![image](docs/img/IDvVDS.png)
-
-![image](docs/img/vtvsL.png)
-
-![image](docs/img/gm_gds.png)
-
-![image](docs/img/ft.png)
-
-![image](docs/img/idwVDS.png)
-
-![image](docs/img/IDWvsgmID.png)
-
-### Command Line Interface (CLI)
-
-`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
-
-## !TODO
-- ~~look_up MODE 3 (ratio vs ratio)~~
-- ~~look_upVGS and lookupVGS~~
-- ~~pchip interpolation~~
-- SPECTRE techsweep
-- Support for non .mat data structures
-- Improved logging for error generation
-
-## Authors
-
-- Cian O'Donnell : cian.odonnell@tyndall.ie
-- Danylo Galach
-
-## Contributors
-
-- José Rui Custódio
-
-A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
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
-
-
+Metadata-Version: 2.1
+Name: pygmid
+Version: 1.0.1
+Summary: A python 3 implementation of the gm/ID starter kit
+Home-page: https://github.com/madrasalach/pygmid
+Author: Cian O`Donnell, Danylo Galach
+Author-email: cian.odonnell@tyndall.ie
+Project-URL: Bug Tracker, https://github.com/madrasalach/pygmid/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.4
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<p align="center">
+  <a>
+    <img src="docs/img/icon.png" width="80">
+  </a>
+
+  <h3 align="center">pygmid</h3>
+
+  <p align="center">
+    A python3 implementation of the gm/ID starter kit
+    <br>
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=bug.md">Report bug</a>
+    ·
+    <a href="https://www.github.com/madrasalach/pygmid/issues/new?template=feature.md&labels=feature">Request feature</a>
+  </p>
+</p>
+
+## Table of contents
+
+- [About](#about)
+- [Installation](#installation)
+- [Usage](#usage)
+- [Authors](#authors)
+
+## About
+
+pygmid is a Python 3 port of the gm/ID starter kit by Prof. Boris Murmann 
+of Stanford University. The package also offers some scripts from the Paul Jesper's book.
+
+For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
+section at Prof. Murmann's website: https://web.stanford.edu/~murmann.
+
+## Installation
+
+To install pygmid from source, download from Github and run pip:
+
+`pip install .`
+
+ in the root directory.
+
+ pygmid can also be installed from PyPI:
+
+`pip install pygmid`
+
+## Usage
+
+### Scripting with the Lookup Class
+A gm/ID lookup object can be generated with the `Lookup` class. The lookup object requires lookup data for initialisation. Currently, only `.mat` files are supported.
+
+You can create a lookup object as follows:
+
+```python
+from pygmid import Lookup as lk
+
+NCH = lk('180nch.mat')
+```
+### Access MOS Data
+The `Lookup` class allows for pseudo array access of the MOS matrix data. You can access data as follows:
+
+```python
+# get VGS data as array from NCH
+VGS_array = NCH['VGS']
+```
+
+Data is returned as a deep copy of the array contained in the `Lookup` object.
+
+### Lookup functionality 
+
+Lookup of interpolated data occurs as follows:
+
+```python
+VDSs = NCH['VDS'] 
+VGSs = np.arange(0.4, 0.6, 0.05)
+# Plot ID versus VDS
+ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs)
+# alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs)
+# check bias
+VGS = NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18)
+print(f'VGS is: {VGS}')
+
+plt.plot(VDSs, np.transpose(ID))
+```
+
+~~Currently only lookup modes 1 and 2 are implemented.~~
+Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The companion lookupVGS function is also included.
+
+### Technology Extraction Functions
+
+The EKV extraction function can be used as follows:
+
+```python
+from pygmid import EKV_param_extraction, XTRACT
+
+(VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT, d2logJS)\
+        = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0)
+
+```
+
+Sample usage of this and other utility functions can be found in `test_utility.py` .
+
+### Examples
+
+Usage of lookup scripts are given in `test_lookup.py` and `test_lookupVGS.py`.
+
+Sample outputs are given below:
+
+![image](docs/img/IDvVDS.png)
+
+![image](docs/img/vtvsL.png)
+
+![image](docs/img/gm_gds.png)
+
+![image](docs/img/ft.png)
+
+![image](docs/img/idwVDS.png)
+
+![image](docs/img/IDWvsgmID.png)
+
+### Command Line Interface (CLI)
+
+`pygmid` also features a CLI which can be used to run techweeps to generate transistor data
+
+## Authors
+
+- Cian O'Donnell : cian.odonnell@mcci.ie
+- Tiarnach Ó Riada : tiarnach.oriada@tyndall.ie
+- Danylo Galach
+
+## Contributors
+
+- José Rui Custódio
+
+A special thanks to Prof. Boris Murmann for giving permission to use his work and release this package under the Apache 2.0 License.
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

#### html2text {}

```diff
@@ -1,58 +1,55 @@
-Metadata-Version: 2.1 Name: pygmid Version: 1.0 Summary: A python 3
+Metadata-Version: 2.1 Name: pygmid Version: 1.0.1 Summary: A python 3
 implementation of the gm/ID starter kit Home-page: https://github.com/
 madrasalach/pygmid Author: Cian O`Donnell, Danylo Galach Author-email:
-cian.odonnell@tyndall.ie License: UNKNOWN Project-URL: Bug Tracker, https://
-github.com/madrasalach/pygmid/issues Platform: UNKNOWN Classifier: Programming
-Language :: Python :: 3 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.4 Description-Content-Type: text/markdown License-File:
-LICENSE
+cian.odonnell@tyndall.ie Project-URL: Bug Tracker, https://github.com/
+madrasalach/pygmid/issues Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent Requires-Python: >=3.4
+Description-Content-Type: text/markdown License-File: LICENSE
                               [docs/img/icon.png]
                                **** pygmid ****
               A python3 implementation of the gm/ID starter kit
                          Report_bug Â· Request_feature
 ## Table of contents - [About](#about) - [Installation](#installation) -
-[Usage](#usage) - [TODO](#todo) - [Authors](#authors) ## About pygmid is a
-Python 3 port of the gm/ID starter kit by Prof. Boris Murmann of Stanford
-University. The package also offers some scripts from the Paul Jesper's book.
-For the gm/ID starter kit, written for MATLAB, please refer to the 'Links'
-section at Prof. Murmann's website: https://web.stanford.edu/~murmann. ##
-Installation To install pygmid from source, download from Github and run pip:
-`pip install .` in the root directory. pygmid can also be installed from PyPI:
-`pip install pygmid` ## Usage ### Scripting with the Lookup Class A gm/ID
-lookup object can be generated with the `Lookup` class. The lookup object
-requires lookup data for initialisation. Currently, only `.mat` files are
-supported. You can create a lookup object as follows: ```python from pygmid
-import Lookup as lk NCH = lk('180nch.mat') ``` ### Access MOS Data The `Lookup`
-class allows for pseudo array access of the MOS matrix data. You can access
-data as follows: ```python # get VGS data as array from NCH VGS_array = NCH
-['VGS'] ``` Data is returned as a deep copy of the array contained in the
-`Lookup` object. ### Lookup functionality Lookup of interpolated data occurs as
-follows: ```python VDSs = NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID
-versus VDS ID = NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup
-can also be used ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS =
-NCH.look_upVGS(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is:
-{VGS}') plt.plot(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1
-and 2 are implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary
-ratio lookup) and mode 3 (cross lookup of ratios) are implemented. The
-companion lookupVGS function is also included. ### Technology Extraction
-Functions The EKV extraction function can be used as follows: ```python from
-pygmid import EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS,
-d2n, d2VT, d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB =
-0.0) ``` Sample usage of this and other utility functions can be found in
+[Usage](#usage) - [Authors](#authors) ## About pygmid is a Python 3 port of the
+gm/ID starter kit by Prof. Boris Murmann of Stanford University. The package
+also offers some scripts from the Paul Jesper's book. For the gm/ID starter
+kit, written for MATLAB, please refer to the 'Links' section at Prof. Murmann's
+website: https://web.stanford.edu/~murmann. ## Installation To install pygmid
+from source, download from Github and run pip: `pip install .` in the root
+directory. pygmid can also be installed from PyPI: `pip install pygmid` ##
+Usage ### Scripting with the Lookup Class A gm/ID lookup object can be
+generated with the `Lookup` class. The lookup object requires lookup data for
+initialisation. Currently, only `.mat` files are supported. You can create a
+lookup object as follows: ```python from pygmid import Lookup as lk NCH = lk
+('180nch.mat') ``` ### Access MOS Data The `Lookup` class allows for pseudo
+array access of the MOS matrix data. You can access data as follows: ```python
+# get VGS data as array from NCH VGS_array = NCH['VGS'] ``` Data is returned as
+a deep copy of the array contained in the `Lookup` object. ### Lookup
+functionality Lookup of interpolated data occurs as follows: ```python VDSs =
+NCH['VDS'] VGSs = np.arange(0.4, 0.6, 0.05) # Plot ID versus VDS ID =
+NCH.look_up('ID', vds=VDSs, vgs=VGSs) # alias function lookup can also be used
+ID = NCH.lookup('ID', vds=VDSs, vgs=VGSs) # check bias VGS = NCH.look_upVGS
+(GM_ID = 10, VDS = 0.6, VSB = 0.1, L = 0.18) print(f'VGS is: {VGS}') plt.plot
+(VDSs, np.transpose(ID)) ``` ~~Currently only lookup modes 1 and 2 are
+implemented.~~ Modes 1 (Simple parameter lookup), mode 2 (arbitrary ratio
+lookup) and mode 3 (cross lookup of ratios) are implemented. The companion
+lookupVGS function is also included. ### Technology Extraction Functions The
+EKV extraction function can be used as follows: ```python from pygmid import
+EKV_param_extraction, XTRACT (VDS, n, VT, JS, d1n, d1VT, d1logJS, d2n, d2VT,
+d2logJS)\ = EKV_param_extraction(NCH, 1, L = 0.18, VDS = 0.6, VSB = 0.0) ```
+Sample usage of this and other utility functions can be found in
 `test_utility.py` . ### Examples Usage of lookup scripts are given in
 `test_lookup.py` and `test_lookupVGS.py`. Sample outputs are given below: !
 [image](docs/img/IDvVDS.png) ![image](docs/img/vtvsL.png) ![image](docs/img/
 gm_gds.png) ![image](docs/img/ft.png) ![image](docs/img/idwVDS.png) ![image]
 (docs/img/IDWvsgmID.png) ### Command Line Interface (CLI) `pygmid` also
 features a CLI which can be used to run techweeps to generate transistor data
-## !TODO - ~~look_up MODE 3 (ratio vs ratio)~~ - ~~look_upVGS and lookupVGS~~ -
-~~pchip interpolation~~ - SPECTRE techsweep - Support for non .mat data
-structures - Improved logging for error generation ## Authors - Cian O'Donnell
-: cian.odonnell@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
+## Authors - Cian O'Donnell : cian.odonnell@mcci.ie - Tiarnach Ã Riada :
+tiarnach.oriada@tyndall.ie - Danylo Galach ## Contributors - JosÃ© Rui
 CustÃ³dio A special thanks to Prof. Boris Murmann for giving permission to use
 his work and release this package under the Apache 2.0 License. Apache License
 Version 2.0, January 2004 http://www.apache.org/licenses/ TERMS AND CONDITIONS
 FOR USE, REPRODUCTION, AND DISTRIBUTION 1. Definitions. "License" shall mean
 the terms and conditions for use, reproduction, and distribution as defined by
 Sections 1 through 9 of this document. "Licensor" shall mean the copyright
 owner or entity authorized by the copyright owner that is granting the License.
```

