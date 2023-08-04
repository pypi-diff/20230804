# Comparing `tmp/plbm_liumou_stable-1.3.9.tar.gz` & `tmp/plbm_liumou_stable-1.4.0.tar.gz`

## Comparing `plbm_liumou_stable-1.3.9.tar` & `plbm_liumou_stable-1.4.0.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/DemoModule.py
--rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/UploadToPypi.py
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/demo.py
--rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/install.py
--rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/req.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/requirements.txt
--rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/demo/package.py
--rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/disk/DiskInformation.py
--rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/file/7z.py
--rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/file/Rename.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/docker.py
--rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/install_pac_list.py
--rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/package.py
--rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/pacman.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/pip.py
--rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/model/source.py
--rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/network/ReplaceIP.py
--rw-r--r--   0        0        0     5547 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/AptManage.py
--rw-r--r--   0        0        0     7108 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Cmd.py
--rw-r--r--   0        0        0     2153 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Docker.py
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Dpkg.py
--rw-r--r--   0        0        0     3088 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/FileManagement.py
--rw-r--r--   0        0        0     6198 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Iptables.py
--rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Jurisdiction.py
--rw-r--r--   0        0        0    10656 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetManagement.py
--rw-r--r--   0        0        0     7160 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetStatus.py
--rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/OsInfo.py
--rw-r--r--   0        0        0     4352 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Package.py
--rw-r--r--   0        0        0     5357 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/README.md
--rw-r--r--   0        0        0     4424 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Service.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Source.py
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Yum.py
--rw-r--r--   0        0        0     1310 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/__init__.py
--rw-r--r--   0        0        0      488 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/base.py
--rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/get.py
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/logger.py
--rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/requirements.txt
--rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/txt.log
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/__init__.py
--rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/firewalld.py
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/.gitignore
--rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/LICENSE
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/README.md
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/pyproject.toml
--rw-r--r--   0        0        0     6111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.3.9/PKG-INFO
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/DemoModule.py
+-rw-r--r--   0        0        0     2906 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/UploadToPypi.py
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/demo.py
+-rw-r--r--   0        0        0     1111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/install.py
+-rw-r--r--   0        0        0       67 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/req.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/requirements.txt
+-rw-r--r--   0        0        0      943 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/demo/package.py
+-rw-r--r--   0        0        0     1922 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/disk/DiskInformation.py
+-rw-r--r--   0        0        0     5614 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/file/7z.py
+-rw-r--r--   0        0        0     4051 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/file/Rename.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/docker.py
+-rw-r--r--   0        0        0      641 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/install_pac_list.py
+-rw-r--r--   0        0        0    10191 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/package.py
+-rw-r--r--   0        0        0     1027 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/pacman.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/pip.py
+-rw-r--r--   0        0        0     2546 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/model/source.py
+-rw-r--r--   0        0        0     6563 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/network/ReplaceIP.py
+-rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/AptManage.py
+-rw-r--r--   0        0        0     7111 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Cmd.py
+-rw-r--r--   0        0        0     2180 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Docker.py
+-rw-r--r--   0        0        0     5046 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Dpkg.py
+-rw-r--r--   0        0        0     6210 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Iptables.py
+-rw-r--r--   0        0        0     3515 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Jurisdiction.py
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NewFileManagement.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NewNetStatus.py
+-rw-r--r--   0        0        0    11543 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NmcliManger.py
+-rw-r--r--   0        0        0     2039 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/OsInfo.py
+-rw-r--r--   0        0        0     4376 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Package.py
+-rw-r--r--   0        0        0     5355 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/README.md
+-rw-r--r--   0        0        0     4433 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Service.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Source.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Yum.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/__init__.py
+-rw-r--r--   0        0        0      492 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/base.py
+-rw-r--r--   0        0        0     1335 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/get.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/logger.py
+-rw-r--r--   0        0        0       12 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/requirements.txt
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/txt.log
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/security/__init__.py
+-rw-r--r--   0        0        0     2103 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/security/firewalld.py
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/.gitignore
+-rw-r--r--   0        0        0    11558 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/LICENSE
+-rw-r--r--   0        0        0     5418 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/README.md
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6122 2020-02-02 00:00:00.000000 plbm_liumou_stable-1.4.0/PKG-INFO
```

### Comparing `plbm_liumou_stable-1.3.9/DemoModule.py` & `plbm_liumou_stable-1.4.0/DemoModule.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/UploadToPypi.py` & `plbm_liumou_stable-1.4.0/UploadToPypi.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/demo.py` & `plbm_liumou_stable-1.4.0/demo.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 	def __init__(self):
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def get(self):
 		try:
 			n = NetManagement()
 			self.logger.info("开始测试获取连接信息")
-			u = n.GetConInfo(con="wifi")
+			u = n.get_con_info(con="wifi")
 			if u["status"]:
 				print("获取成功")
 				print(u)
 			else:
 				print("获取失败")
 			self.logger.info("测试成功")
 		except Exception as e:
```

### Comparing `plbm_liumou_stable-1.3.9/install.py` & `plbm_liumou_stable-1.4.0/install.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/demo/package.py` & `plbm_liumou_stable-1.4.0/demo/package.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 @Time    :   2022-10-24 22:45
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from src.plbm_liumou_Stable import PackageManagement
+from src.plbm_liumou_Stable import NewPackageManagement
 from ColorInfo import ColorLogger
 
 
 class ServiceManager:
 	def __init__(self, pac, password):
 		self.package = pac
-		self.pac = PackageManagement(password=password, package="vsftpd")
+		self.pac = NewPackageManagement(password=password, package="vsftpd")
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def remove(self):
 		if self.pac.installed():
 			self.logger.info(f"已安装: {self.package}")
 			if self.pac.uninstall():
 				self.logger.info(f"卸载成功: {self.package}")
```

### Comparing `plbm_liumou_stable-1.3.9/disk/DiskInformation.py` & `plbm_liumou_stable-1.4.0/disk/DiskInformation.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/file/7z.py` & `plbm_liumou_stable-1.4.0/file/7z.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/file/Rename.py` & `plbm_liumou_stable-1.4.0/file/Rename.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/docker.py` & `plbm_liumou_stable-1.4.0/model/docker.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/install_pac_list.py` & `plbm_liumou_stable-1.4.0/model/install_pac_list.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/package.py` & `plbm_liumou_stable-1.4.0/model/package.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/pacman.py` & `plbm_liumou_stable-1.4.0/model/pacman.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/pip.py` & `plbm_liumou_stable-1.4.0/model/pip.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/model/source.py` & `plbm_liumou_stable-1.4.0/model/source.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/network/ReplaceIP.py` & `plbm_liumou_stable-1.4.0/network/ReplaceIP.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/AptManage.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/AptManage.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 @Time    :   2022-09-05 09:17
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from .Cmd import Command
+from .Cmd import NewCommand
 from .logger import ColorLogger
 from .Jurisdiction import Jurisdiction
 from os import path
 
 
