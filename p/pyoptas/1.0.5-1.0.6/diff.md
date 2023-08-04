# Comparing `tmp/pyoptas-1.0.5.tar.gz` & `tmp/pyoptas-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyoptas-1.0.5.tar", last modified: Tue Jun  6 18:40:24 2023, max compression
+gzip compressed data, was "pyoptas-1.0.6.tar", last modified: Fri Aug  4 08:52:36 2023, max compression
```

## Comparing `pyoptas-1.0.5.tar` & `pyoptas-1.0.6.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.5/LICENSE
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-06-06 18:40:24.538715 pyoptas-1.0.5/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     9692 2023-05-25 12:18:16.000000 pyoptas-1.0.5/README.md
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/optas/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/__init__.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    22737 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    73477 2023-06-06 17:20:20.000000 pyoptas-1.0.5/optas/models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    22041 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    27279 2023-06-06 09:18:27.000000 pyoptas-1.0.5/optas/solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    12825 2023-06-06 17:20:20.000000 pyoptas-1.0.5/optas/spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     4556 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.5/optas/templates.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    43584 2023-05-26 13:04:31.000000 pyoptas-1.0.5/optas/visualize.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/pyoptas.egg-info/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/PKG-INFO
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/SOURCES.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/dependency_links.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/requires.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-06-06 18:40:24.000000 pyoptas-1.0.5/pyoptas.egg-info/top_level.txt
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-06-06 18:40:07.000000 pyoptas-1.0.5/pyproject.toml
--rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-06-06 18:40:24.538715 pyoptas-1.0.5/setup.cfg
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-06-06 18:40:07.000000 pyoptas-1.0.5/setup.py
-drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-06-06 18:40:24.538715 pyoptas-1.0.5/tests/
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_builder.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     2146 2023-05-25 15:59:54.000000 pyoptas-1.0.5/tests/test_examples.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    40304 2023-06-06 17:20:20.000000 pyoptas-1.0.5/tests/test_models.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_optas_utils.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    15344 2023-05-25 15:59:54.000000 pyoptas-1.0.5/tests/test_optimization.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     3115 2023-06-06 09:18:27.000000 pyoptas-1.0.5/tests/test_solver.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.5/tests/test_spatialmath.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/test_sx_container.py
--rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.5/tests/tester_robot_model.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-08-04 08:52:36.386491 pyoptas-1.0.6/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      583 2022-10-10 13:03:33.000000 pyoptas-1.0.6/LICENSE
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-08-04 08:52:36.386491 pyoptas-1.0.6/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     9692 2023-05-25 12:18:16.000000 pyoptas-1.0.6/README.md
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-08-04 08:52:36.386491 pyoptas-1.0.6/optas/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1194 2023-05-26 13:04:31.000000 pyoptas-1.0.6/optas/__init__.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    25557 2023-08-04 08:50:42.000000 pyoptas-1.0.6/optas/builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    73617 2023-08-03 17:58:48.000000 pyoptas-1.0.6/optas/models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    22041 2023-05-26 13:04:31.000000 pyoptas-1.0.6/optas/optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    27279 2023-06-06 09:18:27.000000 pyoptas-1.0.6/optas/solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    12825 2023-06-06 17:20:20.000000 pyoptas-1.0.6/optas/spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     4556 2023-05-26 13:04:31.000000 pyoptas-1.0.6/optas/sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    11538 2023-04-10 19:50:52.000000 pyoptas-1.0.6/optas/templates.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    43683 2023-08-04 07:59:12.000000 pyoptas-1.0.6/optas/visualize.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-08-04 08:52:36.386491 pyoptas-1.0.6/pyoptas.egg-info/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    10591 2023-08-04 08:52:36.000000 pyoptas-1.0.6/pyoptas.egg-info/PKG-INFO
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      586 2023-08-04 08:52:36.000000 pyoptas-1.0.6/pyoptas.egg-info/SOURCES.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        1 2023-08-04 08:52:36.000000 pyoptas-1.0.6/pyoptas.egg-info/dependency_links.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      152 2023-08-04 08:52:36.000000 pyoptas-1.0.6/pyoptas.egg-info/requires.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)        6 2023-08-04 08:52:36.000000 pyoptas-1.0.6/pyoptas.egg-info/top_level.txt
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      800 2023-08-04 08:50:42.000000 pyoptas-1.0.6/pyproject.toml
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)       38 2023-08-04 08:52:36.386491 pyoptas-1.0.6/setup.cfg
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1048 2023-08-04 08:50:42.000000 pyoptas-1.0.6/setup.py
+drwxrwxr-x   0 cm22      (1001) cm22      (1001)        0 2023-08-04 08:52:36.386491 pyoptas-1.0.6/tests/
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    16371 2023-03-07 17:13:56.000000 pyoptas-1.0.6/tests/test_builder.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     2282 2023-08-04 07:59:12.000000 pyoptas-1.0.6/tests/test_examples.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    40304 2023-06-06 17:20:20.000000 pyoptas-1.0.6/tests/test_models.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     5890 2023-03-07 17:13:56.000000 pyoptas-1.0.6/tests/test_optas_utils.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    15344 2023-05-25 15:59:54.000000 pyoptas-1.0.6/tests/test_optimization.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     3115 2023-06-06 09:18:27.000000 pyoptas-1.0.6/tests/test_solver.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)    17271 2023-04-10 19:50:52.000000 pyoptas-1.0.6/tests/test_spatialmath.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)     1773 2023-03-07 17:13:56.000000 pyoptas-1.0.6/tests/test_sx_container.py
+-rw-rw-r--   0 cm22      (1001) cm22      (1001)      874 2023-03-07 17:13:56.000000 pyoptas-1.0.6/tests/tester_robot_model.py
```

### Comparing `pyoptas-1.0.5/LICENSE` & `pyoptas-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/PKG-INFO` & `pyoptas-1.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.5
+Version: 1.0.6
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
```

### Comparing `pyoptas-1.0.5/README.md` & `pyoptas-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/__init__.py` & `pyoptas-1.0.6/optas/__init__.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/builder.py` & `pyoptas-1.0.6/optas/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -332,34 +332,94 @@
         @param rhs Right-hand side for the inequality constraint.
         """
         self.add_leq_inequality_constraint(name + "_l", lhs, mid)
         self.add_leq_inequality_constraint(name + "_r", mid, rhs)
 
     @arrayify_args
     def add_equality_constraint(
-        self, name: str, lhs: CasADiArrayType, rhs: Union[None, CasADiArrayType] = None
+        self,
+        name: str,
+        lhs: CasADiArrayType,
+        rhs: Union[None, CasADiArrayType] = None,
+        reduce_constraint=False,
     ) -> None:
         """! Add the equality constraint lhs == rhs to the optimization problem.
 
         @param name Name for the constraint.
         @param lhs Left-hand side for the inequality constraint.
         @param rhs Right-hand side for the inequality constraint. If None, then it is replaced with the zero array with the same shape as lhs.
