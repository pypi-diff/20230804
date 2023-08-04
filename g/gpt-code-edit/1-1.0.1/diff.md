# Comparing `tmp/gpt-code-edit-1.tar.gz` & `tmp/gpt-code-edit-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt-code-edit-1.tar", last modified: Fri Aug  4 13:19:27 2023, max compression
+gzip compressed data, was "gpt-code-edit-1.0.1.tar", last modified: Fri Aug  4 14:05:12 2023, max compression
```

## Comparing `gpt-code-edit-1.tar` & `gpt-code-edit-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-08-04 13:19:27.382829 gpt-code-edit-1/
--rw-rw-rw-   0        0        0     5997 2023-08-04 13:19:27.381833 gpt-code-edit-1/PKG-INFO
--rw-rw-rw-   0        0        0     4519 2023-08-04 13:17:41.000000 gpt-code-edit-1/README.md
-drwxrwxrwx   0        0        0        0 2023-08-04 13:19:27.293803 gpt-code-edit-1/chatgpt_cli/
--rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1/chatgpt_cli/__init__.py
--rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1/chatgpt_cli/arguement_validator.py
--rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1/chatgpt_cli/code_parser.py
--rw-rw-rw-   0        0        0     6465 2023-08-03 10:26:51.000000 gpt-code-edit-1/chatgpt_cli/gpt_request.py
--rw-rw-rw-   0        0        0     1094 2023-08-04 10:51:39.000000 gpt-code-edit-1/chatgpt_cli/main.py
-drwxrwxrwx   0        0        0        0 2023-08-04 13:19:27.376830 gpt-code-edit-1/gpt_code_edit.egg-info/
--rw-rw-rw-   0        0        0     5997 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      375 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       66 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-08-04 13:19:26.000000 gpt-code-edit-1/gpt_code_edit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-08-04 13:19:27.383830 gpt-code-edit-1/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-08-04 13:18:22.000000 gpt-code-edit-1/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.122372 gpt-code-edit-1.0.1/
+-rw-rw-rw-   0        0        0     5342 2023-08-04 14:05:12.120373 gpt-code-edit-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0     4526 2023-08-04 13:57:08.000000 gpt-code-edit-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.067371 gpt-code-edit-1.0.1/chatgpt_cli/
+-rw-rw-rw-   0        0        0        0 2023-08-04 09:45:39.000000 gpt-code-edit-1.0.1/chatgpt_cli/__init__.py
+-rw-rw-rw-   0        0        0     7541 2023-08-04 09:31:34.000000 gpt-code-edit-1.0.1/chatgpt_cli/arguement_validator.py
+-rw-rw-rw-   0        0        0    11011 2023-07-19 16:18:28.000000 gpt-code-edit-1.0.1/chatgpt_cli/code_parser.py
+-rw-rw-rw-   0        0        0     6467 2023-08-04 13:43:04.000000 gpt-code-edit-1.0.1/chatgpt_cli/gpt_request.py
+-rw-rw-rw-   0        0        0     1061 2023-08-04 13:58:33.000000 gpt-code-edit-1.0.1/chatgpt_cli/main.py
+drwxrwxrwx   0        0        0        0 2023-08-04 14:05:12.118370 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/
+-rw-rw-rw-   0        0        0     5342 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      375 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       46 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       66 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-04 14:05:11.000000 gpt-code-edit-1.0.1/gpt_code_edit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-08-04 14:05:12.123371 gpt-code-edit-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1313 2023-08-04 14:04:56.000000 gpt-code-edit-1.0.1/setup.py
```

### Comparing `gpt-code-edit-1/PKG-INFO` & `gpt-code-edit-1.0.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1
+Version: 1.0.1
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
-License: UNKNOWN
-Description: # My CLI
-        
-        gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
-        
-        ## Prerequisites
-        
-        - Python 3.9
-        - An active OpenAI account with API keys
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
-        
-        ```bash
-        pip install chatgpt-cli
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
-        | `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
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
-        | `<filename>` | The filename of the file containing the code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
-        | `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# GPT Code Edit
+
+gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
+
+## Prerequisites
+
+- Python 3.9
+- An active OpenAI account with API keys
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
+
+```bash
+pip install chatgpt-cli
+```
+
+## Usage
+
+### Set API Key
+
+First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
+
+```bash
+gpt set-api-key <api_key>
+```
+
+#### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<api_key>` | The OpenAI API key for the user. |
+
+### Code Edit
+
+This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
+
+```bash
+gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
+```
+
+**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
+
+#### Arguments
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
+| `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+
+### Review to File
+
+If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
+
+```bash
+gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
+```
+
+#### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
+| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+
```

### Comparing `gpt-code-edit-1/README.md` & `gpt-code-edit-1.0.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# My CLI
+# GPT Code Edit
 
 gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
 
 ## Prerequisites
 
 - Python 3.9
 - An active OpenAI account with API keys
