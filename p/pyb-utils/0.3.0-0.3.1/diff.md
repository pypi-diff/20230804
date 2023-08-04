# Comparing `tmp/pyb_utils-0.3.0.tar.gz` & `tmp/pyb_utils-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyb_utils-0.3.0.tar", max compression
+gzip compressed data, was "pyb_utils-0.3.1.tar", max compression
```

## Comparing `pyb_utils-0.3.0.tar` & `pyb_utils-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.3.0/LICENSE
--rw-r--r--   0        0        0     4155 2023-07-14 19:56:54.274466 pyb_utils-0.3.0/README.md
--rw-r--r--   0        0        0      483 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/__init__.py
--rw-r--r--   0        0        0     8890 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/bodies.py
--rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.3.0/pyb_utils/camera.py
--rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/collision.py
--rw-r--r--   0        0        0     1417 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/frame.py
--rw-r--r--   0        0        0     4742 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/ghost.py
--rw-r--r--   0        0        0      729 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/math.py
--rw-r--r--   0        0        0     2430 2023-07-14 19:47:26.213579 pyb_utils-0.3.0/pyb_utils/named_tuples.py
--rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.3.0/pyb_utils/robots.py
--rw-r--r--   0        0        0      598 2023-07-14 19:47:58.273625 pyb_utils-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     5130 1970-01-01 00:00:00.000000 pyb_utils-0.3.0/setup.py
--rw-r--r--   0        0        0     5014 1970-01-01 00:00:00.000000 pyb_utils-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-03-01 18:44:35.352445 pyb_utils-0.3.1/LICENSE
+-rw-r--r--   0        0        0     4159 2023-07-16 20:07:46.739649 pyb_utils-0.3.1/README.md
+-rw-r--r--   0        0        0      483 2023-07-14 19:47:26.213579 pyb_utils-0.3.1/pyb_utils/__init__.py
+-rw-r--r--   0        0        0     8890 2023-07-14 19:47:26.213579 pyb_utils-0.3.1/pyb_utils/bodies.py
+-rw-r--r--   0        0        0     8332 2023-03-01 18:44:35.352445 pyb_utils-0.3.1/pyb_utils/camera.py
+-rw-r--r--   0        0        0     4587 2023-03-01 18:44:35.356445 pyb_utils-0.3.1/pyb_utils/collision.py
+-rw-r--r--   0        0        0     1417 2023-07-14 19:47:26.213579 pyb_utils-0.3.1/pyb_utils/frame.py
+-rw-r--r--   0        0        0     4742 2023-07-14 19:47:26.213579 pyb_utils-0.3.1/pyb_utils/ghost.py
+-rw-r--r--   0        0        0      710 2023-07-16 20:35:35.956167 pyb_utils-0.3.1/pyb_utils/math.py
+-rw-r--r--   0        0        0     2769 2023-08-04 19:40:41.406979 pyb_utils-0.3.1/pyb_utils/named_tuples.py
+-rw-r--r--   0        0        0      881 2023-03-01 18:44:35.356445 pyb_utils-0.3.1/pyb_utils/robots.py
+-rw-r--r--   0        0        0      598 2023-08-04 19:41:33.967131 pyb_utils-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     5134 1970-01-01 00:00:00.000000 pyb_utils-0.3.1/setup.py
+-rw-r--r--   0        0        0     5018 1970-01-01 00:00:00.000000 pyb_utils-0.3.1/PKG-INFO
```

### Comparing `pyb_utils-0.3.0/LICENSE` & `pyb_utils-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/README.md` & `pyb_utils-0.3.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # create a 1x1x1 cube at the origin
 >>> box = pyb_utils.BulletBody.box(position=[0, 0, 0], half_extents=[0.5, 0.5, 0.5])
 
 # put a ball on top
 >>> ball = pyb_utils.BulletBody.sphere(position=[0, 0, 1.5], radius=0.5)
 
 # now put it somewhere else
