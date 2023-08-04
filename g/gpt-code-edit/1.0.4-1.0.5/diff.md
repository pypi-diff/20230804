# Comparing `tmp/gpt-code-edit-1.0.4.tar.gz` & `tmp/gpt-code-edit-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-code-edit-1.0.4.tar", last modified: Fri Aug  4 15:15:19 2023, max compression
+gzip compressed data, was "gpt-code-edit-1.0.5.tar", last modified: Fri Aug  4 16:22:29 2023, max compression
```

## Comparing `gpt-code-edit-1.0.4.tar` & `gpt-code-edit-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 15:15:19.420145 gpt-code-edit-1.0.4/
--rw-rw-rw-   0        0        0     6378 2023-08-04 15:15:19.418167 gpt-code-edit-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     4816 2023-08-04 15:11:07.000000 gpt-code-edit-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 15:15:19.331148 gpt-code-edit-1.0.4/chatgpt_cli/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.4/chatgpt_cli/__init__.py
--rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.4/chatgpt_cli/arguement_validator.py
--rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.4/chatgpt_cli/code_parser.py
-drwxrwxrwx   0        0        0        0 2023-08-04 15:15:19.346147 gpt-code-edit-1.0.4/chatgpt_cli/commands/
--rw-rw-rw-   0        0        0        0 2023-08-04 14:23:06.000000 gpt-code-edit-1.0.4/chatgpt_cli/commands/__init__.py
--rw-rw-rw-   0        0        0     6609 2023-08-04 14:02:44.000000 gpt-code-edit-1.0.4/chatgpt_cli/commands/code_edit.py
--rw-rw-rw-   0        0        0     3402 2023-08-04 14:35:15.000000 gpt-code-edit-1.0.4/chatgpt_cli/commands/review_to_file.py
--rw-rw-rw-   0        0        0     1090 2023-08-04 13:42:38.000000 gpt-code-edit-1.0.4/chatgpt_cli/commands/set_api_key.py
--rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.4/chatgpt_cli/gpt_request.py
--rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.4/chatgpt_cli/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 15:15:19.413146 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/
--rw-rw-rw-   0        0        0     6378 2023-08-04 15:15:18.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-08-04 15:15:19.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 15:15:19.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-04 15:15:19.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-08-04 15:15:19.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 15:15:19.000000 gpt-code-edit-1.0.4/gpt_code_edit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 15:15:19.420145 gpt-code-edit-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1313 2023-08-04 15:13:25.000000 gpt-code-edit-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5063 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/chatgpt_cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7368 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/arguement_validator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10813 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/code_parser.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/chatgpt_cli/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6504 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/commands/code_edit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3346 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/commands/review_to_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/commands/set_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6309 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/gpt_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1038 2023-08-04 16:22:13.000000 gpt-code-edit-1.0.5/chatgpt_cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5900 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-08-04 16:22:29.000000 gpt-code-edit-1.0.5/gpt_code_edit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-04 16:22:29.731982 gpt-code-edit-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-08-04 16:22:28.000000 gpt-code-edit-1.0.5/setup.py
```

### Comparing `gpt-code-edit-1.0.4/PKG-INFO` & `gpt-code-edit-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,117 @@
-Metadata-Version: 2.1
-Name: gpt-code-edit
-Version: 1.0.4
-Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
-Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
-Author: Ben Speakman
-Author-email: benspeakman23@yahoo.com
-License: UNKNOWN
-Description: # GPT Code Edit
-        
-        gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
-        
-        ## Github
-        
-        https://github.com/ben-23-96/chatgpt_code_improve_cli
-        
-        ## PyPI
-        
-        https://pypi.org/project/gpt-code-edit/
-        
-        ## Prerequisites
-        
-        - Python 3.9
-        - An active OpenAI account with API keys
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
-        
-        ```bash
-        pip install gpt-code-edit
-        ```
-        
-        ## Usage
-        
-        ### Set API Key
-        
-        First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
-        
-        ```bash
-        gpt set-api-key <api_key>
-        ```
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<api_key>` | The OpenAI API key for the user. |
-        
-        ### Code Edit
-        
-        This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
-        
-        ```bash
-        gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
-        ```
-        
-        **Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
-        
-        **Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<filename>` | The filename of the file containing the code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted. |
-        | `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        | `--refactor` | If set, refactor the code. |
-        | `--comments` | If set, add comments to the code. |
-        | `--docstrings` | If set, add docstrings to the code. |
-        | `--error-handling` | If set, add error handling to the code. |
-        | `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
-        | `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
-        | `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-        | `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
-        
-        ### Review to File
-        
-        If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
-        
-        ```bash
-        gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
-        ```
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<filename>` | The filename of the file containing the original code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
-        | `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: gpt-code-edit
+Version: 1.0.5
+Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
+Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
+Author: Ben Speakman
+Author-email: benspeakman23@yahoo.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# GPT Code Edit
+
+gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
+
+## Github
+
+https://github.com/ben-23-96/chatgpt_code_improve_cli
+
+## PyPI
+
+https://pypi.org/project/gpt-code-edit/
+
+## Prerequisites
+
+- Python 3.9
+- An active OpenAI account with API keys
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
+
+```bash
+pip install gpt-code-edit
+```
+
+# Usage
+
+## Set API Key
+
+First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
+
+```bash
+gpt set-api-key <api_key>
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<api_key>` | The OpenAI API key for the user. |
+
+## Code Edit
+
+This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
+
+```bash
+gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
+```
+
+**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
+
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
+**Note**: One of `--target-functions`, `--target-methods` or `--target-classes` must be set. Multiple can be set at the same time.
+
+### Example
+
+The following command would add GPT generated comments into the function foo located in the main.py file.
+
+```bash
+gpt code-edit main.py --target-functions foo --comments --edit-code-in-file
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted. |
+| `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+| `--refactor` | If set, refactor the code. |
+| `--comments` | If set, add comments to the code. |
+| `--docstrings` | If set, add docstrings to the code. |
+| `--error-handling` | If set, add error handling to the code. |
+| `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
+| `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
+| `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+
+## Review to File
+
+If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
+
+```bash
+gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the original code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
+| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+
+
+
```

