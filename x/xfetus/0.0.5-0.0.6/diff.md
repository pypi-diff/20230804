# Comparing `tmp/xfetus-0.0.5.tar.gz` & `tmp/xfetus-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xfetus-0.0.5.tar", last modified: Sat Jul 15 21:58:27 2023, max compression
+gzip compressed data, was "xfetus-0.0.6.tar", last modified: Fri Aug  4 15:33:42 2023, max compression
```

## Comparing `xfetus-0.0.5.tar` & `xfetus-0.0.6.tar`

### file list

```diff
@@ -1,11 +1,14 @@
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 21:58:27.968436 xfetus-0.0.5/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6182 2023-07-15 21:58:27.968436 xfetus-0.0.5/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5481 2023-07-15 21:45:33.000000 xfetus-0.0.5/README.md
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     1037 2023-07-15 21:54:19.000000 xfetus-0.0.5/pyproject.toml
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       38 2023-07-15 21:58:27.968436 xfetus-0.0.5/setup.cfg
-drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-07-15 21:58:27.968436 xfetus-0.0.5/xfetus.egg-info/
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6182 2023-07-15 21:58:27.000000 xfetus-0.0.5/xfetus.egg-info/PKG-INFO
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      173 2023-07-15 21:58:27.000000 xfetus-0.0.5/xfetus.egg-info/SOURCES.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 21:58:27.000000 xfetus-0.0.5/xfetus.egg-info/dependency_links.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-07-15 21:58:27.000000 xfetus-0.0.5/xfetus.egg-info/requires.txt
--rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-07-15 21:58:27.000000 xfetus-0.0.5/xfetus.egg-info/top_level.txt
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-08-04 15:33:42.940049 xfetus-0.0.6/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     7233 2023-08-04 15:33:42.940049 xfetus-0.0.6/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     6565 2023-08-04 13:56:31.000000 xfetus-0.0.6/README.md
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       80 2023-08-04 15:33:32.000000 xfetus-0.0.6/pyproject.toml
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      900 2023-08-04 15:33:42.940049 xfetus-0.0.6/setup.cfg
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-08-04 15:33:42.940049 xfetus-0.0.6/xfetus/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       69 2023-07-15 21:45:33.000000 xfetus-0.0.6/xfetus/__init__.py
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     5567 2023-07-15 21:45:33.000000 xfetus-0.0.6/xfetus/xfetus.py
+drwxrwxr-x   0 mxochicale  (1000) mxochicale  (1000)        0 2023-08-04 15:33:42.940049 xfetus-0.0.6/xfetus.egg-info/
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)     7233 2023-08-04 15:33:42.000000 xfetus-0.0.6/xfetus.egg-info/PKG-INFO
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)      219 2023-08-04 15:33:42.000000 xfetus-0.0.6/xfetus.egg-info/SOURCES.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        1 2023-08-04 15:33:42.000000 xfetus-0.0.6/xfetus.egg-info/dependency_links.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)       35 2023-08-04 15:33:42.000000 xfetus-0.0.6/xfetus.egg-info/requires.txt
+-rw-rw-r--   0 mxochicale  (1000) mxochicale  (1000)        7 2023-08-04 15:33:42.000000 xfetus-0.0.6/xfetus.egg-info/top_level.txt
```

### Comparing `xfetus-0.0.5/PKG-INFO` & `xfetus-0.0.6/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xfetus
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python-based library for Synthesis of Ultrasound Fetal Imaging
-Author-email: Miguel Xochicale <your0@email.com>, Harvey Mannering <your1@email.com>, Sofía Miñano <your2@email.com>
+Author: Miguel Xochicale
 License: MIT