+        @param reduce_constraint When True, the constraints are specified by ||lhs - rhs||^2 = 0. This has the effect of reducing the number of equality constraints in the problem. However, if the constraints are linear they will be treated as nonlinear. Default is False.
         """
         if rhs is None:
             rhs = cs.DM.zeros(*lhs.shape)
         diff = rhs - lhs  # diff == 0
+        if reduce_constraint:
+            diff = cs.sumsqr(diff)
         if self._is_linear_in_x(diff):
             self._lin_eq_constraints[name] = diff
         else:
             self._eq_constraints[name] = diff
 
     #
     # Common constraints
     #
 
+    def sphere_collision_avoidance_constraints(
+        self, name, obstacle_names, link_names=None, base_link=None
+    ) -> None:
+        """! Add collision avoidance constraints, based on spherical representations attached to the robot links and placed in the world.
+
+        @param name Name of the model.
+        @param obstacle_names A list of strings with names of obstacles. For each object, parameters will be created with labels NAME_position (size 3) and NAME_radii (size 1) that represent the obstacle position and radius respectively.
+        @param link_names The links you want to attach collision avoidance constraints onto; for each link a parameter is created with label NAME_radii (size 1). When None is passed, a sphere is attcahed to each link specified in the URDF.
+        @param base_link Name of the base frame link. When None is passed, the root link in the URDF is used.
+        """
+        # Get model
+        model = self.get_model(name)
+        assert isinstance(model, RobotModel), "this method only applies to robot models"
+
+        # Update base link
+        if base_link is None:
+            base_link = model.get_root_link()
+
+        # Get model states
+        Q = self.get_model_states(name)
+        n = Q.shape[1]
+
+        # Setup inks
+        if link_names is None:
+            link_names = model.link_names
+        assert len(link_names), "at least one link should be named"
+        links = {}
+        for name in link_names:
+            links[name] = (
+                model.get_link_position_function(name, base_link),
+                self.add_parameter(name + "_radii"),
+            )
+
+        # Setup obstacles
+        assert len(obstacle_names), "at least one obstacle should be named"
+        obstacles = {}
+        for name in obstacle_names:
+            obstacles[name] = (
+                self.add_parameter(name + "_position", 3),
+                self.add_parameter(name + "_radii"),
+            )
+
+        # Add constraints
+        for t in range(n):
+            q = Q[:, t]
+            for link_name, (pos, linkrad) in links.items():
+                p = pos(q)
+                for obs_name, (obs, obsrad) in obstacles.items():
+                    name = f"sphere_col_avoid_{t}_{link_name}_{obs_name}"
+                    dist2 = cs.sumsqr(p - obs)
+                    bnd2 = (linkrad + obsrad) ** 2
+                    self.add_leq_inequality_constraint(name, bnd2, dist2)
+
     def integrate_model_states(
         self, name: str, time_deriv: int, dt: CasADiArrayType
     ) -> None:
         """! Integrates the model states over time.
 
         @param name Name of the model.
         @param time_deriv The time-deriviative required (i.e. position is 0, velocity is 1, etc.).
