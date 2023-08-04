# Comparing `tmp/tickle-me-email-4.8.0.tar.gz` & `tmp/tickle-me-email-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tickle-me-email-4.8.0.tar", last modified: Thu Sep  1 09:02:15 2022, max compression
+gzip compressed data, was "tickle-me-email-4.9.0.tar", last modified: Fri Aug  4 12:45:47 2023, max compression
```

## Comparing `tickle-me-email-4.8.0.tar` & `tickle-me-email-4.9.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2022-09-01 09:02:15.098307 tickle-me-email-4.8.0/
--rw-r--r--   0 lamby     (1000) lamby     (1000)    35147 2014-12-13 17:25:37.000000 tickle-me-email-4.8.0/COPYING
--rw-r--r--   0 lamby     (1000) lamby     (1000)      316 2022-09-01 09:02:15.098307 tickle-me-email-4.8.0/PKG-INFO
--rw-r--r--   0 lamby     (1000) lamby     (1000)     3343 2019-09-26 11:01:07.000000 tickle-me-email-4.8.0/README.rst
--rw-r--r--   0 lamby     (1000) lamby     (1000)       75 2019-08-02 21:23:12.000000 tickle-me-email-4.8.0/pyproject.toml
--rw-r--r--   0 lamby     (1000) lamby     (1000)       38 2022-09-01 09:02:15.098307 tickle-me-email-4.8.0/setup.cfg
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)      372 2022-09-01 09:02:14.000000 tickle-me-email-4.8.0/setup.py
--rwxr-xr-x   0 lamby     (1000) lamby     (1000)    21421 2022-09-01 08:02:28.000000 tickle-me-email-4.8.0/tickle-me-email
-drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2022-09-01 09:02:15.098307 tickle-me-email-4.8.0/tickle_me_email.egg-info/
--rw-r--r--   0 lamby     (1000) lamby     (1000)      316 2022-09-01 09:02:15.000000 tickle-me-email-4.8.0/tickle_me_email.egg-info/PKG-INFO
--rw-r--r--   0 lamby     (1000) lamby     (1000)      214 2022-09-01 09:02:15.000000 tickle-me-email-4.8.0/tickle_me_email.egg-info/SOURCES.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)        1 2022-09-01 09:02:15.000000 tickle-me-email-4.8.0/tickle_me_email.egg-info/dependency_links.txt
--rw-r--r--   0 lamby     (1000) lamby     (1000)        1 2022-09-01 09:02:15.000000 tickle-me-email-4.8.0/tickle_me_email.egg-info/top_level.txt
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 12:45:47.684282 tickle-me-email-4.9.0/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)    35147 2014-12-13 17:25:37.000000 tickle-me-email-4.9.0/COPYING
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      271 2023-08-04 12:45:47.684282 tickle-me-email-4.9.0/PKG-INFO
+-rw-r--r--   0 lamby     (1000) lamby     (1000)     3343 2019-09-26 11:01:07.000000 tickle-me-email-4.9.0/README.rst
+-rw-r--r--   0 lamby     (1000) lamby     (1000)       75 2019-08-02 21:23:12.000000 tickle-me-email-4.9.0/pyproject.toml
+-rw-r--r--   0 lamby     (1000) lamby     (1000)       38 2023-08-04 12:45:47.684282 tickle-me-email-4.9.0/setup.cfg
+-rwxr-xr-x   0 lamby     (1000) lamby     (1000)      372 2023-08-04 12:45:46.000000 tickle-me-email-4.9.0/setup.py
+-rwxr-xr-x   0 lamby     (1000) lamby     (1000)    21874 2023-08-04 12:23:30.000000 tickle-me-email-4.9.0/tickle-me-email
+drwxr-xr-x   0 lamby     (1000) lamby     (1000)        0 2023-08-04 12:45:47.684282 tickle-me-email-4.9.0/tickle_me_email.egg-info/
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      271 2023-08-04 12:45:47.000000 tickle-me-email-4.9.0/tickle_me_email.egg-info/PKG-INFO
+-rw-r--r--   0 lamby     (1000) lamby     (1000)      214 2023-08-04 12:45:47.000000 tickle-me-email-4.9.0/tickle_me_email.egg-info/SOURCES.txt
+-rw-r--r--   0 lamby     (1000) lamby     (1000)        1 2023-08-04 12:45:47.000000 tickle-me-email-4.9.0/tickle_me_email.egg-info/dependency_links.txt
+-rw-r--r--   0 lamby     (1000) lamby     (1000)        7 2023-08-04 12:45:47.000000 tickle-me-email-4.9.0/tickle_me_email.egg-info/top_level.txt
```

### Comparing `tickle-me-email-4.8.0/COPYING` & `tickle-me-email-4.9.0/COPYING`

 * *Files identical despite different names*

### Comparing `tickle-me-email-4.8.0/README.rst` & `tickle-me-email-4.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `tickle-me-email-4.8.0/tickle-me-email` & `tickle-me-email-4.9.0/tickle-me-email`

 * *Files 2% similar despite different names*

