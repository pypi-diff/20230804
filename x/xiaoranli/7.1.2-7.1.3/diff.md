# Comparing `tmp/xiaoranli-7.1.2-py3-none-any.whl.zip` & `tmp/xiaoranli-7.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,22 +1,22 @@
-Zip file size: 13570 bytes, number of entries: 20
+Zip file size: 13640 bytes, number of entries: 20
 -rw-r--r--  2.0 unx     3808 b- defN 23-Jun-13 09:02 xiaoranli/__init__.py
--rw-r--r--  2.0 unx     1854 b- defN 23-Jun-13 09:06 xiaoranli/data/rc_files/alias
+-rw-r--r--  2.0 unx     1899 b- defN 23-Aug-04 03:09 xiaoranli/data/rc_files/alias
 -rw-r--r--  2.0 unx       75 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/dockerignore
 -rw-r--r--  2.0 unx      393 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/gdbinit
 -rw-r--r--  2.0 unx      124 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/gitconfig
 -rw-r--r--  2.0 unx      561 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/inputrc
 -rw-r--r--  2.0 unx      903 b- defN 23-Jun-12 07:32 xiaoranli/data/rc_files/tmux.config
 -rw-r--r--  2.0 unx      452 b- defN 23-Jun-12 07:33 xiaoranli/data/rc_files/vimrc
 -rw-r--r--  2.0 unx      188 b- defN 23-Jun-12 07:32 xiaoranli/scripts/install_golang.sh
--rw-r--r--  2.0 unx     1874 b- defN 23-Jun-13 08:27 xiaoranli/scripts/install_useful_tools.sh
+-rw-r--r--  2.0 unx     1983 b- defN 23-Aug-03 05:49 xiaoranli/scripts/install_useful_tools.sh
 -rw-r--r--  2.0 unx      451 b- defN 23-Jun-13 08:02 xiaoranli/scripts/install_zsh.sh
 -rw-r--r--  2.0 unx      480 b- defN 23-Jun-12 07:32 xiaoranli/zhijiang/scripts/enhance_python.sh
 -rw-r--r--  2.0 unx     1150 b- defN 23-Jun-12 07:32 xiaoranli/zhijiang/scripts/install_useful_tools.sh
 -rw-r--r--  2.0 unx     7953 b- defN 23-Jun-13 05:36 xiaoranli/zhijiang/scripts/useful_func.py
--rw-r--r--  2.0 unx     1081 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      923 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       45 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       10 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1772 b- defN 23-Jun-13 09:07 xiaoranli-7.1.2.dist-info/RECORD
-20 files, 24189 bytes uncompressed, 10622 bytes compressed:  56.1%
+-rw-r--r--  2.0 unx     1081 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      923 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       45 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       10 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1772 b- defN 23-Aug-04 05:47 xiaoranli-7.1.3.dist-info/RECORD
+20 files, 24343 bytes uncompressed, 10692 bytes compressed:  56.1%
```

## zipnote {}

```diff
@@ -36,26 +36,26 @@
 
 Filename: xiaoranli/zhijiang/scripts/install_useful_tools.sh
 Comment: 
 
 Filename: xiaoranli/zhijiang/scripts/useful_func.py
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/LICENSE.txt
+Filename: xiaoranli-7.1.3.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/METADATA
+Filename: xiaoranli-7.1.3.dist-info/METADATA
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/WHEEL
+Filename: xiaoranli-7.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/entry_points.txt
+Filename: xiaoranli-7.1.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/top_level.txt
+Filename: xiaoranli-7.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xiaoranli-7.1.2.dist-info/RECORD
+Filename: xiaoranli-7.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xiaoranli/data/rc_files/alias

```diff
@@ -5,14 +5,16 @@
 alias top='top c'
 alias sudo="sudo env \"PATH=$PATH\""
 alias j='autojump'
 alias gdb='gdb -q'
 alias df='duf'
 alias pre-commit='pre-commit run --all-files'
 alias py-spy="sudo py-spy dump --nonblocking --full-filenames"
+alias llp='sudo netstat -tulpn|grep LISTEN'
+
 
 plugins=(z extract git zsh-syntax-highlighting zsh-autosuggestions)
 
 eval "$(mcfly init zsh)"
 
 # fzf config
 # Default command to use when input is tty
```

## xiaoranli/scripts/install_useful_tools.sh

```diff
@@ -22,15 +22,15 @@
     echo "Current version is less than $requiredver, exa wouldn't be installed"
 fi
 
 sudo apt install peco mlocate bat python3-pip tig fzf fd-find ripgrep duf zip unzip httpie
 # wget -O /tmp/bat.deb https://github.com/sharkdp/bat/releases/download/v0.21.0/bat-musl_0.21.0_amd64.deb && sudo dpkg -i /tmp/bat.deb
 
 
-sudo pip install  py-spy python3.8-dbg viztracer glances pre-commit
+sudo pip install  py-spy python3.8-dbg viztracer glances pre-commit nvitop
 
 sudo pip install cmake==3.21.4
 
 curl -LSfs https://raw.githubusercontent.com/cantino/mcfly/master/ci/install.sh | sudo sh -s -- --git cantino/mcfly
 echo "eval "$(mcfly init zsh)"" >> ~/.zshrc
 # tab complete of git
 # curl https://raw.githubusercontent.com/git/git/master/contrib/completion/git-completion.bash -o ~/.git-completion.bash
@@ -42,7 +42,11 @@
 wget https://raw.githubusercontent.com/satanson/cpp_etudes/master/calltree.pl
 wget https://raw.githubusercontent.com/satanson/cpp_etudes/master/cpptree.pl
 chmod 777 calltree.pl cpptree.pl
 sudo mv calltree.pl /usr/local/bin/calltree
 sudo mv cpptree.pl /usr/local/bin/cpptree
 )
 sudo pip install gdbgui
+
+git clone https://github.com/gpakosz/.tmux.git
+ln -s -f .tmux/.tmux.conf
+cp .tmux/.tmux.conf.local .
```