### Comparing `gpt-code-edit-1.0.4/README.md` & `gpt-code-edit-1.0.5/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,87 +1,97 @@
-# GPT Code Edit
-
-gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
-
-## Github
-
-https://github.com/ben-23-96/chatgpt_code_improve_cli
-
-## PyPI
-
-https://pypi.org/project/gpt-code-edit/
-
-## Prerequisites
-
-- Python 3.9
-- An active OpenAI account with API keys
-
-## Installation
-
-Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
-
-```bash
-pip install gpt-code-edit
-```
-
-## Usage
-
-### Set API Key
-
-First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
-
-```bash
-gpt set-api-key <api_key>
-```
-
-#### Arguments
-
-| Argument | Description |
-| :--- | :--- |
-| `<api_key>` | The OpenAI API key for the user. |
-
-### Code Edit
-
-This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
-
-```bash
-gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
-```
-
-**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
-
-**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
-
-#### Arguments
-
-| Argument | Description |
-| :--- | :--- |
-| `<filename>` | The filename of the file containing the code (eg. main.py). |
-| `--target-functions` | A space-separated list of function names to be targeted. |
-| `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-| `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-| `--refactor` | If set, refactor the code. |
-| `--comments` | If set, add comments to the code. |
-| `--docstrings` | If set, add docstrings to the code. |
-| `--error-handling` | If set, add error handling to the code. |
-| `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
-| `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
-| `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
-
-### Review to File
-
-If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
-
-```bash
-gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
-```
-
-#### Arguments
-
-| Argument | Description |
-| :--- | :--- |
-| `<filename>` | The filename of the file containing the original code (eg. main.py). |
-| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
-| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-
+# GPT Code Edit
+
+gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
+
+## Github
+
+https://github.com/ben-23-96/chatgpt_code_improve_cli
+
+## PyPI
+
+https://pypi.org/project/gpt-code-edit/
+
+## Prerequisites
+
+- Python 3.9
+- An active OpenAI account with API keys
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
+
+```bash
+pip install gpt-code-edit
+```
+
+# Usage
+
+## Set API Key
+
+First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
+
+```bash
+gpt set-api-key <api_key>
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<api_key>` | The OpenAI API key for the user. |
+
+## Code Edit
+
+This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
+
+```bash
+gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
+```
+
+**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
+
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
+**Note**: One of `--target-functions`, `--target-methods` or `--target-classes` must be set. Multiple can be set at the same time.
+
+### Example
+
+The following command would add GPT generated comments into the function foo located in the main.py file.
+
+```bash
+gpt code-edit main.py --target-functions foo --comments --edit-code-in-file
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted. |
+| `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+| `--refactor` | If set, refactor the code. |
+| `--comments` | If set, add comments to the code. |
+| `--docstrings` | If set, add docstrings to the code. |
+| `--error-handling` | If set, add error handling to the code. |
+| `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
+| `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
+| `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+
+## Review to File
+
+If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
+
+```bash
+gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the original code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
+| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/arguement_validator.py` & `gpt-code-edit-1.0.5/chatgpt_cli/arguement_validator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,173 +1,173 @@
-from argparse import ArgumentTypeError
-from os import listdir
-
-class ArgumentValidator:
-    def __init__(self, args):
-        """
-    Parameters:
-    args (list): A list of arguments from the CLI.
-    """
-        self.args = args
-
-    def check_file_type(self):
-        """
-    Check the file type of the given filename.
-        
-    Raises:
-        ArgumentTypeError: If the file type is not '.py'.
-    """
-        # Get the file type by splitting the filename at the last dot and taking the last part
-        file_type = self.args.filename.split('.')[-1]
-    
-        # if the file type is not '.py' raise a error
-        if file_type != 'py':
-            raise ArgumentTypeError('\nInvalid file type. Only Python (.py) files are allowed.')
-
-    def check_one_of_method_or_class_or_function_provided(self):
-        """
-    Check if at least one of target functions, target methods, or target classes is provided.
-
-    Raises:
-        ArgumentTypeError: If none of the target functions, target methods, or target classes are provided.
-    """
-        if not self.args.target_functions and not self.args.target_methods and not self.args.target_classes:
-            raise ArgumentTypeError('\nAt least one of --target-functions, --target-methods or --target-classes must be provided.')
-
-    def check_one_of_review_or_edit_provided(self):
-        """
-    Checks if either --create-review-file or --edit-code-in-file is set.
-    Raises an ArgumentTypeError if neither option is set.
-    """
-        if not self.args.create_review_file and not self.args.edit_code_in_file:
-            raise ArgumentTypeError('\nEither --create-review-file or --edit-code-in-file must be set. Both can be set.')
-
-    def check_one_of_refactor_or_comments_or_docstrings_or_error_handling_provided(self):
-        """
-    Check if at least one of the options --refactor, --comments, --docstrings, --error-handling is provided.
-    
-    Raises:
-        ArgumentTypeError: If none of the options are provided.
-    """
-        if not self.args.refactor and not self.args.comments and not self.args.docstrings and not self.args.error_handling:
-            raise ArgumentTypeError('\nAt least one of --refactor, --comments, --docstrings, --error-handling must be provided.')
-
-    def check_no_class_and_methods_clash(self):
-        """
-    Check if there is a clash between the target classes and target methods.
-    Raises an ArgumentTypeError if there is a clash.
-    """
-        # Get the class names from the target methods
-        method_classes = [method.split('.')[0] for method in self.args.target_methods]
-    
-        # raise a error if there is any intersection between the target classes and method classes
-        if bool(set(self.args.target_classes) & set(method_classes)):
-            raise ArgumentTypeError(f'\nCannot provide --target-methods and --target-classes that contain the same class.\nTarget methods: {self.args.target_methods}\nTarget classes: {self.args.target_classes}')
-
-    def check_temp_range(self):
-        """
-    Checks if the temperature value is within the range of 0 and 1.
-    
-    Raises:
-        ArgumentTypeError: If the temperature value is not between 0 and 1.
-    """
-        if self.args.temp < 0 or self.args.temp > 1:
-            raise ArgumentTypeError("\ntemp must be between 0 and 1.")
-
-    def check_method_in_correct_format (self):
-        """
-    Check if the methods in the target_methods list are in the correct format.
-    The correct format is ClassName.method, where ClassName starts with an uppercase letter
-    and method is separated from the class name by a dot (.).
-  
-    Raises:
-        ArgumentTypeError: If any method in the target_methods list does not match the correct format.
-    """
-        for method in self.args.target_methods:
-            # Check if the first character of the method is not uppercase or if there is no dot in the method
-            if not method[0].isupper() or '.' not in method:
-                raise ArgumentTypeError(f"\nerror with method formating for {method}, must be ClassName.method")
-
-    def check_file_exists (self):
-        """
-        Check if the filename provided by the user can be opened.
-
-        Raises:
-            FileNotFoundError: If the filename provided cannot be opened.
-        """
-        try:
-            with open(self.args.filename, 'r') as file:
-                pass
-        except FileNotFoundError as e:
-            raise FileNotFoundError(f'\nCannot find the file: {self.args.filename}')
-
-    def check_file_folder_exists_review_to_file(self):
-        """
-    Check if a folder for the filename exists in the gpt_edit_review folder. Used in the review-to-file command.
-
-    Raises:
-        ArgumentTypeError: If the folder for the fiename does not exist.
-    """
-        filename_folder_name = self.args.filename[:-3]
-        if filename_folder_name not in listdir('gpt_edit_review'):
-            raise ArgumentTypeError(f'\nNo folder in gpt_edit_review for filename: {filename_folder_name}. No functions have been edited from the file and placed in the folder for review.')
-        
-    def check_gpt_edit_folder_exists_review_to_file(self):
-        """
-    Check if the gpt_edit_review folder exists. Used in the review-to-file command.
-
-    Raises:
-        ArgumentTypeError: If the gpt_edit_review folder does not exist.
-    """
-        try:
-            listdir('gpt_edit_review')
-        except Exception:
-            raise ArgumentTypeError('\nCannot use the review-to-code command as there is no gpt_edit_review folder. No functions have been edited and placed in the folder for review.')
-
-
-    def gpt_edit_validate(self):
-        """
-    Validates the input provided to the function for the gpt_edit command.
-    """
-        # Check the file type
-        self.check_file_type()
-
-        # Check the file exists
-        self.check_file_exists()
-    
-        # Check if either method, class, or function is provided
-        self.check_one_of_method_or_class_or_function_provided()
-    
-        # Check if either review or edit is provided
-        self.check_one_of_review_or_edit_provided()
-    
-        # Check if either refactor, comments, docstrings, or error handling is provided
-        self.check_one_of_refactor_or_comments_or_docstrings_or_error_handling_provided()
-    
-        # Check for clash between classes and methods
-        self.check_no_class_and_methods_clash()
-    
-        # Check the range of temporary variables
-        self.check_temp_range()
-    
-        # Check if methods are in the correct format
-        self.check_method_in_correct_format()
-
-    def review_to_file_validate(self):
-        """Validates the input provided to the function for the gpt_edit command."""
-        # Check the file type
-        self.check_file_type()
-
-        # Check for clash between classes and methods
-        self.check_no_class_and_methods_clash()
-    
-        # Check if methods are in the correct format
-        self.check_method_in_correct_format()
-        
-        # Check if either method, class, function is provided
-        self.check_one_of_method_or_class_or_function_provided()
-
-        # Check if gpt_edit_review_folder_exists
-        self.check_gpt_edit_folder_exists_review_to_file()
-        
-        # Check if a folder exists for the given filename in gpt_edit_review folder
-        self.check_file_folder_exists_review_to_file()
+from argparse import ArgumentTypeError
+from os import listdir
+
+class ArgumentValidator:
+    def __init__(self, args):
+        """
+    Parameters:
+    args (list): A list of arguments from the CLI.
+    """
+        self.args = args
+
+    def check_file_type(self):
+        """
+    Check the file type of the given filename.
+        
+    Raises:
+        ArgumentTypeError: If the file type is not '.py'.
+    """
+        # Get the file type by splitting the filename at the last dot and taking the last part
+        file_type = self.args.filename.split('.')[-1]
+    
+        # if the file type is not '.py' raise a error
+        if file_type != 'py':
+            raise ArgumentTypeError('\nInvalid file type. Only Python (.py) files are allowed.')
+
+    def check_one_of_method_or_class_or_function_provided(self):
+        """
+    Check if at least one of target functions, target methods, or target classes is provided.
+
+    Raises:
+        ArgumentTypeError: If none of the target functions, target methods, or target classes are provided.
+    """
+        if not self.args.target_functions and not self.args.target_methods and not self.args.target_classes:
+            raise ArgumentTypeError('\nAt least one of --target-functions, --target-methods or --target-classes must be provided.')
+
+    def check_one_of_review_or_edit_provided(self):
+        """
+    Checks if either --create-review-file or --edit-code-in-file is set.
+    Raises an ArgumentTypeError if neither option is set.
+    """
+        if not self.args.create_review_file and not self.args.edit_code_in_file:
+            raise ArgumentTypeError('\nEither --create-review-file or --edit-code-in-file must be set. Both can be set.')
+
+    def check_one_of_refactor_or_comments_or_docstrings_or_error_handling_provided(self):
+        """
+    Check if at least one of the options --refactor, --comments, --docstrings, --error-handling is provided.
+    
+    Raises:
+        ArgumentTypeError: If none of the options are provided.
+    """
+        if not self.args.refactor and not self.args.comments and not self.args.docstrings and not self.args.error_handling:
+            raise ArgumentTypeError('\nAt least one of --refactor, --comments, --docstrings, --error-handling must be provided.')
+
+    def check_no_class_and_methods_clash(self):
+        """
+    Check if there is a clash between the target classes and target methods.
+    Raises an ArgumentTypeError if there is a clash.
+    """
+        # Get the class names from the target methods
+        method_classes = [method.split('.')[0] for method in self.args.target_methods]
+    
+        # raise a error if there is any intersection between the target classes and method classes
+        if bool(set(self.args.target_classes) & set(method_classes)):
+            raise ArgumentTypeError(f'\nCannot provide --target-methods and --target-classes that contain the same class.\nTarget methods: {self.args.target_methods}\nTarget classes: {self.args.target_classes}')
+
+    def check_temp_range(self):
+        """
+    Checks if the temperature value is within the range of 0 and 1.
+    
+    Raises:
+        ArgumentTypeError: If the temperature value is not between 0 and 1.
+    """
+        if self.args.temp < 0 or self.args.temp > 1:
+            raise ArgumentTypeError("\ntemp must be between 0 and 1.")
+
+    def check_method_in_correct_format (self):
+        """
+    Check if the methods in the target_methods list are in the correct format.
+    The correct format is ClassName.method, where ClassName starts with an uppercase letter
+    and method is separated from the class name by a dot (.).
+  
+    Raises:
+        ArgumentTypeError: If any method in the target_methods list does not match the correct format.
+    """
+        for method in self.args.target_methods:
+            # Check if the first character of the method is not uppercase or if there is no dot in the method
+            if not method[0].isupper() or '.' not in method:
+                raise ArgumentTypeError(f"\nerror with method formating for {method}, must be ClassName.method")
+
+    def check_file_exists (self):
+        """
+        Check if the filename provided by the user can be opened.
+
+        Raises:
+            FileNotFoundError: If the filename provided cannot be opened.
+        """
+        try:
+            with open(self.args.filename, 'r') as file:
+                pass
+        except FileNotFoundError as e:
+            raise FileNotFoundError(f'\nCannot find the file: {self.args.filename}')
+
+    def check_file_folder_exists_review_to_file(self):
+        """
+    Check if a folder for the filename exists in the gpt_edit_review folder. Used in the review-to-file command.
+
+    Raises:
+        ArgumentTypeError: If the folder for the fiename does not exist.
+    """
+        filename_folder_name = self.args.filename[:-3]
+        if filename_folder_name not in listdir('gpt_edit_review'):
+            raise ArgumentTypeError(f'\nNo folder in gpt_edit_review for filename: {filename_folder_name}. No functions have been edited from the file and placed in the folder for review.')
+        
+    def check_gpt_edit_folder_exists_review_to_file(self):
+        """
+    Check if the gpt_edit_review folder exists. Used in the review-to-file command.
+
+    Raises:
+        ArgumentTypeError: If the gpt_edit_review folder does not exist.
+    """
+        try:
+            listdir('gpt_edit_review')
+        except Exception:
+            raise ArgumentTypeError('\nCannot use the review-to-code command as there is no gpt_edit_review folder. No functions have been edited and placed in the folder for review.')
+
+
+    def gpt_edit_validate(self):
+        """
+    Validates the input provided to the function for the gpt_edit command.
+    """
+        # Check the file type
+        self.check_file_type()
+
+        # Check the file exists
+        self.check_file_exists()
+    
+        # Check if either method, class, or function is provided
+        self.check_one_of_method_or_class_or_function_provided()
+    
+        # Check if either review or edit is provided
+        self.check_one_of_review_or_edit_provided()
+    
+        # Check if either refactor, comments, docstrings, or error handling is provided
+        self.check_one_of_refactor_or_comments_or_docstrings_or_error_handling_provided()
+    
+        # Check for clash between classes and methods
+        self.check_no_class_and_methods_clash()
+    
+        # Check the range of temporary variables
+        self.check_temp_range()
+    
+        # Check if methods are in the correct format
+        self.check_method_in_correct_format()
+
+    def review_to_file_validate(self):
+        """Validates the input provided to the function for the gpt_edit command."""
+        # Check the file type
+        self.check_file_type()
+
+        # Check for clash between classes and methods
+        self.check_no_class_and_methods_clash()
+    
+        # Check if methods are in the correct format
+        self.check_method_in_correct_format()
+        
+        # Check if either method, class, function is provided
+        self.check_one_of_method_or_class_or_function_provided()
+
+        # Check if gpt_edit_review_folder_exists
+        self.check_gpt_edit_folder_exists_review_to_file()
+        
+        # Check if a folder exists for the given filename in gpt_edit_review folder
+        self.check_file_folder_exists_review_to_file()
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/code_parser.py` & `gpt-code-edit-1.0.5/chatgpt_cli/code_parser.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,199 +1,199 @@
-from redbaron import RedBaron
-from os import makedirs, listdir
-
-class CodeParser:
-    def __init__(self, filename: str, function_names: list = [], class_names: list = [], method_names: list = []):
-        self.filename = filename
-        self.function_names = function_names
-        self.class_names = class_names
-        self.method_names = method_names
-        self.found_code_names_list = []
-        self.found_code_list = []
-        self.not_found_code_names_list = []
-        self.code_review_files = []
-
-    def find_target_code_gpt_edit(self):
-        # open file and parse the contents 
-        with open(self.filename, "r") as source_code:
-            parser = RedBaron(source_code.read())
-        
-        # find the classes methods and functions 
-        for name in self.function_names:
-            self.find_function(parser=parser, function_name=name)
-        for name in self.method_names:
-            self.find_method(parser=parser, class_method_name=name)
-        for name in self.class_names:
-            self.find_class(parser=parser, class_name=name)
-        
-        # return the found functions as strings in a list and the names of the functions not found in another list 
-        return self.found_code_list, self.not_found_code_names_list
-    
-    def find_target_code_in_gpt_edit_review_folder(self):
-        # get a list of the files in the gpt_edit_review/filename folder
-        self.code_review_files = listdir(f'gpt_edit_review/{self.filename[:-3]}')
-        # find the edited versions of the target functions, methods, classes in the gpt_edit_review folder files
-        for name in self.function_names:
-            self.check_code_in_review_file(name, self.find_function)
-    
-        for name in self.class_names:
-            self.check_code_in_review_file(name, self.find_class)
-    
-        for name in self.method_names:
-            self.check_code_in_review_file(name, self.find_method)
-
-        # return the found functions as strings in a list and the names of the functions not found in another list 
-        return self.found_code_list, self.not_found_code_names_list
-
-    def check_code_in_review_file(self, name, process_func):
-        # if a file for the function, method, class exists in gpt_edit_review folder
-        if f'{name}.py' in self.code_review_files:
-            # open the file and find the edited code
-            with open(f'gpt_edit_review/{self.filename[:-3]}/{name}.py', "r") as source_code:
-                parser = RedBaron(source_code.read())
-                process_func(parser, name)
-        # if not found add to not found list
-        else:
-            self.not_found_code_names_list.append(name)
-
-    
-    def find_class(self, parser, class_name):
-        # find the class
-        class_node = parser.find('class', class_name)
-        if not class_node:
-            self.not_found_code_names_list.append(class_name)
-        # find all methods in the class
-        method_nodes = class_node.find_all('def')
-        # create a list of all method names as ClassName.method
-        method_names = [f'{class_name}.{method_node.name}' for method_node in method_nodes]
-        # create a list of the code of each method as a string, replace removes string if class is from gpt_edit_review file
-        methods_code = [method_node.dumps().replace(f'\n##### ORIGINAL CLASS CODE #####\n', '') for method_node in method_nodes]
-        # add found function names
-        self.found_code_names_list.extend(method_names)
-        # add found code strings
-        self.found_code_list.extend(methods_code)
-
-    def find_method(self, parser, class_method_name):
-        # split ClassName.method to ClassName and method
-        class_name, method_name = class_method_name.split('.')
-        # find the class node in the file
-        class_node = parser.find('class', class_name)
-        # if not found add method to not found list
-        if not class_node:
-            self.not_found_code_names_list.append(class_method_name)
-            #continue
-        # find the method on the class
-        method_node = class_node.find('def', method_name)
-        # if not found add method to not found list
-        if not method_node:
-            self.not_found_code_names_list.append(class_method_name)
-            #continue
-        # add found function names to list
-        self.found_code_names_list.append(class_method_name)
-        # add found function code strings to list
-        self.found_code_list.append(method_node.dumps().replace(f'\n##### ORIGINAL METHOD CODE #####\n', ''))
-
-    def find_function(self, parser, function_name):
-        # find the function
-        function_node = parser.find('def', function_name)
-        # if not found add to not found list and continue
-        if not function_node:
-            self.not_found_code_names_list.append(function_name)
-            #continue
-        # add the name of the function to the found functions list
-        self.found_code_names_list.append(function_name)
-        # add the code of the function as a str to a list, replace removes string if function is from gpt_edit_review file
-        self.found_code_list.append(function_node.dumps().replace(f'\n##### ORIGINAL FUNCTION CODE #####\n', ''))
-
-    def replace_target_functions_with_new_functions(self, new_functions: list):
-        # parse the file
-        with open(self.filename, 'r') as source_code:
-            parser = RedBaron(source_code.read())
-        # create zip containing the name of the function or method and the newly edited version of it as a str
-        functions_name_code_zip = zip(self.found_code_names_list, new_functions)
-        
-        for name, function_code in functions_name_code_zip:
-            if '.' in name:
-                # must be class method
-                class_name, method_name = name.split('.')
-                # find the class
-                class_node = parser.find('class', class_name)
-                new_method = RedBaron(function_code)
-                # replace the method in the parser object with the newly edited version of the method
-                class_node.find('def', method_name).value = new_method[0].value.dumps().rstrip()
-            else:
-                # must be function
-                # parse the new function code
-                new_function = RedBaron(function_code).find('def', name)
-                # replace the function in the parser object with the newly edited version of the function
-                parser.find('def', name).value = new_function.value.dumps().rstrip()
-        
-        # write the edited file content from the parser into the file
-        with open(self.filename, 'w') as source_code:
-            source_code.write(parser.dumps())
-    
-    def create_review_code_files(self, new_functions: list):
-        # make folder to store created files
-        makedirs('gpt_edit_review', exist_ok=True)
-        makedirs(f'gpt_edit_review/{self.filename[:-3]}', exist_ok=True)
-        # create zip of function/method name, the original function code, and the newly edited function code
-        functions_zip = zip(self.found_code_names_list, self.found_code_list, new_functions)
-        # create list to store the methods for a class if the whole class was provided in as a --target-class
-        classes_name_code_zip_list= []
-        for function_name, original_code, new_code in functions_zip:
-            # if class method ClassName.method
-            if '.' in function_name:
-                # if ClassName in the class names provided, therefore method code part of a full class provided
-                class_name = function_name.split('.')[0]
-                if class_name in self.class_names:
-                    # add ClassName.method and new function code to list to be used in create_class_code_review_file function
-                    classes_name_code_zip_list.append((function_name, new_code))
-                    continue
-                # else method was not given as part of a full class
-                else:
-                     # write the original code and new code to a file for comparison for a class method
-                    with open(f'gpt_edit_review/{self.filename[:-3]}/{function_name}.py', "w") as f:
-                        f.write('##### NEW METHOD CODE #####\n\n')
-                        f.write(f'class {class_name}:\n    ')
-                        f.write(new_code.replace('\n    ', '\n        '))
-                        f.write('\n\n##### ORIGINAL METHOD CODE #####\n\n')
-                        f.write(f'class {class_name}:\n    ')
-                        f.write(original_code)
-                        continue
-            # write the original code and new code to a file for comparison if function
-            with open(f'gpt_edit_review/{self.filename[:-3]}/{function_name}.py', "w") as f:
-                f.write('##### NEW FUNCTION CODE #####\n\n')
-                f.write(new_code)
-                f.write('\n\n##### ORIGINAL FUNCTION CODE #####\n\n')
-                f.write(original_code)
-            # call method that will write full classes to file for comparison
-            self.create_class_code_review_file(classes_name_code_zip_list)
-
-    def create_class_code_review_file(self, classes_names_code_list):
-        # parse th file
-        with open(self.filename, "r") as source_code:
-            parser = RedBaron(source_code.read())
-        # loop through given classes
-        for class_name in self.class_names:
-            # group all ClassName.methods for given ClassName into list
-            class_tuples = [name_new_code_tuple for name_new_code_tuple in classes_names_code_list if name_new_code_tuple[0].split('.')[0] == class_name]
-            # find the class in parser object
-            class_node = parser.find('class', class_name)
-            # original class code as string
-            original_class_code = class_node.dumps()
-            for name, new_code in class_tuples:
-                new_method = RedBaron(new_code)
-                # replace method with newly edited method in the parser
-                class_node.find('def', name.split('.')[1]).value = new_method[0].value.dumps().rstrip()
-            # new class code as string
-            new_class_code = class_node.dumps()
-            # create output string
-            output_str = '##### NEW CLASS CODE #####\n\n'
-            output_str += new_class_code
-            output_str += '\n\n##### ORIGINAL CLASS CODE #####\n\n'
-            output_str += original_class_code
-            # write original class and new class to file for comparison
-            with open(f'gpt_edit_review/{self.filename[:-3]}/{class_name}.py', "w") as f:
-                f.write(output_str)
-
-    def remove_not_found(self):
+from redbaron import RedBaron
+from os import makedirs, listdir
+
+class CodeParser:
+    def __init__(self, filename: str, function_names: list = [], class_names: list = [], method_names: list = []):
+        self.filename = filename
+        self.function_names = function_names
+        self.class_names = class_names
+        self.method_names = method_names
+        self.found_code_names_list = []
+        self.found_code_list = []
+        self.not_found_code_names_list = []
+        self.code_review_files = []
+
+    def find_target_code_gpt_edit(self):
+        # open file and parse the contents 
+        with open(self.filename, "r") as source_code:
+            parser = RedBaron(source_code.read())
+        
+        # find the classes methods and functions 
+        for name in self.function_names:
+            self.find_function(parser=parser, function_name=name)
+        for name in self.method_names:
+            self.find_method(parser=parser, class_method_name=name)
+        for name in self.class_names:
+            self.find_class(parser=parser, class_name=name)
+        
+        # return the found functions as strings in a list and the names of the functions not found in another list 
+        return self.found_code_list, self.not_found_code_names_list
+    
+    def find_target_code_in_gpt_edit_review_folder(self):
+        # get a list of the files in the gpt_edit_review/filename folder
+        self.code_review_files = listdir(f'gpt_edit_review/{self.filename[:-3]}')
+        # find the edited versions of the target functions, methods, classes in the gpt_edit_review folder files
+        for name in self.function_names:
+            self.check_code_in_review_file(name, self.find_function)
+    
+        for name in self.class_names:
+            self.check_code_in_review_file(name, self.find_class)
+    
+        for name in self.method_names:
+            self.check_code_in_review_file(name, self.find_method)
+
+        # return the found functions as strings in a list and the names of the functions not found in another list 
+        return self.found_code_list, self.not_found_code_names_list
+
+    def check_code_in_review_file(self, name, process_func):
+        # if a file for the function, method, class exists in gpt_edit_review folder
+        if f'{name}.py' in self.code_review_files:
+            # open the file and find the edited code
+            with open(f'gpt_edit_review/{self.filename[:-3]}/{name}.py', "r") as source_code:
+                parser = RedBaron(source_code.read())
+                process_func(parser, name)
+        # if not found add to not found list
+        else:
+            self.not_found_code_names_list.append(name)
+
+    
+    def find_class(self, parser, class_name):
+        # find the class
+        class_node = parser.find('class', class_name)
+        if not class_node:
+            self.not_found_code_names_list.append(class_name)
+        # find all methods in the class
+        method_nodes = class_node.find_all('def')
+        # create a list of all method names as ClassName.method
+        method_names = [f'{class_name}.{method_node.name}' for method_node in method_nodes]
+        # create a list of the code of each method as a string, replace removes string if class is from gpt_edit_review file
+        methods_code = [method_node.dumps().replace(f'\n##### ORIGINAL CLASS CODE #####\n', '') for method_node in method_nodes]
+        # add found function names
+        self.found_code_names_list.extend(method_names)
+        # add found code strings
+        self.found_code_list.extend(methods_code)
+
+    def find_method(self, parser, class_method_name):
+        # split ClassName.method to ClassName and method
+        class_name, method_name = class_method_name.split('.')
+        # find the class node in the file
+        class_node = parser.find('class', class_name)
+        # if not found add method to not found list
+        if not class_node:
+            self.not_found_code_names_list.append(class_method_name)
+            #continue
+        # find the method on the class
+        method_node = class_node.find('def', method_name)
+        # if not found add method to not found list
+        if not method_node:
+            self.not_found_code_names_list.append(class_method_name)
+            #continue
+        # add found function names to list
+        self.found_code_names_list.append(class_method_name)
+        # add found function code strings to list
+        self.found_code_list.append(method_node.dumps().replace(f'\n##### ORIGINAL METHOD CODE #####\n', ''))
+
+    def find_function(self, parser, function_name):
+        # find the function
+        function_node = parser.find('def', function_name)
+        # if not found add to not found list and continue
+        if not function_node:
+            self.not_found_code_names_list.append(function_name)
+            #continue
+        # add the name of the function to the found functions list
+        self.found_code_names_list.append(function_name)
+        # add the code of the function as a str to a list, replace removes string if function is from gpt_edit_review file
+        self.found_code_list.append(function_node.dumps().replace(f'\n##### ORIGINAL FUNCTION CODE #####\n', ''))
+
+    def replace_target_functions_with_new_functions(self, new_functions: list):
+        # parse the file
+        with open(self.filename, 'r') as source_code:
+            parser = RedBaron(source_code.read())
+        # create zip containing the name of the function or method and the newly edited version of it as a str
+        functions_name_code_zip = zip(self.found_code_names_list, new_functions)
+        
+        for name, function_code in functions_name_code_zip:
+            if '.' in name:
+                # must be class method
+                class_name, method_name = name.split('.')
+                # find the class
+                class_node = parser.find('class', class_name)
+                new_method = RedBaron(function_code)
+                # replace the method in the parser object with the newly edited version of the method
+                class_node.find('def', method_name).value = new_method[0].value.dumps().rstrip()
+            else:
+                # must be function
+                # parse the new function code
+                new_function = RedBaron(function_code).find('def', name)
+                # replace the function in the parser object with the newly edited version of the function
+                parser.find('def', name).value = new_function.value.dumps().rstrip()
+        
+        # write the edited file content from the parser into the file
+        with open(self.filename, 'w') as source_code:
+            source_code.write(parser.dumps())
+    
+    def create_review_code_files(self, new_functions: list):
+        # make folder to store created files
+        makedirs('gpt_edit_review', exist_ok=True)
+        makedirs(f'gpt_edit_review/{self.filename[:-3]}', exist_ok=True)
+        # create zip of function/method name, the original function code, and the newly edited function code
+        functions_zip = zip(self.found_code_names_list, self.found_code_list, new_functions)
+        # create list to store the methods for a class if the whole class was provided in as a --target-class
+        classes_name_code_zip_list= []
+        for function_name, original_code, new_code in functions_zip:
+            # if class method ClassName.method
+            if '.' in function_name:
+                # if ClassName in the class names provided, therefore method code part of a full class provided
+                class_name = function_name.split('.')[0]
+                if class_name in self.class_names:
+                    # add ClassName.method and new function code to list to be used in create_class_code_review_file function
+                    classes_name_code_zip_list.append((function_name, new_code))
+                    continue
+                # else method was not given as part of a full class
+                else:
+                     # write the original code and new code to a file for comparison for a class method
+                    with open(f'gpt_edit_review/{self.filename[:-3]}/{function_name}.py', "w") as f:
+                        f.write('##### NEW METHOD CODE #####\n\n')
+                        f.write(f'class {class_name}:\n    ')
+                        f.write(new_code.replace('\n    ', '\n        '))
+                        f.write('\n\n##### ORIGINAL METHOD CODE #####\n\n')
+                        f.write(f'class {class_name}:\n    ')
+                        f.write(original_code)
+                        continue
+            # write the original code and new code to a file for comparison if function
+            with open(f'gpt_edit_review/{self.filename[:-3]}/{function_name}.py', "w") as f:
+                f.write('##### NEW FUNCTION CODE #####\n\n')
+                f.write(new_code)
+                f.write('\n\n##### ORIGINAL FUNCTION CODE #####\n\n')
+                f.write(original_code)
+            # call method that will write full classes to file for comparison
+            self.create_class_code_review_file(classes_name_code_zip_list)
+
+    def create_class_code_review_file(self, classes_names_code_list):
+        # parse th file
+        with open(self.filename, "r") as source_code:
+            parser = RedBaron(source_code.read())
+        # loop through given classes
+        for class_name in self.class_names:
+            # group all ClassName.methods for given ClassName into list
+            class_tuples = [name_new_code_tuple for name_new_code_tuple in classes_names_code_list if name_new_code_tuple[0].split('.')[0] == class_name]
+            # find the class in parser object
+            class_node = parser.find('class', class_name)
+            # original class code as string
+            original_class_code = class_node.dumps()
+            for name, new_code in class_tuples:
+                new_method = RedBaron(new_code)
+                # replace method with newly edited method in the parser
+                class_node.find('def', name.split('.')[1]).value = new_method[0].value.dumps().rstrip()
+            # new class code as string
+            new_class_code = class_node.dumps()
+            # create output string
+            output_str = '##### NEW CLASS CODE #####\n\n'
+            output_str += new_class_code
+            output_str += '\n\n##### ORIGINAL CLASS CODE #####\n\n'
+            output_str += original_class_code
+            # write original class and new class to file for comparison
+            with open(f'gpt_edit_review/{self.filename[:-3]}/{class_name}.py', "w") as f:
+                f.write(output_str)
+
+    def remove_not_found(self):
         self.class_names = [class_name for class_name in self.class_names if not class_name in self.not_found_code_names_list]
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/commands/code_edit.py` & `gpt-code-edit-1.0.5/chatgpt_cli/commands/code_edit.py`

 * *Ordering differences only*

 * *Files 11% similar despite different names*

