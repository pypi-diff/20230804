# Comparing `tmp/h5p-xblock-0.2.4.tar.gz` & `tmp/h5p-xblock-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5p-xblock-0.2.4.tar", last modified: Wed Apr  5 07:31:06 2023, max compression
+gzip compressed data, was "h5p-xblock-0.2.5.tar", last modified: Fri Aug  4 13:02:07 2023, max compression
```

## Comparing `h5p-xblock-0.2.4.tar` & `h5p-xblock-0.2.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5p_xblock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      580 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       51 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       10 2023-04-05 07:31:06.000000 h5p-xblock-0.2.4/h5p_xblock.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5pxblock/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11016 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/h5pxblock.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.625975 h5p-xblock-0.2.4/h5pxblock/public/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5pxblock/public/js/
--rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/public/js/h5pcustom.js
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.625975 h5p-xblock-0.2.4/h5pxblock/static/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5pxblock/static/css/
--rw-r--r--   0 runner    (1001) docker     (122)      793 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/css/student_view.css
--rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/css/studio.css
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5pxblock/static/html/
--rw-r--r--   0 runner    (1001) docker     (122)      235 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/html/author_view.html
--rw-r--r--   0 runner    (1001) docker     (122)      413 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/html/h5pxblock.html
--rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/html/studio.html
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.625975 h5p-xblock-0.2.4/h5pxblock/static/js/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/h5pxblock/static/js/src/
--rw-r--r--   0 runner    (1001) docker     (122)     3439 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/js/src/h5pxblock.js
--rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/static/js/src/studio.js
--rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/h5pxblock/utils.py
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-05 07:31:06.629975 h5p-xblock-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-04-05 07:31:01.000000 h5p-xblock-0.2.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/
+-rw-r--r--   0 runner    (1001) docker     (122)     1064 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1244 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5p_xblock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2258 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      580 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       51 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-08-04 13:02:07.000000 h5p-xblock-0.2.5/h5p_xblock.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5pxblock/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11016 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/h5pxblock.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.669007 h5p-xblock-0.2.5/h5pxblock/public/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5pxblock/public/js/
+-rw-r--r--   0 runner    (1001) docker     (122)     2047 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/public/js/h5pcustom.js
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.669007 h5p-xblock-0.2.5/h5pxblock/static/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5pxblock/static/css/
+-rw-r--r--   0 runner    (1001) docker     (122)      758 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/css/student_view.css
+-rw-r--r--   0 runner    (1001) docker     (122)     1508 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/css/studio.css
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5pxblock/static/html/
+-rw-r--r--   0 runner    (1001) docker     (122)      235 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/html/author_view.html
+-rw-r--r--   0 runner    (1001) docker     (122)      413 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/html/h5pxblock.html
+-rw-r--r--   0 runner    (1001) docker     (122)     7304 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/html/studio.html
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.669007 h5p-xblock-0.2.5/h5pxblock/static/js/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/h5pxblock/static/js/src/
+-rw-r--r--   0 runner    (1001) docker     (122)     3616 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/js/src/h5pxblock.js
+-rw-r--r--   0 runner    (1001) docker     (122)     4202 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/static/js/src/studio.js
+-rw-r--r--   0 runner    (1001) docker     (122)     3371 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/h5pxblock/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-04 13:02:07.673007 h5p-xblock-0.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1682 2023-08-04 13:02:02.000000 h5p-xblock-0.2.5/setup.py
```

### Comparing `h5p-xblock-0.2.4/LICENSE` & `h5p-xblock-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/PKG-INFO` & `h5p-xblock-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5p-xblock
-Version: 0.2.4
+Version: 0.2.5
 Summary: XBlock to play self hosted h5p content inside open edX
 Home-page: https://github.com/edly-io/h5pxblock
 Author: edly
 Author-email: hello@edly.io
 License: MIT
 Description: 
         # Play H5P content in Open edX using h5pxblock
```

### Comparing `h5p-xblock-0.2.4/README.md` & `h5p-xblock-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5p_xblock.egg-info/PKG-INFO` & `h5p-xblock-0.2.5/h5p_xblock.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5p-xblock
-Version: 0.2.4
+Version: 0.2.5
 Summary: XBlock to play self hosted h5p content inside open edX
 Home-page: https://github.com/edly-io/h5pxblock
 Author: edly
 Author-email: hello@edly.io
 License: MIT
 Description: 
         # Play H5P content in Open edX using h5pxblock
