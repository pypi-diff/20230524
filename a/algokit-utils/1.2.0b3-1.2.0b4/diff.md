# Comparing `tmp/algokit_utils-1.2.0b3-py3-none-any.whl.zip` & `tmp/algokit_utils-1.2.0b4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 34339 bytes, number of entries: 15
+Zip file size: 34345 bytes, number of entries: 15
 -rw-r--r--  2.0 unx     4091 b- defN 80-Jan-01 00:00 algokit_utils/__init__.py
 -rw-r--r--  2.0 unx     4410 b- defN 80-Jan-01 00:00 algokit_utils/_ensure_funded.py
 -rw-r--r--  2.0 unx     3569 b- defN 80-Jan-01 00:00 algokit_utils/_transfer.py
 -rw-r--r--  2.0 unx     7364 b- defN 80-Jan-01 00:00 algokit_utils/account.py
 -rw-r--r--  2.0 unx    54130 b- defN 80-Jan-01 00:00 algokit_utils/application_client.py
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_utils/application_specification.py
--rw-r--r--  2.0 unx    34159 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
+-rw-r--r--  2.0 unx    34168 b- defN 80-Jan-01 00:00 algokit_utils/deploy.py
 -rw-r--r--  2.0 unx     2000 b- defN 80-Jan-01 00:00 algokit_utils/logic_error.py
 -rw-r--r--  2.0 unx     5876 b- defN 80-Jan-01 00:00 algokit_utils/models.py
 -rw-r--r--  2.0 unx     4841 b- defN 80-Jan-01 00:00 algokit_utils/network_clients.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_utils/py.typed
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b3.dist-info/LICENSE
--rw-r--r--  2.0 unx     2037 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b3.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b3.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b3.dist-info/RECORD
-15 files, 132370 bytes uncompressed, 32247 bytes compressed:  75.6%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     2038 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1263 b- defN 16-Jan-01 00:00 algokit_utils-1.2.0b4.dist-info/RECORD
+15 files, 132380 bytes uncompressed, 32253 bytes compressed:  75.6%
```

## zipnote {}

```diff
@@ -27,20 +27,20 @@
 
 Filename: algokit_utils/network_clients.py
 Comment: 
 
 Filename: algokit_utils/py.typed
 Comment: 
 
-Filename: algokit_utils-1.2.0b3.dist-info/LICENSE
+Filename: algokit_utils-1.2.0b4.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_utils-1.2.0b3.dist-info/METADATA
+Filename: algokit_utils-1.2.0b4.dist-info/METADATA
 Comment: 
 
-Filename: algokit_utils-1.2.0b3.dist-info/WHEEL
+Filename: algokit_utils-1.2.0b4.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_utils-1.2.0b3.dist-info/RECORD
+Filename: algokit_utils-1.2.0b4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_utils/deploy.py

```diff
@@ -369,15 +369,15 @@
     return None
 
 
 def _strip_comment(line: str) -> str:
     comment_idx = _find_unquoted_string(line, "//")
     if comment_idx is None:
         return line
-    return line[:comment_idx]
+    return line[:comment_idx].rstrip()
 
 
 def strip_comments(program: str) -> str:
     return "\n".join(_strip_comment(line) for line in program.splitlines())
 
 
 def _has_token(program_without_comments: str, token: str) -> bool:
```

## Comparing `algokit_utils-1.2.0b3.dist-info/LICENSE` & `algokit_utils-1.2.0b4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_utils-1.2.0b3.dist-info/METADATA` & `algokit_utils-1.2.0b4.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: algokit-utils
-Version: 1.2.0b3
+Version: 1.2.0b4
 Summary: Utilities for Algorand development for use by AlgoKit
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: py-algorand-sdk (>=2,<3)
+Requires-Dist: py-algorand-sdk (==2.1.2)
 Description-Content-Type: text/markdown
 
 # AlgoKit Python Utilities
 
 A set of core Algorand utilities written in Python and released via PyPi that make it easier to build solutions on Algorand. 
 This project is part of [AlgoKit](https://github.com/algorandfoundation/algokit-cli).
```

## Comparing `algokit_utils-1.2.0b3.dist-info/RECORD` & `algokit_utils-1.2.0b4.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 algokit_utils/__init__.py,sha256=wuh-p9PubCj9Bj2tpxP3tQ5qZPs_nUHzB16BHi9Aq2c,4091
 algokit_utils/_ensure_funded.py,sha256=DjwGnCC_6USLQV5wIMJZRVQFlQ1uLrGDMxRF471atsQ,4410
 algokit_utils/_transfer.py,sha256=K8TMoaFcZE74xZ1rhp1De0Ri4mg8vs8pu-iJLOa5WoE,3569
 algokit_utils/account.py,sha256=UIuOQZe28pQxjEP9TzhtYlOU20tUdzzS-nIIZM9Bp6Y,7364
 algokit_utils/application_client.py,sha256=zeoPAIYhUq2PLrWzRmLFGjVyFFcpYiXekJ3t_sPqlpM,54130
 algokit_utils/application_specification.py,sha256=XusOe7VrGPun2UoNspC9Ei202NzPkxRNx5USXiABuXc,7466
-algokit_utils/deploy.py,sha256=fcG7bZf-GIV37U1R3UdkrcqeUhvtzjOzGuPeXPVdnZA,34159
+algokit_utils/deploy.py,sha256=UmVlJ-0vo91EjPXRC1EjkFBh5frJ0R4nCnlyZABhcRg,34168
 algokit_utils/logic_error.py,sha256=IxsAGS11kuFhPhEHvhheZamQ2KQxb3LQdxiTOvnKKAA,2000
 algokit_utils/models.py,sha256=1IXNhibqtZ7cmuH31mLvNLcpJzaMl9lOD0EqsTPyglU,5876
 algokit_utils/network_clients.py,sha256=0cbUHCEWycFnduEu5cJ4dY6pfDOOzvHO1cXmcxAe83M,4841
 algokit_utils/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-algokit_utils-1.2.0b3.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
-algokit_utils-1.2.0b3.dist-info/METADATA,sha256=338OJjNy7XdntHo2yASZT0PTMrV8ZVXJYubQXY_5E04,2037
-algokit_utils-1.2.0b3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-algokit_utils-1.2.0b3.dist-info/RECORD,,
+algokit_utils-1.2.0b4.dist-info/LICENSE,sha256=J5i7U1Q9Q2c7saUzlvFRmrCCFhQyXb5Juz_LO5omNUw,1076
+algokit_utils-1.2.0b4.dist-info/METADATA,sha256=2QI6lw0DKnJwcJhTw-E51sTmgmbS8L4foQbexmhKMo0,2038
+algokit_utils-1.2.0b4.dist-info/WHEEL,sha256=WGfLGfLX43Ei_YORXSnT54hxFygu34kMpcQdmgmEwCQ,88
+algokit_utils-1.2.0b4.dist-info/RECORD,,
```

