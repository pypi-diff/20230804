# Comparing `tmp/nice65-0.0.3.tar.gz` & `tmp/nice65-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nice65-0.0.3.tar", last modified: Wed Aug  2 11:44:13 2023, max compression
+gzip compressed data, was "nice65-0.0.4.tar", last modified: Fri Aug  4 21:05:06 2023, max compression
```

## Comparing `nice65-0.0.3.tar` & `nice65-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-02 11:44:13.446679 nice65-0.0.3/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 14:08:20.000000 nice65-0.0.3/LICENSE
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3381 2023-08-02 11:44:13.446679 nice65-0.0.3/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)     2961 2023-08-02 11:41:57.000000 nice65-0.0.3/README.md
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-02 11:44:13.446679 nice65-0.0.3/nice65/
--rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-02 11:34:50.000000 nice65-0.0.3/nice65/__init__.py
--rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-02 11:34:54.000000 nice65-0.0.3/nice65/__main__.py
--rwxr-xr-x   0 anderson  (1000) anderson  (1000)     7243 2023-08-02 11:44:01.000000 nice65-0.0.3/nice65/app.py
-drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-02 11:44:13.446679 nice65-0.0.3/nice65.egg-info/
--rw-r--r--   0 anderson  (1000) anderson  (1000)     3381 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/PKG-INFO
--rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/SOURCES.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/dependency_links.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/entry_points.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/requires.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-02 11:44:13.000000 nice65-0.0.3/nice65.egg-info/top_level.txt
--rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-02 11:44:04.000000 nice65-0.0.3/pyproject.toml
--rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-02 11:44:13.446679 nice65-0.0.3/setup.cfg
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     1069 2023-07-30 17:49:06.000000 nice65-0.0.4/LICENSE
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:05:06.461229 nice65-0.0.4/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3210 2023-08-04 21:04:40.000000 nice65-0.0.4/README.md
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/nice65/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       22 2023-08-03 11:55:31.000000 nice65-0.0.4/nice65/__init__.py
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       27 2023-08-03 11:55:31.000000 nice65-0.0.4/nice65/__main__.py
+-rwxr-xr-x   0 anderson  (1000) anderson  (1000)     7822 2023-08-04 20:52:14.000000 nice65-0.0.4/nice65/app.py
+drwxr-xr-x   0 anderson  (1000) anderson  (1000)        0 2023-08-04 21:05:06.461229 nice65-0.0.4/nice65.egg-info/
+-rw-r--r--   0 anderson  (1000) anderson  (1000)     3630 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/PKG-INFO
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      266 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/SOURCES.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        1 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/dependency_links.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       39 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/entry_points.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       12 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/requires.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)        7 2023-08-04 21:05:06.000000 nice65-0.0.4/nice65.egg-info/top_level.txt
+-rw-r--r--   0 anderson  (1000) anderson  (1000)      759 2023-08-04 20:46:54.000000 nice65-0.0.4/pyproject.toml
+-rw-r--r--   0 anderson  (1000) anderson  (1000)       38 2023-08-04 21:05:06.461229 nice65-0.0.4/setup.cfg
```

### Comparing `nice65-0.0.3/LICENSE` & `nice65-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nice65-0.0.3/PKG-INFO` & `nice65-0.0.4/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,37 +1,25 @@
-Metadata-Version: 2.1
-Name: nice65
-Version: 0.0.3
-Summary: Code formatter for CC65 assembly
-Author-email: Andrew Dunai <a@dun.ai>
-Project-URL: Homepage, https://github.com/and3rson/nice65
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # nice65
 Code formatter for CC65 assembly (WIP).
 
 Requirements:
 
 - Python 3.x
 - [Lark](https://github.com/lark-parser/lark)
 
 Features:
 - Makes ugly code less ugly
 - Fixes indentation and letter cases (mnemonics, registers)
 - Understands weird labels, such as colon-less (C64 style) and unnamed (`:`, `:+++`)
+- Support for basic macros
 - Skip files with `; nice65: ignore` comment
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
-- Macros (basic ones might work though).
+- Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
 # Installation
 
 ```sh
 pip install nice65
@@ -56,73 +44,94 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
+.macro foobar aa, bb, cc
+lda aa
+ldx bb
+ldy cc
+.endmacro
+
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-lDa  #0
+start lDa  #0
 LdX #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne fill  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
-cmp A
-lda ($1234), X
+cmp foo+2
+jmp :+
+: lda $1234
 
 @ridiculously_long_label_just_for_the_sake_of_it:PLX
 pla
 
-rts
+end:rts
 ```
 
 After:
 ```asm
-        .data
+.macro  foobar aa, bb, cc
+        LDA aa
+        LDX bb
+        LDY cc
+.endmacro
+
+.data
 foo:    .byte 1
 
-        .code
+.code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-        LDA #0
+start:  LDA #0
         LDX #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE fill        ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
-        CMP A
-        LDA ($1234), X
+        CMP foo+2
+        JMP :+
+    :   LDA $1234
 
     @ridiculously_long_label_just_for_the_sake_of_it:
         PLX
         PLA
 
-        RTS
+end:    RTS
+```
+
+
+## Using with Vim
+
+```vim
+:nnoremap <M-r> :%! nice65 -<CR>
 ```
 
 ## Using with NeoVim
 
-Here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls
+If you want to be fancy, here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls:
 
 1. Make sure you have the following neovim plugins installed:
     - `maxbane/vim-asm_ca65` - sets filetype for CA65 buffers
     - `jose-elias-alvarez/null-ls.nvim` - allows to run custom scripts as language servers
 
 2. Add configuration:
```

### Comparing `nice65-0.0.3/README.md` & `nice65-0.0.4/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,24 +1,38 @@
+Metadata-Version: 2.1
+Name: nice65
+Version: 0.0.4
+Summary: Code formatter for CC65 assembly
+Author-email: Andrew Dunai <a@dun.ai>
+Project-URL: Homepage, https://github.com/and3rson/nice65
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # nice65
 Code formatter for CC65 assembly (WIP).
 
 Requirements:
 
 - Python 3.x
 - [Lark](https://github.com/lark-parser/lark)
 
 Features:
 - Makes ugly code less ugly
 - Fixes indentation and letter cases (mnemonics, registers)
 - Understands weird labels, such as colon-less (C64 style) and unnamed (`:`, `:+++`)
+- Support for basic macros
 - Skip files with `; nice65: ignore` comment
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
-- Macros (basic ones might work though).
+- Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
 # Installation
 
 ```sh
 pip install nice65
@@ -43,73 +57,94 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
+.macro foobar aa, bb, cc
+lda aa
+ldx bb
+ldy cc
+.endmacro
+
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-lDa  #0
+start lDa  #0
 LdX #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne fill  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
-cmp A
-lda ($1234), X
+cmp foo+2
+jmp :+
+: lda $1234
 
 @ridiculously_long_label_just_for_the_sake_of_it:PLX
 pla
 
-rts
+end:rts
 ```
 
 After:
 ```asm
-        .data
+.macro  foobar aa, bb, cc
+        LDA aa
+        LDX bb
+        LDY cc
+.endmacro
+
+.data
 foo:    .byte 1
 
-        .code
+.code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-        LDA #0
+start:  LDA #0
         LDX #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE fill        ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
-        CMP A
-        LDA ($1234), X
+        CMP foo+2
+        JMP :+
+    :   LDA $1234
 
     @ridiculously_long_label_just_for_the_sake_of_it:
         PLX
         PLA
 
-        RTS
+end:    RTS
+```
+
+
+## Using with Vim
+
+```vim
+:nnoremap <M-r> :%! nice65 -<CR>
 ```
 
 ## Using with NeoVim
 
-Here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls
+If you want to be fancy, here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls:
 
 1. Make sure you have the following neovim plugins installed:
     - `maxbane/vim-asm_ca65` - sets filetype for CA65 buffers
     - `jose-elias-alvarez/null-ls.nvim` - allows to run custom scripts as language servers
 
 2. Add configuration:
```

### Comparing `nice65-0.0.3/nice65/app.py` & `nice65-0.0.4/nice65/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,14 +31,16 @@
     'bra', 'phx', 'phy', 'plx', 'ply',
     'rmb0', 'rmb1', 'rmb2', 'rmb3', 'rmb4', 'rmb5', 'rmb6', 'rmb7',
     'smb0', 'smb1', 'smb2', 'smb3', 'smb4', 'smb5', 'smb6', 'smb7',
     'stp', 'stz', 'trb', 'tsb', 'wai',
     # fmt: on
 ]
 
+COL1_COMMANDS = {'segment', 'zeropage', 'data', 'code', 'bss'}
+
 instructions = INSTRUCTIONS + CMOS_INSTRUCTIONS
 
 instructions_def = " | ".join(['"' + instr + '"i' for instr in instructions])
 
 
 definition = (
     # fmt: off
@@ -51,16 +53,18 @@
     %ignore _WS
 
     start: line*
     line: (labeldef statement | statement | labeldef)? comment? "\n"
 
     labeldef: LABEL ":"? | ":"
 
-    statement: asm_statement | control_command | constant_def
+    statement: asm_statement | macro_start | macro_end | control_command | constant_def
     asm_statement: INSTR (_WS+ operand ("," operand)?)?
+    macro_start: ".macro" WORD (_WS+ WORD ("," WORD)*)?
+    macro_end: ".endmacro"
     control_command: "." WORD (_WS+ /[^\n]+/)?
     constant_def: LABEL "=" /[^\n]+/
 
     comment: ";" SENTENCE?
 
     ?operand: REGISTER | (/#/? /[<>]/? expr)
     ?expr: LITERAL (OP expr)?
@@ -78,17 +82,15 @@
 )
 
 grammar = Lark(definition)
 
 
 def main():
     parser = ArgumentParser(formatter_class=ArgumentDefaultsHelpFormatter)
-    parser.add_argument(
-        "infile", help='Input file, pass "-" to read from for stdin'
-    )
+    parser.add_argument("infile", help='Input file, pass "-" to read from for stdin')
     group = parser.add_mutually_exclusive_group()
     group.add_argument(
         "-o",
         "--outfile",
         metavar="outfile",
         help='Output file, defaults to "-" for stdout',
         default="-",
@@ -126,22 +128,18 @@
 
 def fix(infile, outfile, modify_in_place):
     if infile == "-":
         content = sys.stdin.read()
     else:
         with open(infile, "r") as fobj:
             content = fobj.read()
-            options_match = re.findall(
-                r'^[ \t]*;\s*nice65:([^\n]+)$', content, re.MULTILINE
-            )
+            options_match = re.findall(r'^[ \t]*;\s*nice65:([^\n]+)$', content, re.MULTILINE)
             if options_match:
                 options_str = options_match[0].lower().replace(',', ' ')
-                options = set(
-                    filter(None, map(str.strip, options_str.split(' ')))
-                )
+                options = set(filter(None, map(str.strip, options_str.split(' '))))
                 if 'ignore' in options:
                     print("Ignoring", infile)
                     return
 
     tree = grammar.parse(content)
 
     if modify_in_place:
@@ -151,17 +149,15 @@
     else:
         outfile = open(outfile, "w")
 
     for line in tree.children:
         string = ""
         for i, child in enumerate(line.children):
             if child.data == "comment":
-                sentence = (
-                    child.children[0] if child.children else ""
-                ).strip()
+                sentence = (child.children[0] if child.children else "").strip()
                 s_len = len(string)
                 if '\n' in string:
                     s_len = s_len - string.rfind('\n') - 1
                 padding = (24 - s_len) if i > 0 else 0
                 string += " " * padding + ("; " + sentence).strip()
             elif child.data == "labeldef":
                 if child.children:
@@ -182,32 +178,41 @@
                     padding = " " * pad_count
                 else:
                     padding = "\n" + " " * 8
 
                 statement = child.children[0]
 
                 if statement.data == "control_command":
-                    string += padding + "." + " ".join(statement.children)
+                    name = statement.children[0].strip()
+                    string += (
+                        (padding if name not in COL1_COMMANDS else '')
+                        + "."
+                        + name.lower()
+                        + " "
+                        + " ".join(statement.children[1:])
+                    )
+                elif statement.data == "macro_start":
+                    name = statement.children[0].strip()
+                    string += ".macro ".ljust(8, ' ') + name + " " + ", ".join(map(str.strip, statement.children[1:]))
+                elif statement.data == "macro_end":
+                    string += ".endmacro"
                 elif statement.data == "asm_statement":
                     mnemonic = statement.children[0]
                     string += padding + mnemonic.upper()
                     operands = statement.children[1:]
                     if operands:
                         args = []
                         for operand in operands:
                             args.append(flatten_expr(operand))
                         string += " " + ", ".join(args)
                 elif statement.data == "constant_def":
-                    string += padding + \
-                        " = ".join(map(str.strip, statement.children))
+                    string += padding + " = ".join(map(str.strip, statement.children))
                 else:
-                    raise NotImplementedError(
-                        "Unknown statement type: " + child.children[0].data
-                    )
-        print(string, file=outfile)
+                    raise NotImplementedError("Unknown statement type: " + child.children[0].data)
+        print(string.rstrip(), file=outfile)
 
     outfile.close()
 
 
 def flatten_expr(operand):
     parts = []
     if isinstance(operand, Token):
```

### Comparing `nice65-0.0.3/nice65.egg-info/PKG-INFO` & `nice65-0.0.4/nice65.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nice65
-Version: 0.0.3
+Version: 0.0.4
 Summary: Code formatter for CC65 assembly
 Author-email: Andrew Dunai <a@dun.ai>
 Project-URL: Homepage, https://github.com/and3rson/nice65
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
@@ -19,19 +19,20 @@
 - Python 3.x
 - [Lark](https://github.com/lark-parser/lark)
 
 Features:
 - Makes ugly code less ugly
 - Fixes indentation and letter cases (mnemonics, registers)
 - Understands weird labels, such as colon-less (C64 style) and unnamed (`:`, `:+++`)
+- Support for basic macros
 - Skip files with `; nice65: ignore` comment
 - Tested with [C64 Kernal/Basic](https://github.com/mist64/c64rom) and [my 6502-based SBC ROM code](https://github.com/and3rson/deck65)
 
 Not implemented yet:
-- Macros (basic ones might work though).
+- Complex macros
 - Proper formatting of arithmetic expressions
 - Better indentation of comments based on deduced context
 
 # Installation
 
 ```sh
 pip install nice65
@@ -56,73 +57,94 @@
 
 # Recursively reformat all files in directory with extension ".asm"
 nice65 ./samples/ -r -p '*.asm'
 ```
 
 Before:
 ```asm
+.macro foobar aa, bb, cc
+lda aa
+ldx bb
+ldy cc
+.endmacro
+
 .data
 foo:.byte 1
 
 .code
          ;        Fill zeropage with zeroes
 fill:
 PHa
 Phx
 
-lDa  #0
+start lDa  #0
 LdX #0
 @again: sta     $00   ,x  ;Yeah, we can use stz, but I just need some code to test nice65!
    inx
 bne fill  ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
 lda #<($42  +  %10101010- (foo*2))
-cmp A
-lda ($1234), X
+cmp foo+2
+jmp :+
+: lda $1234
 
 @ridiculously_long_label_just_for_the_sake_of_it:PLX
 pla
 
-rts
+end:rts
 ```
 
 After:
 ```asm
-        .data
+.macro  foobar aa, bb, cc
+        LDA aa
+        LDX bb
+        LDY cc
+.endmacro
+
+.data
 foo:    .byte 1
 
-        .code
+.code
 ; Fill zeropage with zeroes
 fill:
         PHA
         PHX
 
-        LDA #0
+start:  LDA #0
         LDX #0
     @again:
         STA $00, X      ; Yeah, we can use stz, but I just need some code to test nice65!
         INX
         BNE fill        ; Repeat
 
 ; Do unnecessary throwaway stuff to test expressions
         LDA #<($42+%10101010-(foo*2))
-        CMP A
-        LDA ($1234), X
+        CMP foo+2
+        JMP :+
+    :   LDA $1234
 
     @ridiculously_long_label_just_for_the_sake_of_it:
         PLX
         PLA
 
-        RTS
+end:    RTS
+```
+
+
+## Using with Vim
+
+```vim
+:nnoremap <M-r> :%! nice65 -<CR>
 ```
 
 ## Using with NeoVim
 
-Here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls
+If you want to be fancy, here's an example on how to have nice65 configured as code formatter for NeoVim with null-ls:
 
 1. Make sure you have the following neovim plugins installed:
     - `maxbane/vim-asm_ca65` - sets filetype for CA65 buffers
     - `jose-elias-alvarez/null-ls.nvim` - allows to run custom scripts as language servers
 
 2. Add configuration:
```

### Comparing `nice65-0.0.3/pyproject.toml` & `nice65-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "nice65"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Andrew Dunai", email="a@dun.ai" },
 ]
 description = "Code formatter for CC65 assembly"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

