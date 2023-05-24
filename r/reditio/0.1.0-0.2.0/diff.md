# Comparing `tmp/reditio-0.1.0.tar.gz` & `tmp/reditio-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "reditio-0.1.0.tar", last modified: Sun May  7 06:11:40 2023, max compression
+gzip compressed data, was "reditio-0.2.0.tar", last modified: Wed May 24 07:06:06 2023, max compression
```

## Comparing `reditio-0.1.0.tar` & `reditio-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-07 06:11:40.883602 reditio-0.1.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-05-07 04:13:06.000000 reditio-0.1.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-07 06:11:40.883602 reditio-0.1.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1650 2023-05-07 06:03:32.000000 reditio-0.1.0/README.md
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-07 06:11:40.883602 reditio-0.1.0/reditio.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-07 06:11:40.000000 reditio-0.1.0/reditio.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      191 2023-05-07 06:11:40.000000 reditio-0.1.0/reditio.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-07 06:11:40.000000 reditio-0.1.0/reditio.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       29 2023-05-07 06:11:40.000000 reditio-0.1.0/reditio.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        8 2023-05-07 06:11:40.000000 reditio-0.1.0/reditio.egg-info/top_level.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3308 2023-05-07 06:11:07.000000 reditio-0.1.0/reditio.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-07 06:11:40.883602 reditio-0.1.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      741 2023-05-07 04:46:31.000000 reditio-0.1.0/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-24 07:06:06.802451 reditio-0.2.0/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-05-07 04:13:06.000000 reditio-0.2.0/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-24 07:06:06.802451 reditio-0.2.0/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1688 2023-05-07 06:13:23.000000 reditio-0.2.0/README.md
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-24 07:06:06.802451 reditio-0.2.0/reditio.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      572 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      191 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       29 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        8 2023-05-24 07:06:06.000000 reditio-0.2.0/reditio.egg-info/top_level.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3604 2023-05-24 07:04:37.000000 reditio-0.2.0/reditio.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-24 07:06:06.802451 reditio-0.2.0/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      741 2023-05-24 07:05:40.000000 reditio-0.2.0/setup.py
```

### Comparing `reditio-0.1.0/LICENSE` & `reditio-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `reditio-0.1.0/PKG-INFO` & `reditio-0.2.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reditio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple typed Python interface to Redis
 Home-page: https://github.com/MatthewScholefield/reditio
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 Keywords: reditio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `reditio-0.1.0/README.md` & `reditio-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,19 @@
 
 *A simple typed Python interface to Redis*
 
 Reditio is a Python library that provides a high-level, typed interface to Redis using Pydantic.
 
 ```python
 reditio = Reditio()
+
 users = reditio.hash('users', User)
 users.set('123', User(name='John'))
+users.set('124', User(name='Mary'))
+
 names = [user.name for user in users.getall().values()]
 print('Users:', ', '.join(names))
 ```
 
 ## Installation
 
 You can install Reditio using pip:
```

### Comparing `reditio-0.1.0/reditio.egg-info/PKG-INFO` & `reditio-0.2.0/reditio.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: reditio
-Version: 0.1.0
+Version: 0.2.0
 Summary: Simple typed Python interface to Redis
 Home-page: https://github.com/MatthewScholefield/reditio
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 Keywords: reditio
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `reditio-0.1.0/reditio.py` & `reditio-0.2.0/reditio.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,65 +20,70 @@
         if isinstance(value, bytes):
             return value.decode()
         return value
 
     def _parse_value(self, value: StrBytes) -> Optional[T]:
         if not value:
             return None
-        if BaseModel in self.model.__bases__:
+        if issubclass(self.model, BaseModel):
             return self.model.parse_raw(value)
+        if not issubclass(self.model, (str, bytes)):
+            raise RuntimeError(f'Invalid model type: {self.model}')
         return value
 
     def _serialize_value(self, value: T) -> StrBytes:
         if self.model is not str:
             return value.json()
         return value
 
 
-class RKey(RedisContainer[T]):
+class RKey(Generic[T], RedisContainer[T]):
     def get(self) -> Optional[T]:
         return self._parse_value(self.red.get(self.key))
 
     def set(self, value: T):
         serialized_value = self._serialize_value(value)
         self.red.set(self.key, serialized_value)
 
 
-class RList(RedisContainer[T]):
+class RList(Generic[T], RedisContainer[T]):
     def getrange(self, start: int, end: int) -> List[T]:
         return [
             self._parse_value(v) for v in self.red.lrange(self.key, start, end)
         ]
 
     def append(self, value: T):
         serialized_value = self._serialize_value(value)
         self.red.rpush(self.key, serialized_value)
 
+    def bpop(self, timeout=0) -> Optional[T]:
+        return self._parse_value(self.red.blpop(self.key, timeout))
 
-class RSet(RedisContainer[T]):
+
+class RSet(Generic[T], RedisContainer[T]):
     def members(self) -> list[T]:
         return [self._parse_value(v) for v in self.red.smembers(self.key)]
 
     def add(self, value: T):
         serialized_value = self._serialize_value(value)
         self.red.sadd(self.key, serialized_value)
 
 
-class RSortedSet(RedisContainer[T]):
+class RSortedSet(Generic[T], RedisContainer[T]):
     def getrange(self, start: int, end: int) -> List[T]:
         return [
             self._parse_value(v) for v in self.red.zrange(self.key, start, end)
         ]
 
     def add(self, value: T, score: float):
         serialized_value = self._serialize_value(value)
         self.red.zadd(self.key, {serialized_value: score})
 
 
-class RHash(RedisContainer[T]):
+class RHash(Generic[T], RedisContainer[T]):
     def getall(self) -> Dict[StrBytes, T]:
         raw_dict = self.red.hgetall(self.key)
         return {
             self._parse_key(k): self._parse_value(v)
             for k, v in raw_dict.items()
         }
```

### Comparing `reditio-0.1.0/setup.py` & `reditio-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='reditio',
-    version='0.1.0',
+    version='0.2.0',
     description='Simple typed Python interface to Redis',
     url='https://github.com/MatthewScholefield/reditio',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