-class AptManagement:
+class NewAptManagement:
 	def __init__(self, password, log=False, terminal=False, package=None, file=None):
 		"""
 		Apt 管理
 		:param password: 主机密码
 		:param log: 是否启用日志
 		:param terminal: 是否使用终端执行命令(针对个别Linux发行部才起作用)
 		:param package: 包名
@@ -26,15 +26,15 @@
 		self.package = package
 		self.terminal = terminal
 		self.log = log
 		self.password = password
 		ju = Jurisdiction(passwd=password, log_file=file)
 		if not ju.verification(name='AptManagement'):
 			exit(1)
-		self.cmd = Command(password=self.password, cmd='which apt', terminal=self.terminal, logs=self.log)
+		self.cmd = NewCommand(password=self.password, cmd='which apt', terminal=self.terminal, logs=self.log)
 		self.logger = ColorLogger(file=file, txt=log, class_name=self.__class__.__name__)
 		# 需要处理的包文件列表
 		self.deb_pac_list = []
 		# 实际存在的包文件列表
 		self.deb_ok_list = []
 		# 不存在的包文件列表
 		self.deb_not_exists = []
@@ -150,15 +150,15 @@
 		"""
 		self.deb_install_str = ''
 		self.deb_ok_list = []
 		self.deb_not_exists = []
 		for i in self.deb_pac_list:
 			if path.isfile(i):
 				self.deb_ok_list.append(i)
-				self.deb_install_str = str(self.deb_install_str) + str(" ") + str(i)
+				self.deb_install_str = str(self.deb_install_str) + str(" %s" % str(i))
 			else:
 				self.deb_not_exists.append(i)
 
 	def local_gui_install_deepin_deb(self, pac=None):
 		"""
 		使用Dde图形化安装程序(deepin-deb-installer)进行安装
 		:param pac: 传入需要安装的文件(字符串-一个文件或者列表-多个文件)
@@ -174,9 +174,7 @@
 			self.logger.info("正在进入安装,安装数量: ", len(self.deb_ok_list))
 		else:
 			self.logger.error("传入的安装文件异常")
 			return False
 		cmd = str("deepin-deb-installer  %s" % self.deb_install_str)
 		self.cmd.getout(cmd=cmd)
 		return True
-
-
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Cmd.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Cmd.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import platform
 from os import system, chdir, path, getcwd, getenv
 from subprocess import getstatusoutput, getoutput
 
 from .logger import ColorLogger
 
 
-class Command:
+class NewCommand:
 	def __init__(self, password, cmd=None, terminal=False, logs=False, work=getcwd()):
 		"""
 		执行系统指令
 		:param terminal: 是否使用图形终端执行, 全局默认,子功能可自定义
 		:param password: 主机密码(string)
 		:param cmd: 需要执行的命令(string)
 		:param logs: 是否使用日志打印信息
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Docker.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 @Time    :   2022-10-25 20:57
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   Docker管理功能
 """
-from .Cmd import Command
+from .Cmd import NewCommand
 from .Jurisdiction import Jurisdiction
 from .logger import ColorLogger
-from .Package import PackageManagement
+from .Package import NewPackageManagement
 from sys import exit
-from .FileManagement import FileManagement
-from .Service import ServiceManagement
+from .NewFileManagement import NewFileManagement
+from .Service import NewServiceManagement
 
 
 class DockerManagement:
 	def __init__(self, password, logs=True, log_file=None, journal=False):
 		"""
 		Docker管理
 		:param password: 主机密码
@@ -28,18 +28,18 @@
 		"""
 		self.logs = logs
 		self.logger = ColorLogger(file=log_file, txt=journal, class_name=self.__class__.__name__)
 		ju = Jurisdiction(passwd=password)
 		if not ju.verification(name='DockerManagement'):
 			self.logger.error("当前用户/密码无法获取sudo权限: %s" % password)
 			exit(1)
-		self.cmd = Command(password=password, logs=logs)
-		self.pac = PackageManagement(password=password, logs=logs, file=log_file, package='docker.io')
-		self.fm = FileManagement()
-		self.service = ServiceManagement(service='docker.service', password=password, log=logs)
+		self.cmd = NewCommand(password=password, logs=logs)
+		self.pac = NewPackageManagement(password=password, logs=logs, file=log_file, package='docker.io')
+		self.fm = NewFileManagement()
+		self.service = NewServiceManagement(service='docker.service', password=password, log=logs)
 
 	def check_install(self):
 		if not self.pac.installed():
 			if not self.pac.installed(pac='docker-ce'):
 				self.logger.error("未安装Docker.io/Docker-ce")
 				return False
 		return True
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Dpkg.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Dpkg.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 @Time    :   2022-09-05 09:17
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from .Cmd import Command
+from .Cmd import NewCommand
 from .logger import ColorLogger
 from os import path
 
 
-class DpkgManagement:
+class NewDpkgManagement:
 	def __init__(self, password, log=False, terminal=False):
 		"""
 		Apt 管理
 		:param password: 主机密码
 		:param log: 是否启用日志
 		:param terminal: 是否使用终端执行命令(针对个别Linux发行部才起作用)
 		"""
@@ -26,15 +26,15 @@
 		# 当前包名称
 		self.local_package_name = ''
 		# 当前获取状态
 		self.get_status = False
 		self.log = log
 		self.terminal = terminal
 		self.password = password
-		self.cmd = Command(password=self.password, cmd='which apt', terminal=self.terminal, logs=self.log)
+		self.cmd = NewCommand(password=self.password, cmd='which apt', terminal=self.terminal, logs=self.log)
 		self.logger = ColorLogger()
 		# 需要安装的安装包文件信息
 		self.file_install = ''
 		# 可安装的文件列表
 		self.install_list = []
 		# 格式错误的文件列表
 		self.format_err = []
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/FileManagement.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NewFileManagement.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 """
 from os import path, makedirs
 from shutil import rmtree, copy2, move
 from subprocess import getstatusoutput
 from .logger import ColorLogger
 
 