-ball.set_pose(position=[2, 0, 0.5])
+>>> ball.set_pose(position=[2, 0, 0.5])
 ```
 
 Third, we wrap some PyBullet functions to return *named* tuples, rather than
 normal tuples. When the tuples have 10+ fields in them, it is rather helpful to
 have names! The names and parameters of these functions are exactly the same as
 the underlying PyBullet ones, to make swapping effortless. Continuing our
 previous example:
```

### Comparing `pyb_utils-0.3.0/pyb_utils/bodies.py` & `pyb_utils-0.3.1/pyb_utils/bodies.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyb_utils/camera.py` & `pyb_utils-0.3.1/pyb_utils/camera.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyb_utils/collision.py` & `pyb_utils-0.3.1/pyb_utils/collision.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyb_utils/frame.py` & `pyb_utils-0.3.1/pyb_utils/frame.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyb_utils/ghost.py` & `pyb_utils-0.3.1/pyb_utils/ghost.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyb_utils/math.py` & `pyb_utils-0.3.1/pyb_utils/math.py`

 * *Files 16% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 def matrix_to_quaternion(C):
     """Convert rotation matrix C to quaternion."""
     return r2q(C, order=QUAT_ORDER)
 
 
 def quaternion_multiply(q0, q1, normalize=True):
     """Hamilton product of two quaternions."""
-    order = "xyzs"
     if normalize:
         q0 = qunit(q0)
         q1 = qunit(q1)
     C0 = quaternion_to_matrix(q0)
     C1 = quaternion_to_matrix(q1)
     return matrix_to_quaternion(C0 @ C1)
```

### Comparing `pyb_utils-0.3.0/pyb_utils/named_tuples.py` & `pyb_utils-0.3.1/pyb_utils/named_tuples.py`

 * *Files 20% similar despite different names*

```diff
@@ -67,33 +67,49 @@
         "erp",
     ],
 )
 
 
 def getDynamicsInfo(bodyUniqueId, linkIndex, physicsClientId=0):
     return DynamicsInfo(
-        *pyb.getDynamicsInfo(bodyUniqueId, linkIndex, physicsClientId)
+        *pyb.getDynamicsInfo(
+            bodyUniqueId=bodyUniqueId,
+            linkIndex=linkIndex,
+            physicsClientId=physicsClientId,
+        )
     )
 
 
 def getContactPoints(
     bodyA=-1, bodyB=-1, linkIndexA=-2, linkIndexB=-2, physicsClientId=0
 ):
     points_raw = pyb.getContactPoints(
-        bodyA, bodyB, linkIndexA, linkIndexB, physicsClientId
+        bodyA=bodyA,
+        bodyB=bodyB,
+        linkIndexA=linkIndexA,
+        linkIndexB=linkIndexB,
+        physicsClientId=physicsClientId,
     )
     return [ContactPoint(*point) for point in points_raw]
 
 
 def getClosestPoints(
     bodyA, bodyB, distance, linkIndexA=-2, linkIndexB=-2, physicsClientId=0
 ):
     points_raw = pyb.getClosestPoints(
-        bodyA, bodyB, distance, linkIndexA, linkIndexB, physicsClientId
+        bodyA=bodyA,
+        bodyB=bodyB,
+        distance=distance,
+        linkIndexA=linkIndexA,
+        linkIndexB=linkIndexB,
+        physicsClientId=physicsClientId,
     )
     return [ContactPoint(*point) for point in points_raw]
 
 
 def getConstraintInfo(constraintUniqueId, physicsClientId=0):
     return ConstraintInfo(
-        *pyb.getConstraintInfo(constraintUniqueId, physicsClientId)
+        *pyb.getConstraintInfo(
+            constraintUniqueId=constraintUniqueId,
+            physicsClientId=physicsClientId,
+        )
     )
```

### Comparing `pyb_utils-0.3.0/pyb_utils/robots.py` & `pyb_utils-0.3.1/pyb_utils/robots.py`

 * *Files identical despite different names*

### Comparing `pyb_utils-0.3.0/pyproject.toml` & `pyb_utils-0.3.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 line-length = 80
 
 [tool.poetry]
 name = "pyb_utils"
