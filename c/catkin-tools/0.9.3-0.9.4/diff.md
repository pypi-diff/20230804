# Comparing `tmp/catkin_tools-0.9.3.tar.gz` & `tmp/catkin_tools-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catkin_tools-0.9.3.tar", last modified: Thu Jun 29 09:31:41 2023, max compression
+gzip compressed data, was "catkin_tools-0.9.4.tar", last modified: Thu Aug  3 23:08:10 2023, max compression
```

## Comparing `catkin_tools-0.9.3.tar` & `catkin_tools-0.9.4.tar`

### file list

```diff
@@ -1,413 +1,414 @@
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/.github/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1782 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/.github/ISSUE_TEMPLATE.md
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/.github/workflows/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1998 2023-02-23 16:54:15.000000 catkin_tools-0.9.3/.github/workflows/workflow.yml
--rw-rw-r--   0 timon     (1000) timon     (1000)      349 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/.gitignore
--rw-rw-r--   0 timon     (1000) timon     (1000)    26060 2023-02-23 16:59:56.000000 catkin_tools-0.9.3/CHANGELOG.rst
--rw-r--r--   0 timon     (1000) timon     (1000)    11335 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/LICENSE
--rw-rw-r--   0 timon     (1000) timon     (1000)       31 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/MANIFEST.in
--rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/PKG-INFO
--rw-rw-r--   0 timon     (1000) timon     (1000)      316 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/README.md
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    16585 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/argument_parsing.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/commands/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/commands/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10098 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/commands/catkin.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    21324 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/common.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     5025 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/config.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    37403 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/context.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/execution/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    31661 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/execution/controllers.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/events.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    15425 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/execution/executor.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10053 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/io.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    12798 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/job_server.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1820 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/jobs.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     6599 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/execution/stages.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools/jobs/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    27764 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/jobs/catkin.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/jobs/cmake/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1918 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake/python.cmake
--rw-rw-r--   0 timon     (1000) timon     (1000)      194 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake/python_install_dir.cmake
--rw-rw-r--   0 timon     (1000) timon     (1000)    16276 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/jobs/cmake.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/jobs/commands/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     9936 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/cmake.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/commands/make.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     8774 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/jobs/utils.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    17302 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/metadata.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/
--rw-r--r--   0 timon     (1000) timon     (1000)      649 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/notifications/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2302 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/impl.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/
--rw-r--r--   0 timon     (1000) timon     (1000)    56725 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon.png
--rw-rw-r--   0 timon     (1000) timon     (1000)    31033 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_red.png
--rw-rw-r--   0 timon     (1000) timon     (1000)    31532 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_yellow.png
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/
--rw-r--r--   0 timon     (1000) timon     (1000)     1610 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Info.plist
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/
--rwxr-xr-x   0 timon     (1000) timon     (1000)    20880 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/catkin build
--rw-r--r--   0 timon     (1000) timon     (1000)        8 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/PkgInfo
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/
--rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/AppIcon.icns
--rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/catkin_blue_logo_only.icns
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/
--rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/Credits.rtf
--rw-r--r--   0 timon     (1000) timon     (1000)       92 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/InfoPlist.strings
--rw-r--r--   0 timon     (1000) timon     (1000)    26323 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/MainMenu.nib
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/
--rw-r--r--   0 timon     (1000) timon     (1000)       74 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/.gitignore
--rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/AppIcon.icns
--rw-rw-r--   0 timon     (1000) timon     (1000)     8026 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/README.markdown
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/
--rw-r--r--   0 timon     (1000) timon     (1000)      122 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.h
--rw-r--r--   0 timon     (1000) timon     (1000)     3113 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.m
--rw-r--r--   0 timon     (1000) timon     (1000)     1178 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Info.plist
--rw-r--r--   0 timon     (1000) timon     (1000)      165 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Prefix.pch
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/
--rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/Credits.rtf
--rw-r--r--   0 timon     (1000) timon     (1000)       45 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/InfoPlist.strings
--rw-r--r--   0 timon     (1000) timon     (1000)    45931 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/MainMenu.xib
--rw-r--r--   0 timon     (1000) timon     (1000)      119 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/main.m
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/
--rw-r--r--   0 timon     (1000) timon     (1000)    13799 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.pbxproj
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/
--rw-r--r--   0 timon     (1000) timon     (1000)      162 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/contents.xcworkspacedata
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/
--rw-r--r--   0 timon     (1000) timon     (1000)     1593 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/Terminal Notifier.xccheckout
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/
--rw-r--r--   0 timon     (1000) timon     (1000)     5102 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/Terminal Notifier.xcscheme
--rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/catkin_blue_logo_only.icns
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.466693 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/
--rw-r--r--   0 timon     (1000) timon     (1000)     1174 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/Contents.json
--rw-r--r--   0 timon     (1000) timon     (1000)     9426 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only128x128.png
--rw-r--r--   0 timon     (1000) timon     (1000)     3212 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only16x16.png
--rw-r--r--   0 timon     (1000) timon     (1000)    16330 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only256x256.png
--rw-r--r--   0 timon     (1000) timon     (1000)     3961 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only32x32.png
--rw-r--r--   0 timon     (1000) timon     (1000)    35515 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only512x512.png
--rw-rw-r--   0 timon     (1000) timon     (1000)     6716 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/resultspace.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/spaces/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      767 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/build.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      826 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/devel.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      755 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/install.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      748 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/log.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      762 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/spaces/source.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     5462 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/terminal_color.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1524 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/utils.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/catkin_tools/verbs/__init__.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/
--rw-r--r--   0 timon     (1000) timon     (1000)      960 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    30330 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/build.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    18708 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/color.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/
--rw-r--r--   0 timon     (1000) timon     (1000)      863 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7474 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/clean.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    17214 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/
--rw-r--r--   0 timon     (1000) timon     (1000)      975 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10902 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/
--rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     6751 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/
--rw-rw-r--   0 timon     (1000) timon     (1000)      965 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     3921 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/
--rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1956 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/
--rw-rw-r--   0 timon     (1000) timon     (1000)      885 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7864 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/
--rw-r--r--   0 timon     (1000) timon     (1000)      871 2022-04-19 21:21:18.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7099 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/cli.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/
--rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    10205 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2975 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_shell_verbs.bash
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/
--rw-rw-r--   0 timon     (1000) timon     (1000)      901 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     7892 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/cli.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     9462 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/test.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/catkin_tools.egg-info/
--rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/PKG-INFO
--rw-rw-r--   0 timon     (1000) timon     (1000)    15182 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)        1 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      985 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/entry_points.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       56 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/requires.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       13 2023-06-29 09:31:41.000000 catkin_tools-0.9.3/catkin_tools.egg-info/top_level.txt
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.470693 catkin_tools-0.9.3/completion/
--rw-rw-r--   0 timon     (1000) timon     (1000)    23450 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/completion/_catkin
--rw-rw-r--   0 timon     (1000) timon     (1000)     5109 2023-02-23 16:54:15.000000 catkin_tools-0.9.3/completion/catkin.bash
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/
--rw-r--r--   0 timon     (1000) timon     (1000)        7 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/.gitignore
--rw-r--r--   0 timon     (1000) timon     (1000)     6786 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/Makefile
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/_static/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/_static/.gitignore
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/_templates/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/_templates/.gitignore
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/advanced/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1001 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/catkin_shell_verbs.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)    41154 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_events.dia
--rw-rw-r--   0 timon     (1000) timon     (1000)    86468 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_events.svg
--rw-rw-r--   0 timon     (1000) timon     (1000)    45234 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_job_lifecycle.svg
--rw-rw-r--   0 timon     (1000) timon     (1000)    78602 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/executor_job_resources.svg
--rw-rw-r--   0 timon     (1000) timon     (1000)     9187 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/job_executor.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     1387 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/linked_develspace.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     3892 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/advanced/verb_customization.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     4580 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/build_types.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)    36590 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/catkin_build.dia
--rw-rw-r--   0 timon     (1000) timon     (1000)   180757 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/catkin_tools_execution.dia
--rw-rw-r--   0 timon     (1000) timon     (1000)     4795 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/cheat_sheet.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     8838 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/conf.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/development/
--rw-rw-r--   0 timon     (1000) timon     (1000)     2867 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/development/adding_build_types.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     5950 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/development/extending_the_catkin_command.rst
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1120 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/README.md
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/
--rwxrwxr-x   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/0_init.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      128 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/1_build_warning.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/2_build_err.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/all.bash
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/docs/examples/failure_ws/src/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/
--rw-rw-r--   0 timon     (1000) timon     (1000)     5270 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/
--rw-rw-r--   0 timon     (1000) timon     (1000)      150 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/CMakeLists.txt
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/
--rw-rw-r--   0 timon     (1000) timon     (1000)     5321 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     1929 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/
--rw-rw-r--   0 timon     (1000) timon     (1000)     5189 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       60 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/main.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)     1923 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/
--rw-rw-r--   0 timon     (1000) timon     (1000)     5199 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/grep-errors.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/main.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.474693 catkin_tools-0.9.3/docs/examples/quickstart_ws/
--rwxrwxr-x   0 timon     (1000) timon     (1000)      914 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/0_quickstart.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      108 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/1_prebuild.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      254 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/1_prebuild.out
--rwxrwxr-x   0 timon     (1000) timon     (1000)      109 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/2_postbuild.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)     1278 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/2_postbuild.out
--rwxrwxr-x   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/quickstart_ws/all.bash
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/
--rw-rw-r--   0 timon     (1000) timon     (1000)      571 2023-06-29 09:20:07.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/0_checkout.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)       99 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/1_init.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      107 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/2_dry_run.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      236 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/3_build.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/4_build_v.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      125 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/5_build_i.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/6_build_partial.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      231 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/7_build_this.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/8_build_start_with.bash
--rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/9_build_no_deps.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/all.bash
--rwxrwxr-x   0 timon     (1000) timon     (1000)      395 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/slowrecord
--rwxrwxr-x   0 timon     (1000) timon     (1000)     1812 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/examples/slowrun
--rw-rw-r--   0 timon     (1000) timon     (1000)    21600 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/executor_job_lifecycle.dia
--rw-rw-r--   0 timon     (1000) timon     (1000)   118107 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/executor_job_lifecycle.svg
--rw-rw-r--   0 timon     (1000) timon     (1000)     6066 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/history.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     4405 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/index.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/installing.rst
--rw-r--r--   0 timon     (1000) timon     (1000)     6713 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/docs/make.bat
--rw-rw-r--   0 timon     (1000) timon     (1000)    20283 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/mechanics.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)    19362 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/migration.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     7960 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/quick_start.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)      479 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/spelling_wordlist.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     2722 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/troubleshooting.rst
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/verbs/
--rw-rw-r--   0 timon     (1000) timon     (1000)    14082 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_build.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     4144 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_clean.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     8995 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_config.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)      403 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_create.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)      500 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_env.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)      998 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_init.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     1338 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_list.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)      398 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_locate.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     6824 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_profile.rst
--rw-rw-r--   0 timon     (1000) timon     (1000)     1931 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/catkin_test.rst
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/docs/verbs/cli/
--rw-rw-r--   0 timon     (1000) timon     (1000)     6864 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_build.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     2920 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_clean.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     8287 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_config.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      631 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_create.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     2669 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_create_pkg.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      822 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_env.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      469 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_init.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     1965 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_list.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     2323 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_locate.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      739 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_add.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      286 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_list.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      186 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_remove.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_rename.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      165 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_set.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     3091 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/catkin_test.txt
--rwxrwxr-x   0 timon     (1000) timon     (1000)      665 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/docs/verbs/cli/dump_cli
--rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/requirements.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       38 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/setup.cfg
--rw-rw-r--   0 timon     (1000) timon     (1000)     5365 2023-02-23 17:00:06.000000 catkin_tools-0.9.3/setup.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      257 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/stdeb.cfg
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1250 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/README.md
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.3/tests/__init__.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/__init__.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/
--rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      425 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/build_type_condition/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/
--rw-rw-r--   0 timon     (1000) timon     (1000)      301 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_args/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/
--rw-rw-r--   0 timon     (1000) timon     (1000)      167 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_err/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/
--rw-rw-r--   0 timon     (1000) timon     (1000)      161 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      311 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/cmake_warning/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/
--rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      404 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/depend_condition/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.478693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/
--rw-rw-r--   0 timon     (1000) timon     (1000)      134 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       37 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/fail.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      299 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_err/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/
--rw-rw-r--   0 timon     (1000) timon     (1000)      135 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)       40 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/make_warning/warn.cpp
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/
--rw-rw-r--   0 timon     (1000) timon     (1000)      636 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/CMakeLists.txt
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/
--rw-rw-r--   0 timon     (1000) timon     (1000)       30 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.develspace.in
--rw-rw-r--   0 timon     (1000) timon     (1000)       32 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.installspace.in
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/
--rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/fun.h
--rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/lib.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/main.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      302 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/
--rw-rw-r--   0 timon     (1000) timon     (1000)      790 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/CMakeLists.txt
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/
--rw-rw-r--   0 timon     (1000) timon     (1000)       36 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.develspace.in
--rw-rw-r--   0 timon     (1000) timon     (1000)       38 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.installspace.in
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/
--rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/fun.h
--rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/lib.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/main.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)      129 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      270 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)      218 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/setup.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.458693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)       33 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/lib.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/
--rw-rw-r--   0 timon     (1000) timon     (1000)      181 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      307 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/setup.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests/test_good.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/
--rw-rw-r--   0 timon     (1000) timon     (1000)      185 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      335 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/setup.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_err/test_bad.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/
--rw-rw-r--   0 timon     (1000) timon     (1000)      225 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      318 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/setup.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/test_bad.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/python_tests_targets/test_good.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)      333 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      287 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/app_pkg/vanilla.cpp
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)      207 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      250 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)       70 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/cmake_pkg/vanilla.cpp
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)     1341 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/Config.cmake.in
--rw-rw-r--   0 timon     (1000) timon     (1000)      248 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)       97 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)       17 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.h
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.482693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)      273 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      281 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_err_pkg/test.cpp
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/
--rw-rw-r--   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)      277 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/package.xml
--rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/test_pkg/test.cpp
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.462693 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/
--rw-rw-r--   0 timon     (1000) timon     (1000)      173 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/CMakeLists.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)       49 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/main.cpp
--rw-rw-r--   0 timon     (1000) timon     (1000)      334 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/resources/ros_pkgs/pkg_with_roslint/package.xml
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/verbs/__init__.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_build/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     3055 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_args.py
--rw-rw-r--   0 timon     (1000) timon     (1000)    18014 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_build.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_bwlists.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      564 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_context.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1126 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_eclipse.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1152 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_modify_ws.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     4604 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_pythonpath.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_unicode_in_env.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_whitespace_in_paths.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     3820 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_clean/clean.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_config/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_config/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2836 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_config/test_config.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_init/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_init/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      838 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_init/test_init.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2610 2023-02-23 16:58:37.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_profile/test_profile.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/system/verbs/catkin_test/
--rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_test/__init__.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     2935 2023-01-30 11:25:43.000000 catkin_tools-0.9.3/tests/system/verbs/catkin_test/test_unit_tests.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     5447 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/system/workspace_factory.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/test_code_format.py
-drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-06-29 09:31:41.486693 catkin_tools-0.9.3/tests/unit/
--rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 15:57:45.000000 catkin_tools-0.9.3/tests/unit/__init__.py
--rw-r--r--   0 timon     (1000) timon     (1000)       13 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/tests/unit/ascii_text.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     2437 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_common.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     4649 2023-02-23 15:52:56.000000 catkin_tools-0.9.3/tests/unit/test_config.py
--rw-rw-r--   0 timon     (1000) timon     (1000)      374 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_io.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     4351 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_job_flag_regex.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1137 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/unit/test_jobs.py
--rw-r--r--   0 timon     (1000) timon     (1000)       17 2022-04-19 16:00:24.000000 catkin_tools-0.9.3/tests/unit/unicode_text.txt
--rw-rw-r--   0 timon     (1000) timon     (1000)     5260 2023-02-23 15:52:45.000000 catkin_tools-0.9.3/tests/utils.py
--rw-rw-r--   0 timon     (1000) timon     (1000)     1234 2022-07-01 22:27:33.000000 catkin_tools-0.9.3/tests/workspace_assertions.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/.github/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1782 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/.github/ISSUE_TEMPLATE.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/.github/workflows/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1908 2023-08-03 15:02:31.000000 catkin_tools-0.9.4/.github/workflows/workflow.yml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      349 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/.gitignore
+-rw-rw-r--   0 timon     (1000) timon     (1000)      572 2023-08-03 15:02:28.000000 catkin_tools-0.9.4/.readthedocs.yaml
+-rw-rw-r--   0 timon     (1000) timon     (1000)    26317 2023-08-03 15:04:24.000000 catkin_tools-0.9.4/CHANGELOG.rst
+-rw-r--r--   0 timon     (1000) timon     (1000)    11335 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/LICENSE
+-rw-rw-r--   0 timon     (1000) timon     (1000)       31 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/MANIFEST.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/PKG-INFO
+-rw-rw-r--   0 timon     (1000) timon     (1000)      316 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/README.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/catkin_tools/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    16585 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/argument_parsing.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/commands/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/catkin_tools/commands/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10098 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/commands/catkin.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    21324 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/common.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5025 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/config.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    37403 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/catkin_tools/context.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/execution/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31661 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/catkin_tools/execution/controllers.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2304 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/events.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    15425 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/catkin_tools/execution/executor.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10053 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/io.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    12798 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/job_server.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1820 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/jobs.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6599 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/execution/stages.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/jobs/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    27764 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/catkin_tools/jobs/catkin.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/jobs/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1918 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/cmake/python.cmake
+-rw-rw-r--   0 timon     (1000) timon     (1000)      194 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/cmake/python_install_dir.cmake
+-rw-rw-r--   0 timon     (1000) timon     (1000)    16276 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/catkin_tools/jobs/cmake.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/jobs/commands/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/commands/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9936 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/commands/cmake.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/commands/make.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8774 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/jobs/utils.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    17302 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/catkin_tools/metadata.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/notifications/
+-rw-r--r--   0 timon     (1000) timon     (1000)      649 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/notifications/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2302 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/notifications/impl.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/
+-rw-r--r--   0 timon     (1000) timon     (1000)    56725 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31033 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon_red.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)    31532 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon_yellow.png
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1610 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Info.plist
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/
+-rwxr-xr-x   0 timon     (1000) timon     (1000)    20880 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/catkin build
+-rw-r--r--   0 timon     (1000) timon     (1000)        8 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/PkgInfo
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/
+-rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/AppIcon.icns
+-rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/catkin_blue_logo_only.icns
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/Credits.rtf
+-rw-r--r--   0 timon     (1000) timon     (1000)       92 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/InfoPlist.strings
+-rw-r--r--   0 timon     (1000) timon     (1000)    26323 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/MainMenu.nib
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/
+-rw-r--r--   0 timon     (1000) timon     (1000)       74 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/.gitignore
+-rw-r--r--   0 timon     (1000) timon     (1000)    67336 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/AppIcon.icns
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8026 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/README.markdown
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/
+-rw-r--r--   0 timon     (1000) timon     (1000)      122 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.h
+-rw-r--r--   0 timon     (1000) timon     (1000)     3113 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.m
+-rw-r--r--   0 timon     (1000) timon     (1000)     1178 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Info.plist
+-rw-r--r--   0 timon     (1000) timon     (1000)      165 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Prefix.pch
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)      436 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/Credits.rtf
+-rw-r--r--   0 timon     (1000) timon     (1000)       45 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/InfoPlist.strings
+-rw-r--r--   0 timon     (1000) timon     (1000)    45931 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/MainMenu.xib
+-rw-r--r--   0 timon     (1000) timon     (1000)      119 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/main.m
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/
+-rw-r--r--   0 timon     (1000) timon     (1000)    13799 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.pbxproj
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/
+-rw-r--r--   0 timon     (1000) timon     (1000)      162 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1593 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/Terminal Notifier.xccheckout
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/
+-rw-r--r--   0 timon     (1000) timon     (1000)     5102 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/Terminal Notifier.xcscheme
+-rw-r--r--   0 timon     (1000) timon     (1000)   107025 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/catkin_blue_logo_only.icns
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.379527 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/
+-rw-r--r--   0 timon     (1000) timon     (1000)     1174 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/Contents.json
+-rw-r--r--   0 timon     (1000) timon     (1000)     9426 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only128x128.png
+-rw-r--r--   0 timon     (1000) timon     (1000)     3212 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only16x16.png
+-rw-r--r--   0 timon     (1000) timon     (1000)    16330 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only256x256.png
+-rw-r--r--   0 timon     (1000) timon     (1000)     3961 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only32x32.png
+-rw-r--r--   0 timon     (1000) timon     (1000)    35515 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only512x512.png
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6716 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/resultspace.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/spaces/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      767 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      826 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/devel.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      755 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/install.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      748 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/log.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      762 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/spaces/source.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5462 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/terminal_color.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1524 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/utils.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/catkin_tools/verbs/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/
+-rw-r--r--   0 timon     (1000) timon     (1000)      960 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    30330 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    18708 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/color.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/
+-rw-r--r--   0 timon     (1000) timon     (1000)      863 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7474 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/clean.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    17214 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_config/
+-rw-r--r--   0 timon     (1000) timon     (1000)      975 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_config/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10902 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_config/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_create/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_create/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6751 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_create/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.391528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_env/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      965 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_env/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3921 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_env/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_init/
+-rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_init/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1956 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_init/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_list/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      885 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_list/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7864 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_list/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_locate/
+-rw-r--r--   0 timon     (1000) timon     (1000)      871 2022-04-19 21:21:18.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_locate/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7099 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_locate/cli.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_profile/
+-rw-r--r--   0 timon     (1000) timon     (1000)      868 2022-04-19 19:39:53.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_profile/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    10205 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_profile/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2975 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_shell_verbs.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      901 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7892 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/cli.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9462 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/test.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.387528 catkin_tools-0.9.4/catkin_tools.egg-info/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      615 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 timon     (1000) timon     (1000)    15200 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)        1 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      985 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       56 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/requires.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       13 2023-08-03 23:08:10.000000 catkin_tools-0.9.4/catkin_tools.egg-info/top_level.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/completion/
+-rw-rw-r--   0 timon     (1000) timon     (1000)    23450 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/completion/_catkin
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5109 2023-02-23 16:54:15.000000 catkin_tools-0.9.4/completion/catkin.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/docs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        7 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/docs/.gitignore
+-rw-r--r--   0 timon     (1000) timon     (1000)     6786 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/docs/Makefile
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/docs/_static/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/docs/_static/.gitignore
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/docs/_templates/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/docs/_templates/.gitignore
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/docs/advanced/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1001 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/catkin_shell_verbs.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    41154 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/executor_events.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)    86468 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/executor_events.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)    45234 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/executor_job_lifecycle.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)    78602 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/executor_job_resources.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     9187 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/job_executor.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1387 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/linked_develspace.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3892 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/advanced/verb_customization.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4580 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/build_types.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    36590 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/catkin_build.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)   180757 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/catkin_tools_execution.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4795 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/cheat_sheet.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8838 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/conf.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.395528 catkin_tools-0.9.4/docs/development/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2867 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/development/adding_build_types.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5950 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/development/extending_the_catkin_command.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1120 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/README.md
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/
+-rwxrwxr-x   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/0_init.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      128 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/1_build_warning.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/2_build_err.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/all.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/docs/examples/failure_ws/src/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5270 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      150 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/sub/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5321 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1929 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5189 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       60 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1923 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5199 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/grep-errors.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1926 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/quickstart_ws/
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      914 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/0_quickstart.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      108 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/1_prebuild.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      254 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/1_prebuild.out
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      109 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/2_postbuild.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1278 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/2_postbuild.out
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/quickstart_ws/all.bash
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      571 2023-08-03 15:02:28.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/0_checkout.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)       99 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/1_init.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      107 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/2_dry_run.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      236 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/3_build.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      118 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/4_build_v.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      125 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/5_build_i.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/6_build_partial.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      231 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/7_build_this.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      124 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/8_build_start_with.bash
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/9_build_no_deps.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      601 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/all.bash
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      395 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/slowrecord
+-rwxrwxr-x   0 timon     (1000) timon     (1000)     1812 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/examples/slowrun
+-rw-rw-r--   0 timon     (1000) timon     (1000)    21600 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/executor_job_lifecycle.dia
+-rw-rw-r--   0 timon     (1000) timon     (1000)   118107 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/executor_job_lifecycle.svg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6066 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/history.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4405 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/index.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2601 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/installing.rst
+-rw-r--r--   0 timon     (1000) timon     (1000)     6713 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/docs/make.bat
+-rw-rw-r--   0 timon     (1000) timon     (1000)    20283 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/mechanics.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)    19362 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/migration.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     7960 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/quick_start.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      479 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/spelling_wordlist.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2722 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/troubleshooting.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.399529 catkin_tools-0.9.4/docs/verbs/
+-rw-rw-r--   0 timon     (1000) timon     (1000)    14082 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_build.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4144 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_clean.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8995 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_config.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      403 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_create.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      500 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_env.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      998 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_init.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1338 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_list.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)      398 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_locate.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6824 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_profile.rst
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1931 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/catkin_test.rst
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/docs/verbs/cli/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     6864 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_build.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2920 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_clean.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     8287 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_config.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      631 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_create.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2669 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_create_pkg.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      822 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_env.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      469 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_init.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1965 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_list.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2323 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_locate.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      739 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_add.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      286 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_list.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      186 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_remove.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      309 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_rename.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      165 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_set.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3091 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/catkin_test.txt
+-rwxrwxr-x   0 timon     (1000) timon     (1000)      665 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/docs/verbs/cli/dump_cli
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/requirements.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       38 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/setup.cfg
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5365 2023-08-03 15:04:38.000000 catkin_tools-0.9.4/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      266 2023-08-03 15:02:31.000000 catkin_tools-0.9.4/stdeb.cfg
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1250 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/README.md
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2019-10-23 19:39:08.000000 catkin_tools-0.9.4/tests/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.4/tests/system/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/build_type_condition/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/build_type_condition/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      425 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/build_type_condition/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_args/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      301 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_args/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_args/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      167 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_warning/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      161 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_warning/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      311 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/cmake_warning/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/depend_condition/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       69 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/depend_condition/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      404 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/depend_condition/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      134 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       37 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_err/fail.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      299 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_err/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_warning/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      135 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_warning/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      304 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_warning/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       40 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/make_warning/warn.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      636 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       30 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.develspace.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)       32 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/cmake/extras.cmake.installspace.in
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/include/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/include/make_products_0/fun.h
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/lib.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      302 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      790 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/CMakeLists.txt
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.403529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/cmake/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       36 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.develspace.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)       38 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/cmake/extras.cmake.installspace.in
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/include/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/
+-rw-rw-r--   0 timon     (1000) timon     (1000)       43 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/include/make_products_0/fun.h
+-rw-rw-r--   0 timon     (1000) timon     (1000)       76 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/lib.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      308 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      129 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      270 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      218 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/setup.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/src/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)       33 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_pkg/src/python_pkg/lib.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      181 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      307 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests/test_good.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_err/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      185 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_err/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      335 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_err/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_err/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_err/test_bad.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      225 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      318 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      160 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/setup.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      360 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/test_bad.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      361 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/python_tests_targets/test_good.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/app_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      333 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/app_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      287 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/app_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)      104 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/app_pkg/vanilla.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/cmake_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      207 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/cmake_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      250 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/cmake_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       70 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/cmake_pkg/vanilla.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1341 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      110 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/Config.cmake.in
+-rw-rw-r--   0 timon     (1000) timon     (1000)      248 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       97 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)       17 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/vanilla.h
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_err_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      273 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_err_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      281 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_err_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_err_pkg/test.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_pkg/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      269 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_pkg/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)      277 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_pkg/package.xml
+-rw-rw-r--   0 timon     (1000) timon     (1000)       92 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/test_pkg/test.cpp
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.383528 catkin_tools-0.9.4/tests/system/resources/ros_pkgs/
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/resources/ros_pkgs/pkg_with_roslint/
+-rw-rw-r--   0 timon     (1000) timon     (1000)      173 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/ros_pkgs/pkg_with_roslint/CMakeLists.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)       49 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/ros_pkgs/pkg_with_roslint/main.cpp
+-rw-rw-r--   0 timon     (1000) timon     (1000)      334 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/resources/ros_pkgs/pkg_with_roslint/package.xml
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.407529 catkin_tools-0.9.4/tests/system/verbs/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.4/tests/system/verbs/__init__.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_build/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 21:21:14.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3055 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_args.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)    18014 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_build.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_bwlists.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      564 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_context.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1126 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_eclipse.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1152 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_modify_ws.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4604 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_pythonpath.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      606 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_unicode_in_env.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      871 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_whitespace_in_paths.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_clean/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_clean/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     3820 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_clean/clean.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_config/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_config/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2836 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_config/test_config.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_init/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_init/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      838 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_init/test_init.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_profile/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_profile/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2610 2023-02-23 16:58:37.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_profile/test_profile.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/system/verbs/catkin_test/
+-rw-rw-r--   0 timon     (1000) timon     (1000)        0 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_test/__init__.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2935 2023-01-30 11:25:43.000000 catkin_tools-0.9.4/tests/system/verbs/catkin_test/test_unit_tests.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5447 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/system/workspace_factory.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      666 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/test_code_format.py
+drwxrwxr-x   0 timon     (1000) timon     (1000)        0 2023-08-03 23:08:10.411529 catkin_tools-0.9.4/tests/unit/
+-rw-r--r--   0 timon     (1000) timon     (1000)        0 2022-04-19 15:57:45.000000 catkin_tools-0.9.4/tests/unit/__init__.py
+-rw-r--r--   0 timon     (1000) timon     (1000)       13 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/tests/unit/ascii_text.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     2437 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/unit/test_common.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4649 2023-02-23 15:52:56.000000 catkin_tools-0.9.4/tests/unit/test_config.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)      374 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/unit/test_io.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     4351 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/unit/test_job_flag_regex.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1137 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/unit/test_jobs.py
+-rw-r--r--   0 timon     (1000) timon     (1000)       17 2022-04-19 16:00:24.000000 catkin_tools-0.9.4/tests/unit/unicode_text.txt
+-rw-rw-r--   0 timon     (1000) timon     (1000)     5260 2023-02-23 15:52:45.000000 catkin_tools-0.9.4/tests/utils.py
+-rw-rw-r--   0 timon     (1000) timon     (1000)     1234 2022-07-01 22:27:33.000000 catkin_tools-0.9.4/tests/workspace_assertions.py
```

### Comparing `catkin_tools-0.9.3/.github/ISSUE_TEMPLATE.md` & `catkin_tools-0.9.4/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/.github/workflows/workflow.yml` & `catkin_tools-0.9.4/.github/workflows/workflow.yml`

 * *Files 12% similar despite different names*

```diff
@@ -4,18 +4,15 @@
 
 jobs:
   build:
     strategy:
       fail-fast: false
       matrix:
         versions:
-          - dist: ubuntu-18.04
-            python: "3.7"
-            catkin: indigo-devel
-          - dist: ubuntu-18.04
+          - dist: ubuntu-20.04
             python: "3.8"
             catkin: indigo-devel
           - dist: ubuntu-20.04
             python: "3.8"
             catkin: noetic-devel
           - dist: ubuntu-20.04
             python: "3.9"
@@ -28,17 +25,17 @@
             catkin: noetic-devel
           - dist: ubuntu-22.04
             python: "3.11"
             catkin: noetic-devel
 
     runs-on: ${{ matrix.versions.dist }}
     steps:
-      - uses: actions/checkout@v2
+      - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.versions.python }}
-        uses: actions/setup-python@v2
+        uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.versions.python }}
       - name: Install package and dependencies
         run: |
           python -m pip install --upgrade pip
           pip install .
           # Fix some sphinx versions until python 3.7 support is dropped
```

### Comparing `catkin_tools-0.9.3/CHANGELOG.rst` & `catkin_tools-0.9.4/CHANGELOG.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,23 @@
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 Changelog for package catkin_tools
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 Upcoming
 --------
 
+0.9.4 (2023-08-03)
+------------------
+
+* Update action versions (#757)
+* Add bookworm as a python3 target (#753)
+* Fix typo in documentation (#755)
+* Create .readthedocs.yaml (#756)
+* Contributors: Jonas Zohren, Timon Engelke, Tully Foote, William Woodall
+
 0.9.3 (2023-02-23)
 ------------------
 
 * Fix deprecated asyncio.wait() usage (#741)
 * Fix bash completion for catkin clean (#746)
 * Fix behavior when a different profile is set on the first launch (#728)
 * Update workflows with python > 3.9 (#745)
```

### Comparing `catkin_tools-0.9.3/LICENSE` & `catkin_tools-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/PKG-INFO` & `catkin_tools-0.9.4/catkin_tools.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: catkin_tools
-Version: 0.9.3
+Name: catkin-tools
+Version: 0.9.4
 Summary: Command line tools for working with catkin.
 Home-page: https://catkin-tools.readthedocs.org/
 Author: William Woodall
 Author-email: william@osrfoundation.org
 Maintainer: William Woodall
 Maintainer-email: william@osrfoundation.org
 License: Apache 2.0
```

### Comparing `catkin_tools-0.9.3/catkin_tools/argument_parsing.py` & `catkin_tools-0.9.4/catkin_tools/argument_parsing.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/commands/catkin.py` & `catkin_tools-0.9.4/catkin_tools/commands/catkin.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/common.py` & `catkin_tools-0.9.4/catkin_tools/common.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/config.py` & `catkin_tools-0.9.4/catkin_tools/config.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/context.py` & `catkin_tools-0.9.4/catkin_tools/context.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/controllers.py` & `catkin_tools-0.9.4/catkin_tools/execution/controllers.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/events.py` & `catkin_tools-0.9.4/catkin_tools/execution/events.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/executor.py` & `catkin_tools-0.9.4/catkin_tools/execution/executor.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/io.py` & `catkin_tools-0.9.4/catkin_tools/execution/io.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/job_server.py` & `catkin_tools-0.9.4/catkin_tools/execution/job_server.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/jobs.py` & `catkin_tools-0.9.4/catkin_tools/execution/jobs.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/execution/stages.py` & `catkin_tools-0.9.4/catkin_tools/execution/stages.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/catkin.py` & `catkin_tools-0.9.4/catkin_tools/jobs/catkin.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/cmake/python.cmake` & `catkin_tools-0.9.4/catkin_tools/jobs/cmake/python.cmake`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/cmake.py` & `catkin_tools-0.9.4/catkin_tools/jobs/cmake.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/commands/cmake.py` & `catkin_tools-0.9.4/catkin_tools/jobs/commands/cmake.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/commands/make.py` & `catkin_tools-0.9.4/catkin_tools/jobs/commands/make.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/jobs/utils.py` & `catkin_tools-0.9.4/catkin_tools/jobs/utils.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/metadata.py` & `catkin_tools-0.9.4/catkin_tools/metadata.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/__init__.py` & `catkin_tools-0.9.4/catkin_tools/notifications/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/impl.py` & `catkin_tools-0.9.4/catkin_tools/notifications/impl.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_red.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon_red.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/linux/catkin_icon_yellow.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/linux/catkin_icon_yellow.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Info.plist` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Info.plist`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/catkin build` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/MacOS/catkin build`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/AppIcon.icns` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/catkin_blue_logo_only.icns` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/catkin_blue_logo_only.icns`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/MainMenu.nib` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin build.app/Contents/Resources/en.lproj/MainMenu.nib`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/AppIcon.icns` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/AppIcon.icns`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/README.markdown` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/README.markdown`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.m` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/AppDelegate.m`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Info.plist` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/Terminal Notifier-Info.plist`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/MainMenu.xib` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier/en.lproj/MainMenu.xib`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.pbxproj` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/Terminal Notifier.xccheckout` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/project.xcworkspace/xcshareddata/Terminal Notifier.xccheckout`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/Terminal Notifier.xcscheme` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/Terminal Notifier.xcodeproj/xcshareddata/xcschemes/Terminal Notifier.xcscheme`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/catkin_blue_logo_only.icns` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/catkin_blue_logo_only.icns`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/Contents.json` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/Contents.json`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only128x128.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only128x128.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only16x16.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only16x16.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only256x256.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only256x256.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only32x32.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only32x32.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only512x512.png` & `catkin_tools-0.9.4/catkin_tools/notifications/resources/osx/catkin_build_notifier_src/terminal-notifier/Images.xcassets/AppIcon.appiconset/catkin_blue_logo_only512x512.png`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/resultspace.py` & `catkin_tools-0.9.4/catkin_tools/resultspace.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/spaces/build.py` & `catkin_tools-0.9.4/catkin_tools/spaces/build.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/spaces/devel.py` & `catkin_tools-0.9.4/catkin_tools/spaces/devel.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/spaces/install.py` & `catkin_tools-0.9.4/catkin_tools/spaces/install.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/spaces/log.py` & `catkin_tools-0.9.4/catkin_tools/spaces/log.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/spaces/source.py` & `catkin_tools-0.9.4/catkin_tools/spaces/source.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/terminal_color.py` & `catkin_tools-0.9.4/catkin_tools/terminal_color.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/utils.py` & `catkin_tools-0.9.4/catkin_tools/utils.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/build.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/build.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_build/color.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_build/color.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/clean.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/clean.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_clean/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_clean/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_config/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_config/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_config/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_create/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_create/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_create/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_env/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_env/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_env/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_init/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_init/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_init/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_list/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_list/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_list/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_locate/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_locate/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_locate/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_profile/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_profile/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_profile/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_shell_verbs.bash` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_shell_verbs.bash`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/__init__.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/__init__.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/cli.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/cli.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools/verbs/catkin_test/test.py` & `catkin_tools-0.9.4/catkin_tools/verbs/catkin_test/test.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/catkin_tools.egg-info/PKG-INFO` & `catkin_tools-0.9.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: catkin-tools
-Version: 0.9.3
+Name: catkin_tools
+Version: 0.9.4
 Summary: Command line tools for working with catkin.
 Home-page: https://catkin-tools.readthedocs.org/
 Author: William Woodall
 Author-email: william@osrfoundation.org
 Maintainer: William Woodall
 Maintainer-email: william@osrfoundation.org
 License: Apache 2.0
```

### Comparing `catkin_tools-0.9.3/catkin_tools.egg-info/SOURCES.txt` & `catkin_tools-0.9.4/catkin_tools.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 .gitignore
+.readthedocs.yaml
 CHANGELOG.rst
 LICENSE
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 stdeb.cfg
```

### Comparing `catkin_tools-0.9.3/catkin_tools.egg-info/entry_points.txt` & `catkin_tools-0.9.4/catkin_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/completion/_catkin` & `catkin_tools-0.9.4/completion/_catkin`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/completion/catkin.bash` & `catkin_tools-0.9.4/completion/catkin.bash`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/Makefile` & `catkin_tools-0.9.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/catkin_shell_verbs.rst` & `catkin_tools-0.9.4/docs/advanced/catkin_shell_verbs.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/executor_events.dia` & `catkin_tools-0.9.4/docs/advanced/executor_events.dia`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/executor_events.svg` & `catkin_tools-0.9.4/docs/advanced/executor_events.svg`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/executor_job_lifecycle.svg` & `catkin_tools-0.9.4/docs/advanced/executor_job_lifecycle.svg`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/executor_job_resources.svg` & `catkin_tools-0.9.4/docs/advanced/executor_job_resources.svg`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/job_executor.rst` & `catkin_tools-0.9.4/docs/advanced/job_executor.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/linked_develspace.rst` & `catkin_tools-0.9.4/docs/advanced/linked_develspace.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/advanced/verb_customization.rst` & `catkin_tools-0.9.4/docs/advanced/verb_customization.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/build_types.rst` & `catkin_tools-0.9.4/docs/build_types.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/catkin_build.dia` & `catkin_tools-0.9.4/docs/catkin_build.dia`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/catkin_tools_execution.dia` & `catkin_tools-0.9.4/docs/catkin_tools_execution.dia`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/cheat_sheet.rst` & `catkin_tools-0.9.4/docs/cheat_sheet.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/conf.py` & `catkin_tools-0.9.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/development/adding_build_types.rst` & `catkin_tools-0.9.4/docs/development/adding_build_types.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/development/extending_the_catkin_command.rst` & `catkin_tools-0.9.4/docs/development/extending_the_catkin_command.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/README.md` & `catkin_tools-0.9.4/docs/examples/README.md`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/CMakeLists.txt` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_err/package.xml` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_err/package.xml`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/CMakeLists.txt` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/package.xml` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_cmake_warn/package.xml`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/CMakeLists.txt` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_err/package.xml` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_err/package.xml`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/CMakeLists.txt` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/failure_ws/src/catkin_pkg_make_warn/package.xml` & `catkin_tools-0.9.4/docs/examples/failure_ws/src/catkin_pkg_make_warn/package.xml`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/quickstart_ws/0_quickstart.bash` & `catkin_tools-0.9.4/docs/examples/quickstart_ws/0_quickstart.bash`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/quickstart_ws/2_postbuild.out` & `catkin_tools-0.9.4/docs/examples/quickstart_ws/2_postbuild.out`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/0_checkout.bash` & `catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/0_checkout.bash`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 export ROS_DISTRO=noetic                                 # Set ROS distribution
 mkdir -p /tmp/ros_tutorials_ws/src                       # Create workspace
 cd /tmp/ros_tutorials_ws/src                             # Navigate to source space
-rosinstall_generator --deps ros_tutorials > .rosinstall  # Get list of pakcages
+rosinstall_generator --deps ros_tutorials > .rosinstall  # Get list of packages
 wstool update                                            # Checkout all packages
 cd /tmp/ros_tutorials_ws                                 # Navigate to ros workspace root
 catkin init                                              # Initialize workspace
```

### Comparing `catkin_tools-0.9.3/docs/examples/ros_tutorials_ws/all.bash` & `catkin_tools-0.9.4/docs/examples/ros_tutorials_ws/all.bash`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/examples/slowrun` & `catkin_tools-0.9.4/docs/examples/slowrun`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/executor_job_lifecycle.dia` & `catkin_tools-0.9.4/docs/executor_job_lifecycle.dia`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/executor_job_lifecycle.svg` & `catkin_tools-0.9.4/docs/executor_job_lifecycle.svg`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/history.rst` & `catkin_tools-0.9.4/docs/history.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/index.rst` & `catkin_tools-0.9.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/installing.rst` & `catkin_tools-0.9.4/docs/installing.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/make.bat` & `catkin_tools-0.9.4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/mechanics.rst` & `catkin_tools-0.9.4/docs/mechanics.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/migration.rst` & `catkin_tools-0.9.4/docs/migration.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/quick_start.rst` & `catkin_tools-0.9.4/docs/quick_start.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/troubleshooting.rst` & `catkin_tools-0.9.4/docs/troubleshooting.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_build.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_build.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_clean.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_clean.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_config.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_config.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_init.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_init.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_list.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_list.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_profile.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_profile.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/catkin_test.rst` & `catkin_tools-0.9.4/docs/verbs/catkin_test.rst`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_build.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_build.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_clean.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_clean.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_config.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_config.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_create.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_create.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_create_pkg.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_create_pkg.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_env.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_env.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_list.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_list.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_locate.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_locate.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_profile.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_profile.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_profile_add.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_profile_add.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/catkin_test.txt` & `catkin_tools-0.9.4/docs/verbs/cli/catkin_test.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/docs/verbs/cli/dump_cli` & `catkin_tools-0.9.4/docs/verbs/cli/dump_cli`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/setup.py` & `catkin_tools-0.9.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,15 +87,15 @@
                 mode = ((os.stat(file)[ST_MODE]) | 0o444) & 0o7777
                 log.info("changing permissions of %s to %o" % (file, mode))
                 os.chmod(file, mode)
 
 
 setup(
     name='catkin_tools',
-    version='0.9.3',
+    version='0.9.4',
     python_requires='>=3.5',
     packages=find_packages(exclude=['tests*', 'docs']),
     package_data={
         'catkin_tools': [
             'jobs/cmake/python.cmake',
             'jobs/cmake/python_install_dir.cmake',
             'verbs/catkin_shell_verbs.bash',
```

### Comparing `catkin_tools-0.9.3/tests/README.md` & `catkin_tools-0.9.4/tests/README.md`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_0/CMakeLists.txt` & `catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_0/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/resources/catkin_pkgs/products_unicode/CMakeLists.txt` & `catkin_tools-0.9.4/tests/system/resources/catkin_pkgs/products_unicode/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/resources/cmake_pkgs/lib_pkg/CMakeLists.txt` & `catkin_tools-0.9.4/tests/system/resources/cmake_pkgs/lib_pkg/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_args.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_args.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_build.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_build.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_bwlists.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_bwlists.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_context.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_context.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_eclipse.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_eclipse.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_modify_ws.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_modify_ws.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_pythonpath.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_pythonpath.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_unicode_in_env.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_unicode_in_env.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_build/test_whitespace_in_paths.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_build/test_whitespace_in_paths.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_clean/clean.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_clean/clean.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_config/test_config.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_config/test_config.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_init/test_init.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_init/test_init.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_profile/test_profile.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_profile/test_profile.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/verbs/catkin_test/test_unit_tests.py` & `catkin_tools-0.9.4/tests/system/verbs/catkin_test/test_unit_tests.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/system/workspace_factory.py` & `catkin_tools-0.9.4/tests/system/workspace_factory.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/test_code_format.py` & `catkin_tools-0.9.4/tests/test_code_format.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/unit/test_common.py` & `catkin_tools-0.9.4/tests/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/unit/test_config.py` & `catkin_tools-0.9.4/tests/unit/test_config.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/unit/test_job_flag_regex.py` & `catkin_tools-0.9.4/tests/unit/test_job_flag_regex.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/unit/test_jobs.py` & `catkin_tools-0.9.4/tests/unit/test_jobs.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/utils.py` & `catkin_tools-0.9.4/tests/utils.py`

 * *Files identical despite different names*

### Comparing `catkin_tools-0.9.3/tests/workspace_assertions.py` & `catkin_tools-0.9.4/tests/workspace_assertions.py`

 * *Files identical despite different names*