-class FileManagement:
+class NewFileManagement:
 	def __init__(self, target=None, log=True, log_file=None, txt_log=False):
 		"""
 		文件管理模块
 		:param target: 管理目标
 		:param log: 是否开启日志
 		:param log_file: 日志文件
 		:param txt_log: 是否开启文件日志
@@ -115,11 +115,11 @@
 				get = True
 		else:
 			self.logger.warning('文件不存在: %s' % filename)
 		return get
 
 
 if __name__ == "__main__":
-	fm = FileManagement(target='/etc/hosts')
+	fm = NewFileManagement(target='/etc/hosts')
 	fm.get_md5()
 	fm.mkdir_p(target='/home/liumou', mode=666)
 	fm.rmdir(target='/home/liumou')
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Iptables.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Iptables.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 @Desc    :   防火墙管理
 """
 
 from subprocess import getstatusoutput
 from sys import exit
 
 from .Jurisdiction import Jurisdiction
-from .Service import ServiceManagement
-from .Cmd import Command
+from .Service import NewServiceManagement
+from .Cmd import NewCommand
 from .logger import ColorLogger
 
 
 class IpTables:
 	def __init__(self, password=None, logs=False, log_file=None, port=80, source=None, zone=None, direction="INPUT"):
 		"""
 		Iptables防火墙软件配置
 		:param password: 主机密码(root用户不需要)
 		:param logs: 是否显示详细信息
 		"""
 		self.log_file = log_file
 		self.logs = logs
 		self.logger = ColorLogger(file=log_file, txt=logs)
-		self.cmd = Command(password=password, logs=logs)
+		self.cmd = NewCommand(password=password, logs=logs)
 		ju = Jurisdiction(passwd=password, logs=logs)
 		if not ju.verification(name='IpTables'):
 			self.logger.error("sudo权限验证失败,请检查密码是否正确或者账号是否有权限")
 			exit(1)
 
 		self.agreement = 'TCP'
 		self.port = int(port)
@@ -53,15 +53,15 @@
 		# 记录端口详细情况
 		self.port_dic = {}
 		# 查看已配置且接受的端口列表
 		self.port_accept_list = []
 		# 记录ID和端口的关系
 		self.port_id_port = {}
 		self.service_name = 'ipsec'
-		self.service = ServiceManagement(service=self.service_name, password=password, log=logs)
+		self.service = NewServiceManagement(service=self.service_name, password=password, log=logs)
 	
 	def open_port_appoint_ip(self):
 		"""
 		开放特定端口给特定主机
 		:return:
 		"""
 		pass
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Jurisdiction.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Jurisdiction.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetManagement.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NmcliManger.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 # -*- encoding: utf-8 -*-
 """
-@File    :   NetManagement.py
+@File    :   NmcliManger.py
 @Time    :   2022/04/17 01:06:40
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   liumou.site@qq.com
 @Homepage : https://liumou.site
 @Desc    :   网络管理模块
 """
 import ipaddress
+import re
+import socket
+import subprocess
 
-from .Cmd import Command
-from .base import ListRemoveNone, ListGetLen
+from .Cmd import NewCommand
+from .base import list_get_len
 from .logger import ColorLogger
 
-
 class NetManagement(object):
 	def __init__(self, password=None, ip=None, gw=None, mask=24, dns1=None, dns2=None, net=None, dev=None, log=True):
 		"""
 		网络管理模块,参数均为可选传参，请根据实际需求传入
 		:param password: (str, optional): 设置主机密码. Defaults to None.
 		:param ip: (str, optional): 设置IP地址. Defaults to "192.168.1.138".
 		:param gw: (str, optional): 设置网关. Defaults to "192.168.1.1".
@@ -71,97 +73,134 @@
 		self.DefaultDev = None  # 默认网卡设备名称
 		self.deviceList = []  # 网卡列表
 		self.logger = ColorLogger()
 		# ju = Jurisdiction(passwd=password)
 		# if not ju.verification(name='NetManagement'):
 		# 	self.logger.error('密码错误/用户无权限')
 		# 	exit(1)
-		self.cmd = Command(password=password)
+		self.cmd = NewCommand(password=password)
 		self.debug = False
+		self.Err = None
+		self.get_default()
+
+	def get_default(self):
+		"""
+		获取默认网卡信息
+		:return:
+		"""
+		self._get_default_ipv4_socket()
+		self._get_default_gateway()
+
+	def _get_default_gateway(self):
+		output = subprocess.check_output('ip route show default', shell=True)
+		match = re.search(r'default via (\d+\.\d+\.\d+\.\d+) dev (\w+)', output.decode())
+		if match:
+			self.logger.info("默认网关获取成功")
+			self.DefaultGw = match.group(1)
+		else:
+			self.logger.error("默认网关获取失败")
+			self.DefaultGw = None
+			self.Err = "无法获取默认网关"
+
+	def _get_default_ipv4_socket(self):
+		"""
+		通过socket 获取本机IP,通过DefaultIp4获取实际值
+		:return: bool
+		"""
+		try:
+			hostname = socket.gethostname()
+			self.DefaultIp4 = socket.gethostbyname(hostname)
+			return True
+		except Exception as e:
+			self.logger.error(str(e))
+			self.Err = str(e)
+		return False
 
 	def connect_create(self, name="Y", mode='auto'):
 		"""
 		创建连接
 		:param name: (str, optional): 连接名称. Defaults to "Y".
 		:param mode: (str, optional): 连接模式. Defaults to "auto".
