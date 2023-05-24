# Comparing `tmp/cryptbuddy-0.0.1.tar.gz` & `tmp/cryptbuddy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cryptbuddy-0.0.1.tar", max compression
+gzip compressed data, was "cryptbuddy-0.0.5.tar", max compression
```

## Comparing `cryptbuddy-0.0.1.tar` & `cryptbuddy-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0        0 2023-05-17 10:45:49.638052 cryptbuddy-0.0.1/README.md
--rw-r--r--   0        0        0        0 2023-05-17 10:45:49.638052 cryptbuddy-0.0.1/cryptbuddy/__init__.py
--rw-r--r--   0        0        0     1621 2023-05-17 10:54:07.284159 cryptbuddy-0.0.1/cryptbuddy/commands/chain.py
--rw-r--r--   0        0        0     2371 2023-05-17 10:54:01.561146 cryptbuddy-0.0.1/cryptbuddy/commands/symmetric.py
--rw-r--r--   0        0        0      471 2023-05-17 10:53:02.995015 cryptbuddy-0.0.1/cryptbuddy/cryptlib/constants.py
--rw-r--r--   0        0        0     1598 2023-05-17 10:53:06.696024 cryptbuddy-0.0.1/cryptbuddy/cryptlib/decrypt.py
--rw-r--r--   0        0        0     1949 2023-05-17 10:53:10.443032 cryptbuddy-0.0.1/cryptbuddy/cryptlib/encrypt.py
--rw-r--r--   0        0        0     1463 2023-05-17 10:53:22.552059 cryptbuddy-0.0.1/cryptbuddy/cryptlib/file_io.py
--rw-r--r--   0        0        0     1822 2023-05-17 10:53:43.696106 cryptbuddy-0.0.1/cryptbuddy/cryptlib/initialize.py
--rw-r--r--   0        0        0     5882 2023-05-17 10:53:47.589115 cryptbuddy-0.0.1/cryptbuddy/cryptlib/key_io.py
--rw-r--r--   0        0        0     2461 2023-05-17 10:52:19.281918 cryptbuddy-0.0.1/cryptbuddy/cryptlib/keychain.py
--rw-r--r--   0        0        0     1873 2023-05-17 10:52:51.046989 cryptbuddy-0.0.1/cryptbuddy/cryptlib/symmetric/decrypt.py
--rw-r--r--   0        0        0     1989 2023-05-17 10:52:56.266001 cryptbuddy-0.0.1/cryptbuddy/cryptlib/symmetric/encrypt.py
--rw-r--r--   0        0        0      812 2023-05-17 10:45:49.638052 cryptbuddy-0.0.1/cryptbuddy/cryptlib/utils.py
--rw-r--r--   0        0        0     4021 2023-05-17 10:52:24.904931 cryptbuddy-0.0.1/cryptbuddy/main.py
--rw-r--r--   0        0        0      533 2023-05-17 11:07:58.842002 cryptbuddy-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1029 1970-01-01 00:00:00.000000 cryptbuddy-0.0.1/setup.py
--rw-r--r--   0        0        0      690 1970-01-01 00:00:00.000000 cryptbuddy-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-17 10:45:49.638052 cryptbuddy-0.0.5/README.md
+-rw-r--r--   0        0        0        0 2023-05-17 10:45:49.638052 cryptbuddy-0.0.5/cryptbuddy/__init__.py
+-rw-r--r--   0        0        0     1421 2023-05-24 17:08:12.062333 cryptbuddy-0.0.5/cryptbuddy/commands/chain.py
+-rw-r--r--   0        0        0     3933 2023-05-24 20:04:22.660063 cryptbuddy-0.0.5/cryptbuddy/commands/symmetric.py
+-rw-r--r--   0        0        0      493 2023-05-24 14:18:12.157084 cryptbuddy-0.0.5/cryptbuddy/lib/constants.py
+-rw-r--r--   0        0        0     2880 2023-05-24 14:18:31.655130 cryptbuddy-0.0.5/cryptbuddy/lib/decrypt.py
+-rw-r--r--   0        0        0     2660 2023-05-24 15:12:39.102046 cryptbuddy-0.0.5/cryptbuddy/lib/encrypt.py
+-rw-r--r--   0        0        0     2550 2023-05-24 17:16:31.899481 cryptbuddy-0.0.5/cryptbuddy/lib/file_io.py
+-rw-r--r--   0        0        0     2451 2023-05-24 14:56:28.402912 cryptbuddy-0.0.5/cryptbuddy/lib/initialize.py
+-rw-r--r--   0        0        0     9515 2023-05-24 14:58:42.689204 cryptbuddy-0.0.5/cryptbuddy/lib/key_io.py
+-rw-r--r--   0        0        0     3955 2023-05-24 15:29:23.587277 cryptbuddy-0.0.5/cryptbuddy/lib/keychain.py
+-rw-r--r--   0        0        0     2514 2023-05-24 14:18:59.922197 cryptbuddy-0.0.5/cryptbuddy/lib/symmetric/decrypt.py
+-rw-r--r--   0        0        0     2659 2023-05-24 14:19:14.087230 cryptbuddy-0.0.5/cryptbuddy/lib/symmetric/encrypt.py
+-rw-r--r--   0        0        0     2718 2023-05-24 15:27:18.793000 cryptbuddy-0.0.5/cryptbuddy/lib/utils.py
+-rw-r--r--   0        0        0     6072 2023-05-24 17:18:09.220705 cryptbuddy-0.0.5/cryptbuddy/main.py
+-rw-r--r--   0        0        0      609 2023-05-24 20:16:42.129943 cryptbuddy-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1044 1970-01-01 00:00:00.000000 cryptbuddy-0.0.5/setup.py
+-rw-r--r--   0        0        0      729 1970-01-01 00:00:00.000000 cryptbuddy-0.0.5/PKG-INFO
```

### Comparing `cryptbuddy-0.0.1/cryptbuddy/commands/chain.py` & `cryptbuddy-0.0.5/cryptbuddy/commands/chain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,62 +1,54 @@
 from pathlib import Path
 from typing import Optional
 
 import typer
