# Comparing `tmp/pyMSVC-0.5.2.tar.gz` & `tmp/pyMSVC-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyMSVC-0.5.2.tar", last modified: Wed May 24 03:55:59 2023, max compression
+gzip compressed data, was "pyMSVC-0.5.3.tar", last modified: Wed May 24 05:38:29 2023, max compression
```

## Comparing `pyMSVC-0.5.2.tar` & `pyMSVC-0.5.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.506242 pyMSVC-0.5.2/
--rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.5.2/LICENSE
--rw-rw-rw-   0        0        0      404 2023-05-24 03:55:59.506242 pyMSVC-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     8235 2022-08-02 05:12:16.000000 pyMSVC-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.489228 pyMSVC-0.5.2/pyMSVC/
--rw-rw-rw-   0        0        0   128072 2023-05-24 03:54:01.000000 pyMSVC-0.5.2/pyMSVC/__init__.py
--rw-rw-rw-   0        0        0    43493 2022-10-20 23:05:10.000000 pyMSVC-0.5.2/pyMSVC/vswhere.py
-drwxrwxrwx   0        0        0        0 2023-05-24 03:55:59.505240 pyMSVC-0.5.2/pyMSVC.egg-info/
--rw-rw-rw-   0        0        0      404 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      227 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-24 03:55:59.000000 pyMSVC-0.5.2/pyMSVC.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2023-05-23 03:40:23.000000 pyMSVC-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-24 03:55:59.507240 pyMSVC-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0      590 2023-05-24 03:54:01.000000 pyMSVC-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:38:29.859583 pyMSVC-0.5.3/
+-rw-rw-rw-   0        0        0     1265 2022-08-01 05:24:54.000000 pyMSVC-0.5.3/LICENSE
+-rw-rw-rw-   0        0        0      404 2023-05-24 05:38:29.859583 pyMSVC-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     8235 2022-08-02 05:12:16.000000 pyMSVC-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 05:38:29.842575 pyMSVC-0.5.3/pyMSVC/
+-rw-rw-rw-   0        0        0   127506 2023-05-24 05:35:00.000000 pyMSVC-0.5.3/pyMSVC/__init__.py
+-rw-rw-rw-   0        0        0    43493 2022-10-20 23:05:10.000000 pyMSVC-0.5.3/pyMSVC/vswhere.py
+drwxrwxrwx   0        0        0        0 2023-05-24 05:38:29.858576 pyMSVC-0.5.3/pyMSVC.egg-info/
+-rw-rw-rw-   0        0        0      404 2023-05-24 05:38:29.000000 pyMSVC-0.5.3/pyMSVC.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      227 2023-05-24 05:38:29.000000 pyMSVC-0.5.3/pyMSVC.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 05:38:29.000000 pyMSVC-0.5.3/pyMSVC.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-05-24 05:38:29.000000 pyMSVC-0.5.3/pyMSVC.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-24 05:38:29.000000 pyMSVC-0.5.3/pyMSVC.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2023-05-23 03:40:23.000000 pyMSVC-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 05:38:29.860583 pyMSVC-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0      590 2023-05-24 05:35:00.000000 pyMSVC-0.5.3/setup.py
```

### Comparing `pyMSVC-0.5.2/LICENSE` & `pyMSVC-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.2/README.md` & `pyMSVC-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.2/pyMSVC/__init__.py` & `pyMSVC-0.5.3/pyMSVC/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,17 @@
 
 import os
 import sys
 import ctypes
 import subprocess
 import winreg
 import logging
+import platform
 from typing import Optional, Union
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 _IS_WIN = sys.platform.startswith('win')
 
 logger = logging.getLogger(__name__)
 
 
 def _setup_logging():
@@ -462,14 +463,42 @@
             py_architecture=self.architecture,
             py_dependency=self.dependency,
             py_libraries=self.libraries,
             py_includes=self.includes
         )
 
 