```diff
@@ -1,106 +1,106 @@
-from tqdm import tqdm
-from ..arguement_validator import ArgumentValidator
-from ..code_parser import CodeParser
-from ..gpt_request import GptRequest
-
-def code_edit_parser(subparsers):
-    # set the command name to be used in termainal
-    parser = subparsers.add_parser('code-edit')
-    
-    # set the arguments
-    parser.add_argument('filename', type=str,
-                        help='The filename of the file containing the code to be used. eg. main.py')
-    parser.add_argument('--target-functions', type=str, nargs='*', default=[],
-                        help='A space-separated list of function names to be targeted.')
-    parser.add_argument('--target-classes', type=str, nargs='*', default=[],
-                        help='A space-separated list of class names to be targeted. Should be provied as ClassName, targets every method in each class provided. Cannot be used if --target-methods also used on a method within one of the given classes.')
-    parser.add_argument('--target-methods', type=str, nargs='*', default=[],
-                        help='A space-separated list of method names to be targeted. Each method should be given as ClassName.method. Cannot be used if --target-classes also used on the class the method is from.')
-    parser.add_argument('--refactor', action='store_true',
-                        help='If set, refactor the code.')
-    parser.add_argument('--comments', action='store_true',
-                        help='If set, add comments to the code.')
-    parser.add_argument('--docstrings', action='store_true',
-                        help='If set, add docstrings to the code.')
-    parser.add_argument('--error-handling', action='store_true',
-                        help='If set, add error handling to the code.')
-    parser.add_argument('--gpt-4', action='store_true',
-                        help='If set, GPT-4 will be used instead of the default GPT-3.')
-    parser.add_argument('--temp', type=float, default=0.4, help='Affects the randomness of the output. Higher more creative lower more structured. Must be between 1 and 0. Default 0.4.')
-    parser.add_argument('--create-review-file', action='store_true', help='If set, creates a file {function_name}.py in a folder gpt_edit_review containing the newly edited function code and the old function code. Allowing you to review before replacing the code in the actual file. Remember to gitignore or delete the folder created when done. Either this or edit-code-in-file must be set. Both can be set.')
-    parser.add_argument('--edit-code-in-file', action='store_true', help='If set, rewrites the selected function with the newly edited version returned from gpt. If used advisable for code to be commited and saved in case of erroneus changes. Either this or create-review-file must be set. Both can be set.')
-    return parser
-
-def code_edit_function (args):
-    
-    # create the class instances
-    argument_valiadator = ArgumentValidator(args)
-
-    code_parser = CodeParser(filename=args.filename, function_names=args.target_functions, class_names=args.target_classes, method_names=args.target_methods)
-
-    gpt_request = GptRequest(gpt_4=args.gpt_4)
-
-    try:
-        gpt_request.get_api_key()
-    except Exception as e:
-        print(e)
-        return
-    
-    # tasks for the terminal progress bar
-    total_tasks = 4 + args.create_review_file + args.edit_code_in_file
-
-    with tqdm(total=total_tasks) as progress_bar:
-    
-        try:
-            # check arguements fit the requirements
-            argument_valiadator.gpt_edit_validate()
-            progress_bar.set_description('Validated Arguments.')
-            progress_bar.update()
-        except Exception as e:
-            print(e)
-            return
-        
-        # find the code as str of the required functions, methods, classes
-        functions_code_list, not_found_list = code_parser.find_target_code_gpt_edit()
-        
-        # if some functions were not found
-        if len(not_found_list) > 0:
-            # if no functions were found print message and return
-            if len(functions_code_list) == 0:
-                function_names_str = (', ').join(args.target_functions)
-                class_names_str = (', ').join(args.target_classes)
-                method_names_str = (', ').join(args.target_methods)
-                print(f'Unable to find any of the given functions, methods or classes in {args.filename}.\nFunctions provided: {function_names_str}\nMethods provided: {method_names_str}\nClasses provided: {class_names_str}')
-                return
-            # some functions were found display functions not found to user ask if to continue
-            not_found_str = (', ').join(not_found_list)
-            user_continue = input(f'In {args.filename} unable to find: {not_found_str}.\n Do you wish to continue with the functions that were found successfully ? y/n  ')
-            if user_continue == 'y':
-                # if continue remove not found items in class attributes
-                code_parser.remove_not_found()
-            else:
-                # if not continue return
-                return
-        progress_bar.set_description('Retrieved target code as strings from file.')
-        progress_bar.update()
-        
-        # create prompts message strings to be send to gpt api
-        gpt_request.create_prompts(functions=functions_code_list, refactor=args.refactor, comments=args.comments, docstrings=args.docstrings, error_handling=args.error_handling)
-        progress_bar.set_description('Created prompts to be sent to GPT.')
-        progress_bar.update()
-        
-        # send the requests to the api return the newly edited functions as strings
-        new_functions = gpt_request.make_GPT_requests()
-        progress_bar.set_description('Retrieved responses from GPT.')
-        progress_bar.update()
-        if args.create_review_file:
-            # create a file to view the original function or class and the gpt edited one for comparison
-            code_parser.create_review_code_files(new_functions=new_functions)
-            progress_bar.set_description('Created review code files.')
-            progress_bar.update()
-        if args.edit_code_in_file:
-            # edit the code in the file replacing the class or function or method with the gpt edited one
-            code_parser.replace_target_functions_with_new_functions(new_functions=new_functions)
-            progress_bar.set_description('Edited code in file.')
-            progress_bar.update()
+from tqdm import tqdm
+from ..arguement_validator import ArgumentValidator
+from ..code_parser import CodeParser
+from ..gpt_request import GptRequest
+
+def code_edit_parser(subparsers):
+    # set the command name to be used in termainal
+    parser = subparsers.add_parser('code-edit')
+    
+    # set the arguments
+    parser.add_argument('filename', type=str,
+                        help='The filename of the file containing the code to be used. eg. main.py')
+    parser.add_argument('--target-functions', type=str, nargs='*', default=[],
+                        help='A space-separated list of function names to be targeted.')
+    parser.add_argument('--target-classes', type=str, nargs='*', default=[],
+                        help='A space-separated list of class names to be targeted. Should be provied as ClassName, targets every method in each class provided. Cannot be used if --target-methods also used on a method within one of the given classes.')
+    parser.add_argument('--target-methods', type=str, nargs='*', default=[],
+                        help='A space-separated list of method names to be targeted. Each method should be given as ClassName.method. Cannot be used if --target-classes also used on the class the method is from.')
+    parser.add_argument('--refactor', action='store_true',
+                        help='If set, refactor the code.')
+    parser.add_argument('--comments', action='store_true',
+                        help='If set, add comments to the code.')
+    parser.add_argument('--docstrings', action='store_true',
+                        help='If set, add docstrings to the code.')
+    parser.add_argument('--error-handling', action='store_true',
+                        help='If set, add error handling to the code.')
+    parser.add_argument('--gpt-4', action='store_true',
+                        help='If set, GPT-4 will be used instead of the default GPT-3.')
+    parser.add_argument('--temp', type=float, default=0.4, help='Affects the randomness of the output. Higher more creative lower more structured. Must be between 1 and 0. Default 0.4.')
+    parser.add_argument('--create-review-file', action='store_true', help='If set, creates a file {function_name}.py in a folder gpt_edit_review containing the newly edited function code and the old function code. Allowing you to review before replacing the code in the actual file. Remember to gitignore or delete the folder created when done. Either this or edit-code-in-file must be set. Both can be set.')
+    parser.add_argument('--edit-code-in-file', action='store_true', help='If set, rewrites the selected function with the newly edited version returned from gpt. If used advisable for code to be commited and saved in case of erroneus changes. Either this or create-review-file must be set. Both can be set.')
+    return parser
+
+def code_edit_function (args):
+    
+    # create the class instances
+    argument_valiadator = ArgumentValidator(args)
+
+    code_parser = CodeParser(filename=args.filename, function_names=args.target_functions, class_names=args.target_classes, method_names=args.target_methods)
+
+    gpt_request = GptRequest(gpt_4=args.gpt_4)
+
+    try:
+        gpt_request.get_api_key()
+    except Exception as e:
+        print(e)
+        return
+    
+    # tasks for the terminal progress bar
+    total_tasks = 4 + args.create_review_file + args.edit_code_in_file
+
+    with tqdm(total=total_tasks) as progress_bar:
+    
+        try:
+            # check arguements fit the requirements
+            argument_valiadator.gpt_edit_validate()
+            progress_bar.set_description('Validated Arguments.')
+            progress_bar.update()
+        except Exception as e:
+            print(e)
+            return
+        
+        # find the code as str of the required functions, methods, classes
+        functions_code_list, not_found_list = code_parser.find_target_code_gpt_edit()
+        
+        # if some functions were not found
+        if len(not_found_list) > 0:
+            # if no functions were found print message and return
+            if len(functions_code_list) == 0:
+                function_names_str = (', ').join(args.target_functions)
+                class_names_str = (', ').join(args.target_classes)
+                method_names_str = (', ').join(args.target_methods)
+                print(f'Unable to find any of the given functions, methods or classes in {args.filename}.\nFunctions provided: {function_names_str}\nMethods provided: {method_names_str}\nClasses provided: {class_names_str}')
+                return
+            # some functions were found display functions not found to user ask if to continue
+            not_found_str = (', ').join(not_found_list)
+            user_continue = input(f'In {args.filename} unable to find: {not_found_str}.\n Do you wish to continue with the functions that were found successfully ? y/n  ')
+            if user_continue == 'y':
+                # if continue remove not found items in class attributes
+                code_parser.remove_not_found()
+            else:
+                # if not continue return
+                return
+        progress_bar.set_description('Retrieved target code as strings from file.')
+        progress_bar.update()
+        
+        # create prompts message strings to be send to gpt api
+        gpt_request.create_prompts(functions=functions_code_list, refactor=args.refactor, comments=args.comments, docstrings=args.docstrings, error_handling=args.error_handling)
+        progress_bar.set_description('Created prompts to be sent to GPT.')
+        progress_bar.update()
+        
+        # send the requests to the api return the newly edited functions as strings
+        new_functions = gpt_request.make_GPT_requests()
+        progress_bar.set_description('Retrieved responses from GPT.')
+        progress_bar.update()
+        if args.create_review_file:
+            # create a file to view the original function or class and the gpt edited one for comparison
+            code_parser.create_review_code_files(new_functions=new_functions)
+            progress_bar.set_description('Created review code files.')
+            progress_bar.update()
+        if args.edit_code_in_file:
+            # edit the code in the file replacing the class or function or method with the gpt edited one
+            code_parser.replace_target_functions_with_new_functions(new_functions=new_functions)
+            progress_bar.set_description('Edited code in file.')
+            progress_bar.update()
     print('COMPLETED')
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/commands/review_to_file.py` & `gpt-code-edit-1.0.5/chatgpt_cli/commands/review_to_file.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,57 +1,57 @@
-from ..arguement_validator import ArgumentValidator
-from ..code_parser import CodeParser
-
-def review_to_file_parser(subparsers):
-    # set the command name to be used in termainal
-    parser = subparsers.add_parser('review-to-file')
-    
-    # set the arguments
-    parser.add_argument('filename', type=str,
-                        help='The filename of the file containing the original code. eg. main.py')
-    parser.add_argument('--target-functions', type=str, nargs='*', default=[],
-                        help='A space-separated list of function names to be targeted from the corresponding gpt_edit_review/filename folder.')
-    parser.add_argument('--target-classes', type=str, nargs='*', default=[],
-                        help='A space-separated list of function names to be targeted from the corresponding gpt_edit_review/filename folder. Should be provied as ClassName. Cannot be used if --target-methods also used on a method within one of the given classes.')
-    parser.add_argument('--target-methods', type=str, nargs='*', default=[],
-                        help='A space-separated list of method names to be targeted from the corresponding gpt_edit_review/filename folder. Each method should be given as ClassName.method. Cannot be used if --target-classes also used on the class the method is from.')
-    
-    return parser
-
-def review_to_file_function(args):
-     # create the class instances
-    argument_valiadator = ArgumentValidator(args)
-
-    code_parser = CodeParser(filename=args.filename, function_names=args.target_functions, class_names=args.target_classes, method_names=args.target_methods)
-
-    try:
-        # check arguements fit the requirements
-        argument_valiadator.review_to_file_validate()
-    except Exception as e:
-        print(e)
-        return
-    
-    # find the edited code inn th gpt_edit_review folder files
-    code_list, not_found_list = code_parser.find_target_code_in_gpt_edit_review_folder()
-
-    # if some functions were not found
-    if len(not_found_list) > 0:
-        # if no functions were found print message and return
-        if len(code_list) == 0:
-            function_names_str = (', ').join(args.target_functions)
-            class_names_str = (', ').join(args.target_classes)
-            method_names_str = (', ').join(args.target_methods)
-            print(f'Unable to find any of the given functions, methods or classes in gpt_edit_review/{args.filename[:-3]} folder.\nFunctions provided: {function_names_str}\nMethods provided: {method_names_str}\nClasses provided: {class_names_str}')
-            return
-        # some functions were found display functions not found to user ask if to continue
-        not_found_str = (', ').join(not_found_list)
-        user_continue = input(f'In gpt_edit_review/{args.filename[:-3]} folder unable to find: {not_found_str}.\n Do you wish to continue with the functions that were found successfully ? y/n  ')
-        if user_continue == 'y':
-            # if continue remove not found items in class attributes
-            code_parser.remove_not_found()
-        else:
-            # if not continue return
-            return
-        
-    # edit the code in the file replacing the class or function or method with the gpt edited one
-    code_parser.replace_target_functions_with_new_functions(new_functions=code_list)
+from ..arguement_validator import ArgumentValidator
+from ..code_parser import CodeParser
+
+def review_to_file_parser(subparsers):
+    # set the command name to be used in termainal
+    parser = subparsers.add_parser('review-to-file')
+    
+    # set the arguments
+    parser.add_argument('filename', type=str,
+                        help='The filename of the file containing the original code. eg. main.py')
+    parser.add_argument('--target-functions', type=str, nargs='*', default=[],
+                        help='A space-separated list of function names to be targeted from the corresponding gpt_edit_review/filename folder.')
+    parser.add_argument('--target-classes', type=str, nargs='*', default=[],
+                        help='A space-separated list of function names to be targeted from the corresponding gpt_edit_review/filename folder. Should be provied as ClassName. Cannot be used if --target-methods also used on a method within one of the given classes.')
+    parser.add_argument('--target-methods', type=str, nargs='*', default=[],
+                        help='A space-separated list of method names to be targeted from the corresponding gpt_edit_review/filename folder. Each method should be given as ClassName.method. Cannot be used if --target-classes also used on the class the method is from.')
+    
+    return parser
+
+def review_to_file_function(args):
+     # create the class instances
+    argument_valiadator = ArgumentValidator(args)
+
+    code_parser = CodeParser(filename=args.filename, function_names=args.target_functions, class_names=args.target_classes, method_names=args.target_methods)
+
+    try:
+        # check arguements fit the requirements
+        argument_valiadator.review_to_file_validate()
+    except Exception as e:
+        print(e)
+        return
+    
+    # find the edited code inn th gpt_edit_review folder files
+    code_list, not_found_list = code_parser.find_target_code_in_gpt_edit_review_folder()
+
+    # if some functions were not found
+    if len(not_found_list) > 0:
+        # if no functions were found print message and return
+        if len(code_list) == 0:
+            function_names_str = (', ').join(args.target_functions)
+            class_names_str = (', ').join(args.target_classes)
+            method_names_str = (', ').join(args.target_methods)
+            print(f'Unable to find any of the given functions, methods or classes in gpt_edit_review/{args.filename[:-3]} folder.\nFunctions provided: {function_names_str}\nMethods provided: {method_names_str}\nClasses provided: {class_names_str}')
+            return
+        # some functions were found display functions not found to user ask if to continue
+        not_found_str = (', ').join(not_found_list)
+        user_continue = input(f'In gpt_edit_review/{args.filename[:-3]} folder unable to find: {not_found_str}.\n Do you wish to continue with the functions that were found successfully ? y/n  ')
+        if user_continue == 'y':
+            # if continue remove not found items in class attributes
+            code_parser.remove_not_found()
+        else:
+            # if not continue return
+            return
+        
+    # edit the code in the file replacing the class or function or method with the gpt edited one
+    code_parser.replace_target_functions_with_new_functions(new_functions=code_list)
     print('COMPLETED')
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/commands/set_api_key.py` & `gpt-code-edit-1.0.5/chatgpt_cli/commands/set_api_key.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,31 +1,31 @@
-from os import path, makedirs
-
-def set_api_key_parser(subparsers):
-    # set the command name to be used in termainal
-    parser = subparsers.add_parser('set-api-key')
-
-    # set the arguments
-    parser.add_argument('api_key', type=str, help='The open ai api key for the user. Key can be found here https://platform.openai.com/account/api-keys if you have a valid openai account.')
-
-    return parser
-
-def set_api_key_function(args):
-    """
-    Prompts the user for their OpenAI API key and saves it to a configuration file in the user's home directory.
-    """
-
-    # api key supplied by the user
-    api_key = args.api_key
-    
-    # Define the directory and file path for the configuration file
-    config_dir = path.expanduser('~/.gpt_code_edit/')
-    config_file = path.join(config_dir, 'config.txt')
-    
-    # Create the configuration directory if it doesn't exist
-    makedirs(config_dir, exist_ok=True)
-    
-    # write the API key to the configuration file
-    with open(config_file, 'w') as f:
-        f.write(api_key)
-
+from os import path, makedirs
+
+def set_api_key_parser(subparsers):
+    # set the command name to be used in termainal
+    parser = subparsers.add_parser('set-api-key')
+
+    # set the arguments
+    parser.add_argument('api_key', type=str, help='The open ai api key for the user. Key can be found here https://platform.openai.com/account/api-keys if you have a valid openai account.')
+
+    return parser
+
+def set_api_key_function(args):
+    """
+    Prompts the user for their OpenAI API key and saves it to a configuration file in the user's home directory.
+    """
+
+    # api key supplied by the user
+    api_key = args.api_key
+    
+    # Define the directory and file path for the configuration file
+    config_dir = path.expanduser('~/.gpt_code_edit/')
+    config_file = path.join(config_dir, 'config.txt')
+    
+    # Create the configuration directory if it doesn't exist
+    makedirs(config_dir, exist_ok=True)
+    
+    # write the API key to the configuration file
+    with open(config_file, 'w') as f:
+        f.write(api_key)
+
     print('API key saved.')
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/gpt_request.py` & `gpt-code-edit-1.0.5/chatgpt_cli/gpt_request.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,158 +1,158 @@
-import asyncio
-import aiohttp
-import json
-from os import path
-from markdown_it import MarkdownIt
-
-class GptRequest:
-    def __init__(self, gpt_4: bool = False, temp: float = 0.4):
-        """
-    Parameters:
-    - gpt_4 (bool): Whether to use GPT-4 API or not. Default is False.
-    - temp (float): The temperature parameter for generating responses. Default is 0.4.
-    """
-        self.gpt_4 = gpt_4
-        self.temp = temp
-        self.prompts = []
-        self.GPT_API_KEY = ""
-        self.edited_functions = []
-
-    def get_api_key(self):
-        """
-        Retrieve the OpenAI API key from a configuration file in the user's home directory.
-    
-        Raises:
-            Exception: If the configuration file is not found.
-        """
-    
-        # Define the directory and file path for the configuration file
-        config_dir = path.expanduser('~/.gpt_code_edit/')
-        config_file = path.join(config_dir, 'config.txt')
-    
-        try:
-            # Attempt to open and read the API key from the configuration file
-            with open(config_file, 'r') as f:
-                # set the api_key to the one found in the file
-                self.GPT_API_KEY = f.read().strip()
-        except FileNotFoundError:
-            # If the file is not found, raise an exception instructing the user to set the API key
-            raise Exception('API key not found. Please set your API key using set-api-key command.')
-
-    def create_prompts(self, functions: list, refactor: bool = False, comments: bool = False, docstrings: bool = False, error_handling: bool = False):
-        """
-    Creates the prompts to be sent to GPT API.
-    
-    Args:
-        functions (list): A list of Python functions.
-        refactor (bool, optional): Whether to refactor the code for better readability and performance. Defaults to False.
-        comments (bool, optional): Whether to add comments to explain the function code. Defaults to False.
-        docstrings (bool, optional): Whether to add a docstring to the function. Defaults to False.
-        error_handling (bool, optional): Whether to improve the error handling. Defaults to False.
-    """
-        for function in functions:
-            prompt = f"Here is a Python function and I want you to do the following to it:"
-        
-            if refactor:
-                prompt += "\n • Refactor the code for better readability and performance."
-            if comments:
-                prompt += "\n • Add comments to explain the function code."
-            if docstrings:
-                prompt += "\n • Add a docstring to the function."
-            if error_handling:
-                prompt += "\n • Improve the error handling."
-    
-            prompt += f"\n\nPlease make sure to return only the newly edited function code in your response, without any additional text or explanation outside of the function code. The code should be enclosed in triple backticks like this:\n\n\\```python\n<your code here>\n\\```\nThe original function is:\n\n{function}"
-
-            self.prompts.append(prompt)
-
-    def make_GPT_requests(self):
-        """
-    Makes GPT requests asynchronously using asyncio.
-    
-    Returns:
-        edited_functions (list): A list of edited functions.
-    """
-        loop = asyncio.get_event_loop()
-        loop.run_until_complete(self.async_GPT_requests())
-        return self.edited_functions
-
-    async def async_GPT_requests(self):
-        """
-    Sends asynchronous requests to GPT and extracts code from the responses.
-    """
-        tasks = []
-        sem = asyncio.Semaphore(5)  # Adjust to preferred concurrent request limit
-
-        async with aiohttp.ClientSession() as session:
-            # make requests to api asynchronously
-            for prompt in self.prompts:
-                tasks.append(self.send_request(session, prompt))
-            responses = await asyncio.gather(*tasks)
-
-        for response in responses:
-            # get the code as a string from the api response
-            response_object = json.loads(response)
-            message_content = response_object["choices"][0]["message"]["content"]
-            self.extract_code_from_response(message_content)
-
-    async def send_request(self, session, prompt):
-        """
-    Sends a request to the OpenAI API to generate a completion based on the given prompt.
-
-    Args:
-        session: An async session object for making HTTP requests.
-        prompt: The prompt containing the function to edit and how it is to be edited.
-
-    Returns:
-        The generated completion as a string.
-    """
-        # Determine the model to use based on the value of self.gpt_4
-        if self.gpt_4:
-            model = 'gpt-4'
-        else:
-            model = 'gpt-3.5-turbo-16k'
-    
-        # Create the prompt message with system and user roles
-        prompt_message = [
-            {"role": "system", "content": "You are a helpful assistant."},
-            {"role": "user", "content": prompt}
-        ]
-    
-        # URL for the API endpoint
-        url = "https://api.openai.com/v1/chat/completions"
-    
-        # headers for the HTTP request
-        headers = {
-            'Content-Type': 'application/json',
-            'Authorization': f'Bearer {self.GPT_API_KEY}'
-        }
-    
-        # data payload for the HTTP request
-        data = {
-            'model': model,
-            'messages': prompt_message,
-            'temperature': self.temp
-        }
-    
-        # Send the HTTP request to the API endpoint and retrieve the response
-        async with session.post(url, headers=headers, data=json.dumps(data)) as resp:
-            return await resp.text()
-
-    def extract_code_from_response(self, response: str):
-        """
-    Extracts Python code blocks from a Markdown response.
-
-    Args:
-        response (str): The Markdown response.
-
-    Returns:
-        str: The extracted Python code block.
-    """
-        md = MarkdownIt()  # Create an instance of the MarkdownIt class
-
-        tokens = md.parse(response)  # Parse the Markdown response into tokens
-
-        # Extract code blocks that are written in Python
-        code_blocks = [t.content for t in tokens if t.type == 'fence' and t.info == 'python']
-
-        self.edited_functions.append(code_blocks[0])  # Append the first code block to the edited_functions list
+import asyncio
+import aiohttp
+import json
+from os import path
+from markdown_it import MarkdownIt
+
+class GptRequest:
+    def __init__(self, gpt_4: bool = False, temp: float = 0.4):
+        """
+    Parameters:
+    - gpt_4 (bool): Whether to use GPT-4 API or not. Default is False.
+    - temp (float): The temperature parameter for generating responses. Default is 0.4.
+    """
+        self.gpt_4 = gpt_4
+        self.temp = temp
+        self.prompts = []
+        self.GPT_API_KEY = ""
+        self.edited_functions = []
+
+    def get_api_key(self):
+        """
+        Retrieve the OpenAI API key from a configuration file in the user's home directory.
+    
+        Raises:
+            Exception: If the configuration file is not found.
+        """
+    
+        # Define the directory and file path for the configuration file
+        config_dir = path.expanduser('~/.gpt_code_edit/')
+        config_file = path.join(config_dir, 'config.txt')
+    
+        try:
+            # Attempt to open and read the API key from the configuration file
+            with open(config_file, 'r') as f:
+                # set the api_key to the one found in the file
+                self.GPT_API_KEY = f.read().strip()
+        except FileNotFoundError:
+            # If the file is not found, raise an exception instructing the user to set the API key
+            raise Exception('API key not found. Please set your API key using set-api-key command.')
+
+    def create_prompts(self, functions: list, refactor: bool = False, comments: bool = False, docstrings: bool = False, error_handling: bool = False):
+        """
+    Creates the prompts to be sent to GPT API.
+    
+    Args:
+        functions (list): A list of Python functions.
+        refactor (bool, optional): Whether to refactor the code for better readability and performance. Defaults to False.
+        comments (bool, optional): Whether to add comments to explain the function code. Defaults to False.
+        docstrings (bool, optional): Whether to add a docstring to the function. Defaults to False.
+        error_handling (bool, optional): Whether to improve the error handling. Defaults to False.
+    """
+        for function in functions:
+            prompt = f"Here is a Python function and I want you to do the following to it:"
+        
+            if refactor:
+                prompt += "\n • Refactor the code for better readability and performance."
+            if comments:
+                prompt += "\n • Add comments to explain the function code."
+            if docstrings:
+                prompt += "\n • Add a docstring to the function."
+            if error_handling:
+                prompt += "\n • Improve the error handling."
+    
+            prompt += f"\n\nPlease make sure to return only the newly edited function code in your response, without any additional text or explanation outside of the function code. The code should be enclosed in triple backticks like this:\n\n\\```python\n<your code here>\n\\```\nThe original function is:\n\n{function}"
+
+            self.prompts.append(prompt)
+
+    def make_GPT_requests(self):
+        """
+    Makes GPT requests asynchronously using asyncio.
+    
+    Returns:
+        edited_functions (list): A list of edited functions.
+    """
+        loop = asyncio.get_event_loop()
+        loop.run_until_complete(self.async_GPT_requests())
+        return self.edited_functions
+
+    async def async_GPT_requests(self):
+        """
+    Sends asynchronous requests to GPT and extracts code from the responses.
+    """
+        tasks = []
+        sem = asyncio.Semaphore(5)  # Adjust to preferred concurrent request limit
+
+        async with aiohttp.ClientSession() as session:
+            # make requests to api asynchronously
+            for prompt in self.prompts:
+                tasks.append(self.send_request(session, prompt))
+            responses = await asyncio.gather(*tasks)
+
+        for response in responses:
+            # get the code as a string from the api response
+            response_object = json.loads(response)
+            message_content = response_object["choices"][0]["message"]["content"]
+            self.extract_code_from_response(message_content)
+
+    async def send_request(self, session, prompt):
+        """
+    Sends a request to the OpenAI API to generate a completion based on the given prompt.
+
+    Args:
+        session: An async session object for making HTTP requests.
+        prompt: The prompt containing the function to edit and how it is to be edited.
+
+    Returns:
+        The generated completion as a string.
+    """
+        # Determine the model to use based on the value of self.gpt_4
+        if self.gpt_4:
+            model = 'gpt-4'
+        else:
+            model = 'gpt-3.5-turbo-16k'
+    
+        # Create the prompt message with system and user roles
+        prompt_message = [
+            {"role": "system", "content": "You are a helpful assistant."},
+            {"role": "user", "content": prompt}
+        ]
+    
+        # URL for the API endpoint
+        url = "https://api.openai.com/v1/chat/completions"
+    
+        # headers for the HTTP request
+        headers = {
+            'Content-Type': 'application/json',
+            'Authorization': f'Bearer {self.GPT_API_KEY}'
+        }
+    
+        # data payload for the HTTP request
+        data = {
+            'model': model,
+            'messages': prompt_message,
+            'temperature': self.temp
+        }
+    
+        # Send the HTTP request to the API endpoint and retrieve the response
+        async with session.post(url, headers=headers, data=json.dumps(data)) as resp:
+            return await resp.text()
+
+    def extract_code_from_response(self, response: str):
+        """
+    Extracts Python code blocks from a Markdown response.
+
+    Args:
+        response (str): The Markdown response.
+
+    Returns:
+        str: The extracted Python code block.
+    """
+        md = MarkdownIt()  # Create an instance of the MarkdownIt class
+
+        tokens = md.parse(response)  # Parse the Markdown response into tokens
+
+        # Extract code blocks that are written in Python
+        code_blocks = [t.content for t in tokens if t.type == 'fence' and t.info == 'python']
+
+        self.edited_functions.append(code_blocks[0])  # Append the first code block to the edited_functions list
```