-		:return:
+		:return: bool
 		"""
+		self.Err = None
 		c = str("""nmcli connection add type ethernet  con-name {0} ifname {1}""".format(name, self.device))
 		get = self.cmd.shell(cmd=c)
 		if get:
 			self.logger.info("连接创建成功")
 		else:
 			print(c)
-			self.logger.error("连接创建失败")
+			self.Err = "连接创建失败"
+			self.logger.error(self.Err)
 			return False
 		if mode != "auto":
 			self.logger.debug("使用静态IP配置")
 			c = str("""nmcli connection modify {0} ipv4.method manual ipv4.addresses {1}""".format(name, self.ipv4))
-
 		else:
 			self.logger.debug("使用自动获取IP")
 			c = str("""nmcli connection modify {0} ipv4.method auto""".format(name))
-		self.run(c=c, n_="IP获取模式配置")
+		return self.run(c=c, n_="IP获取模式配置")
 
 	def run(self, c, n_):
 		"""
 		运行命令
 		:param c: 需要执行的命令
 		:param n_: 命令名称
 		:return: bool
 		"""
 		get = self.cmd.shell(cmd=c)
 		if get:
 			self.logger.info("[ %s ]成功" % n_)
 			return True
 		else:
 			print(c)
-			self.logger.warning("[ %s ]失败" % n_)
+			self.Err = "[ %s ]失败" % n_
+			self.logger.warning(self.Err)
 		return False
 
-	def GetConUuid(self, name):
+	def get_con_uuid(self, name):
 		"""
 		通过名称或者关键词获取一个连接的UUID
 		:param name:
 		:return:
 		"""
 		c = str("""nmcli connection  | grep "%s" """ % name)
 		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
 			sp = str(get).split(" ")
-			sp = ListGetLen(sp, 10)  # 获取元素长度大于10的元素
+			sp = list_get_len(sp, 10)  # 获取元素长度大于10的元素
 			if len(sp) == 1:
 				return sp[0]
 			if len(sp) > 1:
 				for i in sp:
 					ts = str(i).split("-")
 					if len(ts) == 5:
 						return i
 		return False
 
-	def ConnectDelete(self, con):
+	def con_delete(self, con):
 		"""
 		删除连接
 		:param con: 需要删除的连接名称/名称关键词或者UUID
 		:return: bool
 		"""
 		if con is None:
 			con = self.connect_name
-		cl = self.GetConUuid(name=con)
+		cl = self.get_con_uuid(name=con)
 		if cl:
 			c = str("""nmcli connection  delete %s""" % cl)
 			self.cmd.shell(c)
 			if self.cmd.code != 0:
 				self.logger.error("删除失败")
 				return False
 		else:
 			self.logger.warning("无法获取连接")
 		return True
 
-	def GetDevList(self):
+	def get_dev_list(self):
 		"""
 		获取设备列表
 		:return:bool(数据请通过 self.deviceList 获取)
 		"""
 		c = str("""ip link show up | grep '<' | sed 's/://g' | awk '{print $2}' | grep -v ^docker | grep -v ^lo""")
 		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
@@ -184,88 +223,75 @@
 				ip = ipaddress.IPv4Address(i)
 				return ip
 			except:
 				continue
 		self.logger.warning("无法获取到IP地址")
 		return False
 
-	def GetEthDns(self, eth):
+	def get_eth_dns_list(self, eth):
 		"""
 		获取当前系统默认DNS信息
 		:param eth: 获取指定网卡设备的DNS地址
 		:return: list
 		"""
 		# d = []
-		c = str("""nmcli device show %s  | grep DNS | awk '{print $2}'""" % eth)
+		c = str("""nmcli device show %s | grep DNS | grep IP4| awk '{print $2}'""" % eth)
 		get = self.cmd.getout(cmd=c)
 		if self.cmd.code == 0:
 			print(get)
 			sp = str(get).split("\n")
 			if len(sp) >= 1:
 				return sp
 		print(c)
 		self.logger.warning("无法获取网卡的DNS信息: %s" % eth)
 		return False
 
-	def GetDefaultDev(self):
+	def get_default_dev(self):
 		"""
 		获取默认网卡设备信息，获取到的信息请通过实例变量(Default开头)获取(网卡名称、网关、子网掩码、IP地址)
 		:return: bool
 		"""
-		c = str("ip r | grep default |sed -n 1p")
-		get = self.cmd.getout(cmd=c)
+		# c = str("ip r | grep default |sed -n 1p")
+		# get = self.cmd.getout(cmd=c)
+		self.DefaultDev = self.cmd.getout("ip r | grep default | sed -n 1p | awk '{print $5}'")
+		self.DefaultGw = self.cmd.getout("ip r | grep default | sed -n 1p | awk '{print $3}'")
+		self.DefaultDnsList = self.get_eth_dns_list(self.DefaultDev)
+		c = str("""ip addr show %s  | grep inet | sed -n 1p | awk '{print $2}'""" % self.DefaultDev)
+		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
-			sp = str(get).split(" ")
-			sp = ListRemoveNone(sp)
-			if len(sp) >= 3:
-				self.DefaultDev = sp[4]
-				self.DefaultGw = sp[2]
-				self.DefaultIp4 = sp[8]
-				# 获取DNS信息
-				self.DefaultDnsList = self.GetEthDns(self.DefaultDev)
-				# 获取子网掩码
-				c = str("""ip addr show %s  | grep inet | sed -n 1p | awk '{print $2}'""" % self.DefaultDev)
-				get = self.cmd.getout(c)
-				if self.cmd.code == 0:
-					self.DefaultMask = str(get).split("/")[-1]
-				# self.DefaultMask =
-				return True
-			else:
-				print(sp)
-				print(c)
-				self.logger.warning("无法获取默认设备信息")
+			self.DefaultMask = str(get).split("/")[-1]
 		return False
 
-	def GetConListAllUuid(self):
+	def get_con_uuid_all(self):
 		"""
 		获取所有可用的连接UUID列表,返回数据格式: ['7dc597e8-23ad-4360-8dc3-87058a2d08aa', 'b3a484ff-73a6-4e0e-8c1a-0e829b36a848']
 		:return: bool/list
 		"""
 		c = """nmcli con  show --active | grep -v loopback| grep -v ^NAME | grep -v ^docker0  | awk '{print $2}'"""
 		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
 			sp = str(get).split("\n")
 			if len(sp) >= 1:
 				return sp
 		return False
 
-	def GetConListEthUuid(self, eth):
+	def get_con_list_eth_uuid(self, eth):
 		"""
 		获取指定网卡的连接配置的UUID列表,返回数据格式: ['7dc597e8-23ad-4360-8dc3-87058a2d08aa', 'b3a484ff-73a6-4e0e-8c1a-0e829b36a848']
 		:return:bool/list
 		"""
 		c = str("""nmcli connection show | grep %s | awk '{print $2}'""" % eth)
 		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
 			sp = str(get).split("\n")
 			if len(sp) >= 1:
 				return sp
 		return False
 
-	def GetEthInfo(self, eth):
+	def get_eth_info(self, eth):
 		"""
 		获取指定网卡的网络配置信息,包含: IP4、网关、掩码、DNS
 		:param eth: 需要获取的网卡名称
 		:return:
 		"""
 		c = str("""ip address show %s  | grep inet | sed -n 1p  | awk '{print $2}'""" % eth)
 		info = {}
@@ -280,23 +306,23 @@
 		c = str("""nmcli device show %s  | grep IP4.GATE | awk '{print $2}'""" % eth)
 		get = self.cmd.shell(c)
 		if self.cmd.code == 0:
 			info["gw"] = get
 		else:
 			self.logger.warning("网关获取失败")
 			info["gw"] = None
-		dns = self.GetEthDns(eth=eth)
+		dns = self.get_eth_dns_list(eth=eth)
 		if dns:
 			info["dns"] = dns
 		else:
 			info["dns"] = []
 			self.logger.warning("DNS获取失败")
 		return info
 
-	def GetConDns(self, con):
+	def get_con_dns(self, con):
 		"""
 		获取指定连接的DNS信息
 		:param con: 需要获取的连接名称或者uuid
 		:return:list
 		"""
 		c = str("""nmcli con show %s  | grep IP4.DNS | awk '{print $2}'""" % con)
 		if self.debug:
@@ -307,15 +333,15 @@
 			if self.debug:
 				self.logger.debug("ds: ", str(ds))
 			if len(ds) >= 1:
 				return ds
 		self.logger.warning("无法获取连接的DNS信息")
 		return [None]
 
-	def GetConGw(self, con):
+	def get_con_gw(self, con):
 		"""
 		获取连接的网关信息
 		:param con: 需要获取的连接名称或者uuid
 		:return:
 		"""
 		c = str("""nmcli con show %s  | grep IP4.GATE | awk '{print $2}'""" % con)
 		if self.debug:
@@ -323,15 +349,15 @@
 		get = self.cmd.getout(c)
 		if self.cmd.code == 0:
 			return get
 		else:
 			self.logger.warning("网关获取失败")
 		return None
 
-	def GetConIp(self, con):
+	def get_con_ip(self, con):
 		"""
 		获取连接的IP地址
 		:param con: 需要获取的连接名称或者uuid
 		:return:
 		"""
 		info = {}
 		c = str("""nmcli con show %s  | grep IP4.ADD | awk '{print $2}'""" % con)
@@ -350,36 +376,36 @@
 
 		else:
 			self.logger.warning("网关获取失败")
 		info["ip"] = None
 		info["mask"] = 0
 		return info
 
-	def GetConInfo(self, con):
+	def get_con_info(self, con):
 		"""
 		获取指定连接的网络配置信息,通过status判断获取结构, 格式: {'ip': '10.1.1.18', 'mask': 24, 'gw': '10.1.1.1', 'dns': ['10.1.1.1'], 'status': True}
 		:param con: 连接名称或UUID
 		:return: dict
 		"""
 		info = {}
 		# 首先获取UUID
-		c = self.GetConUuid(name=con)
+		c = self.get_con_uuid(name=con)
 		if c:
-			ip = self.GetConIp(con=con)
+			ip = self.get_con_ip(con=con)
 			info = ip
-			gw = self.GetConGw(con=con)
+			gw = self.get_con_gw(con=con)
 			info["gw"] = gw
-			dns = self.GetConDns(con=con)
+			dns = self.get_con_dns(con=con)
 			if self.debug:
 				self.logger.debug(str(dns))
 			info["dns"] = dns
 			info["status"] = True
 			return info
 		else:
 			self.logger.error("无法获取连接信息,请检查配置参数")
 			info["status"] = False
 		return info
 
 
 if __name__ == "__main__":
 	n = NetManagement()
-	n.GetDefaultDev()
+	n.get_default_dev()
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/NetStatus.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/NewNetStatus.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,19 +8,19 @@
 @Homepage : https://liumou.site
 @Desc    :   网络管理
 """
 import socket
 from os import path, getcwd
 from sys import platform
 