```

### Comparing `h5p-xblock-0.2.4/h5p_xblock.egg-info/SOURCES.txt` & `h5p-xblock-0.2.5/h5p_xblock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5pxblock/h5pxblock.py` & `h5p-xblock-0.2.5/h5pxblock/h5pxblock.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
         """
         context = {
             "h5pblock": self,
         }
         template = self.render_template("static/html/h5pxblock.html", context)
         frag = Fragment(template)
         frag.add_css(self.resource_string("static/css/student_view.css"))
-        frag.add_javascript_url('https://cdn.jsdelivr.net/npm/h5p-standalone@3.5.1/dist/main.bundle.js')
+        frag.add_javascript_url('https://cdn.jsdelivr.net/npm/h5p-standalone@3.6.0/dist/main.bundle.js')
         frag.add_javascript(self.resource_string("static/js/src/h5pxblock.js"))
         user_service = self.runtime.service(self, 'user')
         user = user_service.get_current_user()
         save_freq = self.save_freq if self.save_freq > 0 else False
         frag.initialize_js(
             'H5PPlayerXBlock',
             json_args={
```

### Comparing `h5p-xblock-0.2.4/h5pxblock/public/js/h5pcustom.js` & `h5p-xblock-0.2.5/h5pxblock/public/js/h5pcustom.js`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5pxblock/static/css/studio.css` & `h5p-xblock-0.2.5/h5pxblock/static/css/studio.css`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5pxblock/static/html/studio.html` & `h5p-xblock-0.2.5/h5pxblock/static/html/studio.html`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5pxblock/static/js/src/h5pxblock.js` & `h5p-xblock-0.2.5/h5pxblock/static/js/src/h5pxblock.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -11,76 +11,78 @@
         if (el && $(el).children('.h5p-iframe-wrapper').length == 0) {
             const userObj = {
                 'name': args.user_full_name,
                 'mail': args.user_email
             };
             const options = {
                 h5pJsonPath: args.h5pJsonPath,
-                frameJs: 'https://cdn.jsdelivr.net/npm/h5p-standalone@3.5.1/dist/frame.bundle.js',
-                frameCss: 'https://cdn.jsdelivr.net/npm/h5p-standalone@3.5.1/dist/styles/h5p.css',
+                frameJs: 'https://cdn.jsdelivr.net/npm/h5p-standalone@3.6.0/dist/frame.bundle.js',
+                frameCss: 'https://cdn.jsdelivr.net/npm/h5p-standalone@3.6.0/dist/styles/h5p.css',
                 frame: args.frame,
                 copyright: args.copyright,
                 icon: args.icon,
                 fullScreen: args.fullScreen,
                 user: userObj,
                 saveFreq: args.saveFreq,
                 customJs: args.customJsPath,
                 contentUserData: [{
                     state: args.userData
                 }],
                 ajax: {
                     contentUserDataUrl: contentUserDataUrl
                 }
             }
+
             return new H5PStandalone.H5P(el, options).then(function() {
                 $(el).siblings('.spinner-container').find('.spinner-border').hide();
                 $(el).show();
+                H5P.externalDispatcher.on("xAPI", (event) => {
+
+                    let hasStatement = event && event.data && event.data.statement;
+                    if (!hasStatement) {
+                        return;
+                    }
+
+                    let statement = event.data.statement;
+                    let validVerb = statement.verb && statement.verb.display && statement.verb.display['en-US'];
+                    if (!validVerb) {
+                        return;
+                    }
+
+                    let isCompleted = statement.verb.display['en-US'] === 'answered' ||
+                        statement.verb.display['en-US'] === 'completed';
+                    let isChild = statement.context && statement.context.contextActivities &&
+                        statement.context.contextActivities.parent &&
+                        statement.context.contextActivities.parent[0] &&
+                        statement.context.contextActivities.parent[0].id;
+
+                    // Store only completed root events.
+                    if (isCompleted && !isChild) {
+                        $.ajax({
+                            type: "POST",
+                            url: contentxResultSaveUrl,
+                            data: JSON.stringify(event.data.statement)
+                        });
+                    }
+                    // uncomment to see all xAPI events triggered by H5P content
+                    //console.log("xAPI event: ", event);
+                });
+
             });
         }
     };
 
     const h5pel = document.getElementById('h5p-' + args.player_id);
-    window.H5PPlayerXBlockPromises.push(h5pel);
+    window.H5PPlayerXBlockPromises.push(playerPromise(h5pel));
     window.H5PXBlockPlayersInitlized = false;
 
     $(function($) {
         if (!H5PXBlockPlayersInitlized) {
             window.H5PXBlockPlayersInitlized = true;
             window.H5PPlayerXBlockPromises.reduce(
-                (p, x) =>
-                p.then(_ => playerPromise(x)),
-                Promise.resolve()
-            )
-            H5P.externalDispatcher.on("xAPI", (event) => {
-
-                let hasStatement = event && event.data && event.data.statement;
-                if (!hasStatement) {
-                    return;
-                }
-
-                let statement = event.data.statement;
-                let validVerb = statement.verb && statement.verb.display && statement.verb.display['en-US'];
-                if (!validVerb) {
-                    return;
-                }
-
-                let isCompleted = statement.verb.display['en-US'] === 'answered' ||
-                    statement.verb.display['en-US'] === 'completed';
-                let isChild = statement.context && statement.context.contextActivities &&
-                    statement.context.contextActivities.parent &&
-                    statement.context.contextActivities.parent[0] &&
-                    statement.context.contextActivities.parent[0].id;
-
-                // Store only completed root events.
-                if (isCompleted && !isChild) {
-                    $.ajax({
-                        type: "POST",
-                        url: contentxResultSaveUrl,
-                        data: JSON.stringify(event.data.statement)
-                    });
-                }
-                // uncomment to see all xAPI events triggered by H5P content
-                //console.log("xAPI event: ", event);
-            });
+                function(prevPromise, curPromise) {
+                    return prevPromise.then(curPromise);
+                }, Promise.resolve()
+            );
         }
     });
 }
```

### Comparing `h5p-xblock-0.2.4/h5pxblock/static/js/src/studio.js` & `h5p-xblock-0.2.5/h5pxblock/static/js/src/studio.js`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/h5pxblock/utils.py` & `h5p-xblock-0.2.5/h5pxblock/utils.py`

 * *Files identical despite different names*

### Comparing `h5p-xblock-0.2.4/setup.py` & `h5p-xblock-0.2.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
                 data.append(os.path.relpath(os.path.join(dirname, fname), pkg))
 
     return {pkg: data}
 
 
 setup(
     name='h5p-xblock',
-    version='0.2.4',
+    version='0.2.5',
     description='XBlock to play self hosted h5p content inside open edX',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/edly-io/h5pxblock',
     license='MIT',
     author='edly',
     author_email='hello@edly.io',
```