### Comparing `gpt-code-edit-1.0.4/chatgpt_cli/main.py` & `gpt-code-edit-1.0.5/chatgpt_cli/main.py`

 * *Ordering differences only*

 * *Files 21% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-from argparse import ArgumentParser
-from .commands.code_edit import code_edit_parser, code_edit_function
-from .commands.review_to_file import review_to_file_parser, review_to_file_function
-from .commands.set_api_key import set_api_key_parser, set_api_key_function
-
-
-def main():
-    parser = ArgumentParser(
-        description='Command line to interact with ChatGPT API to refactor code, add comments and docstrings, or add error handling.')
-    # create subparser for multiple commands
-    subparsers = parser.add_subparsers()
-    # set arguments and function for code-edit command
-    code_edit_parser(subparsers).set_defaults(func=code_edit_function)
-    # set arguments and function for review-to-file command
-    review_to_file_parser(subparsers).set_defaults(func=review_to_file_function)
-    # set arguments and function for config command
-    set_api_key_parser(subparsers).set_defaults(func=set_api_key_function)
-    # parse the arguments
-    args = parser.parse_args()
-
-    args.func(args)
-
-if __name__ == '__main__':
+from argparse import ArgumentParser
+from .commands.code_edit import code_edit_parser, code_edit_function
+from .commands.review_to_file import review_to_file_parser, review_to_file_function
+from .commands.set_api_key import set_api_key_parser, set_api_key_function
+
+
+def main():
+    parser = ArgumentParser(
+        description='Command line to interact with ChatGPT API to refactor code, add comments and docstrings, or add error handling.')
+    # create subparser for multiple commands
+    subparsers = parser.add_subparsers()
+    # set arguments and function for code-edit command
+    code_edit_parser(subparsers).set_defaults(func=code_edit_function)
+    # set arguments and function for review-to-file command
+    review_to_file_parser(subparsers).set_defaults(func=review_to_file_function)
+    # set arguments and function for config command
+    set_api_key_parser(subparsers).set_defaults(func=set_api_key_function)
+    # parse the arguments
+    args = parser.parse_args()
+
+    args.func(args)
+
+if __name__ == '__main__':
     main()