-from . import FileManagement, Command, get
+from . import NewFileManagement, NewCommand, get
 from .logger import ColorLogger
 
 
-class NetworkCardInfo:
+class NewNetworkCardInfo:
 	def __init__(self, eth=None, debug=False):
 		"""
 		获取本地网卡信息
 		:param eth: 设置网卡名,当不设置的时候则自动检测
 		"""
 		# Dns地址列表
 		self.dns = None
@@ -40,15 +40,15 @@
 		self.mac = None
 		# 设置子网掩码
 		self.mask = 24
 		# 设置连接名称
 		self.connect = None
 		# 连接速率
 		self.rate = None
-		self.cmd = Command(password="pd")
+		self.cmd = NewCommand(password="pd")
 		self.logger = ColorLogger()
 
 	def show(self):
 		"""
 		显示网卡信息
 		:return:
 		"""
@@ -159,31 +159,32 @@
 			self.sub = str("%s.%s.%s." % (tu[0], tu[1], tu[2]))
 			return True
 		except Exception as e:
 			self.logger.error(str(e))
 			return False
 
 
-class NetStatus:
-	def __init__(self, ip=None, port=80, log_file=None, txt_log=False):
+class NewNetStatus:
+	def __init__(self, ip=None, port=80, log_file=None, txt_log=False, debug=True):
 		"""
 		网络工具，用于判断网络是否正常
 		:param ip: 需要判断的IP
 		:param port:  需要判断的端口. Defaults to None.
 		:param log_file: 日志文件
 		:param txt_log: 是否开启文本日志
 		"""
+		self.debug = debug
 		self.ip = ip
 		self.port = port
 		self.status = False
 		#
 		self.headers = {}
 		self.headers = get.headers
-		self.cmd = Command(password='Gxxc@123')
-		self.fm = FileManagement()
+		self.cmd = NewCommand(password='Gxxc@123')
+		self.fm = NewFileManagement()
 		self.logger = ColorLogger(file=log_file, txt=txt_log)
 
 	def ping_status(self, server=None):
 		"""
 		使用ping检测网络连接
 		:param server: 设置服务器地址. Defaults to self.ip.
 		:return:
@@ -240,11 +241,37 @@
 					return False
 			return True
 		self.logger.error("下载失败: %s" % filename)
 		self.logger.error("下载链接: ", url)
 		self.logger.error("保存路径: ", filename)
 		return False
 
+	def tcp_port_status(self, port, timeout=5, ip=None):
+		"""
+		检测TCP端口是否开放
+		:param ip: 
+		:param port: 
+		:param timeout: 
+		:return: 
+		"""
+		if ip is None:
+			if self.ip is None:
+				self.logger.error("未设置对端IP地址")
+			else:
+				self.logger.debug("使用实例配置IP进行检测")
+				ip = self.ip
+		else:
+			self.logger.debug("使用函数传入IP")
+		self.logger.info("正在检测地址: [", ip, "] - 端口: [ ", port, " ]")
+		
+		sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+		sock.settimeout(timeout)
+		try:
+			sock.connect((self.ip, port))
+			return True
+		except socket.error:
+			return False
+
 
 if __name__ == "__main__":
-	up = NetStatus()
+	up = NewNetStatus()
 	up.ping_status(server='baidu.com')
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/OsInfo.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/OsInfo.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Package.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Package.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,39 @@
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   Linux包管理工具
 """
 from os import path, system
 
 from .logger import ColorLogger