```

### Comparing `pyoptas-1.0.5/optas/models.py` & `pyoptas-1.0.6/optas/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1219,60 +1219,60 @@
         """! Compute the geometric Jacobian matrix in the global frame.
 
         @param link Name of the end-effector link.
         @param q Joint position array.
         @return Geometric Jacobian.
         """
 
+        root = self.urdf.get_root()
+
         e = self.get_global_link_position(link, q)
 
-        w = cs.DM.zeros(3)
         pdot = cs.DM.zeros(3)
 
         joint_index_order = []
         jacobian_columns = []
 
-        past_in_chain = False
-
         for joint in self.urdf.joints:
+
             if joint.type == "fixed":
                 continue
 
-            if joint.child == link:
-                past_in_chain = True
-
             joint_index = self.get_actuated_joint_index(joint.name)
             joint_index_order.append(joint_index)
             qi = q[joint_index]
 
-            if past_in_chain:
-                jcol = cs.DM.zeros(6)
-                jacobian_columns.append(jcol)
-
-            elif joint.type in {"revolute", "continuous"}:
-                axis = self.get_joint_axis(joint)
-                R = self.get_global_link_rotation(joint.child, q)
-                R = R @ angvec2r(qi, axis)
-                p = self.get_global_link_position(joint.child, q)
+            if joint.name in self.urdf.get_chain(root, link, links=False):
+                # if joint in chain check type of join
+                if joint.type in {"revolute", "continuous"}:
+                    axis = self.get_joint_axis(joint)
+                    R = self.get_global_link_rotation(joint.child, q)
+                    R = R @ angvec2r(qi, axis)
+                    p = self.get_global_link_position(joint.child, q)
+
+                    z = R @ axis
+                    pdot = cs.cross(z, e - p)
+
+                    jcol = cs.vertcat(pdot, z)
+                    jacobian_columns.append(jcol)
+
+                elif joint.type == "prismatic":
+                    axis = self.get_joint_axis(joint)
+                    R = self.get_global_link_rotation(joint.child, q)
+                    z = R @ axis
+                    jcol = cs.vertcat(z, cs.DM.zeros(3))
+                    jacobian_columns.append(jcol)
 
-                z = R @ axis
-                pdot = cs.cross(z, e - p)
-
-                jcol = cs.vertcat(pdot, z)
-                jacobian_columns.append(jcol)
-
-            elif joint.type == "prismatic":
-                axis = self.get_joint_axis(joint)
-                R = self.get_global_link_rotation(joint.child, q)
-                z = R @ axis
-                jcol = cs.vertcat(z, cs.DM.zeros(3))
+                else:
+                    raise JointTypeNotSupported(joint.type)
+            else:
+                # if joint not in chain add zeros
+                jcol = cs.DM.zeros(6)
                 jacobian_columns.append(jcol)
 