## Comparing `xiaoranli-7.1.2.dist-info/LICENSE.txt` & `xiaoranli-7.1.3.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `xiaoranli-7.1.2.dist-info/METADATA` & `xiaoranli-7.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xiaoranli
-Version: 7.1.2
+Version: 7.1.3
 Summary: setup linux env, such as bashrc etc.
 Home-page: https://github.com/xiaoranliMS/env-setup.git
 Author: Li Xiaoran
 Author-email: 1240897116@qq.com
 Project-URL: Funding,  https://github.com/xiaoranliMS
 Project-URL: Source, https://github.com/xiaoranliMS/env-setup.git
 Keywords: env setup,development,xiaoranli
```

## Comparing `xiaoranli-7.1.2.dist-info/RECORD` & `xiaoranli-7.1.3.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 xiaoranli/__init__.py,sha256=h1E19jN92KaWNDe55BGV6PZHC7Bl2Wxn1NW8qfroYEs,3808
-xiaoranli/data/rc_files/alias,sha256=14B42RVy8JjFnp-EnIwDU6Iix0eJRTbxRJAC92uhZIw,1854
+xiaoranli/data/rc_files/alias,sha256=ng-Jl31xSyANbQSM78s9gp5xfizww-vIj2YJxLQpdj0,1899
 xiaoranli/data/rc_files/dockerignore,sha256=fNTcMXrdUU9h9Y0tkLpfQKbLhwRwaVNd-MyP-ycI3sE,75
 xiaoranli/data/rc_files/gdbinit,sha256=Om1pIhhf-_lIfLgx8Gt730W2R4vvZLr05hbgnhNy0Hs,393
 xiaoranli/data/rc_files/gitconfig,sha256=sSooqGwfXpEHUvL047wvYQOMl1zQUgN8GVWWMhRLYII,124
 xiaoranli/data/rc_files/inputrc,sha256=yl22z2lj2jWLaE85I9QpV9NjoYoOhpmPemNxEsxMC5Y,561
 xiaoranli/data/rc_files/tmux.config,sha256=kk88x2Skt6csucriayhCNORaufCV8FsLMycVzEkrwHA,903
 xiaoranli/data/rc_files/vimrc,sha256=z4s0auYUgfiGZ5lZPLpcGhJqVoU8sz2SMxMxxSqyuV8,452
 xiaoranli/scripts/install_golang.sh,sha256=sR2H-HL-Bj6dj9bTD0apJsRLlEQaLoD0Ay5S3qUycxc,188
-xiaoranli/scripts/install_useful_tools.sh,sha256=3hq21Dqrvm6dEVsmXpW5SgA_dviJbX4jZwN8dzKEyuY,1874
+xiaoranli/scripts/install_useful_tools.sh,sha256=XyCAyqe1MEfwdnf_i2-ZM492NDf0OhnRFxA1PVg0oxE,1983
 xiaoranli/scripts/install_zsh.sh,sha256=zdgMuJi8a0-5RapD01oSXoQvErMsCDktz9uMCdAUTWo,451
 xiaoranli/zhijiang/scripts/enhance_python.sh,sha256=l9YzkTTMLRzUV_nkCi8PS029QqIx8__bKmD3HCkEycE,480
 xiaoranli/zhijiang/scripts/install_useful_tools.sh,sha256=7C287YLb57j0hxKWLWeM2KIZcI6cM1L4DDHGIlju9UE,1150
 xiaoranli/zhijiang/scripts/useful_func.py,sha256=jgQgWXUkBYSNqC88yOymtlW2MLkL9MYHDnFpiJLKNqk,7953
-xiaoranli-7.1.2.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
-xiaoranli-7.1.2.dist-info/METADATA,sha256=AsJUG3Qkxqm09IWt4DFYc0B4lB2xrO6aYU-rL9kxcR0,923
-xiaoranli-7.1.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-xiaoranli-7.1.2.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
-xiaoranli-7.1.2.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
-xiaoranli-7.1.2.dist-info/RECORD,,
+xiaoranli-7.1.3.dist-info/LICENSE.txt,sha256=ceC9ZJOV9H6CtQDcYmHOS46NA3dHJ_WD4J9blH513pc,1081
+xiaoranli-7.1.3.dist-info/METADATA,sha256=FFIlu-ESRH11IInIAFNInhpnSTIf3zsM8TfZZPLxRp8,923
+xiaoranli-7.1.3.dist-info/WHEEL,sha256=2wepM1nk4DS4eFpYrW1TTqPcoGNfHhhO_i5m4cOimbo,92
+xiaoranli-7.1.3.dist-info/entry_points.txt,sha256=T3ZBwdXMY38i4JvMaIXq1WIMdrDEDrVkaWIgKfVsrTc,45
+xiaoranli-7.1.3.dist-info/top_level.txt,sha256=DjwPuFyAkwL8uNM0Z41wNraAt9-71lDJ8SRwYTqRRcs,10
+xiaoranli-7.1.3.dist-info/RECORD,,
```