-from .Cmd import Command
+from .Cmd import NewCommand
 from .Yum import YumManager
-from .Dpkg import DpkgManagement
-from .AptManage import AptManagement
+from .Dpkg import NewDpkgManagement
+from .AptManage import NewAptManagement
 from .Jurisdiction import Jurisdiction
 
 
-class PackageManagement:
+class NewPackageManagement:
 	def __init__(self, password, logs=True, file=None, package=None):
 		"""
 		Linux包管理模块
 		:param password: 主机密码
 		:param logs: 是否开启日志
 		:param file: 需要安装的文件
 		:param package: 需要安装的包
 		"""
 		self.package = package
 		self.file = file
 		self.logs = logs
 		self.password = password
-		self.cmd = Command(password=password, logs=logs)
+		self.cmd = NewCommand(password=password, logs=logs)
 		self.ju = Jurisdiction(passwd=password, logs=logs)
 		self.install_tools = 'apt'
-		self.manger = AptManagement(password=password, log=logs)
-		self.local = DpkgManagement(password=password, log=logs)
+		self.manger = NewAptManagement(password=password, log=logs)
+		self.local = NewDpkgManagement(password=password, log=logs)
 		if int(system('which yum')) == 0:
 			self.install_tools = 'yum'
 		self.logger = ColorLogger(file=file, txt=logs, class_name=self.__class__.__name__)
 		self.init()
 	
 	def init(self):
 		"""
@@ -147,15 +147,15 @@
 		"""
 		升级系统
 		:param update_index: 是否更新索引
 		:param dist: 温柔的更新(针对apt)
 		:return:
 		"""
 		if self.install_tools.lower() == 'apt':
-			self.manger = AptManagement(password=self.password, log=self.logs)
+			self.manger = NewAptManagement(password=self.password, log=self.logs)
 			if dist:
 				return self.manger.upgrade_dist(update=update_index)
 			else:
 				return self.manger.upgrade(update=update_index)
 		else:
 			self.manger = YumManager(password=self.password, log=self.logs)
 			return self.manger.update(update=update_index)
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/README.md` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 │   ├── cmd.py
 │   ├── dpkg.py
 │   ├── FileManagement.py
 │   ├── get.py
 │   ├── __init__.py
 │   ├── Jurisdiction.py
 │   ├── logger.py
-│   ├── NetManagement.py
+│   ├── NmcliManger.py
 │   ├── NetStatus.py
 │   ├── Package.py
 │   ├── pacman.py
 │   ├── README.md
 │   ├── Service.py
 │   ├── setup.py
 │   ├── source.py
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Service.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Service.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 @Time    :   2022-10-23 23:00
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from . import Jurisdiction, Command
+from . import Jurisdiction, NewCommand
 from .logger import ColorLogger
 from .OsInfo import OsInfo
 from os import path
 
 
-class ServiceManagement:
+class NewServiceManagement:
 	def __init__(self, service, password, log=True):
 		"""
 		服务管理
 		:param service: 服务名称
 		:param password: 密码
 		:param log: 是否开启文本日志
 		"""
 		self.log = log
 		self.password = password
 		self.service = service
 		file = path.join(OsInfo().home_dir, 'ServiceManagement.log')
 		self.logger = ColorLogger(file=file, txt=log, class_name=self.__class__.__name__)
 		self.ju = Jurisdiction(passwd=password, logs=log)
-		self.cmd = Command(password=password, logs=log)
+		self.cmd = NewCommand(password=password, logs=log)
 
 	def _sudo(self):
 		"""
 		检查是否已有sudo权限
 		:return:
 		"""
 		if self.ju.verification(name='ServiceManagement'):
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Source.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Source.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 #!/usr/bin/env python3
 # -*- encoding: utf-8 -*-
 from os import path
-from . import Command, AptManagement
+from . import NewCommand, NewAptManagement
 from .logger import ColorLogger
 from subprocess import getoutput
 
 
 class Source:
 	def __init__(self, passwd, debug=False, mirrors="mirrors.cloud.tencent.com"):
 		self.mirrors = mirrors
 		self.source = '/etc/apt/sources.list'
 		self.source_bak = '/etc/apt/sources.list.bak'
-		self.cmd = Command(password=passwd)
+		self.cmd = NewCommand(password=passwd)
 		self.release = getoutput("cat /etc/os-release  | grep ^ID=").split("=")[1].lower()
-		self.apt = AptManagement(password=passwd)
+		self.apt = NewAptManagement(password=passwd)
 		self.logger = ColorLogger(txt=debug)
 
 	def bak(self):
 		if not path.isfile(self.source_bak) and path.isfile(self.source):
 			self.cmd.sudo(cmd="cp -rf %s %s" % (self.source, self.source_bak), name='Bak Sources')
 
 	def get(self):
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/Yum.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/Yum.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   Yum包管理工具
 """
 
-from .Cmd import Command
+from .Cmd import NewCommand
 from .logger import ColorLogger
 
 
 class YumManager:
 	def __init__(self, password, log=False, terminal=False, package=None, log_file=None):
 		"""
 		yum 管理
@@ -23,15 +23,15 @@
 		:param terminal: 是否使用终端执行命令(针对个别Linux发行部才起作用)
 		:param package: 需要管理的包
 		"""
 		self.package = package
 		self.terminal = terminal
 		self.log = log
 		self.password = password
-		self.cmd = Command(password=self.password, cmd='which yum', terminal=self.terminal, logs=self.log)
+		self.cmd = NewCommand(password=self.password, cmd='which yum', terminal=self.terminal, logs=self.log)
 		self.logger = ColorLogger(file=log_file, txt=self.log, class_name=self.__class__.__name__)
 
 	def install(self, pac='git', update=False):
 		"""
 		安装在线包
 		:param update: 是否更新源索引(默认不会更新源索引)
 		:param pac: 需要安装的包(字符串)
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/__init__.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,30 +6,30 @@
 @Author  :   坐公交也用券
 @Version :   1.1.5
 @Contact :   liumou.site@qq.com
 @Homepage : https://liumou.site
 @Desc    :   这是一个Linux管理脚本的基础库，通过对Linux基本功能进行封装，实现快速开发的效果
 """
 
