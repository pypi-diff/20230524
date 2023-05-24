# Comparing `tmp/py-bsdauth-1.1.1.tar.gz` & `tmp/py-bsdauth-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/py-bsdauth-1.1.1.tar", last modified: Wed Jan 20 16:16:13 2021, max compression
+gzip compressed data, was "py-bsdauth-1.1.2.tar", last modified: Wed May 24 04:11:58 2023, max compression
```

## Comparing `py-bsdauth-1.1.1.tar` & `py-bsdauth-1.1.2.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 pogi      (1000) pogi      (1000)        0 2021-01-20 16:16:13.001296 py-bsdauth-1.1.1/
--rw-r--r--   0 pogi      (1000) pogi      (1000)        0 2021-01-14 20:19:11.000000 py-bsdauth-1.1.1/MANIFEST.in
--rw-r--r--   0 pogi      (1000) pogi      (1000)     1170 2021-01-20 16:16:13.001296 py-bsdauth-1.1.1/PKG-INFO
--rw-r--r--   0 pogi      (1000) pogi      (1000)      554 2021-01-17 18:33:00.000000 py-bsdauth-1.1.1/README.md
-drwxr-xr-x   0 pogi      (1000) pogi      (1000)        0 2021-01-20 16:16:12.993171 py-bsdauth-1.1.1/bsdauth/
--rw-r--r--   0 pogi      (1000) pogi      (1000)       22 2021-01-20 16:15:36.000000 py-bsdauth-1.1.1/bsdauth/__init__.py
--rw-r--r--   0 pogi      (1000) pogi      (1000)     3342 2021-01-17 14:57:56.000000 py-bsdauth-1.1.1/bsdauth/bsdauth.py
-drwxr-xr-x   0 pogi      (1000) pogi      (1000)        0 2021-01-20 16:16:12.993171 py-bsdauth-1.1.1/py_bsdauth.egg-info/
--rw-r--r--   0 pogi      (1000) pogi      (1000)     1170 2021-01-20 16:16:12.000000 py-bsdauth-1.1.1/py_bsdauth.egg-info/PKG-INFO
--rw-r--r--   0 pogi      (1000) pogi      (1000)      205 2021-01-20 16:16:12.000000 py-bsdauth-1.1.1/py_bsdauth.egg-info/SOURCES.txt
--rw-r--r--   0 pogi      (1000) pogi      (1000)        1 2021-01-20 16:16:12.000000 py-bsdauth-1.1.1/py_bsdauth.egg-info/dependency_links.txt
--rw-r--r--   0 pogi      (1000) pogi      (1000)        8 2021-01-20 16:16:12.000000 py-bsdauth-1.1.1/py_bsdauth.egg-info/top_level.txt
--rw-r--r--   0 pogi      (1000) pogi      (1000)       38 2021-01-20 16:16:13.001296 py-bsdauth-1.1.1/setup.cfg
--rw-r--r--   0 pogi      (1000) pogi      (1000)      774 2021-01-20 16:15:36.000000 py-bsdauth-1.1.1/setup.py
+drwxr-xr-x   0 eking     (1000) eking     (1000)        0 2023-05-24 04:11:58.620709 py-bsdauth-1.1.2/
+-rw-r--r--   0 eking     (1000) eking     (1000)      749 2023-05-24 00:06:11.000000 py-bsdauth-1.1.2/LICENSE
+-rw-r--r--   0 eking     (1000) eking     (1000)        0 2023-05-24 00:06:11.000000 py-bsdauth-1.1.2/MANIFEST.in
+-rw-r--r--   0 eking     (1000) eking     (1000)      965 2023-05-24 04:11:58.620709 py-bsdauth-1.1.2/PKG-INFO
+-rw-r--r--   0 eking     (1000) eking     (1000)      556 2023-05-24 04:11:47.000000 py-bsdauth-1.1.2/README.md
+drwxr-xr-x   0 eking     (1000) eking     (1000)        0 2023-05-24 04:11:58.620709 py-bsdauth-1.1.2/bsdauth/
+-rw-r--r--   0 eking     (1000) eking     (1000)       22 2023-05-24 00:06:11.000000 py-bsdauth-1.1.2/bsdauth/__init__.py
+-rw-r--r--   0 eking     (1000) eking     (1000)     3213 2023-05-24 01:23:13.000000 py-bsdauth-1.1.2/bsdauth/bsdauth.py
+drwxr-xr-x   0 eking     (1000) eking     (1000)        0 2023-05-24 04:11:58.620709 py-bsdauth-1.1.2/py_bsdauth.egg-info/
+-rw-r--r--   0 eking     (1000) eking     (1000)      965 2023-05-24 04:11:58.000000 py-bsdauth-1.1.2/py_bsdauth.egg-info/PKG-INFO
+-rw-r--r--   0 eking     (1000) eking     (1000)      213 2023-05-24 04:11:58.000000 py-bsdauth-1.1.2/py_bsdauth.egg-info/SOURCES.txt
+-rw-r--r--   0 eking     (1000) eking     (1000)        1 2023-05-24 04:11:58.000000 py-bsdauth-1.1.2/py_bsdauth.egg-info/dependency_links.txt
+-rw-r--r--   0 eking     (1000) eking     (1000)        8 2023-05-24 04:11:58.000000 py-bsdauth-1.1.2/py_bsdauth.egg-info/top_level.txt
+-rw-r--r--   0 eking     (1000) eking     (1000)       38 2023-05-24 04:11:58.620709 py-bsdauth-1.1.2/setup.cfg
+-rw-r--r--   0 eking     (1000) eking     (1000)      774 2023-05-24 01:26:56.000000 py-bsdauth-1.1.2/setup.py
```

### Comparing `py-bsdauth-1.1.1/bsdauth/bsdauth.py` & `py-bsdauth-1.1.2/bsdauth/bsdauth.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,17 +12,14 @@
 WHATSOEVER RESULTING FROM LOSS OF USE, DATA OR PROFITS, WHETHER IN AN
 ACTION OF CONTRACT, NEGLIGENCE OR OTHER TORTIOUS ACTION, ARISING OUT OF
 OR IN CONNECTION WITH THE USE OR PERFORMANCE OF THIS SOFTWARE.
 """
 from ctypes import CDLL, c_char_p
 import os, pwd, re
 
-def _get_username():
-    return pwd.getpwuid( os.getuid() )[ 0 ]
-
 
 class Validator(object):
     def is_username_valid(self, username):
         """
            Validate username based on OpenBSD's passwd(5) username specs.
         """
         if re.search('^[a-z]+[0-9|\-|_|a-z]+$', username) and len(username) <= 31:
@@ -66,17 +63,14 @@
         """
             Using OpenBSD's auth_userokay(3) from libc BSD Auth api. auth_userokay(3)
             deletes the password from memory for security reasons. Be sure to
             instanciate this class every after self.login() call if you need to login
             again. If calling process is not owned by root return None. root privilege 
             is required by BSD Auth.
         """
-        if _get_username() != 'root':
-            return None
-
         sofile = '/usr/lib/libc.so*'
         authstyle = c_char_p()
         authstyle.value = str.encode('passwd')
         authtype = c_char_p()
         authtype.value = str.encode('auth-python')
         auth = CDLL(sofile)
         ret = auth.auth_userokay(self.username, authstyle, authtype, self.password)
```

### Comparing `py-bsdauth-1.1.1/setup.py` & `py-bsdauth-1.1.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="py-bsdauth",
-    version="1.1.1",
+    version="1.1.2",
     description="Python interface to OpenBSD's BSD Auth.",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/rbaylon/py-bsdauth",
     author="Ricardo Baylon",
     author_email="rbaylon@outlook.com",
     license="ISC",
```