-from cryptbuddy.cryptlib.key_io import AppPublicKey
-from cryptbuddy.cryptlib.keychain import keychain
-from cryptbuddy.cryptlib.utils import *
+from cryptbuddy.lib.key_io import AppPublicKey
+from cryptbuddy.lib.keychain import Keychain
+from cryptbuddy.lib.utils import *
 from typing_extensions import Annotated
 
 app = typer.Typer()
-chain = keychain()
+chain = Keychain()
 
 
 @app.command()
-def add(key: Annotated[Path, typer.Option(help="Public key file path")]):
+def add(key: Annotated[Path, typer.Argument(help="Path to the public key", exists=True, file_okay=True, dir_okay=False, readable=True, resolve_path=True)]):
     """
     Add a key to your keychain
     """
-    if not key.exists():
-        error("File not found")
 
-    # Create the public key object from file
     public_key = AppPublicKey.from_file(key)
 
-    # Add the packed key to the keychain
-    chain.add_key(public_key.meta.name, public_key.packed)
+    chain.add_key(public_key)
     success(f"{public_key.meta.name}'s public key added to the keychain")
 
 
 @app.command()
-def delete(name: Annotated[Optional[str], typer.Option(help="Name of the user whose public key to delete")] = None,
+def delete(name: Annotated[Optional[str], typer.Argument(help="Name of the user whose public key to delete")] = None,
            id: Annotated[Optional[int], typer.Option(help="ID of the public key to delete")] = None):
     """
     Delete a key from your keychain
     """
     if not name and not id:
         error("Please specify either name or ID")
 
-    # Delete the key from the keychain
     if id:
         chain.delete_key(id=id)
         success(f"Key with ID {id} deleted from the keychain")
     else:
         chain.delete_key(name=name)
 
     success(f"{name}'s public key deleted from the keychain")
 
 
 @app.command()
 def list():
     """
     List all the keys in your keychain
     """
-    # Get the names of all the keys
     keys = chain.get_names()
-
-    # Print the table
     print_table(keys, [['ID', 'Name']])
 
 
 if __name__ == "__main__":
     app()
```

### Comparing `cryptbuddy-0.0.1/cryptbuddy/cryptlib/decrypt.py` & `cryptbuddy-0.0.5/cryptbuddy/lib/decrypt.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,48 +1,90 @@
 from pathlib import Path
+from typing import List
 
-from cryptbuddy.cryptlib.file_io import cache_dir, shred_file
-from cryptbuddy.cryptlib.key_io import AppPrivateKey
-from cryptbuddy.cryptlib.symmetric.decrypt import symmetric_decrypt
+from cryptbuddy.lib.constants import *
+from cryptbuddy.lib.file_io import cache_dir, shred_file
+from cryptbuddy.lib.key_io import AppPrivateKey
+from cryptbuddy.lib.symmetric.decrypt import symmetric_decrypt
+from cryptbuddy.lib.utils import info
 from msgpack import loads
 from nacl.public import SealedBox
 
 
-def asymmetric_decrypt(file: Path, password: str, private_key_object: AppPrivateKey):
+def asymmetric_decrypt(file: Path, password: str, private_key_object: AppPrivateKey) -> List[bytes]:
     """
-    Returns the decrypted chunks. `file` is the file to be 
-    decrypted. `password` is the password of your private key. 
-    `private_key_object` is the private key object.
+    Decrypts a file asymmetrically a private key. The file must have been encrypted using the corresponding
+    `asymmetric_encrypt` function.
+
+    Parameters
+    ----------
+    file : `Path`
+        The path to the file to be decrypted.
+    password : `str`
+        The password used for decryption.
+    private_key_object : `AppPrivateKey`
+        The private key object used for decryption.
+
+    Returns
+    -------
+    `List[bytes]`
+        A list of decrypted data chunks.
+
+    Raises
+    ------
+    `ValueError`
+        If the delimiter is not found or is preceded by an escape sequence.
+    `Exception`
+        If an error occurs during decryption.
+
+    Notes
+    -----
+    The file must have been encrypted using the corresponding `asymmetric_encrypt` function.
+
     """
 
+    info(f"Decrypting {file}")
+
     # Get the decrypted NaCl private key object
     name = private_key_object.meta.name
     private_key = private_key_object.decrypted_key(password)
 
-    # Create a sealed box with the private key
     unseal_box = SealedBox(private_key)
 
     # Read the serialized keys before the first newline
     with open(file, "rb") as infile:
-        contents = infile.read()
-        newline_index = contents.index(b'\n')
-        packed_keys = contents[:newline_index]
-        encrypted_chunks = contents[newline_index+1:]
+        file_data = infile.read()
+
+    # Find the index of the first delimiter
+    delimiter_index = file_data.find(delimiter)
+    while delimiter_index > 0 and file_data[delimiter_index - len(escape_sequence):delimiter_index] == escape_sequence:
+        # The delimiter is part of the packed keys, search for the next occurrence
+        delimiter_index = file_data.find(delimiter, delimiter_index + 1)
+
+    if delimiter_index == -1:
+        raise ValueError("Delimiter not found or preceded by escape sequence")
+
+    packed_keys = file_data[:delimiter_index]
+    encrypted_chunks = file_data[delimiter_index + len(delimiter):]
+
+    # Process the escape sequences within the packed keys
+    packed_keys = packed_keys.replace(escape_sequence + delimiter, delimiter)
 
-    # Decrypt the symmetric key using your private key
     keys = loads(packed_keys)
     my_key = keys[name]
     symmetric_key = unseal_box.decrypt(my_key)
 
     # Store the encrypted chunks to a temporary file
-    tmp = Path(f"{cache_dir}/{str(file)}")
+    tmp = Path(f"{cache_dir}/{str(file.name)}")
     with open(tmp, "wb") as infile:
         infile.write(encrypted_chunks)
 
-    # Decrypt the file using the symmetric key
-    chunks = symmetric_decrypt(tmp, key=symmetric_key)
+    try:
+        # Decrypt the file using the symmetric key
+        chunks = symmetric_decrypt(tmp, key=symmetric_key)
+    except Exception as e:
+        raise Exception("Error decrypting file") from e
 
     # Shred the temporary file
     shred_file(tmp)
 
-    # Return the decrypted chunks
     return chunks
```

### Comparing `cryptbuddy-0.0.1/cryptbuddy/cryptlib/encrypt.py` & `cryptbuddy-0.0.5/cryptbuddy/lib/encrypt.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,58 @@
 from pathlib import Path
+from typing import List
 
-from cryptbuddy.cryptlib.constants import *
-from cryptbuddy.cryptlib.key_io import AppPublicKey
-from cryptbuddy.cryptlib.keychain import keychain
-from cryptbuddy.cryptlib.symmetric.encrypt import symmetric_encrypt
+from cryptbuddy.lib.constants import *
+from cryptbuddy.lib.key_io import AppPublicKey
+from cryptbuddy.lib.keychain import Keychain
+from cryptbuddy.lib.symmetric.encrypt import symmetric_encrypt
+from cryptbuddy.lib.utils import *
 from msgpack import dumps
 from nacl import utils
 from nacl.public import PublicKey, SealedBox
 
 
-def asymmetric_encrypt(user: list, file: Path):
+def asymmetric_encrypt(users: List[str], file: Path) -> List[bytes]:
     """
-    Returns asymmetrically encrypted chunks. `user` is a list of 
-    usernames whose public keys will be used to encrypt the file. 
-    `file` is the file to be encrypted.
+    Encrypts a file asymmetrically for multiple users. This function generates 
+    a random symmetric key, encrypts it with the public keys of the specified 
+    users, and stores the encrypted symmetric keys in the file. The file is then 
+    symmetrically encrypted using the symmetric key, and the encrypted symmetric 
+    keys are stored in the file as well.
+
+    Parameters
+    ----------
+    users : `List[str]`
+        The list of users for whom the file is encrypted.
+    file : `Path`
+        The path to the file to be encrypted.
+
+    Returns
+    -------
+    `List[bytes]`
+        A list of encrypted data chunks.
+
+    Raises
+    ------
+    `Exception`
+        If no public keys are found.
+
+    Notes
+    -----
+    The file must be decrypted using the corresponding `asymmetric_decrypt` function.
+
     """
 
-    # Initialize the keychain
-    db = keychain()
+    info(f"Encrypting {file} for {users}")
+
+    db = Keychain()
 
-    # Get the public keys of the users from the keychain
     public_keys_packed = []
-    for u in user:
-        public_keys_packed.append(db.get_key(name=u))
+    for u in users:
+        public_keys_packed.append(db.get_key(name=u).packed)
     if len(public_keys_packed) == 0:
         raise Exception("No public keys found")
 
     # Deserialize the public keys
     public_keys = {}
     for key in public_keys_packed:
         unpacked_key = AppPublicKey.from_packed(key)
@@ -45,14 +71,14 @@
         encrypted = sealed_box.encrypt(symmetric_key)
         encrypted_symmetric_keys[name] = encrypted
 
     # Encrypt the file symmetrically with the symmetric key
     chunks = symmetric_encrypt(file, key=symmetric_key)
 
     # Serialize the encrypted symmetric keys and prepend it
-    # using a newline
+    # using a delimiter
     packed_keys = dumps(encrypted_symmetric_keys)
-    chunks.insert(0, b'\n')
+    packed_keys = packed_keys.replace(delimiter, escape_sequence + delimiter)
+    chunks.insert(0, delimiter)
     chunks.insert(0, packed_keys)
 
-    # Return the encrypted chunks
     return chunks
```

### Comparing `cryptbuddy-0.0.1/cryptbuddy/cryptlib/symmetric/decrypt.py` & `cryptbuddy-0.0.5/cryptbuddy/lib/symmetric/decrypt.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,52 @@
 from pathlib import Path
+from typing import List
 
-from cryptbuddy.cryptlib.constants import *
+from cryptbuddy.lib.constants import *
+from cryptbuddy.lib.utils import info
 from nacl import pwhash, secret
 from nacl.bindings import sodium_increment
 
 
-def symmetric_decrypt(file: Path, password: str = None, key: bytes = None) -> bytelist:
+def symmetric_decrypt(file: Path, password: str = None, key: bytes = None) -> List[bytes]:
     """
-    Returns the decrypted chunks after symmetrically decrypting the file.
-    `file` is the file to be decrypted. `password` is the password to be
-    used to retrieve the key. `key` is the key to be used to decrypt the
-    file. Either `password` or `key` must be provided.
+    Decrypts a file symmetrically using a password or key.
+
+    Parameters
+    ----------
+    file : `Path`
+        The path to the file to be decrypted.
+    password : `str`, optional
+        The password used for decryption (default is `None`).
+    key : `bytes`, optional
+        The key used for decryption (default is `None`).
+
+    Returns
+    -------
+    `List[bytes]`
+        A list of decrypted data chunks.
+
+    Raises
+    ------
+    `FileNotFoundError`
+        If the specified file does not exist.
+    `ValueError`
+        If neither a password nor a key is provided.
+    `Exception`
+        If an error occurs during decryption.
+
+    Note
+    -----
+    This function is used to decrypt files that were symmetrically encrypted
+    using the `symmetric_encrypt` function.
+
     """
 
-    # Check if the file exists and if the password or key is provided
+    info(f"Decrypting {file} symmetrically")
+
     if not file.exists():
         raise FileNotFoundError("File does not exist")
     if not password and not key:
         raise ValueError("Password or key must be provided")
 
     with open(file, "rb") as infile:
         outchunks = []
@@ -31,22 +60,24 @@
         mem = int(encodedMem.decode(encoding='UTF-8'))
 
         # Generate the key from the password if not already provided
         if not key:
             key = kdf(keysize, password.encode(),
                       salt, opslimit=ops, memlimit=mem)
 
-        # Create the box
         box = secret.SecretBox(key)
         _newline = infile.read(1)
 
         # Decrypt the file data in chunks of given size
         while 1:
             rchunk = infile.read(chunksize + macsize)
             if len(rchunk) == 0:
                 break
-            dchunk = box.decrypt(rchunk, nonce)
+            try:
+                dchunk = box.decrypt(rchunk, nonce)
+            except Exception as e:
+                raise Exception("Error during decryption") from e
             assert len(dchunk) == len(rchunk) - macsize
             outchunks.append(dchunk)
             nonce = sodium_increment(nonce)
 
     return outchunks
```

### Comparing `cryptbuddy-0.0.1/pyproject.toml` & `cryptbuddy-0.0.5/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 [tool.poetry]
 name = "cryptbuddy"
-version = "0.0.1"
+version = "0.0.5"
 description = ""
 authors = ["Kush Patel <kush@kush.in>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 typer = {extras = ["all"], version = "^0.9.0"}
 PyNaCl = "^1.5.0"
 msgpack = "^1.0.5"
 password-strength = "^0.0.3.post2"
 appdirs = "^1.4.4"
 tabulate = "^0.9.0"
+pytest = "^7.3.1"
 
 [tool.poetry.scripts]
 cryptbuddy = "cryptbuddy.main:app"
 crypt = "cryptbuddy.main:app"
 cb = "cryptbuddy.main:app"
 
 
+[tool.poetry.group.dev.dependencies]
+autopep8 = "^2.0.2"
+
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `cryptbuddy-0.0.1/setup.py` & `cryptbuddy-0.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['cryptbuddy',
  'cryptbuddy.commands',
- 'cryptbuddy.cryptlib',
- 'cryptbuddy.cryptlib.symmetric']
+ 'cryptbuddy.lib',
+ 'cryptbuddy.lib.symmetric']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['PyNaCl>=1.5.0,<2.0.0',
  'appdirs>=1.4.4,<2.0.0',
  'msgpack>=1.0.5,<2.0.0',
  'password-strength>=0.0.3.post2,<0.0.4',
+ 'pytest>=7.3.1,<8.0.0',
  'tabulate>=0.9.0,<0.10.0',
  'typer[all]>=0.9.0,<0.10.0']
 
 entry_points = \
 {'console_scripts': ['cb = cryptbuddy.main:app',
                      'crypt = cryptbuddy.main:app',
                      'cryptbuddy = cryptbuddy.main:app']}
 
 setup_kwargs = {
     'name': 'cryptbuddy',
-    'version': '0.0.1',
+    'version': '0.0.5',
     'description': '',
     'long_description': '',
     'author': 'Kush Patel',
     'author_email': 'kush@kush.in',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cryptbuddy-0.0.1/PKG-INFO` & `cryptbuddy-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: cryptbuddy
-Version: 0.0.1
+Version: 0.0.5
 Summary: 
 Author: Kush Patel
 Author-email: kush@kush.in
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: PyNaCl (>=1.5.0,<2.0.0)
 Requires-Dist: appdirs (>=1.4.4,<2.0.0)
 Requires-Dist: msgpack (>=1.0.5,<2.0.0)
 Requires-Dist: password-strength (>=0.0.3.post2,<0.0.4)
+Requires-Dist: pytest (>=7.3.1,<8.0.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: typer[all] (>=0.9.0,<0.10.0)
 Description-Content-Type: text/markdown
```

