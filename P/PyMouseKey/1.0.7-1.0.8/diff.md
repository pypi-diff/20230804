# Comparing `tmp/PyMouseKey-1.0.7-py3-none-any.whl.zip` & `tmp/PyMouseKey-1.0.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,7 +1,7 @@
-Zip file size: 6506 bytes, number of entries: 5
--rw-rw-rw-  2.0 fat    20926 b- defN 23-Aug-02 18:32 pymousekey/__init__.py
--rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      389 b- defN 23-Aug-02 18:32 PyMouseKey-1.0.7.dist-info/RECORD
-5 files, 21888 bytes uncompressed, 5780 bytes compressed:  73.6%
+Zip file size: 6644 bytes, number of entries: 5
+-rw-rw-rw-  2.0 fat    21517 b- defN 23-Aug-04 06:41 pymousekey/__init__.py
+-rw-rw-rw-  2.0 fat      470 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       11 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      389 b- defN 23-Aug-04 06:42 PyMouseKey-1.0.8.dist-info/RECORD
+5 files, 22479 bytes uncompressed, 5918 bytes compressed:  73.7%
```

## zipnote {}

```diff
@@ -1,16 +1,16 @@
 Filename: pymousekey/__init__.py
 Comment: 
 
-Filename: PyMouseKey-1.0.7.dist-info/METADATA
+Filename: PyMouseKey-1.0.8.dist-info/METADATA
 Comment: 
 
-Filename: PyMouseKey-1.0.7.dist-info/WHEEL
+Filename: PyMouseKey-1.0.8.dist-info/WHEEL
 Comment: 
 
-Filename: PyMouseKey-1.0.7.dist-info/top_level.txt
+Filename: PyMouseKey-1.0.8.dist-info/top_level.txt
 Comment: 
 
-Filename: PyMouseKey-1.0.7.dist-info/RECORD
+Filename: PyMouseKey-1.0.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pymousekey/__init__.py

```diff
@@ -46,14 +46,15 @@
 WM_RBUTTONDOWN = 0x0204
 WM_RBUTTONUP = 0x0205
 WM_RBUTTONCLICK = WM_RBUTTONDOWN + WM_RBUTTONUP
 WM_MBUTTONDOWN = 0x0207
 WM_MBUTTONUP = 0x0208
 WM_MBUTTONCLICK = WM_MBUTTONDOWN + WM_MBUTTONUP
 WM_HOTKEY = 0x0312
+WM_XBUTTONDOWN = 0x020B
 
 WM_NCHITTEST = 0x0084
 WM_MOUSEMOVE = 0x0200
 WM_SETCURSOR = 0x0020
 
 MK_LBUTTON = 0x0001
 MK_MBUTTON = 0x0010
@@ -244,14 +245,19 @@
     'numpad 5': 0x65,
     'numpad 6': 0x66,
     'numpad 7': 0x67,
     'numpad 8': 0x68,
     'numpad 9': 0x69,
     'multiply': 0x6A,
     'add': 0x6B,
+    '+': 0xBB,
+    ',': 0xBC,	
+    'minus': 0xBD,
+    '-': 0xBD,
+    '.': 0xBE,
     'seperator': 0x6C,
     'subtract': 0x6D,
     'decimal': 0x6E,
     'divide': 0x6F,
     'f1': 0x70,
     'f2': 0x71,
     'f3': 0x72,
@@ -288,14 +294,22 @@
     'rcontrol': 0xA3,
     'rctrl': 0xA3,
     'right control': 0xA3,
     'lalt': 0xA4,
     'left alt': 0xA4,
     'ralt': 0xA5,
     'right alt': 0xA5,
+    '?': 0xBF,
+    'tilde': 0xC0,
+    '[': 0xDB,
+    '\\': 0xDC,
+    ']': 0xDD,
+    '"': 0xDE,
+    "'": 0xDE,
+    'clear': 0xFE,
 }
 
 class KeyBdInput(ctypes.Structure):
     _fields_ = [("wVk", ctypes.c_ushort),
                 ("wScan", ctypes.c_ushort),
                 ("dwFlags", ctypes.c_ulong),
                 ("time", ctypes.c_ulong),
@@ -537,18 +551,18 @@
         return
 
     ii_ = Input_I()
     ii_.ki = KeyBdInput(0, KEYS[key.lower()], KEYEVENTF_SCANCODE | KEYEVENTF_KEYUP, 0, ctypes.pointer(ctypes.c_ulong(0)))
     x = Input(ctypes.c_ulong(1), ii_)
     ctypes.windll.user32.SendInput(1, ctypes.pointer(x), ctypes.sizeof(x))
 
-
-def add_hotkey(key, callback, args=()):
+def add_hotkey(key, callback, args=(), suppress=True):
     """
-    Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate daemon thread
+    Registers a system wide hotkey with optional args using ctypes and GetMessageW starting it in a seperate daemon thread\n
+    If suppress is true then block the original function of the key
 
     """
     def add_hotkey_thread(key, callback, args=()):
         key_id = len(registered_hotkeys) + 1
         registered_hotkeys[VK_KEYS[key]] = key_id
         hotkey_threads[VK_KEYS[key]] = hotkey_thread.native_id
 
@@ -558,14 +572,18 @@
 
         while ctypes.windll.user32.GetMessageW(ctypes.byref(msg), 0, 0, 0) != 0:
             if msg.message == WM_HOTKEY:
                 if args:
                     callback(args)
                 else:
                     callback()
+                if not suppress:
+                    ctypes.windll.user32.UnregisterHotKey(None, key_id , None, VK_KEYS[key])
+                    press(key, 0, False)
+                    ctypes.windll.user32.RegisterHotKey(None, key_id , None, VK_KEYS[key])
                 ctypes.windll.user32.TranslateMessage(ctypes.byref(msg))
                 ctypes.windll.user32.DispatchMessageW(ctypes.byref(msg))
         
         try:
             ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
         except(KeyError):
             pass
@@ -582,15 +600,14 @@
     """
     if VK_KEYS[key] in registered_hotkeys:
         ctypes.windll.user32.UnregisterHotKey(None, registered_hotkeys[VK_KEYS[key]])
         ctypes.windll.user32.PostThreadMessageW(hotkey_threads[VK_KEYS[key]], WM_QUIT, 0, 0)
         del registered_hotkeys[VK_KEYS[key]]
         del hotkey_threads[VK_KEYS[key]]
 
-
 def remove_all_hotkeys():
     """
     Unregisters and removes all currently registered hotkeys
     
     """
     for key in registered_hotkeys.values():
         ctypes.windll.user32.UnregisterHotKey(None, key)
```