+_MSVC_BUILD_TO_VERSION = {
+    1933: 14.33,
+    1932: 14.32,
+    1931: 14.31,
+    1930: 14.30,
+    1929: 14.29,
+    1928: 14.28,
+    1927: 14.27,
+    1926: 14.26,
+    1925: 14.25,
+    1924: 14.24,
+    1923: 14.21,
+    1922: 14.21,
+    1921: 14.21,
+    1920: 14.20,
+    1916: 14.16,
+    1914: 14.14,
+    1913: 14.13,
+    1912: 14.12,
+    1911: 14.11,
+    1910: 14.10,
+    1900: 14.00,
+    1800: 12.00,
+    1700: 11.00,
+    1600: 10.00,
+    1500: 9.00
+}
+
 class VisualCInfo(object):
     """
     Information about the Visual C or Visual Studio installation.
     """
 
     def __init__(
             self,
@@ -497,40 +526,46 @@
         self._msbuild_path = None
         self._product_semantic_version = None
         self._devinit_path = None
 
         self._strict_toolkit_version = strict_toolkit_version
         self._minimum_toolkit_version = minimum_toolkit_version
 
-        py_version = sys.version_info[:2]
-        if py_version in ((3, 4),):
-            min_visual_c_version = 10.0
-        elif py_version in ((3, 5), (3, 6), (3, 7), (3, 8)):
-            min_visual_c_version = 14.0
-        elif py_version in ((3, 9), (3, 10)):
-            min_visual_c_version = 14.2
-        elif py_version in ((3, 11), (3, 12)):
-            min_visual_c_version = 14.3
-        else:
-            raise RuntimeError(
-                'This library does not support '
-                'python version %d.%d' % py_version
-            )
+        compiler_version = int(
+            platform.python_compiler().split('.')[-1].split(' ')[0]
+        )
+
+        min_visual_c_version = _MSVC_BUILD_TO_VERSION.get(compiler_version, None)
+
+        if min_visual_c_version is None:
+            min_visual_c_version = (compiler_version - 5000) / 100.0
+
+        if minimum_c_version is None:
+            minimum_c_version = min_visual_c_version
 
         if (
             strict_c_version is not None and
             strict_c_version < min_visual_c_version
         ):
-            raise RuntimeError(
-                'The set minimum compiler version is lower then the '
-                'required compiler version for Python'
-            )
+            msg = (
+                'Set strict MSVC version ({0}) is lower than '
+                'the MSVC version that Python has '
+                'been compiled with ({1})'
+            ).format(strict_c_version, min_visual_c_version)
+
+            logging.warning(msg)
+
+        if minimum_c_version < min_visual_c_version:
+            msg = (
+                'Set minimum MSVC version ({0}) is lower than '
+                'the MSVC version that Python has '
+                'been compiled with ({1})'
+            ).format(minimum_c_version, min_visual_c_version)
 
-        if minimum_c_version is None:
-            minimum_c_version = min_visual_c_version
+            logging.warning(msg)
 
         if strict_toolkit_version is not None:
             strict_toolkit_version = str(strict_toolkit_version / 10.0)
 
         if minimum_toolkit_version is not None:
             minimum_toolkit_version = str(minimum_toolkit_version / 10.0)
 
@@ -562,16 +597,16 @@
                     try:
                         if isinstance(vs_version, str):
                             display_version = str(
                                 installation.catalog.product_display_version
                             )
 
                             if (
-                                    installation.version != vs_version and
-                                    display_version != vs_version
+                                installation.version != vs_version and
+                                display_version != vs_version
                             ):
                                 continue
                         else:
                             product_line_version = int(
                                 installation.catalog.product_line_version
                             )
 
@@ -580,22 +615,22 @@
 
                     except:  # NOQA
                         continue
 
                 for package in installation.packages.vsix:
                     if package.id == cpp_id:
                         if (
-                                self.strict_c_version is not None and
-                                package != self.strict_c_version
+                            self.strict_c_version is not None and
+                            package != self.strict_c_version
                         ):
                             continue
 
                         if (
-                                self.minimum_c_version is not None and
-                                package < self.minimum_c_version
+                            self.minimum_c_version is not None and
+                            package < self.minimum_c_version
                         ):
                             continue
 
                         if cpp_version is None:
                             cpp_version = package
                             cpp_installation = installation
                         elif package > cpp_version:
@@ -613,15 +648,15 @@
                     'Tools',
                     'MSVC'
                 )
 
                 for package in cpp_installation.packages.vsix:
                     if package.id == tools_id:
                         if not os.path.exists(
-                                os.path.join(tools_path, package.version)
+                            os.path.join(tools_path, package.version)
                         ):
                             continue
 
                         if strict_toolkit_version is not None:
                             if package == strict_toolkit_version:
                                 tools_version = package
                                 break
