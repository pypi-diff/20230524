# Comparing `tmp/hashwire-0.0.1.tar.gz` & `tmp/hashwire-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hashwire-0.0.1.tar", last modified: Tue May 23 14:21:01 2023, max compression
+gzip compressed data, was "hashwire-0.0.2.tar", last modified: Wed May 24 11:28:38 2023, max compression
```

## Comparing `hashwire-0.0.1.tar` & `hashwire-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.301603 hashwire-0.0.1/
--rw-rw-rw-   0        0        0     1071 2023-05-23 09:09:27.000000 hashwire-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1956 2023-05-23 14:21:01.299602 hashwire-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      188 2023-05-23 09:12:24.000000 hashwire-0.0.1/README.md
--rw-rw-rw-   0        0        0      809 2023-05-23 14:19:33.000000 hashwire-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-23 14:21:01.302604 hashwire-0.0.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.269442 hashwire-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.283639 hashwire-0.0.1/src/hashwire/
--rw-rw-rw-   0        0        0        0 2023-05-23 14:08:00.000000 hashwire-0.0.1/src/hashwire/__init__.py
--rw-rw-rw-   0        0        0     4018 2023-05-23 08:00:11.000000 hashwire-0.0.1/src/hashwire/hash.py
-drwxrwxrwx   0        0        0        0 2023-05-23 14:21:01.297604 hashwire-0.0.1/src/hashwire.egg-info/
--rw-rw-rw-   0        0        0     1956 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      222 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 14:21:01.000000 hashwire-0.0.1/src/hashwire.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-24 11:28:38.363956 hashwire-0.0.2/
+-rw-rw-rw-   0        0        0     1071 2023-05-23 09:09:27.000000 hashwire-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     5772 2023-05-24 11:28:38.362957 hashwire-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3921 2023-05-24 11:26:53.000000 hashwire-0.0.2/README.md
+-rw-rw-rw-   0        0        0      809 2023-05-24 11:21:34.000000 hashwire-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-24 11:28:38.364955 hashwire-0.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-24 11:28:38.323835 hashwire-0.0.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-24 11:28:38.346955 hashwire-0.0.2/src/hashwire/
+-rw-rw-rw-   0        0        0       37 2023-05-23 17:05:26.000000 hashwire-0.0.2/src/hashwire/__init__.py
+-rw-rw-rw-   0        0        0     4391 2023-05-24 10:11:21.000000 hashwire-0.0.2/src/hashwire/hash.py
+drwxrwxrwx   0        0        0        0 2023-05-24 11:28:38.359955 hashwire-0.0.2/src/hashwire.egg-info/
+-rw-rw-rw-   0        0        0     5772 2023-05-24 11:28:38.000000 hashwire-0.0.2/src/hashwire.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      222 2023-05-24 11:28:38.000000 hashwire-0.0.2/src/hashwire.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 11:28:38.000000 hashwire-0.0.2/src/hashwire.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-24 11:28:38.000000 hashwire-0.0.2/src/hashwire.egg-info/top_level.txt
```

### Comparing `hashwire-0.0.1/LICENSE` & `hashwire-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hashwire-0.0.1/pyproject.toml` & `hashwire-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "setuptools>=61.0.0",
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = 'hashwire'
-version = '0.0.1'
+version = '0.0.2'
 description = 'Hashwire creates a optimized hash multichain commitment'
 readme = 'README.md'
 authors = [
     { name = 'Hugo Labraaten', email='hugokinner@gmail.com' }
 ]
 license = {file = 'LICENSE'}
 dependencies = [
```

### Comparing `hashwire-0.0.1/src/hashwire/hash.py` & `hashwire-0.0.2/src/hashwire/hash.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,22 +27,23 @@
         hash_chain.append(commitment)
     return hash_chain, seed
 
 
 # %%
 
 # Hash multichains is an hash chain per digit position.
-def get_hash_multichain(int_value):
+def get_hash_multichain(int_value, seeds=None):
     num_digits = math.ceil(math.log10(int_value+1))
 
     # generate seed and multi_hash_chain using dictionary comprehension
-    seed = [get_seed() for _ in range(num_digits)]
-    hash_multichain = {i: get_hash_chain(10, seed[i])[0] for i in range(num_digits)}
+    if not seeds:
+        seeds = [get_seed() for _ in range(num_digits)]
+    hash_multichain = {i: get_hash_chain(10, seeds[i])[0] for i in range(num_digits)}
 
-    return hash_multichain, seed
+    return hash_multichain, seeds
 
 
 # MDP
 def mdp(x, base=10):
     # this does the same as: len(str(x))
     num_digits = math.ceil(math.log(x+1, base))
 
@@ -126,17 +127,25 @@
             self.create_commitments()
 
     def set_hash_chains(self, seeds=None, hash_chains=None):
         if (seeds and hash_chains) and \
                 (len(seeds) == len(hash_chains)):
             self.seeds = seeds
             self.hash_chains = hash_chains
-
-    def create_hash_chains(self, int_value):
-        h, s = get_hash_multichain(int_value)
+        elif (seeds and not hash_chains):
+            # update hashchain when seed is changed
+            # mdp must be set before this is used!
+            self.create_hash_chains(self.mdp[0], seeds)
+
+    def create_hash_chains(self, int_value, seeds=None):
+        if seeds:
+            h, s = get_hash_multichain(int_value, seeds)
+        else:
+            h, s = get_hash_multichain(int_value)
+        # set values
         self.set_hash_chains(s, h)
 
     def create_mdp_list(self, int_value):
         self.mdp = mdp(int_value)
 
     def create_commitments(self):
         self.commitments = get_commitment_hash_wire(self.mdp, self.hash_chains)
```