-from .AptManage import AptManagement
-from .Cmd import Command
-from .Dpkg import DpkgManagement
-from .FileManagement import FileManagement
+from .AptManage import NewAptManagement
+from .Cmd import NewCommand
+from .Dpkg import NewDpkgManagement
+from .NewFileManagement import NewFileManagement
 from .Iptables import IpTables
 from .Jurisdiction import Jurisdiction
-from .NetManagement import NetManagement
-from .NetStatus import NetStatus, NetworkCardInfo
+from .NmcliManger import NetManagement
+from .NewNetStatus import NewNetStatus, NewNetworkCardInfo
 from .OsInfo import *
 from .OsInfo import OsInfo
-from .Package import PackageManagement
-from .Service import ServiceManagement
+from .Package import NewPackageManagement
+from .Service import NewServiceManagement
 from .Yum import YumManager
 from .get import headers, cookies
-from .base import ListGetLen, ListRemoveNone
-from .logger import ColorLogger, log
+from .base import list_get_len, list_remove_none
+from .logger import ColorLogger
 
-__all__ = ["Command", "AptManagement", "DpkgManagement", "FileManagement", "Jurisdiction",
-           "NetManagement", "NetStatus", "PackageManagement", "ServiceManagement", "YumManager", "IpTables",
-           "OsInfo", "NetworkCardInfo", "ListGetLen", "ListRemoveNone", "ColorLogger", "log"]
+__all__ = ["NewCommand", "NewAptManagement", "NewDpkgManagement", "NewFileManagement", "Jurisdiction",
+           "NetManagement", "NewNetStatus", "NewPackageManagement", "NewServiceManagement", "YumManager", "IpTables",
+           "OsInfo", "NewNetworkCardInfo", "list_get_len", "list_remove_none", "ColorLogger"]
 
 if platform.system().lower() != 'linux'.lower():
 	print('Plmb模块仅支持Linux系统')
```

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/get.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/get.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/logger.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/logger.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/src/plbm_liumou_Stable/security/firewalld.py` & `plbm_liumou_stable-1.4.0/src/plbm_liumou_Stable/security/firewalld.py`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/LICENSE` & `plbm_liumou_stable-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `plbm_liumou_stable-1.3.9/README.md` & `plbm_liumou_stable-1.4.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -14,17 +14,17 @@
 * 完全使用内置模块进行开发，拿来即用
 * 使用Python基础语法进行编写，兼容新旧版本Python3，告别语法冲突(例如3.5及以下版本无法使用f"{}"语法)
 * 完全开源、永久免费
 
 
 # 更新内容
 
-## `1.3.9`
+## `1.4.0`
 
-* 修正日志无法输出的问题
+* 全部类使用`New`开头
 
 
 # 使用方法
 
 ## 安装
 
 具体可以访问Pypi项目地址[https://pypi.org/project/plbm-liumou-Stable/](https://pypi.org/project/plbm-liumou-Stable/)
@@ -58,23 +58,23 @@
 @Time    :   2022-10-24 22:45
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from plbm_liumou_Stable import PackageManagement
+from plbm_liumou_Stable import NewPackageManagement
 from ColorInfo import ColorLogger
 
 
 
 class ServiceManager:
 	def __init__(self, pac, password):
 		self.package = pac
-		self.pac = PackageManagement(password=password, package="vsftpd")
+		self.pac = NewPackageManagement(password=password, package="vsftpd")
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def remove(self):
 		if self.pac.installed():
 			self.logger.info(f"已安装: {self.package}")
 			if self.pac.uninstall():
 				self.logger.info(f"卸载成功: {self.package}")
@@ -89,15 +89,15 @@
 	demo = ServiceManager(pac="vsftpd", password="demo")
 	demo.remove()
 root@l:~/data/git/PythonLinuxBasicModule/demo# python3 package.py 
 /usr/lib/python3/dist-packages/requests/__init__.py:91: RequestsDependencyWarning: urllib3 (1.26.12) or chardet (3.0.4) doesn't match a supported version!
   RequestsDependencyWarning)
 2023-01-06 22:42:31 Jurisdiction.py  line: 79 - Class: Jurisdiction Function: verification - INFO : 已处于root权限
 2023-01-06 22:42:31 Cmd.py  line: 188 - Class: ComMand Function: getout - DEBUG : dpkg -s vsftpd
-2023-01-06 22:42:31 Package.py  line: 141 - Class: PackageManagement Function: installed - INFO : 已安装: vsftpd
+2023-01-06 22:42:31 Package.py  line: 141 - Class: NewPackageManagement Function: installed - INFO : 已安装: vsftpd
 2023-01-06 22:42:31 package.py  line: 23 - Class: ServiceManager Function: remove - INFO : 已安装: vsftpd
 2023-01-06 22:42:31 Dpkg.py  line: 113 Function: uninstall - INFO : UnInstalling UnInstall vsftpd ...
 (Reading database ... 92009 files and directories currently installed.)
 Removing vsftpd (3.0.3-12) ...
 Purging configuration files for vsftpd (3.0.3-12) ...
 locale: Cannot set LC_MESSAGES to default locale: No such file or directory
 locale: Cannot set LC_ALL to default locale: No such file or directory
@@ -118,22 +118,22 @@
 @Time    :   2022-10-24 22:45
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from plbm_liumou_Stable import ServiceManagement
+from plbm_liumou_Stable import NewServiceManagement
 from ColorInfo import ColorLogger
 
 
 class ServiceManager:
 	def __init__(self, services, password):
 		self.services = services
-		self.manager = ServiceManagement(service=services, password=password)
+		self.manager = NewServiceManagement(service=services, password=password)
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def restart(self):
 		if self.manager.restart(reload=True):
 			self.logger.info("服务重启成功")
 		else:
 			self.logger.warning("服务重启失败")
@@ -143,11 +143,11 @@
 	demo = ServiceManager(services="vsftpd", password="demo")
 	demo.restart()
 root@l:~/data/git/PythonLinuxBasicModule# python3 demo.py 
 /usr/lib/python3/dist-packages/requests/__init__.py:91: RequestsDependencyWarning: urllib3 (1.26.12) or chardet (3.0.4) doesn't match a supported version!
   RequestsDependencyWarning)
 [ 重载服务配置 ] 执行成功
 [ Restart vsftpd ] 执行成功
-2023-01-06 22:36:41 Service.py  line: 141 - Class: ServiceManagement Function: restart - INFO : 重启成功: vsftpd
+2023-01-06 22:36:41 Service.py  line: 141 - Class: NewServiceManagement Function: restart - INFO : 重启成功: vsftpd
 2023-01-06 22:36:41 demo.py  line: 23 - Class: ServiceManager Function: restart - INFO : 服务重启成功
 root@l:~/data/git/PythonLinuxBasicModule# 
 ```