@@ -635,36 +670,38 @@
                         elif tools_version > package:
                             tools_version = package
 
                 if tools_version is None:
                     for file in os.listdir(tools_path):
                         if strict_toolkit_version is not None:
                             tk_version = file[:len(strict_toolkit_version)]
+
                             if tk_version == strict_toolkit_version:
                                 tools_version = file
                                 break
 
                         if minimum_toolkit_version is not None:
                             tk_version = file[:len(minimum_toolkit_version)]
+
                             if tk_version < minimum_toolkit_version:
                                 continue
 
                         if tools_version is None:
                             tools_version = file
                         elif tools_version < file:
                             tools_version = file
 
                 else:
                     tools_version = tools_version.version
 
                 if tools_version is not None:
                     tools_version = tools_version.split('.')
                     self._toolset_version = (
-                            'v' + tools_version[0] +
-                            tools_version[1][0]
+                        'v' + tools_version[0] +
+                        tools_version[1][0]
                     )
                     self._tools_version = '.'.join(tools_version)
 
                     self._tools_install_directory = os.path.join(
                         tools_path, self._tools_version
                     )
 
@@ -673,15 +710,15 @@
                             'Tools',
                             'Redist'
                         )
                     )
 
                     if os.path.exists(tools_redist_directory):
                         self._tools_redist_directory = (
-                                tools_redist_directory + '\\'
+                            tools_redist_directory + '\\'
                         )
 
                         msvc_dll_path = os.path.join(
                             tools_redist_directory,
                             environ.python.architecture,
                             'Microsoft.VC{0}.CRT'.format(
                                 self._toolset_version[1:]
@@ -704,15 +741,15 @@
                     'Bin',
                     'MSBuild.exe'
                 )
 
                 if os.path.exists(msbuild_path):
                     msbuild_version = _get_file_version(msbuild_path)
                     self._msbuild_version = '.'.join(
-                        str(item) for item in msbuild_version
+                        str(itm) for itm in msbuild_version
                     )
                     self._msbuild_path = msbuild_path
 
                 ide_directory = os.path.join(
                     cpp_installation.path,
                     'Common7',
                     'IDE',
@@ -808,15 +845,15 @@
             if os.path.exists(ninja_path):
                 paths.append(ninja_path)
 
         return paths
 
     @property
     def cpp_installation(
-            self
+        self
     ) -> Union[vswhere.ISetupInstance, vswhere.ISetupInstance2]:
         return self._cpp_installation
 
     @property
     def f_sharp_path(self) -> Optional[str]:
         """
         Path to F#
@@ -928,15 +965,18 @@
 
             def add(vers):
                 for base_pth, ver in vers:
                     if os.path.exists(base_pth):
                         try:
                             base_ver = float(int(ver.split('.')[0]))
                         except ValueError:
-                            base_ver = float(int(ver.replace('vc', '').split('.')[0]))
+                            ver = ver.replace('vc', '')
+                            base_ver = float(
+                                int(ver.replace('vc', '').split('.')[0])
+                            )
 
                         self.__installed_versions[ver] = dict(
                             base=base_pth,
                             root=base_pth
                         )
                         self.__installed_versions[base_ver] = dict(
                             base=base_pth,
@@ -1006,18 +1046,17 @@
                     version = path.split('\\VC\\bin')[0]
                 elif '\\bin\\Host' in path:
                     version = path.split('\\bin\\Host')[0]
                 else:
                     continue
 
                 version = os.path.split(version)[1]
-                version = version.replace(
-                    'Microsoft Visual Studio',
-                    ''
-                ).strip()
+                version = (
+                    version.replace('Microsoft Visual Studio', '').strip()
+                )
                 base_version = float(int(version.split('.')[0]))
 
                 base_path = path.split('\\VC\\')[0] + '\\VC'
                 if os.path.exists(os.path.join(base_path, 'include')):
                     vc_root = base_path
                 else:
                     vc_root = path.split('\\bin\\')[0]
@@ -1041,18 +1080,18 @@
                     version = float(key)
                 except ValueError:
                     continue
 
                 path = _get_reg_value(reg_path, key)
 
                 if (
-                        (
-                                os.path.exists(path) and
-                                version not in self.__installed_versions
-                        ) or version == 15.0
+                    (
+                        os.path.exists(path) and
+                        version not in self.__installed_versions
+                    ) or version == 15.0
                 ):
 
                     if version == 15.0:
                         version = 14.0
 
                     if not os.path.split(path)[1] == 'VC':
                         path = os.path.join(path, 'VC')
@@ -1141,17 +1180,17 @@
         :rtype: str
         """
 
         if self._toolset_version is None:
             tools_version = self.tools_version.split('.')
 
             self._toolset_version = (
-                    'v' +
-                    tools_version[0] +
-                    tools_version[1][:1]
+                'v' +
+                tools_version[0] +
+                tools_version[1][:1]
             )
 
         return self._toolset_version
 
     @property
     def msvc_dll_version(self) -> Optional[str]:
         """
@@ -1191,39 +1230,41 @@
                 'Microsoft.VC{0}.CRT'.format(toolset_version[1:]),
             )
 
             redist_path = self.tools_redist_directory
 
             for root, dirs, files in os.walk(redist_path):
                 def pass_directory():
-                    for item in ('onecore', 'arm', 'spectre'):
-                        if item in root.lower():
+                    for itm in ('onecore', 'arm', 'spectre'):
+                        if itm in root.lower():
                             return True
+
                     return False
 
                 if pass_directory():
                     continue
 
                 for folder_name in folder_names:
                     if folder_name in dirs:
                         if x64 and ('amd64' in root or 'x64' in root):
                             self._msvc_dll_path = os.path.join(
                                 root,
                                 folder_name
                             )
                             break
                         elif (
-                                not x64 and
-                                'amd64' not in root
-                                and 'x64' not in root
+                            not x64 and
+                            'amd64' not in root
+                            and 'x64' not in root
                         ):
                             self._msvc_dll_path = os.path.join(
                                 root,
                                 folder_name
                             )
+
                             break
 
         return self._msvc_dll_path
 
     @property
     def tools_redist_directory(self) -> Optional[str]:
         """
@@ -1239,16 +1280,16 @@
 
             if 'MSVC' in tools_install_path:
                 redist_path = tools_install_path.replace(
                     'Tools',
                     'Redist'
                 )
                 if (
-                        not os.path.exists(redist_path) and
-                        'BuildTools' in tools_install_path
+                    not os.path.exists(redist_path) and
+                    'BuildTools' in tools_install_path
                 ):
                     redist_path = redist_path.replace(
                         'BuildRedist', 'BuildTools'
                     )
             else:
                 redist_path = os.path.join(
                     tools_install_path,
@@ -1257,15 +1298,15 @@
 
             if not os.path.exists(redist_path):
                 redist_path = os.path.split(redist_path)[0]
                 tools_version = None
 
                 for version in os.listdir(redist_path):
                     if not os.path.isdir(
-                            os.path.join(redist_path, version)
+                        os.path.join(redist_path, version)
                     ):
                         continue
 
                     if version.startswith('v'):
                         continue
 
                     if self._strict_toolkit_version is not None:
@@ -1295,16 +1336,16 @@
                 else:
                     self._tools_redist_directory = ''
 
             else:
                 self._tools_redist_directory = redist_path
 
             if (
-                    self._tools_redist_directory and
-                    not self._tools_redist_directory.endswith('\\')
+                self._tools_redist_directory and
+                not self._tools_redist_directory.endswith('\\')
             ):
                 self._tools_redist_directory += '\\'
 
         return self._tools_redist_directory
 
     @property
     def tools_install_directory(self) -> Optional[str]:
@@ -1314,16 +1355,16 @@
         Gets set to the VCToolsInstallDir environment variable.
         Gets added to the INCLUDE, LIBPATH, LIB and PATH environment variables.
 
         :rtype: Optional, str
         :return: Path to the compiler tools or `None`
         """
         if self._tools_install_directory is None:
-
             vc_version = float(int(self.version.split('.')[0]))
+
             if vc_version >= 14.0:
                 vc_tools_path = self._installed_c_paths[vc_version]['root']
             else:
                 vc_tools_path = self._installed_c_paths[vc_version]['base']
 
             # lib_path = os.path.join(vc_tools_path, 'lib')
             tools_path = os.path.join(vc_tools_path, 'Tools', 'MSVC')
@@ -1842,17 +1883,17 @@
             atlmfc_path=self.atlmfc_path,
         )
 
 
 class VisualStudioInfo(object):
 
     def __init__(
-            self,
-            environ: "Environment",
-            c_info: VisualCInfo
+        self,
+        environ: "Environment",
+        c_info: VisualCInfo
     ):
         self.environment = environ
         self.__devenv_version = None
         self.c_info = c_info
         self._install_directory = None
         self._dev_env_directory = None
         self._common_tools = None
@@ -2100,31 +2141,18 @@
         env = dict(
             Path=self.path,
             VSINSTALLDIR=install_directory,
             DevEnvDir=dev_env_directory,
             VisualStudioVersion=self.version
         )
 
-        toolsets = {
-            'v142': '160',
-            'v141': '150',
-            'v140': '140',
-            'v120': '120',
-            'v110': '110',
-            'v100': '100',
-            'v90': '90'
-        }
-
-        toolset_version = self.c_info.toolset_version
-
-        if toolset_version in toolsets:
-            comn_tools = 'VS{0}COMNTOOLS'.format(
-                toolsets[toolset_version]
-            )
-            env[comn_tools] = self.common_tools
+        comn_tools = 'VS{0}COMNTOOLS'.format(
+            str(int(self.version * 10))
+        )
+        env[comn_tools] = self.common_tools
 
         for key, value in env.items():
             if value is not None and value:
                 if isinstance(value, list):
                     value = os.pathsep.join(value)
                 yield key, str(value)
 
@@ -3933,39 +3961,14 @@
             'This script will only work with a Windows opperating system.'
         )
 
     logger.debug(
         'Setting up Windows build environment, please wait.....'
     )
 
-    python_version = sys.version_info[:2]
-    if minimum_c_version is None:
-        if python_version == (3, 12):
-            minimum_c_version = 14.3
-        elif python_version == (3, 11):
-            minimum_c_version = 14.3
-        elif python_version == (3, 10):
-            minimum_c_version = 14.2
-        elif python_version == (3, 9):
-            minimum_c_version = 14.2
-        elif python_version == (3, 8):
-            minimum_c_version = 14.0
-        elif python_version == (3, 7):
-            minimum_c_version = 14.0
-        elif python_version == (3, 6):
-            minimum_c_version = 14.0
-        elif python_version == (3, 5):
-            minimum_c_version = 12.0
-        elif python_version == (3, 4):
-            minimum_c_version = 12.0
-        else:
-            raise RuntimeError(
-                'Python version not supported'
-            )
-
     environment = Environment(
         minimum_c_version,
         strict_c_version,
         minimum_toolkit_version,
         strict_toolkit_version,
         minimum_sdk_version,
         strict_sdk_version,
```

### Comparing `pyMSVC-0.5.2/pyMSVC/vswhere.py` & `pyMSVC-0.5.3/pyMSVC/vswhere.py`

 * *Files identical despite different names*

### Comparing `pyMSVC-0.5.2/setup.py` & `pyMSVC-0.5.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 
 from setuptools import setup
 
 
 setup(
     name='pyMSVC',
-    version='0.5.2',
+    version='0.5.3',
     url='https://github.com/kdschlosser/python_msvc',
     packages=['pyMSVC'],
     author='Kevin Schlosser',
     description='Simple to use MSVC build environment setup tool.',
     long_description=(
         'Distutils and setup tools not working properly to compile on Windows?\n'
         'Tired of having a new visual studio version break your setup program?\n'
```

