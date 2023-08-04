# Comparing `tmp/ghast_scanner-1.4.5.tar.gz` & `tmp/ghast_scanner-1.4.6.tar.gz`

## Comparing `ghast_scanner-1.4.5.tar` & `ghast_scanner-1.4.6.tar`

### file list

```diff
@@ -1,35 +1,35 @@
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/.pylintrc
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/__about__.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/action.yml
--rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/colors.py
--rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/main.py
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/requirements.txt
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/.github/workflows/ghast-scan.yml
--rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-create-or-approves-pr-using-curl.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-creates-or-approves-pr-using-gh-cli.yml
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-creates-or-approves-pr-using-gh-script.yml
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-using-github-cache.yml
--rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-using-self-hosted-runner-in-matrix.yml
--rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-using-self-hosted-runner-referenced-by-group.yml
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-using-self-hosted-runners.yml
--rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-dangerous-gh-context-variables.yml
--rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-dangerous-gh-variables-2.yml
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-dangerous-gh-variables.yml
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-inline-script.yml
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-pull-request-target.yml
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-remote-script.yml
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-unsecure-command-env-var.yml
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-write-all-permissions.yml
--rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-write-permissions-all-jobs.yml
--rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/actions/action-with-write-permissions-one-job.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/analyzer/__init__.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/analyzer/analyzer.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/analyzer/analyzer_test.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/analyzer/regex.py
--rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/images/ghast-stdout.png
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/LICENSE
--rw-r--r--   0        0        0     5264 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/README.md
--rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/pyproject.toml
--rw-r--r--   0        0        0     6375 2020-02-02 00:00:00.000000 ghast_scanner-1.4.5/PKG-INFO
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.pylintrc
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/__about__.py
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/action.yml
+-rw-r--r--   0        0        0      665 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/colors.py
+-rw-r--r--   0        0        0     5071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/main.py
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/requirements.txt
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.github/workflows/ghast-scan.yml
+-rw-r--r--   0        0        0      683 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-create-or-approves-pr-using-curl.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-creates-or-approves-pr-using-gh-cli.yml
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-creates-or-approves-pr-using-gh-script.yml
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-configure-aws-creds-non-oidc-auth.yml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-github-cache.yml
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runner-in-matrix.yml
+-rw-r--r--   0        0        0      187 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runner-referenced-by-group.yml
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-using-self-hosted-runners.yml
+-rw-r--r--   0        0        0      274 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-context-variables.yml
+-rw-r--r--   0        0        0      453 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-variables-2.yml
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-dangerous-gh-variables.yml
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-inline-script.yml
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-pull-request-target.yml
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-remote-script.yml
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-unsecure-command-env-var.yml
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-all-permissions.yml
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-permissions-all-jobs.yml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/actions/action-with-write-permissions-one-job.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/__init__.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/analyzer.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/analyzer_test.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/analyzer/regex.py
+-rw-r--r--   0        0        0  2360423 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/images/ghast-stdout.png
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/LICENSE
+-rw-r--r--   0        0        0     5272 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/README.md
+-rw-r--r--   0        0        0     3249 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/pyproject.toml
+-rw-r--r--   0        0        0     6383 2020-02-02 00:00:00.000000 ghast_scanner-1.4.6/PKG-INFO
```

### Comparing `ghast_scanner-1.4.5/action.yml` & `ghast_scanner-1.4.6/action.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,58 +1,57 @@
-name: 'actions-security-analyzer'
-description: 'Scan your GitHub actions folder for common security vulnerabilities'
-author: 'bin3xish477'
+name: "actions-security-analyzer"
+description: "Scan your GitHub actions folder for common security vulnerabilities"
+author: "bin3xish477"
 branding:
-  icon: 'shield'
-  color: 'green'
+  icon: "shield"
+  color: "green"
 inputs:
   dir:
-    description: 'path to directory with GitHub Actions files to scan'
+    description: "path to directory with GitHub Actions files to scan"
     required: false
-    default: './.github/workflows'
+    default: "./.github/workflows"
   ignore-checks:
-    description: 'specify checks to ignore'
+    description: "specify checks to ignore"
     required: false
   ignore-warnings:
-    description: 'ignore checks labeled as WARN'
+    description: "ignore checks labeled as WARN"
     required: false
   no-summary:
     description: "don't show tool summary in output"
     required: false
   verbose:
-    description: 'enable verbose output'
+    description: "enable verbose output"
     required: false
 runs:
   using: composite
   steps:
-  - uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1 # v4.7.0
-    with:
-      python-version: '3.11' 
-  - run: |
-      pip install actions-security-analyzer
-      args=()
+    - uses: actions/setup-python@61a6322f88396a6271a6ee3565807d608ecaddd1 # v4.7.0
+      with:
+        python-version: "3.11"
+    - run: |
+        pip install ghast-scanner
+        args=()
+
+        dir=$( echo ${{ inputs.dir }} | tr '[:upper:]' '[:lower:]')
+        ignore_warnings=$( echo ${{ inputs.ignore-warnings }} | tr '[:upper:]' '[:lower:]')
+        ignore_checks=$( echo ${{ inputs.ignore-checks }} | tr '[:upper:]' '[:lower:]')
+        no_summary=$( echo ${{ inputs.no-summary }} | tr '[:upper:]' '[:lower:]')
+        verbose=$( echo ${{ inputs.verbose }} | tr '[:upper:]' '[:lower:]')
+
+        [ ! -z $dir ] && args+=('--dir', ${{ inputs.dir }})
+        [ ! -z $ignore_warnings ] && [[ $ignore_warnings != "false" ]] && args+=('--ignore-warnings')
+        [ ! -z $no_summary ] && [[ $no_summary != "false" ]] && args+=('--no-summary')
+        [ ! -z $verbose ] && [[ $verbose != "false" ]] && args+=('--verbose')
+
+        if [[ ! -z "$ignore_checks" ]]; then
+          checks=()
+          for check in $(echo $ignore_checks)
+          do
+            checks+=("$check")
+          done
+          args+=('--ignore-checks', ${checks[@]/,/ })
+        fi
 
-      dir=$( echo ${{ inputs.dir }} | tr '[:upper:]' '[:lower:]')
-      ignore_warnings=$( echo ${{ inputs.ignore-warnings }} | tr '[:upper:]' '[:lower:]')
-      ignore_checks=$( echo ${{ inputs.ignore-checks }} | tr '[:upper:]' '[:lower:]')
-      no_summary=$( echo ${{ inputs.no-summary }} | tr '[:upper:]' '[:lower:]')
-      verbose=$( echo ${{ inputs.verbose }} | tr '[:upper:]' '[:lower:]')
-
-      [ ! -z $dir ] && args+=('--dir', ${{ inputs.dir }})
-      [ ! -z $ignore_warnings ] && [[ $ignore_warnings != "false" ]] && args+=('--ignore-warnings')
-      [ ! -z $no_summary ] && [[ $no_summary != "false" ]] && args+=('--no-summary')
-      [ ! -z $verbose ] && [[ $verbose != "false" ]] && args+=('--verbose')
-
-      if [[ ! -z "$ignore_checks" ]]; then
-        checks=()
-        for check in $(echo $ignore_checks)
-        do
-          checks+=("$check")
-        done
-        args+=('--ignore-checks', ${checks[@]/,/ })
-      fi
-
-      echo "ARGS: ${args[@]/,/ }"
-      asa ${args[@]/,/ }
-
-    shell: bash
+        echo "ARGS: ${args[@]/,/ }"
+        ghast ${args[@]/,/ }
 
+      shell: bash
```

### Comparing `ghast_scanner-1.4.5/colors.py` & `ghast_scanner-1.4.6/colors.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/main.py` & `ghast_scanner-1.4.6/main.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/.github/workflows/ghast-scan.yml` & `ghast_scanner-1.4.6/.github/workflows/ghast-scan.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/actions/action-create-or-approves-pr-using-curl.yml` & `ghast_scanner-1.4.6/actions/action-create-or-approves-pr-using-curl.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/actions/action-using-configure-aws-creds-non-oidc-auth.yml` & `ghast_scanner-1.4.6/actions/action-using-configure-aws-creds-non-oidc-auth.yml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/analyzer/analyzer.py` & `ghast_scanner-1.4.6/analyzer/analyzer.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/analyzer/analyzer_test.py` & `ghast_scanner-1.4.6/analyzer/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/analyzer/regex.py` & `ghast_scanner-1.4.6/analyzer/regex.py`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/images/ghast-stdout.png` & `ghast_scanner-1.4.6/images/ghast-stdout.png`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/.gitignore` & `ghast_scanner-1.4.6/.gitignore`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/LICENSE` & `ghast_scanner-1.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/README.md` & `ghast_scanner-1.4.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ![ghast-stdout](/images/ghast-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
-pip install ghast
+pip install ghast-scanner
 ```
 
 ### Usage
 
 ```
 ghast --file action.yml
 ghast -d directory-with-actions/ --verbose
```

### Comparing `ghast_scanner-1.4.5/pyproject.toml` & `ghast_scanner-1.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ghast_scanner-1.4.5/PKG-INFO` & `ghast_scanner-1.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghast-scanner
-Version: 1.4.5
+Version: 1.4.6
 Summary: Analyze the security posture of your GitHub Actions
 Project-URL: Documentation, https://github.com/bin3xish477/ghast#readme
 Project-URL: Issues, https://github.com/bin3xish477/ghast/issues
 Project-URL: Source, https://github.com/bin3xish477/ghast
 Author-email: Alexis Rodriguez <arodriguez99@protonmail.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -32,15 +32,15 @@
 ![ghast-stdout](/images/ghast-stdout.png)
 
 ### Installation
 
 > Make sure you have `$HOME/.local/bin` in your PATH
 
 ```
-pip install ghast
+pip install ghast-scanner
 ```
 
 ### Usage
 
 ```
 ghast --file action.yml
 ghast -d directory-with-actions/ --verbose
```