```

### Comparing `gpt-code-edit-1.0.4/gpt_code_edit.egg-info/PKG-INFO` & `gpt-code-edit-1.0.5/gpt_code_edit.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,105 +1,117 @@
-Metadata-Version: 2.1
-Name: gpt-code-edit
-Version: 1.0.4
-Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
-Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
-Author: Ben Speakman
-Author-email: benspeakman23@yahoo.com
-License: UNKNOWN
-Description: # GPT Code Edit
-        
-        gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
-        
-        ## Github
-        
-        https://github.com/ben-23-96/chatgpt_code_improve_cli
-        
-        ## PyPI
-        
-        https://pypi.org/project/gpt-code-edit/
-        
-        ## Prerequisites
-        
-        - Python 3.9
-        - An active OpenAI account with API keys
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
-        
-        ```bash
-        pip install gpt-code-edit
-        ```
-        
-        ## Usage
-        
-        ### Set API Key
-        
-        First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
-        
-        ```bash
-        gpt set-api-key <api_key>
-        ```
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<api_key>` | The OpenAI API key for the user. |
-        
-        ### Code Edit
-        
-        This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
-        
-        ```bash
-        gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
-        ```
-        
-        **Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
-        
-        **Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<filename>` | The filename of the file containing the code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted. |
-        | `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        | `--refactor` | If set, refactor the code. |
-        | `--comments` | If set, add comments to the code. |
-        | `--docstrings` | If set, add docstrings to the code. |
-        | `--error-handling` | If set, add error handling to the code. |
-        | `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
-        | `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
-        | `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
-        | `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
-        
-        ### Review to File
-        
-        If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
-        
-        ```bash
-        gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
-        ```
-        
-        #### Arguments
-        
-        | Argument | Description |
-        | :--- | :--- |
-        | `<filename>` | The filename of the file containing the original code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
-        | `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        
-        
-Platform: UNKNOWN
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Description-Content-Type: text/markdown
+Metadata-Version: 2.1
+Name: gpt-code-edit
+Version: 1.0.5
+Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
+Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
+Author: Ben Speakman
+Author-email: benspeakman23@yahoo.com
+License: UNKNOWN
+Platform: UNKNOWN
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+
+# GPT Code Edit
+
+gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
+
+## Github
+
+https://github.com/ben-23-96/chatgpt_code_improve_cli
+
+## PyPI
+
+https://pypi.org/project/gpt-code-edit/
+
+## Prerequisites
+
+- Python 3.9
+- An active OpenAI account with API keys
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install GPT code edit.
+
+```bash
+pip install gpt-code-edit
+```
+
+# Usage
+
+## Set API Key
+
+First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
+
+```bash
+gpt set-api-key <api_key>
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<api_key>` | The OpenAI API key for the user. |
+
+## Code Edit
+
+This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
+
+```bash
+gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
+```
+
+**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
+
+**Note**: One of `--refactor`, `--comments`, `--docstrings` or `--error-handling` must be set. Multiple can be set at the same time.
+
+**Note**: One of `--target-functions`, `--target-methods` or `--target-classes` must be set. Multiple can be set at the same time.
+
+### Example
+
+The following command would add GPT generated comments into the function foo located in the main.py file.
+
+```bash
+gpt code-edit main.py --target-functions foo --comments --edit-code-in-file
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted. |
+| `--target-classes` | A space-separated list of class names to be targeted. Each class should be provided as `ClassName`. This will target every method in each class provided. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+| `--refactor` | If set, refactor the code. |
+| `--comments` | If set, add comments to the code. |
+| `--docstrings` | If set, add docstrings to the code. |
+| `--error-handling` | If set, add error handling to the code. |
+| `--gpt-4` | If set, GPT-4 will be used instead of the default GPT-3. |
+| `--temp` | Affects the randomness of the output. A higher value makes the output more creative and a lower value makes it more structured. Must be between 1 and 0. The default is 0.4. |
+| `--create-review-file` | If set, creates a file `{function_name}.py` in a folder `gpt_edit_review` containing the newly edited function code and the old function code. This allows you to review the code before replacing it in the actual file. Remember to gitignore or delete the folder created when done. |
+| `--edit-code-in-file` | If set, rewrites the selected code within the file with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+
+## Review to File
+
+If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
+
+```bash
+gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
+```
+
+### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the original code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
+| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+
+
+
```

### Comparing `gpt-code-edit-1.0.4/gpt_code_edit.egg-info/SOURCES.txt` & `gpt-code-edit-1.0.5/gpt_code_edit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