-version = "0.3.0"
+version = "0.3.1"
 description = "Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras."
 authors = ["Adam Heins <mail@adamheins.com>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.11"
```

### Comparing `pyb_utils-0.3.0/setup.py` & `pyb_utils-0.3.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,17 +13,17 @@
  'numpy>=1.21.5,<2.0.0',
  'opencv-python>=4.5.5,<5.0.0',
  'pybullet>=3.2.1,<4.0.0',
  'spatialmath-python>=1.0.0']
 
 setup_kwargs = {
     'name': 'pyb-utils',
-    'version': '0.3.0',
+    'version': '0.3.1',
     'description': 'Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras.',
-    'long_description': "# pyb_utils: utilities for PyBullet\n\nThis is a collection of utilities I've found useful for working with PyBullet,\nincluding:\n* Collision detection: conveniently set up shortest distance computations and\n  collision checking between arbitrary objects in arbitrary configurations with\n  PyBullet. See the accompanying [blog post](https://adamheins.com/blog/collision-detection-pybullet).\n* Ghost objects: add purely visual objects to the simulation, optionally\n  attached to another body.\n* Camera: virtual camera from which to get RGBA, depth, segmentation, and point\n  cloud data. Also provides video recording using OpenCV.\n* Convenience class for easily creating rigid bodies.\n* Versions of some PyBullet functions that return *named* tuples, for easy\n  field access.\n* Basic quaternion functions.\n\n## Install and run\nThis package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,\n18.04, and 20.04.\n\n### From pip\n```\npip install pyb_utils\n```\n\n### From source\nClone the repo:\n```bash\ngit clone https://github.com/adamheins/pyb_utils\ncd pyb_utils\n```\n\nInstall using [poetry](https://python-poetry.org/):\n```bash\npoetry install\npoetry run python examples/collision_detection_example.py  # for example\n```\n\nOr using pip:\n```bash\npython -m pip install .\n```\n\n## Usage and examples\nThis package provides a few basic quality of life utilities. First, PyBullet\nrepresents rotations using quaternions (in `[x, y, z, w]` order). We provide a\nfew helper routines to convert to rotation matrices and rotate points (using\n[spatialmath](https://github.com/bdaiinstitute/spatialmath-python) under the\nhood):\n```python\n>>> import pyb_utils\n>>> q = (0, 0, np.sqrt(2) / 2, np.sqrt(2) / 2)  # 90 deg rotation about z-axis\n\n>>> pyb_utils.quaternion_to_matrix(q)  # convert to rotation matrix\narray([[ 1.,  0.,  0.],\n       [ 0., -0., -1.],\n       [ 0.,  1., -0.]])\n\n>>> pyb_utils.quaternion_multiply(q, q)  # rotate two quaternions together\narray([0, 0, -1, 0])                     # 180 deg rotate about z\n\n>>> pyb_utils.quaternion_rotate(q, [1, 0, 0])  # rotate a point\narray([0, 1, 0])\n```\n\nSecond, we provide a simple class to quickly create rigid bodies\nprogrammatically, which is useful for adding basic objects to manipulate or act\nas obstacles:\n```python\n>>> import pybullet as pyb\n>>> import pyb_utils\n\n>>> pyb.connect(pyb.GUI)\n\n# create a 1x1x1 cube at the origin\n>>> box = pyb_utils.BulletBody.box(position=[0, 0, 0], half_extents=[0.5, 0.5, 0.5])\n\n# put a ball on top\n>>> ball = pyb_utils.BulletBody.sphere(position=[0, 0, 1.5], radius=0.5)\n\n# now put it somewhere else\nball.set_pose(position=[2, 0, 0.5])\n```\n\nThird, we wrap some PyBullet functions to return *named* tuples, rather than\nnormal tuples. When the tuples have 10+ fields in them, it is rather helpful to\nhave names! The names and parameters of these functions are exactly the same as\nthe underlying PyBullet ones, to make swapping effortless. Continuing our\nprevious example:\n```python\n# built-in PyBullet method\n# the output is not easy to read!\n>>> pyb.getDynamicsInfo(box.uid, -1)\n(1.0,\n 0.5,\n (0.16666666666666666, 0.16666666666666666, 0.16666666666666666),\n (0.0, 0.0, 0.0),\n (0.0, 0.0, 0.0, 1.0),\n 0.0,\n 0.0,\n 0.0,\n -1.0,\n -1.0,\n 2,\n 0.001)\n\n# switch to the pyb_utils version\n# now we can access fields by name\n>>> info = pyb_utils.getDynamicsInfo(box.uid, -1)\n>>> info.mass\n1.0\n>>> info.localInertiaPos\n(0.0, 0.0, 0.0)\n```\n\nAnd there's more! You can find example scripts of all of this package's\nutilities in the `examples/` directory:\n\n* [rigid bodies](examples/bodies_example.py)\n* [camera](examples/camera_example.py)\n* [collision detection](examples/collision_detection_example.py)\n* [ghost objects](examples/ghost_object_example.py)\n* [named tuples](examples/named_tuples_example.py)\n* [video](examples/video_example.py)\n\n## Known issues\nFeel free to open issues (or better yet, a pull request!) if you find a\nproblem. Currently known issues:\n\n* Video recording does not output MP4 videos correctly. The AVI format works,\n  however.\n* Ghost objects sometimes flicker (spooky, but undesirable).\n\n## License\n[MIT](https://github.com/adamheins/pyb_utils/blob/main/LICENSE)\n",
+    'long_description': "# pyb_utils: utilities for PyBullet\n\nThis is a collection of utilities I've found useful for working with PyBullet,\nincluding:\n* Collision detection: conveniently set up shortest distance computations and\n  collision checking between arbitrary objects in arbitrary configurations with\n  PyBullet. See the accompanying [blog post](https://adamheins.com/blog/collision-detection-pybullet).\n* Ghost objects: add purely visual objects to the simulation, optionally\n  attached to another body.\n* Camera: virtual camera from which to get RGBA, depth, segmentation, and point\n  cloud data. Also provides video recording using OpenCV.\n* Convenience class for easily creating rigid bodies.\n* Versions of some PyBullet functions that return *named* tuples, for easy\n  field access.\n* Basic quaternion functions.\n\n## Install and run\nThis package requires **Python 3.7+**. It has been tested on Ubuntu 16.04,\n18.04, and 20.04.\n\n### From pip\n```\npip install pyb_utils\n```\n\n### From source\nClone the repo:\n```bash\ngit clone https://github.com/adamheins/pyb_utils\ncd pyb_utils\n```\n\nInstall using [poetry](https://python-poetry.org/):\n```bash\npoetry install\npoetry run python examples/collision_detection_example.py  # for example\n```\n\nOr using pip:\n```bash\npython -m pip install .\n```\n\n## Usage and examples\nThis package provides a few basic quality of life utilities. First, PyBullet\nrepresents rotations using quaternions (in `[x, y, z, w]` order). We provide a\nfew helper routines to convert to rotation matrices and rotate points (using\n[spatialmath](https://github.com/bdaiinstitute/spatialmath-python) under the\nhood):\n```python\n>>> import pyb_utils\n>>> q = (0, 0, np.sqrt(2) / 2, np.sqrt(2) / 2)  # 90 deg rotation about z-axis\n\n>>> pyb_utils.quaternion_to_matrix(q)  # convert to rotation matrix\narray([[ 1.,  0.,  0.],\n       [ 0., -0., -1.],\n       [ 0.,  1., -0.]])\n\n>>> pyb_utils.quaternion_multiply(q, q)  # rotate two quaternions together\narray([0, 0, -1, 0])                     # 180 deg rotate about z\n\n>>> pyb_utils.quaternion_rotate(q, [1, 0, 0])  # rotate a point\narray([0, 1, 0])\n```\n\nSecond, we provide a simple class to quickly create rigid bodies\nprogrammatically, which is useful for adding basic objects to manipulate or act\nas obstacles:\n```python\n>>> import pybullet as pyb\n>>> import pyb_utils\n\n>>> pyb.connect(pyb.GUI)\n\n# create a 1x1x1 cube at the origin\n>>> box = pyb_utils.BulletBody.box(position=[0, 0, 0], half_extents=[0.5, 0.5, 0.5])\n\n# put a ball on top\n>>> ball = pyb_utils.BulletBody.sphere(position=[0, 0, 1.5], radius=0.5)\n\n# now put it somewhere else\n>>> ball.set_pose(position=[2, 0, 0.5])\n```\n\nThird, we wrap some PyBullet functions to return *named* tuples, rather than\nnormal tuples. When the tuples have 10+ fields in them, it is rather helpful to\nhave names! The names and parameters of these functions are exactly the same as\nthe underlying PyBullet ones, to make swapping effortless. Continuing our\nprevious example:\n```python\n# built-in PyBullet method\n# the output is not easy to read!\n>>> pyb.getDynamicsInfo(box.uid, -1)\n(1.0,\n 0.5,\n (0.16666666666666666, 0.16666666666666666, 0.16666666666666666),\n (0.0, 0.0, 0.0),\n (0.0, 0.0, 0.0, 1.0),\n 0.0,\n 0.0,\n 0.0,\n -1.0,\n -1.0,\n 2,\n 0.001)\n\n# switch to the pyb_utils version\n# now we can access fields by name\n>>> info = pyb_utils.getDynamicsInfo(box.uid, -1)\n>>> info.mass\n1.0\n>>> info.localInertiaPos\n(0.0, 0.0, 0.0)\n```\n\nAnd there's more! You can find example scripts of all of this package's\nutilities in the `examples/` directory:\n\n* [rigid bodies](examples/bodies_example.py)\n* [camera](examples/camera_example.py)\n* [collision detection](examples/collision_detection_example.py)\n* [ghost objects](examples/ghost_object_example.py)\n* [named tuples](examples/named_tuples_example.py)\n* [video](examples/video_example.py)\n\n## Known issues\nFeel free to open issues (or better yet, a pull request!) if you find a\nproblem. Currently known issues:\n\n* Video recording does not output MP4 videos correctly. The AVI format works,\n  however.\n* Ghost objects sometimes flicker (spooky, but undesirable).\n\n## License\n[MIT](https://github.com/adamheins/pyb_utils/blob/main/LICENSE)\n",
     'author': 'Adam Heins',
     'author_email': 'mail@adamheins.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `pyb_utils-0.3.0/PKG-INFO` & `pyb_utils-0.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyb-utils
-Version: 0.3.0
+Version: 0.3.1
 Summary: Basic utilities for PyBullet, including collision detection, ghost (i.e. visual-only) objects, and cameras.
 License: MIT
 Author: Adam Heins
 Author-email: mail@adamheins.com
 Requires-Python: >=3.7,<3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -97,15 +97,15 @@
 # create a 1x1x1 cube at the origin
 >>> box = pyb_utils.BulletBody.box(position=[0, 0, 0], half_extents=[0.5, 0.5, 0.5])
 
 # put a ball on top
 >>> ball = pyb_utils.BulletBody.sphere(position=[0, 0, 1.5], radius=0.5)
 
 # now put it somewhere else
-ball.set_pose(position=[2, 0, 0.5])
+>>> ball.set_pose(position=[2, 0, 0.5])
 ```
 
 Third, we wrap some PyBullet functions to return *named* tuples, rather than
 normal tuples. When the tuples have 10+ fields in them, it is rather helpful to
 have names! The names and parameters of these functions are exactly the same as
 the underlying PyBullet ones, to make swapping effortless. Continuing our
 previous example:
```

