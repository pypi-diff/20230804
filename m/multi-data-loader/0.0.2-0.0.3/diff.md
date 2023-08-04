# Comparing `tmp/multi_data_loader-0.0.2.tar.gz` & `tmp/multi_data_loader-0.0.3.tar.gz`

## Comparing `multi_data_loader-0.0.2.tar` & `multi_data_loader-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,21 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/.DS_Store
--rw-r--r--   0        0        0      260 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/demo.py
--rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/.idea/.gitignore
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/.idea/workspace.xml
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/src/.DS_Store
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/src/multi_data_loader/.DS_Store
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/src/multi_data_loader/__init__.py
--rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/src/multi_data_loader/bases.py
--rw-r--r--   0        0        0    16102 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/src/multi_data_loader/data_loader.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/LICENSE
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/README.md
--rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      854 2020-02-02 00:00:00.000000 multi_data_loader-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.DS_Store
+-rw-r--r--   0        0        0      261 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/demo.py
+-rw-r--r--   0        0        0    54415 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/test.jpg
+-rw-r--r--   0        0        0      176 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/.gitignore
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/git_toolbox_prj.xml
+-rw-r--r--   0        0        0      201 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/misc.xml
+-rw-r--r--   0        0        0      286 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/modules.xml
+-rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/multi_data_loader.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/vcs.xml
+-rw-r--r--   0        0        0     7004 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/workspace.xml
+-rw-r--r--   0        0        0     2399 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/src/.DS_Store
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/src/multi_data_loader/.DS_Store
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/src/multi_data_loader/__init__.py
+-rw-r--r--   0        0        0      650 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/src/multi_data_loader/bases.py
+-rw-r--r--   0        0        0    16039 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/src/multi_data_loader/data_loader.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2570 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/README.md
+-rw-r--r--   0        0        0      629 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     3145 2020-02-02 00:00:00.000000 multi_data_loader-0.0.3/PKG-INFO
```

### Comparing `multi_data_loader-0.0.2/src/.DS_Store` & `multi_data_loader-0.0.3/src/.DS_Store`

 * *Files identical despite different names*

### Comparing `multi_data_loader-0.0.2/src/multi_data_loader/.DS_Store` & `multi_data_loader-0.0.3/src/multi_data_loader/.DS_Store`

 * *Files identical despite different names*

### Comparing `multi_data_loader-0.0.2/src/multi_data_loader/bases.py` & `multi_data_loader-0.0.3/src/multi_data_loader/bases.py`

 * *Files identical despite different names*

### Comparing `multi_data_loader-0.0.2/src/multi_data_loader/data_loader.py` & `multi_data_loader-0.0.3/src/multi_data_loader/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -379,14 +379,15 @@
                 break
 
             ret_val, frame = self.cap.read()
 
             self.count += 1
             ret_timestamp = int(self.timestamp)
             self.timestamp += 1000 / self.fps
+            frame_counter += 1
 
         im = Image.fromarray(frame)
 
         # im = image_resize(im)
         img_size = im.size
         res = np.array(im)
         if self.mode == 'BGR':
@@ -496,24 +497,22 @@
         try:
             while True:
                 raw_image = self.pipe.stdout.read(self.width * self.height * 3)  # 从管道里读取一帧，字节数为(宽*高*3)有三个通道
                 image = np.frombuffer(raw_image, dtype='uint8')  # 把读取到的二进制数据转换成numpy数组
                 if len(image) == 0:  # 如果全部读取完了就结束循环
                     break
                 image = image.reshape((self.height, self.width, 3))  # 把图像转变成应有形状
-                cv2.imwrite('img/%05d.jpg'%self.count, image)  # 用 cv2保存图像
+                # cv2.imwrite('img/%05d.jpg'%self.count, image)  # 用 cv2保存图像
                 self.pipe.stdout.flush()  # 充管道
                 self.count += 1
-                return image, self.timestamp
+                return image, self.timestamp, (self.width, self.height)
         except Exception as e:
             raise StopIteration
 
     def release(self):
         try:
             self.cap.release()
         except Exception as error:
             print(str(error))
 
 if __name__ == "__main__":
-    loader = UrlStreamLoader(path=[stream_url], mode="RGB", sample_rate=1)
-    for image, timestamp in loader:
-        print(image)
+    pass
```

### Comparing `multi_data_loader-0.0.2/LICENSE` & `multi_data_loader-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `multi_data_loader-0.0.2/pyproject.toml` & `multi_data_loader-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "multi_data_loader"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name = "KeleiJiang", email = "18852088031@gmail.com" },
 ]
 description = "Multi Data Loader"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