-            else:
-                raise JointTypeNotSupported(joint.type)
 
         # Sort columns of jacobian
         jacobian_columns_ordered = [jacobian_columns[idx] for idx in joint_index_order]
 
         # Build jacoian array
         J = jacobian_columns_ordered.pop(0)
         while jacobian_columns_ordered:
```

### Comparing `pyoptas-1.0.5/optas/optimization.py` & `pyoptas-1.0.6/optas/optimization.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/solver.py` & `pyoptas-1.0.6/optas/solver.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/spatialmath.py` & `pyoptas-1.0.6/optas/spatialmath.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/sx_container.py` & `pyoptas-1.0.6/optas/sx_container.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/templates.py` & `pyoptas-1.0.6/optas/templates.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/optas/visualize.py` & `pyoptas-1.0.6/optas/visualize.py`

 * *Files 1% similar despite different names*

```diff
@@ -370,14 +370,16 @@
             alpha_max = alpha_spec.get("alpha_max", 1.0)
             alphas = [alpha_min] * (n - 1) + [alpha_max]
         elif alpha_spec["style"] == "C":
             alpha_start = alpha_spec.get("alpha_start", 1.0)
             alpha_mid = alpha_spec.get("alpha_mid", 0.1)
             alpha_end = alpha_spec.get("alpha_end", 1.0)
             alphas = [alpha_start] + [alpha_mid] * (n - 2) + [alpha_end]
+        elif alpha_spec['style'] == 'const':
+            alphas = [alpha_spec.get("alpha", 1.0)]*n
 
         sphere_traj = []
         if animate:
             self.actors.stop_adding_actors()
 
         actors = []
         for i, alpha in enumerate(alphas):
```

### Comparing `pyoptas-1.0.5/pyoptas.egg-info/PKG-INFO` & `pyoptas-1.0.6/pyoptas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyoptas
-Version: 1.0.5
+Version: 1.0.6
 Summary: An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.
 Home-page: https://github.com/cmower/optas
 Author: Christopher E. Mower
 Author-email: "Christopher E. Mower" <christopher.mower@kcl.ac.uk>
 License: Apache License, Version 2.0
 Project-URL: Homepage, https://cmower.github.io/optas/
 Project-URL: Documentation, https://cmower.github.io/optas/
```

### Comparing `pyoptas-1.0.5/pyoptas.egg-info/SOURCES.txt` & `pyoptas-1.0.6/pyoptas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/pyproject.toml` & `pyoptas-1.0.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyoptas"
-version = "1.0.5"
+version = "1.0.6"
 authors = [
   { name="Christopher E. Mower", email="christopher.mower@kcl.ac.uk" },
 ]
 description = "An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pyoptas-1.0.5/setup.py` & `pyoptas-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyoptas",
     description="An optimization-based task specification library for task and motion planning (TAMP), trajectory optimization, and model predictive control.",
-    version="1.0.5",
+    version="1.0.6",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/cmower/optas",
     project_urls={
         "Bug Tracker": "https://github.com/cmower/optas/issues",
     },
     author="Christopher E. Mower",
```

### Comparing `pyoptas-1.0.5/tests/test_builder.py` & `pyoptas-1.0.6/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_examples.py` & `pyoptas-1.0.6/tests/test_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,10 +85,15 @@
 
 
 def test_simple_joint_space_planner():
     main = load_main_function("simple_joint_space_planner.py")
     assert main(gui=False) == 0
 
 
+def test_sphere_collision_avoidance():
+    main = load_main_function("sphere_collision_avoidance.py")
+    assert main(vis=False) == 0
+
+
 # def test_example():
 #     path = examples_path / "example.py"
 #     module = import_module(path)
```

### Comparing `pyoptas-1.0.5/tests/test_models.py` & `pyoptas-1.0.6/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_optas_utils.py` & `pyoptas-1.0.6/tests/test_optas_utils.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_optimization.py` & `pyoptas-1.0.6/tests/test_optimization.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_solver.py` & `pyoptas-1.0.6/tests/test_solver.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_spatialmath.py` & `pyoptas-1.0.6/tests/test_spatialmath.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/test_sx_container.py` & `pyoptas-1.0.6/tests/test_sx_container.py`

 * *Files identical despite different names*

### Comparing `pyoptas-1.0.5/tests/tester_robot_model.py` & `pyoptas-1.0.6/tests/tester_robot_model.py`

 * *Files identical despite different names*