```diff
@@ -127,15 +127,18 @@
         if not self.select_mailbox(src):
             # No messages
             return
 
         messages = self.get_messages()
 
         for idx in sorted(messages, reverse=True):
-            self.move_message(self.get_uid(idx), dst)
+            uid = self.get_uid(idx)
+            if self.options.move_unread:
+                self.flag_message(uid, r"Seen", False)
+            self.move_message(uid, dst)
 
         self.log.info("Moved %d message(s) from %s -> %s", len(messages), src, dst)
 
     def handle_rotate(self, template, start, stop, target):
         self.connect_imap()
 
         start, stop = int(start), int(stop)
@@ -258,26 +261,37 @@
             r"\SEEN" if self.options.todo_read else "",
             imaplib.Time2Internaldate(time.time()),
             msg.as_string().encode("utf-8"),
         )
 
         self.check_response(response, "Error adding TODO item")
 
-    def handle_subjects(self):
+    def handle_subjects(self, *args):
         self.connect_imap()
 
-        if not self.select_mailbox(self.options.subjects_mailbox):
-            # No messages
-            return
+        def fn(mailbox):
+            if not self.select_mailbox(mailbox):
+                # No messages
+                return
 
-        for x, y in self.get_fields(("Subject", "From")):
-            print(x.replace("\n", " ").replace("\r", " "), end="")
+            for x, y in self.get_fields(("Subject", "From")):
+                print(x.replace("\n", " ").replace("\r", " "), end="")
+
+                if self.options.subjects_include_from and y != self.options.todo_email:
+                    print(" ({})".format(self.parseaddr(y)), end="")
+                print()
+
+        args = sys.stdin.read().splitlines() if args == ("-",) else args
+
+        if not args:
+            return fn(self.options.subjects_mailbox)
 
-            if self.options.subjects_include_from and y != self.options.todo_email:
-                print(" ({})".format(self.parseaddr(y)), end="")
+        for mailbox in args:
+            print(mailbox)
+            fn(mailbox)
             print()
 
     def handle_sent(self):
         self.connect_imap()
 
         num_today = 0
         today = datetime.date.today().strftime("%d-%b-%Y").lstrip("0")
@@ -436,14 +450,15 @@
         for type_, x, y, default in (
             (str, "todo", "email", "TODO <nobody@example.com>"),
             (str, "todo", "prefix", "TODO: "),
             (str, "todo", "mailbox", "INBOX"),
             (bool, "todo", "read", "0"),
             (str, "imap", "sent_items", "INBOX.Sent Items"),
             (str, "mbox", "mailbox", "INBOX"),
+            (bool, "move", "unread", "0"),
             (str, "draft", "to", ""),
             (str, "draft", "cc", ""),
             (str, "draft", "bcc", ""),
             (str, "draft", "subject", ""),
             (str, "draft", "mailbox", "INBOX.Drafts"),
             (str, "draft", "attachment", None),
             (str, "draft", "extra_headers", ""),
```