-Project-URL: homepage, https://github.com/budai4medtech/medisynth
+Project-URL: Source, https://github.com/budai4medtech/xfetus
+Project-URL: Tracker, https://github.com/budai4medtech/xfetus/issues
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # xfetus - library for synthesis of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning:
 [![PyPI version](https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/xfetus)
 
 xfetus is a python-based library to syntheses fetal ultrasound images using GAN, transformers and diffusion models.
@@ -97,22 +98,44 @@
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
+		<a href="https://github.com/seansunn"><img src="https://avatars1.githubusercontent.com/u/91659063?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Zhanxiang (Sean) Sun</b> </sub>        
+		</a>
+		<br />
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Research">  🔬 🤔  </a>
+	</td>
+	<!-- CONTRIBUTOR -->
+	<td align="center">
 		<a href="https://github.com/harveymannering"><img src="https://avatars1.githubusercontent.com/u/60523103?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Harvey Mannering</b> </sub>        
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
 	</td>
+    <!-- CONTRIBUTOR -->
+	<td align="center">
+		<!-- ADD GITHUB USERNAME AND HASH FOR GITHUB PHOTO -->
+		<a href="https://github.com/michellepi"><img src="https://avatars1.githubusercontent.com/u/57605186?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Michelle Iskandar</b> </sub>        
+		</a>
+		<br />
+			<!-- ADD GITHUB REPOSITORY AND PROJECT, TITLE AND EMOJIS -->
+            <a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Code">💻</a>
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Research">  🔬 🤔  </a>
+	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/budai4medtech"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
 			<br />
 			<sub><b>Miguel Xochicale</b></sub>          
 			<br />
 		</a>
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1 Name: xfetus Version: 0.0.5 Summary: Python-based library
-for Synthesis of Ultrasound Fetal Imaging Author-email: Miguel Xochicale
-email.com>, Harvey Mannering
-email.com>, SofÃ­a MiÃ±ano
-email.com> License: MIT Project-URL: homepage, https://github.com/
-budai4medtech/medisynth Keywords: artificial intelligence,diffusion models
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.11 Description-
-Content-Type: text/markdown # xfetus - library for synthesis of ultrasound
-fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning: [![PyPI version]
-(https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/xfetus) xfetus
-is a python-based library to syntheses fetal ultrasound images using GAN,
-transformers and diffusion models. It also includes methods to quantify the
-quality of synthesis (FID, PSNR, SSIM, and visual touring tests). ##
-Installation ``` $ pip install xfetus ``` You can develop locally: * Generate
-your SSH keys as suggested [here](https://docs.github.com/en/github/
+Metadata-Version: 2.1 Name: xfetus Version: 0.0.6 Summary: Python-based library
+for Synthesis of Ultrasound Fetal Imaging Author: Miguel Xochicale License: MIT
+Project-URL: Source, https://github.com/budai4medtech/xfetus Project-URL:
+Tracker, https://github.com/budai4medtech/xfetus/issues Keywords: artificial
+intelligence,diffusion models Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python :: 3 Requires-Python:
+>=3.11 Description-Content-Type: text/markdown # xfetus - library for synthesis
+of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning: [!
+[PyPI version](https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/
+xfetus) xfetus is a python-based library to syntheses fetal ultrasound images
+using GAN, transformers and diffusion models. It also includes methods to
+quantify the quality of synthesis (FID, PSNR, SSIM, and visual touring tests).
+## Installation ``` $ pip install xfetus ``` You can develop locally: *
+Generate your SSH keys as suggested [here](https://docs.github.com/en/github/
 authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-
 agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
 * Clone the repository by typing (or copying) the following line in a terminal
 at your selected path in your machine: ``` cd && mkdir -p $HOME/repositories/
 budai4medtech && cd $HOME/repositories/budai4medtech git clone git@github.com:
 budai4medtech/xfetus.git ``` ## References ### Presentation Good practices in
 AI/ML for Ultrasound Fetal Brain Imaging Synthesis Harvey Mannering, Sofia
@@ -45,14 +43,14 @@
 {iskandar2023realistic, author={ Michelle Iskandar and Harvey Mannering and
 Zhanxiang Sun and Jacqueline Matthew and Hamideh Kerdegari and Laura Peralta
 and Miguel Xochicale}, title={Towards Realistic Ultrasound Fetal Brain Imaging
 Synthesis}, year={2023}, eprint={2304.03941}, archivePrefix={arXiv},
 primaryClass={eess.IV} } ``` ## Contributors Thanks goes to all these people (
 [emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-                         Sofia_MiÃ±ano           Harvey_Mannering
- ADD_NAME_SURNAME                                                             Miguel_Xochicale
-                         ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
-     ð¬_ð¤
+                         Sofia_MiÃ±ano         Zhanxiang_(Sean)_Sun         Harvey_Mannering
+ ADD_NAME_SURNAME                                                                                        Michelle_Iskandar           Miguel_Xochicale
+                         ð» ð¬_ð�      ð» ð¬_ð�      ð» ð¬_ð�                                   ð» ð_ð§
+     ð¬_ð¤                                                                                     ð» ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `xfetus-0.0.5/README.md` & `xfetus-0.0.6/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -81,22 +81,44 @@
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
+		<a href="https://github.com/seansunn"><img src="https://avatars1.githubusercontent.com/u/91659063?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Zhanxiang (Sean) Sun</b> </sub>        
+		</a>
+		<br />
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Research">  🔬 🤔  </a>
+	</td>
+	<!-- CONTRIBUTOR -->
+	<td align="center">
 		<a href="https://github.com/harveymannering"><img src="https://avatars1.githubusercontent.com/u/60523103?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Harvey Mannering</b> </sub>        
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
 	</td>
+    <!-- CONTRIBUTOR -->
+	<td align="center">
+		<!-- ADD GITHUB USERNAME AND HASH FOR GITHUB PHOTO -->
+		<a href="https://github.com/michellepi"><img src="https://avatars1.githubusercontent.com/u/57605186?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Michelle Iskandar</b> </sub>        
+		</a>
+		<br />
+			<!-- ADD GITHUB REPOSITORY AND PROJECT, TITLE AND EMOJIS -->
+            <a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Code">💻</a>
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Research">  🔬 🤔  </a>
+	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/budai4medtech"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
 			<br />
 			<sub><b>Miguel Xochicale</b></sub>          
 			<br />
 		</a>
@@ -107,8 +129,8 @@
 </table>
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
 
 <!-- ALL-CONTRIBUTORS-LIST:END -->
 
 This work follows the [all-contributors](https://github.com/all-contributors/all-contributors) specification.  
-Contributions of any kind welcome!
+Contributions of any kind welcome!
```

#### html2text {}

```diff
@@ -35,14 +35,14 @@
 Iskandar and Harvey Mannering and Zhanxiang Sun and Jacqueline Matthew and
 Hamideh Kerdegari and Laura Peralta and Miguel Xochicale}, title={Towards
 Realistic Ultrasound Fetal Brain Imaging Synthesis}, year={2023}, eprint=
 {2304.03941}, archivePrefix={arXiv}, primaryClass={eess.IV} } ``` ##
 Contributors Thanks goes to all these people ([emoji key](https://
 allcontributors.org/docs/en/emoji-key)):
 
-                         Sofia_MiÃ±ano           Harvey_Mannering
- ADD_NAME_SURNAME                                                             Miguel_Xochicale
-                         ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
-     ð¬_ð¤
+                         Sofia_MiÃ±ano         Zhanxiang_(Sean)_Sun         Harvey_Mannering
+ ADD_NAME_SURNAME                                                                                        Michelle_Iskandar           Miguel_Xochicale
+                         ð» ð¬_ð�      ð» ð¬_ð�      ð» ð¬_ð�                                   ð» ð_ð§
+     ð¬_ð¤                                                                                     ð» ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

### Comparing `xfetus-0.0.5/xfetus.egg-info/PKG-INFO` & `xfetus-0.0.6/xfetus.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: xfetus
-Version: 0.0.5
+Version: 0.0.6
 Summary: Python-based library for Synthesis of Ultrasound Fetal Imaging
-Author-email: Miguel Xochicale <your0@email.com>, Harvey Mannering <your1@email.com>, Sofía Miñano <your2@email.com>
+Author: Miguel Xochicale
 License: MIT
-Project-URL: homepage, https://github.com/budai4medtech/medisynth
+Project-URL: Source, https://github.com/budai4medtech/xfetus
+Project-URL: Tracker, https://github.com/budai4medtech/xfetus/issues
 Keywords: artificial intelligence,diffusion models
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
 
 # xfetus - library for synthesis of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning:
 [![PyPI version](https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/xfetus)
 
 xfetus is a python-based library to syntheses fetal ultrasound images using GAN, transformers and diffusion models.
@@ -97,22 +98,44 @@
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=sfmig" title="Research">  🔬 🤔  </a>
 	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
+		<a href="https://github.com/seansunn"><img src="https://avatars1.githubusercontent.com/u/91659063?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Zhanxiang (Sean) Sun</b> </sub>        
+		</a>
+		<br />
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Code">💻</a> 
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=seansunn" title="Research">  🔬 🤔  </a>
+	</td>
+	<!-- CONTRIBUTOR -->
+	<td align="center">
 		<a href="https://github.com/harveymannering"><img src="https://avatars1.githubusercontent.com/u/60523103?v=4?s=100" width="100px;" alt=""/>
 		<br />
 			<sub> <b>Harvey Mannering</b> </sub>        
 		</a>
 		<br />
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Code">💻</a> 
 			<a href="https://github.com/budai4medtech/xfetus/commits?author=harveymannering" title="Research">  🔬 🤔  </a>
 	</td>
+    <!-- CONTRIBUTOR -->
+	<td align="center">
+		<!-- ADD GITHUB USERNAME AND HASH FOR GITHUB PHOTO -->
+		<a href="https://github.com/michellepi"><img src="https://avatars1.githubusercontent.com/u/57605186?v=4?s=100" width="100px;" alt=""/>
+		<br />
+			<sub> <b>Michelle Iskandar</b> </sub>        
+		</a>
+		<br />
+			<!-- ADD GITHUB REPOSITORY AND PROJECT, TITLE AND EMOJIS -->
+            <a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Code">💻</a>
+			<a href="https://github.com/budai4medtech/xfetus/commits?author=michellepi" title="Research">  🔬 🤔  </a>
+	</td>
 	<!-- CONTRIBUTOR -->
 	<td align="center">
 		<a href="https://github.com/budai4medtech"><img src="https://avatars1.githubusercontent.com/u/11370681?v=4?s=100" width="100px;" alt=""/>
 			<br />
 			<sub><b>Miguel Xochicale</b></sub>          
 			<br />
 		</a>
```

#### html2text {}

```diff
@@ -1,25 +1,23 @@
-Metadata-Version: 2.1 Name: xfetus Version: 0.0.5 Summary: Python-based library
-for Synthesis of Ultrasound Fetal Imaging Author-email: Miguel Xochicale
-email.com>, Harvey Mannering
-email.com>, SofÃ­a MiÃ±ano
-email.com> License: MIT Project-URL: homepage, https://github.com/
-budai4medtech/medisynth Keywords: artificial intelligence,diffusion models
-Classifier: Development Status :: 2 - Pre-Alpha Classifier: Intended Audience
-:: Developers Classifier: Topic :: Scientific/Engineering :: Artificial
-Intelligence Classifier: License :: OSI Approved :: MIT License Classifier:
-Programming Language :: Python :: 3.8 Requires-Python: >=3.11 Description-
-Content-Type: text/markdown # xfetus - library for synthesis of ultrasound
-fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning: [![PyPI version]
-(https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/xfetus) xfetus
-is a python-based library to syntheses fetal ultrasound images using GAN,
-transformers and diffusion models. It also includes methods to quantify the
-quality of synthesis (FID, PSNR, SSIM, and visual touring tests). ##
-Installation ``` $ pip install xfetus ``` You can develop locally: * Generate
-your SSH keys as suggested [here](https://docs.github.com/en/github/
+Metadata-Version: 2.1 Name: xfetus Version: 0.0.6 Summary: Python-based library
+for Synthesis of Ultrasound Fetal Imaging Author: Miguel Xochicale License: MIT
+Project-URL: Source, https://github.com/budai4medtech/xfetus Project-URL:
+Tracker, https://github.com/budai4medtech/xfetus/issues Keywords: artificial
+intelligence,diffusion models Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Intended Audience :: Developers Classifier: Topic :: Scientific/
+Engineering :: Artificial Intelligence Classifier: License :: OSI Approved ::
+MIT License Classifier: Programming Language :: Python :: 3 Requires-Python:
+>=3.11 Description-Content-Type: text/markdown # xfetus - library for synthesis
+of ultrasound fetal imaging (:baby: :brain: :robot:) :warning: WIP :warning: [!
+[PyPI version](https://badge.fury.io/py/xfetus.svg)](https://badge.fury.io/py/
+xfetus) xfetus is a python-based library to syntheses fetal ultrasound images
+using GAN, transformers and diffusion models. It also includes methods to
+quantify the quality of synthesis (FID, PSNR, SSIM, and visual touring tests).
+## Installation ``` $ pip install xfetus ``` You can develop locally: *
+Generate your SSH keys as suggested [here](https://docs.github.com/en/github/
 authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-
 agent) (or [here](https://github.com/mxochicale/tools/blob/main/github/SSH.md))
 * Clone the repository by typing (or copying) the following line in a terminal
 at your selected path in your machine: ``` cd && mkdir -p $HOME/repositories/
 budai4medtech && cd $HOME/repositories/budai4medtech git clone git@github.com:
 budai4medtech/xfetus.git ``` ## References ### Presentation Good practices in
 AI/ML for Ultrasound Fetal Brain Imaging Synthesis Harvey Mannering, Sofia
@@ -45,14 +43,14 @@
 {iskandar2023realistic, author={ Michelle Iskandar and Harvey Mannering and
 Zhanxiang Sun and Jacqueline Matthew and Hamideh Kerdegari and Laura Peralta
 and Miguel Xochicale}, title={Towards Realistic Ultrasound Fetal Brain Imaging
 Synthesis}, year={2023}, eprint={2304.03941}, archivePrefix={arXiv},
 primaryClass={eess.IV} } ``` ## Contributors Thanks goes to all these people (
 [emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
-                         Sofia_MiÃ±ano           Harvey_Mannering
- ADD_NAME_SURNAME                                                             Miguel_Xochicale
-                         ð» ð¬_ð�      ð» ð¬_ð�       ð» ð_ð§
-     ð¬_ð¤
+                         Sofia_MiÃ±ano         Zhanxiang_(Sean)_Sun         Harvey_Mannering
+ ADD_NAME_SURNAME                                                                                        Michelle_Iskandar           Miguel_Xochicale
+                         ð» ð¬_ð�      ð» ð¬_ð�      ð» ð¬_ð�                                   ð» ð_ð§
+     ð¬_ð¤                                                                                     ð» ð¬_ð¤
    This work follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome!
```