```

### Comparing `gpt-code-edit-1/chatgpt_cli/arguement_validator.py` & `gpt-code-edit-1.0.1/chatgpt_cli/arguement_validator.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1/chatgpt_cli/code_parser.py` & `gpt-code-edit-1.0.1/chatgpt_cli/code_parser.py`

 * *Files identical despite different names*

### Comparing `gpt-code-edit-1/chatgpt_cli/gpt_request.py` & `gpt-code-edit-1.0.1/chatgpt_cli/gpt_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         Retrieve the OpenAI API key from a configuration file in the user's home directory.
     
         Raises:
             Exception: If the configuration file is not found.
         """
     
         # Define the directory and file path for the configuration file
-        config_dir = path.expanduser('~/.chatgpt_cli/')
+        config_dir = path.expanduser('~/.gpt_code_edit/')
         config_file = path.join(config_dir, 'config.txt')
     
         try:
             # Attempt to open and read the API key from the configuration file
             with open(config_file, 'r') as f:
                 # set the api_key to the one found in the file
                 self.GPT_API_KEY = f.read().strip()
```

### Comparing `gpt-code-edit-1/chatgpt_cli/main.py` & `gpt-code-edit-1.0.1/chatgpt_cli/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from argparse import ArgumentParser
-from chatgpt_cli.commands.code_edit import code_edit_parser, code_edit_function
-from chatgpt_cli.commands.review_to_file import review_to_file_parser, review_to_file_function
-from chatgpt_cli.commands.set_api_key import set_api_key_parser, set_api_key_function
+from .commands.code_edit import code_edit_parser, code_edit_function
+from .commands.review_to_file import review_to_file_parser, review_to_file_function
+from .commands.set_api_key import set_api_key_parser, set_api_key_function
 
 
 def main():
     parser = ArgumentParser(
         description='Command line to interact with ChatGPT API to refactor code, add comments and docstrings, or add error handling.')
     # create subparser for multiple commands
     subparsers = parser.add_subparsers()
```

### Comparing `gpt-code-edit-1/gpt_code_edit.egg-info/PKG-INFO` & `gpt-code-edit-1.0.1/gpt_code_edit.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,95 +1,93 @@
 Metadata-Version: 2.1
 Name: gpt-code-edit
-Version: 1
+Version: 1.0.1
 Summary: A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.
 Home-page: https://github.com/ben-23-96/chatgpt_code_improve_cli
 Author: Ben Speakman
 Author-email: benspeakman23@yahoo.com
-License: UNKNOWN
-Description: # My CLI
-        
-        gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
-        
-        ## Prerequisites
-        
-        - Python 3.9
-        - An active OpenAI account with API keys
-        
-        ## Installation
-        
-        Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
-        
-        ```bash
-        pip install chatgpt-cli
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
-        | `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
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
-        | `<filename>` | The filename of the file containing the code (eg. main.py). |
-        | `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
-        | `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
-        | `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
-        
-        
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+
+# GPT Code Edit
+
+gpt-code-edit is a Command Line Interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits on them including refactoring, adding comments, adding docstrings, or adding error handling. 
+
+## Prerequisites
+
+- Python 3.9
+- An active OpenAI account with API keys
+
+## Installation
+
+Use the package manager [pip](https://pip.pypa.io/en/stable/) to install My CLI.
+
+```bash
+pip install chatgpt-cli
+```
+
+## Usage
+
+### Set API Key
+
+First, you need to set your OpenAI API key. You can find your key at [OpenAI Platform](https://platform.openai.com/account/api-keys) if you have a valid OpenAI account.
+
+```bash
+gpt set-api-key <api_key>
+```
+
+#### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<api_key>` | The OpenAI API key for the user. |
+
+### Code Edit
+
+This command allows you to target specific functions, classes, or methods in a file and perform several edits on the code including refactoring, adding comments, adding docstrings, or adding error handling.
+
+```bash
+gpt code-edit <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...] [--refactor] [--comments] [--docstrings] [--error-handling] [--gpt-4] [--temp <temperature>] [--create-review-file] [--edit-code-in-file]
+```
+
+**Note**: One of `--create-review-file` or `--edit-code-in-file` must be set. Both can be set at the same time.
+
+#### Arguments
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
+| `--edit-code-in-file` | If set, rewrites the selected function with the newly edited version returned from GPT. If used, it is advisable for code to be committed and saved in case of erroneous changes. |
+
+### Review to File
+
+If when using code-edit the --create-review-file flag has been used so the edited code has been placed in a file for review, this command allows you to apply the changes to the actual file.
+
+```bash
+gpt review-to-file <filename> [--target-functions <function1> <function2> ...] [--target-classes <class1> <class2> ...] [--target-methods <class1.method1> <class2.method2> ...]
+```
+
+#### Arguments
+
+| Argument | Description |
+| :--- | :--- |
+| `<filename>` | The filename of the file containing the code (eg. main.py). |
+| `--target-functions` | A space-separated list of function names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. |
+| `--target-classes` | A space-separated list of class names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each class should be provided as `ClassName`. This cannot be used if `--target-methods` is also used on a method within one of the given classes. |
+| `--target-methods` | A space-separated list of method names to be targeted from the corresponding `gpt_edit_review/<filename>` folder. Each method should be given as `ClassName.method`. This cannot be used if `--target-classes` is also used on the class the method is from. |
+
```

### Comparing `gpt-code-edit-1/setup.py` & `gpt-code-edit-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="gpt-code-edit",
-    version="1",
+    version="1.0.1",
     packages=find_packages(),
 
     # Metadata
     author="Ben Speakman",
     author_email="benspeakman23@yahoo.com",
     description="A command line interface that allows you to target specific functions, classes, or methods in a file and use chatgpt to perform several edits including refactoring, adding comments, adding docstrings, or adding error handling.",
     long_description=open('README.md').read(),
```