```

### Comparing `plbm_liumou_stable-1.3.9/pyproject.toml` & `plbm_liumou_stable-1.4.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "plbm_liumou_Stable"
-version = "1.3.9"
+version = "1.4.0"
 authors = [
   { name="坐公交也用券", email="liumou.site@qq.com" },
 ]
 description = "使用Python3进行编写的一个开源系统管理工具， 通过封装Linux系统都软件包管理、磁盘管理、文件管理、网络管理、安全管理、服务管理等内容从而实现快速开发的效果"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `plbm_liumou_stable-1.3.9/PKG-INFO` & `plbm_liumou_stable-1.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plbm_liumou_Stable
-Version: 1.3.9
+Version: 1.4.0
 Summary: 使用Python3进行编写的一个开源系统管理工具， 通过封装Linux系统都软件包管理、磁盘管理、文件管理、网络管理、安全管理、服务管理等内容从而实现快速开发的效果
 Project-URL: Homepage, https://gitee.com/liumou_site/plbm
 Project-URL: Bug Tracker, https://gitee.com/liumou_site/plbm/issues
 Author-email: 坐公交也用券 <liumou.site@qq.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -28,17 +28,17 @@
 * 完全使用内置模块进行开发，拿来即用
 * 使用Python基础语法进行编写，兼容新旧版本Python3，告别语法冲突(例如3.5及以下版本无法使用f"{}"语法)
 * 完全开源、永久免费
 
 
 # 更新内容
 
-## `1.3.9`
+## `1.4.0`
 
-* 修正日志无法输出的问题
+* 全部类使用`New`开头
 
 
 # 使用方法
 
 ## 安装
 
 具体可以访问Pypi项目地址[https://pypi.org/project/plbm-liumou-Stable/](https://pypi.org/project/plbm-liumou-Stable/)
@@ -72,23 +72,23 @@
 @Time    :   2022-10-24 22:45
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from plbm_liumou_Stable import PackageManagement
+from plbm_liumou_Stable import NewPackageManagement
 from ColorInfo import ColorLogger
 
 
 
 class ServiceManager:
 	def __init__(self, pac, password):
 		self.package = pac
-		self.pac = PackageManagement(password=password, package="vsftpd")
+		self.pac = NewPackageManagement(password=password, package="vsftpd")
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def remove(self):
 		if self.pac.installed():
 			self.logger.info(f"已安装: {self.package}")
 			if self.pac.uninstall():
 				self.logger.info(f"卸载成功: {self.package}")
@@ -103,15 +103,15 @@
 	demo = ServiceManager(pac="vsftpd", password="demo")
 	demo.remove()
 root@l:~/data/git/PythonLinuxBasicModule/demo# python3 package.py 
 /usr/lib/python3/dist-packages/requests/__init__.py:91: RequestsDependencyWarning: urllib3 (1.26.12) or chardet (3.0.4) doesn't match a supported version!
   RequestsDependencyWarning)
 2023-01-06 22:42:31 Jurisdiction.py  line: 79 - Class: Jurisdiction Function: verification - INFO : 已处于root权限
 2023-01-06 22:42:31 Cmd.py  line: 188 - Class: ComMand Function: getout - DEBUG : dpkg -s vsftpd
-2023-01-06 22:42:31 Package.py  line: 141 - Class: PackageManagement Function: installed - INFO : 已安装: vsftpd
+2023-01-06 22:42:31 Package.py  line: 141 - Class: NewPackageManagement Function: installed - INFO : 已安装: vsftpd
 2023-01-06 22:42:31 package.py  line: 23 - Class: ServiceManager Function: remove - INFO : 已安装: vsftpd
 2023-01-06 22:42:31 Dpkg.py  line: 113 Function: uninstall - INFO : UnInstalling UnInstall vsftpd ...
 (Reading database ... 92009 files and directories currently installed.)
 Removing vsftpd (3.0.3-12) ...
 Purging configuration files for vsftpd (3.0.3-12) ...
 locale: Cannot set LC_MESSAGES to default locale: No such file or directory
 locale: Cannot set LC_ALL to default locale: No such file or directory
@@ -132,22 +132,22 @@
 @Time    :   2022-10-24 22:45
 @Author  :   坐公交也用券
 @Version :   1.0
 @Contact :   faith01238@hotmail.com
 @Homepage : https://liumou.site
 @Desc    :   当前文件作用
 """
-from plbm_liumou_Stable import ServiceManagement
+from plbm_liumou_Stable import NewServiceManagement
 from ColorInfo import ColorLogger
 
 
 class ServiceManager:
 	def __init__(self, services, password):
 		self.services = services
-		self.manager = ServiceManagement(service=services, password=password)
+		self.manager = NewServiceManagement(service=services, password=password)
 		self.logger = ColorLogger(class_name=self.__class__.__name__)
 
 	def restart(self):
 		if self.manager.restart(reload=True):
 			self.logger.info("服务重启成功")
 		else:
 			self.logger.warning("服务重启失败")
@@ -157,11 +157,11 @@
 	demo = ServiceManager(services="vsftpd", password="demo")
 	demo.restart()
 root@l:~/data/git/PythonLinuxBasicModule# python3 demo.py 
 /usr/lib/python3/dist-packages/requests/__init__.py:91: RequestsDependencyWarning: urllib3 (1.26.12) or chardet (3.0.4) doesn't match a supported version!
   RequestsDependencyWarning)
 [ 重载服务配置 ] 执行成功
 [ Restart vsftpd ] 执行成功
-2023-01-06 22:36:41 Service.py  line: 141 - Class: ServiceManagement Function: restart - INFO : 重启成功: vsftpd
+2023-01-06 22:36:41 Service.py  line: 141 - Class: NewServiceManagement Function: restart - INFO : 重启成功: vsftpd
 2023-01-06 22:36:41 demo.py  line: 23 - Class: ServiceManager Function: restart - INFO : 服务重启成功
 root@l:~/data/git/PythonLinuxBasicModule# 
 ```
```

