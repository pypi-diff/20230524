# Comparing `tmp/bhv-0.3.1.tar.gz` & `tmp/bhv-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bhv-0.3.1.tar", last modified: Sun May 14 01:05:28 2023, max compression
+gzip compressed data, was "bhv-0.4.2.tar", last modified: Wed May 24 14:40:26 2023, max compression
```

## Comparing `bhv-0.3.1.tar` & `bhv-0.4.2.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/
--rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.3.1/LICENSE
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-14 01:05:28.014141 bhv-0.3.1/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3607 2023-05-14 00:49:43.000000 bhv-0.3.1/README.md
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/bhv/
--rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.3.1/bhv/__init__.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    12914 2023-05-12 20:34:13.000000 bhv-0.3.1/bhv/abstract.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.3.1/bhv/embedding.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11610 2023-05-10 11:54:44.000000 bhv-0.3.1/bhv/np.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.3.1/bhv/poibin.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.3.1/bhv/positions.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     8226 2023-05-02 19:26:10.000000 bhv-0.3.1/bhv/pytorch.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     2769 2023-05-03 12:10:28.000000 bhv-0.3.1/bhv/shared.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1152 2023-04-24 02:20:49.000000 bhv-0.3.1/bhv/slice.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)    24409 2023-05-13 22:37:13.000000 bhv-0.3.1/bhv/symbolic.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)     3505 2023-05-14 00:55:07.000000 bhv-0.3.1/bhv/vanilla.py
--rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.3.1/bhv/visualization.py
-drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-14 01:05:28.014141 bhv-0.3.1/bhv.egg-info/
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/PKG-INFO
--rw-r--r--   0 adamv     (1000) adamv     (1000)      344 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/SOURCES.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/dependency_links.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/requires.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-14 01:05:28.000000 bhv-0.3.1/bhv.egg-info/top_level.txt
--rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-14 01:05:28.014141 bhv-0.3.1/setup.cfg
--rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-14 00:43:56.000000 bhv-0.3.1/setup.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    35149 2023-04-23 16:58:42.000000 bhv-0.4.2/LICENSE
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-24 14:40:26.105539 bhv-0.4.2/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3846 2023-05-23 17:55:24.000000 bhv-0.4.2/README.md
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/bhv/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       64 2023-04-24 11:50:09.000000 bhv-0.4.2/bhv/__init__.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    12999 2023-05-24 13:43:57.000000 bhv-0.4.2/bhv/abstract.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     2120 2023-05-09 10:08:10.000000 bhv-0.4.2/bhv/embedding.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11721 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/np.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    11425 2023-04-24 21:41:56.000000 bhv-0.4.2/bhv/poibin.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1683 2023-04-28 18:20:39.000000 bhv-0.4.2/bhv/positions.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     8293 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/pytorch.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3360 2023-05-15 19:33:58.000000 bhv-0.4.2/bhv/shared.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1195 2023-05-23 15:35:44.000000 bhv-0.4.2/bhv/slice.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)    26856 2023-05-23 16:18:47.000000 bhv-0.4.2/bhv/symbolic.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1747 2023-05-23 17:48:54.000000 bhv-0.4.2/bhv/unification.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     3456 2023-05-24 13:05:15.000000 bhv-0.4.2/bhv/vanilla.py
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      782 2023-04-28 16:55:18.000000 bhv-0.4.2/bhv/visualization.py
+drwxr-xr-x   0 adamv     (1000) adamv     (1000)        0 2023-05-24 14:40:26.105539 bhv-0.4.2/bhv.egg-info/
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1002 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/PKG-INFO
+-rw-r--r--   0 adamv     (1000) adamv     (1000)      363 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/SOURCES.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        1 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/dependency_links.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       45 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/requires.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)        4 2023-05-24 14:40:26.000000 bhv-0.4.2/bhv.egg-info/top_level.txt
+-rw-r--r--   0 adamv     (1000) adamv     (1000)       38 2023-05-24 14:40:26.105539 bhv-0.4.2/setup.cfg
+-rw-r--r--   0 adamv     (1000) adamv     (1000)     1290 2023-05-24 14:35:52.000000 bhv-0.4.2/setup.py
```

### Comparing `bhv-0.3.1/LICENSE` & `bhv-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bhv-0.3.1/PKG-INFO` & `bhv-0.4.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.3.1
+Version: 0.4.2
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.3.1/README.md` & `bhv-0.4.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 - Multiple types of random vector generation
 - Random and indexed select between vectors
 - Ability to slightly modify a vector, for example by flipping a fraction of its bits
 - Permutation, roll, and swapping with multiple interfaces
 - Hashing and encoding
 - Majority with multiple implementation
 - AND, OR, and XOR operators
+- Composite operations like SELECT (or MUX) and FLIP-FRAC (flipping a fraction of the bits)
 - Hamming, jaccard, cosine, and bit-error-rate "metrics"
 - A system for relatedness, unrelatedness, and standard deviations apart
 - zscore and pvalue
 
 Additionally, provided are
 - A symbolic implementation with analysis, plotting and pretty printing
+- Law and unification backed expression simplification
+- Compilation to operation sequences
 - Efficient bit-packed representation
 - Three redundant implementations on NumPy for performance and correctness
+- A (performant) plain Python reference implementation
 - A minimal abstraction for permutations with caching and composition
 - Very basic embeddings for other datatypes (more to come)
 - Graph visualization of distances in hyperdimensional space ([see example](examples/viz_distances.py)).
 - Boolean expression and network synthesis
 
 ## Installation
 Make sure you have an up-to-date Python version, 3.10 recommended.
```

### Comparing `bhv-0.3.1/bhv/abstract.py` & `bhv-0.4.2/bhv/abstract.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,72 +12,75 @@
     # so for some active fractions, it should be a lot cheaper than for others
     # hence a specialized method for 2^-n
     @classmethod
     def rand(cls) -> Self:
         raise NotImplementedError()
 
     @classmethod
-    def nrand(cls, n) -> list[Self]:
+    def nrand(cls, n: int) -> list[Self]:
         return [cls.rand() for _ in range(n)]
 
     @classmethod
-    def rand2(cls, power=1) -> Self:
+    def rand2(cls, power: int) -> Self:
+        assert power >= 0
         r = cls.rand()
-        return r if power == 1 else r & cls.rand2(power - 1)
+        return r if power == 0 else r & cls.rand2(power - 1)
 
     @classmethod
-    def nrand2(cls, n, power=1) -> list[Self]:
+    def nrand2(cls, n: int, power: int) -> list[Self]:
+        assert power >= 0
         return [cls.rand2(power) for _ in range(n)]
 
     @classmethod
-    def random(cls, active=0.5) -> Self:
+    def random(cls, active: float) -> Self:
         raise NotImplementedError()
 
     @classmethod
-    def nrandom(cls, n, active=0.5) -> list[Self]:
+    def nrandom(cls, n: int, active: float) -> list[Self]:
+        assert 0. <= active <= 1.
         return [cls.random(active) for _ in range(n)]
 
-    def select_rand(self, other) -> Self:
+    def select_rand(self, other: Self) -> Self:
         return self.rand().select(self, other)
 
-    def select_rand2(self, other, power_left=1) -> Self:
+    def select_rand2(self, other: Self, power_left: int) -> Self:
         return self.rand2(power_left).select(self, other)
 
-    def select_random(self, other, frac_left=0.5) -> Self:
+    def select_random(self, other: Self, frac_left: float) -> Self:
         return self.random(frac_left).select(self, other)
 
     def randomize_half(self) -> Self:
-        return self.select_rand(self.rand())
+        return self.rand().select_rand(self)
 
-    def randomize_pow(self, pow_randomize=1) -> Self:
+    def randomize_pow(self, pow_randomize: int) -> Self:
         return self.rand().select_rand2(self, pow_randomize)
 
-    def randomize_frac(self, frac_randomize=0.5) -> Self:
+    def randomize_frac(self, frac_randomize: float) -> Self:
         return self.rand().select_random(self, frac_randomize)
 
     def flip_half(self) -> Self:
         return self ^ self.rand()
 
-    def flip_pow(self, pow_flip=1) -> Self:
+    def flip_pow(self, pow_flip: int) -> Self:
         return self ^ self.rand2(pow_flip)
 
-    def flip_pow_on(self, flip_on_frac) -> Self:
-        return self | self.flip_pow(flip_on_frac + 1)
+    def flip_pow_on(self, pow_flip_on: int) -> Self:
+        return self | ~self.rand2(pow_flip_on)
 
-    def flip_pow_off(self, flip_off_frac) -> Self:
-        return self & self.flip_pow(flip_off_frac + 1)
+    def flip_pow_off(self, pow_flip_off: int) -> Self:
+        return self & self.rand2(pow_flip_off)
 
-    def flip_frac(self, frac_flip=0.5) -> Self:
+    def flip_frac(self, frac_flip: float) -> Self:
         return self ^ self.random(frac_flip)
 
-    def flip_frac_on(self, flip_on_frac) -> Self:
-        return self | self.flip_frac(2*flip_on_frac)
+    def flip_frac_on(self, frac_flip_on: float) -> Self:
+        return self | self.random(frac_flip_on)
 
-    def flip_frac_off(self, flip_off_frac) -> Self:
-        return self & self.flip_frac(2*flip_off_frac)
+    def flip_frac_off(self, frac_flip_off: float) -> Self:
+        return self & self.random(1. - frac_flip_off)
 
     def permute(self, permutation_id: int) -> Self:
         raise NotImplementedError()
 
     def swap_halves(self) -> Self:
         raise NotImplementedError()
 
@@ -148,27 +151,22 @@
     def __and__(self, other: Self) -> Self:
         raise NotImplementedError()
 
     def __or__(self, other: Self) -> Self:
         raise NotImplementedError()
 
     def __invert__(self) -> Self:
-        raise NotImplementedError()
+        return self ^ self.ONE
 
     def select(self, when1: Self, when0: Self) -> Self:
         return when0 ^ (self & (when0 ^ when1))
 
     def active(self) -> int:
         raise NotImplementedError()
 
-    def bias_rel(self, other: Self, rel: Self) -> float:
-        rel_l = rel.select(self, self.ZERO).active()
-        rel_r = rel.select(other, self.ZERO).active()
-        return rel_l / (rel_l + rel_r)
-
     def active_fraction(self) -> float:
         return self.active()/DIMENSION
 
     def hamming(self, other: Self) -> int:
         return (self ^ other).active()
 
     def bit_error_rate(self, other: Self) -> float:
@@ -189,45 +187,50 @@
         res = (self & other).active() / (s_active*o_active)**.5
         return 1. - res if distance else res
 
     def std_apart(self, other: Self, invert=False) -> float:
         return self.frac_to_std(self.bit_error_rate(other), invert)
 
     @staticmethod
+    def normal(mean=0., p=.5):
+        return NormalDist(mean, (DIMENSION*p*(1 - p))**.5)
+
+    @staticmethod
     def frac_to_std(frac, invert=False):
-        p = 0.5
-        n = NormalDist(0, (DIMENSION*p*(1 - p))**.5)
-        estdvs = n.zscore(p*DIMENSION)
+        n = AbstractBHV.normal(0.0)
+        estdvs = n.zscore(0.5*DIMENSION)
         stdvs = n.zscore(frac*DIMENSION)
         return estdvs - stdvs if invert else stdvs
 
     @staticmethod
     def std_to_frac(std, invert=False):
-        p = 0.5
-        n = NormalDist(0, (DIMENSION*p*(1 - p))**.5)
+        n = AbstractBHV.normal(0.0)
         frac = (std*n.stdev + n.mean)/DIMENSION
         return 1. - frac if invert else frac
 
     def zscore(self) -> float:
-        p = 0.5
-        n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
+        n = AbstractBHV.normal(0.5*DIMENSION)
         return n.zscore(self.active())
 
     def pvalue(self) -> float:
-        p = 0.5
-        n = NormalDist(DIMENSION*p, (DIMENSION*p*(1 - p))**.5)
+        n = AbstractBHV.normal(0.5*DIMENSION)
         s = n.cdf(self.active())
         return 2.*min(s, 1. - s)
 
     def related(self, other: Self, stdvs=6) -> bool:
         return abs(self.std_apart(other)) < stdvs
 
     def unrelated(self, other: Self, stdvs=6) -> bool:
         return abs(self.std_apart(other, invert=True)) < stdvs
 
+    def bias_rel(self, other: Self, rel: Self) -> float:
+        rel_l = rel.hamming(self)
+        rel_r = rel.hamming(other)
+        return rel_l/(rel_l + rel_r)
+
     # Alternative implementations
 
     @classmethod
     def _majority3_select(cls, a: Self, b: Self, c: Self) -> Self:
         # C:  1 0 0 1 0 1 1
 
         # |:  1 1 1 1 0 1 0
```

### Comparing `bhv-0.3.1/bhv/embedding.py` & `bhv-0.4.2/bhv/embedding.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.1/bhv/np.py` & `bhv-0.4.2/bhv/np.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,16 @@
         self.data: np.ndarray = array
 
     @classmethod
     def rand(cls) -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.random.randint(0, high=2, size=DIMENSION, dtype=np.bool_))
 
     @classmethod
-    def random(cls, active=0.5) -> 'NumPyBoolBHV':
+    def random(cls, active: float) -> 'NumPyBoolBHV':
+        assert 0. <= active <= 1.
         return NumPyBoolBHV(np.random.binomial(1, active, DIMENSION))
 
     def select(self, when1: 'NumPyBoolBHV', when0: 'NumPyBoolBHV') -> 'NumPyBoolBHV':
         return NumPyBoolBHV(np.where(self.data, when1.data, when0.data))
 
     def swap_halves(self) -> 'NumPyBoolBHV':
         return self.roll_bits(DIMENSION//2)
@@ -128,15 +129,16 @@
         self.data: np.ndarray = array
 
     @classmethod
     def rand(cls) -> 'NumPyPacked8BHV':
         return NumPyPacked8BHV(np.random.randint(0, 255, DIMENSION//8, dtype=np.uint8))
 
     @classmethod
-    def random(cls, active=0.5) -> 'NumPyPacked8BHV':
+    def random(cls, active: float) -> 'NumPyPacked8BHV':
+        assert 0. <= active <= 1.
         return NumPyBoolBHV.random(active).pack8()
 
     def roll_bytes(self, n: int) -> 'NumPyPacked8BHV':
         assert abs(n) < DIMENSION//8, "only supports DIMENSION/8 rolls"
         return NumPyPacked8BHV(np.roll(self.data, n))
 
     def swap_halves(self) -> 'NumPyPacked8BHV':
@@ -222,15 +224,16 @@
         self.data: np.ndarray = array
 
     @classmethod
     def rand(cls) -> 'NumPyPacked64BHV':
         return NumPyPacked64BHV(cls.rng.random_raw(DIMENSION//64))
 
     @classmethod
-    def random(cls, active=0.5) -> 'NumPyPacked64BHV':
+    def random(cls, active: float) -> 'NumPyPacked64BHV':
+        assert 0. <= active <= 1.
         return NumPyBoolBHV.random(active).pack64()
 
     @classmethod
     def _majority_via_unpacked(cls, vs: list['NumPyPacked64BHV']) -> 'NumPyPacked64BHV':
         return NumPyBoolBHV.majority([v.unpack() for v in vs]).pack64()
 
     def swap_halves(self) -> 'NumPyPacked64BHV':
```

### Comparing `bhv-0.3.1/bhv/poibin.py` & `bhv-0.4.2/bhv/poibin.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.1/bhv/positions.py` & `bhv-0.4.2/bhv/positions.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.1/bhv/pytorch.py` & `bhv-0.4.2/bhv/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -55,15 +55,16 @@
         self.data: torch.BoolTensor = tensor
 
     @classmethod
     def rand(cls) -> 'TorchBoolBHV':
         return TorchBoolBHV(torch.empty(DIMENSION, dtype=torch.bool).random_())
 
     @classmethod
-    def random(cls, active=0.5) -> 'TorchBoolBHV':
+    def random(cls, active: float) -> 'TorchBoolBHV':
+        assert 0. <= active <= 1.
         return TorchBoolBHV(torch.empty(DIMENSION, dtype=torch.bool).bernoulli_(active))
 
     def select(self, when1: 'TorchBoolBHV', when0: 'TorchBoolBHV') -> 'TorchBoolBHV':
         return TorchBoolBHV(torch.where(self.data, when1.data, when0.data))
 
     @classmethod
     def majority(cls, vs: list['TorchBoolBHV']) -> 'TorchBoolBHV':
@@ -156,15 +157,16 @@
         self.data: torch.LongTensor = tensor
 
     @classmethod
     def rand(cls) -> Self:
         return TorchPackedBHV(torch.randint(-9223372036854775808, 9223372036854775807, size=(DIMENSION//64,), dtype=torch.long))
 
     @classmethod
-    def random(cls, active=0.5) -> Self:
+    def random(cls, active) -> Self:
+        assert 0. <= active <= 1.
         return TorchBoolBHV.random(active).pack()
 
     def roll_words(self, n: int) -> 'TorchPackedBHV':
         return TorchPackedBHV(torch.roll(self.data, n))
 
     def permute_words(self, permutation: TorchWordPermutation) -> 'TorchPackedBHV':
         return TorchPackedBHV(self.data[permutation.data])
```

### Comparing `bhv-0.3.1/bhv/shared.py` & `bhv-0.4.2/bhv/shared.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 try:
     from typing import Self
 except ImportError:
     Self = 'AbstractBHV'
 
 DIMENSION = 8192
 
+from itertools import groupby
 from functools import partial
 from dataclasses import fields, is_dataclass
 from base64 import _urlsafe_encode_translation
 import hashlib
 import binascii
 import sys
 
@@ -89,7 +90,24 @@
 
 def bin_bitmask(m):
     return ''.join("01"[x] for x in m)
 
 
 def bitconfigs(n):
     return [to_bitmask(binw(i, n)) for i in range(2**n)]
+
+
+def unique_by_id(xs):
+    return list(reversed({id(x): x for x in reversed(xs)}.values()))
+
+
+def format_multiple(xs, start="", sep="", end="", indent="", aindent="", newline_threshold=40):
+    ss = list(map(str, xs))
+    maxlen = max(map(len, ss))
+    if maxlen >= newline_threshold:
+        return start + sep.rstrip(" ").join("\n" + aindent + indent + s for s in ss) + "\n" + aindent + end
+    else:
+        return start + sep.join(s for s in ss) + end
+
+
+def format_list(xs, **kwargs):
+    return format_multiple(xs, start="[", sep=", ", end="]", **kwargs)
```

### Comparing `bhv-0.3.1/bhv/slice.py` & `bhv-0.4.2/bhv/slice.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,19 +4,20 @@
 
 class Slice(AbstractBHV):
     def __init__(self, b):
         self.b = b
 
     @classmethod
     def rand(cls) -> Self:
-        return cls.random()
+        return cls.random(.5)
 
     @classmethod
-    def random(cls, active=0.5) -> Self:
-        return Slice(random.random() > .5)
+    def random(cls, active: float) -> Self:
+        assert 0. <= active <= 1.
+        return Slice(random.random() > active)
 
     def permute(self, permutation_id: int) -> Self:
         raise NotImplementedError()
 
     def swap_halves(self) -> Self:
         raise NotImplementedError()
```

### Comparing `bhv-0.3.1/bhv/symbolic.py` & `bhv-0.4.2/bhv/symbolic.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,50 +1,95 @@
 from dataclasses import dataclass, field, fields
 from .abstract import *
-from .shared import stable_hashcode, bitconfigs
+from .shared import stable_hashcode, bitconfigs, unique_by_id, format_multiple, format_list
 from .slice import Slice
 
 
 class Symbolic:
+    name = None
+
+    def named(self, name):
+        if name is not None: self.name = name
+        return self
+
     def nodename(self, **kwargs):
-        return f"{type(self).__name__.upper()}"
+        return self.name or f"{type(self).__name__.upper()}"
 
     def nodeid(self, structural=False, **kwargs):
         return f"{type(self).__name__}{stable_hashcode(self, try_cache=True).replace('-', '') if structural else str(id(self))}"
 
-    def children(self, **kwargs):
+    def labeled_children(self, **kwargs):
         return [(getattr(self, f.name), f.name) for f in fields(self) if type(f.type) is type and issubclass(f.type, Symbolic)]
 
+    def children(self, **kwargs):
+        return [c for c, _ in self.labeled_children(**kwargs)]
+
+    def vars(self) -> list[str]:
+        return [v.name for v in self.preorder(lambda x: isinstance(x, Var))]
+
+    def substitute(self, vars):
+        if isinstance(self, Var) and self.name in vars:
+            return vars[self.name]
+        else:
+            return self.map(lambda x: x.substitute(vars))
+
+    def substitute_term(self, f):
+        res = f(self)
+        if res:
+            return res
+        else:
+            return self.map(lambda x: x.substitute_term(f))
+
     def reconstruct(self, *cs):
-        assert not self.children()
+        assert not self.labeled_children()
         return self
 
+    def map(self, f):
+        return self.reconstruct(*map(f, self.children())).named(self.name)
+
+    def constant(self):
+        return self.map(lambda x: None)
+
     def draw_node(self, **kwargs):
         print(f"{self.nodeid(**kwargs)} [label=\"{self.nodename(**kwargs)}\"];")
 
     def draw_edges(self, **kwargs):
-        for c, label in self.children(**kwargs):
+        for c, label in self.labeled_children(**kwargs):
             print(f"{c.nodeid(**kwargs)} -> {self.nodeid(**kwargs)} [label=\"{label}\"];")
 
     def draw_children(self, **kwargs):
-        for c, label in self.children(**kwargs):
+        for c, label in self.labeled_children(**kwargs):
             c.graphviz(**kwargs)
 
     def graphviz(self, structural=False, done=None, **kwargs):
         noden = self.nodeid(structural, **kwargs)
         if done is None:
             done = set()
         if noden in done:
             return
         done.add(noden)
         kwargs |= dict(done=done, structural=structural)
         self.draw_node(**kwargs)
         self.draw_edges(**kwargs)
         self.draw_children(**kwargs)
 
+    def show_program(self, name="f", indent="    ", **kwargs):
+        kwargs["indent"] = indent
+        kwargs["aindent"] = indent
+        kwargs["toplevel"] = True
+        def extracted(x: Symbolic):
+            return x.map(lambda x: x if isinstance(x, Var) else Var(f"_{subexpressions.index(x)}"))
+        subexpressions = unique_by_id(self.preorder(lambda x: not isinstance(x, Var))[1:])
+        subexpressions.reverse()
+        free_vars = unique_by_id(self.preorder(lambda x: isinstance(x, Var)))
+        arguments = [fv.show(**kwargs) for fv in free_vars]
+        lines = [(x.name or f"_{i}") + " = " + extracted(x).show(**kwargs) for i, x in enumerate(subexpressions)]
+        last = f"return {extracted(self).show(**kwargs)}"
+        code = format_multiple([*lines, last], start=f"def {name}({format_multiple(arguments, sep=', ')}):", indent=indent, newline_threshold=0)
+        return code
 
     def show(self, **kwargs):
         """
         Shows the expression tree code-style.
         Only works on referentially transparent DAGs.
         :param kwargs: drawing options
         :return: str
@@ -76,15 +121,15 @@
         if form is None: form = {}
         kwargs |= dict(form=form)
 
         sh = stable_hashcode(self, try_cache=True)
         if sh in form:
             return form[sh]
         else:
-            r = self.reconstruct(*(c.optimal_sharing(**kwargs) for c, _ in self.children()))
+            r = self.map(lambda c: c.optimal_sharing(**kwargs))
             shr = stable_hashcode(r, try_cache=True)
             if shr in form:
                 raise RuntimeError("Includes check failed")
             form[shr] = r
             return r
 
     def internal_size(self):
@@ -93,67 +138,67 @@
     def size(self, counted=None, recount=False, **kwargs):
         if counted is None: counted = {}
         kwargs |= dict(counted=counted)
         if id(self) in counted:
             return counted[id(self)] if recount else 0
         else:
             t = self.internal_size()
-            for c, _ in self.children():
+            for c in self.children():
                 t += c.size(**kwargs)
             counted[id(self)] = t
             return t
 
     def simplify(self, **kwargs):
         x = self
         while True:
-            x_ = x.reduce(**kwargs)
+            x_ = x.map(lambda x: x.simplify(**kwargs)).reduce(**kwargs)
             if x_ is None:
                 raise RuntimeError(f"{x} reduced to non (under {kwargs})")
             if x == x_:
                 return x
             else:
                 x = x_
 
     def reduce(self, **kwargs):
-        return self.reconstruct(*[c.simplify(**kwargs) for c, _ in self.children()])
+        return self.map(lambda c: c.simplify(**kwargs))
 
     def preorder(self, p=lambda x: True):
-        return [self]*p(self) + [v for c, _ in self.children() for v in c.preorder(p)]
+        return [self]*p(self) + [v for c in self.children() for v in c.preorder(p)]
 
     def truth_assignments(self, vars):
         configs = bitconfigs(len(vars))
 
         return [self.execute(vars={v.name: Slice(b) for b, v in zip(config, vars)}, bhv=Slice).b
                 for config in configs]
 
 
 @dataclass
 class List(Symbolic):
-    name: str
     xs: list[Symbolic]
 
     def show(self, **kwargs):
-        return self.name + " {\n" + '\n'.join("  " + x.show(**kwargs) + ";" for x in self.xs) + "\n}"
+        return format_list((x.show(**kwargs) for x in self.xs),
+                           **{k: kwargs[k] for k in ["indent", "aindent", "newline_threshold"] if k in kwargs})
 
-    def children(self, **kwargs):
+    def labeled_children(self, **kwargs):
         return [(x, str(i)) for i, x in enumerate(self.xs)]
 
     def reconstruct(self, *cs):
-        return List(self.name, cs)
+        return List(cs)
 
     def graphviz(self, structural=False, done=None, **kwargs):
         noden = self.nodeid(structural, **kwargs)
         if done is None:
             done = set()
         if noden in done:
             return
         done.add(noden)
         kwargs |= dict(done=done, structural=structural)
-        print(f"subgraph cluster_{self.name} " + "{")
-        print(f"label = \"{self.name}\";")
+        print(f"subgraph cluster_{self.nodename()} " + "{")
+        print(f"label = \"{self.nodename()}\";")
         for c in self.xs:
             c.draw_node(**kwargs)
         print("}")
         for c in self.xs:
             c.draw_edges(**kwargs)
             c.draw_children(**kwargs)
 
@@ -225,27 +270,29 @@
     l: SymbolicPermutation
     r: SymbolicPermutation
 
     def reconstruct(self, l, r):
         return PermCompose(l, r)
 
     def show(self, **kwargs):
-        return f"({self.l.show(**kwargs)} * {self.r.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"{self.l.show(**kwargs)} * {self.r.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) * self.r.execute(**kwargs)
 @dataclass
 class PermInvert(SymbolicPermutation):
     p: SymbolicPermutation
 
     def reconstruct(self, p):
         return PermInvert(p)
 
     def show(self, **kwargs):
-        return f"(~{self.p.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"~{self.p.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return ~self.p.execute(**kwargs)
 
 
 class SymbolicBHV(Symbolic, AbstractBHV):
     @classmethod
@@ -259,19 +306,21 @@
             return cls.ONE if t[0] else cls.ZERO
 
     @classmethod
     def rand(cls) -> Self:
         return Rand()
 
     @classmethod
-    def rand2(cls, power=1) -> Self:
+    def rand2(cls, power: int) -> Self:
+        assert power >= 0
         return Rand2(power)
 
     @classmethod
-    def random(cls, active=0.5) -> Self:
+    def random(cls, active: float) -> Self:
+        assert 0. <= active <= 1.
         return Random(active)
 
     @classmethod
     def majority(cls, vs: list[Self]) -> Self:
         return Majority(vs)
 
     def permute(self, permutation_id: 'int | tuple[int, ...]') -> Self:
@@ -279,17 +328,14 @@
 
     def swap_halves(self) -> Self:
         return SwapHalves(self)
 
     def rehash(self) -> Self:
         return ReHash(self)
 
-    def __eq__(self, other: Self) -> bool:
-        return Eq(self, other)
-
     def __xor__(self, other: Self) -> Self:
         return Xor(self, other)
 
     def __and__(self, other: Self) -> Self:
         return And(self, other)
 
     def __or__(self, other: Self) -> Self:
@@ -434,22 +480,23 @@
 
     def expected_active_fraction(self, **kwargs):
         return self.frac
 @dataclass
 class Majority(SymbolicBHV):
     vs: list[SymbolicBHV]
 
-    def children(self, **kwargs):
+    def labeled_children(self, **kwargs):
         return list(zip(self.vs, map(str, range(len(self.vs)))))
 
     def reconstruct(self, *cs):
         return Majority(cs)
 
     def show(self, **kwargs):
-        return kwargs.get("impl", "") + f"majority({[v.show(**kwargs) for v in self.vs]})"
+        args = format_list((v.show(**kwargs) for v in self.vs), **{k: kwargs[k] for k in ["indent", "aindent", "newline_threshold"] if k in kwargs})
+        return kwargs.get("impl", "") + f"majority({args})"
 
     def instantiate(self, **kwargs):
         return kwargs.get("bhv").majority([v.execute(**kwargs) for v in self.vs])
 
     def expected_active_fraction(self, **kwargs):
         from .poibin import PoiBin
         return 1. - PoiBin([v.expected_active_fraction(**kwargs) for v in self.vs]).cdf(len(self.vs)//2)
@@ -496,60 +543,66 @@
 
     def instantiate(self, **kwargs):
         return self.v.execute(**kwargs).rehash()
 
     def expected_active_fraction(self, **kwargs):
         return .5
 @dataclass
-class Eq:
+class Eq(Symbolic):
     l: SymbolicBHV
     r: SymbolicBHV
 
+    def swap(self):
+        return Eq(self.r, self.l)
+
     def reconstruct(self, l, r):
         return Eq(l, r)
 
-    def show(self, **kwargs):
-        return f"({self.l.show(**kwargs)} == {self.r.show(**kwargs)})"
+    def show(self, toplevel=True, **kwargs):
+        brackets = not toplevel
+        kwargs["toplevel"] = False
+        return "("*brackets + f"{self.l.show(**kwargs)} == {self.r.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) == self.r.execute(**kwargs)
 @dataclass
 class Xor(SymbolicBHV):
     l: SymbolicBHV
     r: SymbolicBHV
 
     def reconstruct(self, l, r):
         return Xor(l, r)
 
     def show(self, **kwargs):
-        return f"({self.l.show(**kwargs)} ^ {self.r.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"{self.l.show(**kwargs)} ^ {self.r.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) ^ self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
         if self.l == self.ONE:
-            return ~self.r.simplify(**kwargs)
+            return ~self.r
         elif self.r == self.ONE:
-            return ~self.l.simplify(**kwargs)
+            return ~self.l
         elif self.l == self.ZERO:
-            return self.r.simplify(**kwargs)
+            return self.r
         elif self.r == self.ZERO:
-            return self.l.simplify(**kwargs)
+            return self.l
         elif self.l == self.r:
             return self.ZERO
         elif self.l == ~self.r or ~self.l == self.r:
             return self.ONE
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
-            return ~Xor(self.l.v.simplify(**kwargs), self.r.v.simplify(**kwargs))
+            return Xor(self.l.v, self.r.v)
         elif isinstance(self.l, And) and isinstance(self.r, And):
-            if self.l.l == self.r.l: return And(self.l.l, Xor(self.l.r, self.r.r)).simplify(**kwargs)
-            elif self.l.l == self.r.r: return And(self.l.l, Xor(self.l.r, self.r.l)).simplify(**kwargs)
-            elif self.l.r == self.r.l: return And(self.l.r, Xor(self.l.l, self.r.r)).simplify(**kwargs)
-            elif self.l.r == self.r.r: return And(self.l.r, Xor(self.l.l, self.r.l)).simplify(**kwargs)
+            if self.l.l == self.r.l: return And(self.l.l, Xor(self.l.r, self.r.r))
+            elif self.l.l == self.r.r: return And(self.l.l, Xor(self.l.r, self.r.l))
+            elif self.l.r == self.r.l: return And(self.l.r, Xor(self.l.l, self.r.r))
+            elif self.l.r == self.r.r: return And(self.l.r, Xor(self.l.l, self.r.l))
             else: return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
         else:
             return Xor(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
@@ -559,28 +612,33 @@
     l: SymbolicBHV
     r: SymbolicBHV
 
     def reconstruct(self, l, r):
         return And(l, r)
 
     def show(self, **kwargs):
-        return f"({self.l.show(**kwargs)} & {self.r.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"{self.l.show(**kwargs)} & {self.r.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) & self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
         if self.l == self.ZERO or self.r == self.ZERO:
             return self.ZERO
         elif self.l == self.ONE:
-            return self.r.simplify(**kwargs)
+            return self.r
         elif self.r == self.ONE:
-            return self.l.simplify(**kwargs)
+            return self.l
+        elif isinstance(self.l, Invert) and self.l.v == self.r:
+            return self.ZERO
+        elif isinstance(self.r, Invert) and self.r.v == self.l:
+            return self.ZERO
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
-            return Invert(Or(self.l.v.simplify(**kwargs), self.r.v.simplify(**kwargs)))
+            return Invert(Or(self.l.v, self.r.v))
         else:
             return And(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return afl*afr
@@ -589,28 +647,33 @@
     l: SymbolicBHV
     r: SymbolicBHV
 
     def reconstruct(self, l, r):
         return Or(l, r)
 
     def show(self, **kwargs):
-        return f"({self.l.show(**kwargs)} | {self.r.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"{self.l.show(**kwargs)} | {self.r.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return self.l.execute(**kwargs) | self.r.execute(**kwargs)
 
     def reduce(self, **kwargs):
         if self.l == self.ONE or self.r == self.ONE:
             return self.ONE
         elif self.l == self.ZERO:
-            return self.r.simplify(**kwargs)
+            return self.r
         elif self.r == self.ZERO:
-            return self.l.simplify(**kwargs)
+            return self.l
+        elif isinstance(self.l, Invert) and self.l.v == self.r:
+            return self.ONE
+        elif isinstance(self.r, Invert) and self.r.v == self.l:
+            return self.ONE
         elif isinstance(self.l, Invert) and isinstance(self.r, Invert):
-            return Invert(And(self.l.v.simplify(**kwargs), self.r.v.simplify(**kwargs)))
+            return Invert(And(self.l.v, self.r.v))
         else:
             return Or(self.l.simplify(**kwargs), self.r.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afl = self.l.expected_active_fraction(**kwargs)
         afr = self.r.expected_active_fraction(**kwargs)
         return 1. - ((1. - afl)*(1. - afr))
@@ -618,26 +681,27 @@
 class Invert(SymbolicBHV):
     v: SymbolicBHV
 
     def reconstruct(self, v):
         return Invert(v)
 
     def show(self, **kwargs):
-        return f"(~{self.v.show(**kwargs)})"
+        brackets = not kwargs.get("toplevel", False)
+        return "("*brackets + f"~{self.v.show(**kwargs)}" + ")"*brackets
 
     def instantiate(self, **kwargs):
         return ~self.v.execute(**kwargs)
 
     def reduce(self, **kwargs):
         if self.v == self.ONE:
             return self.ZERO
         elif self.v == self.ZERO:
             return self.ONE
         elif isinstance(self.v, Invert):
-            return self.v.v.simplify(**kwargs)
+            return self.v.v
         else:
             return Invert(self.v.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         return 1. - self.v.expected_active_fraction(**kwargs)
 @dataclass
 class Select(SymbolicBHV):
@@ -647,16 +711,16 @@
 
     def reconstruct(self, c, w1, w0):
         return Select(c, w1, w0)
 
     def nodename(self, compact_select=False, **kwargs):
         return f"ON {self.cond.nodename()}" if compact_select else super().nodename(**kwargs)
 
-    def children(self, compact_select=False, **kwargs):
-        return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().children(**kwargs)
+    def labeled_children(self, compact_select=False, **kwargs):
+        return [(self.when1, "1"), (self.when0, "0")] if compact_select else super().labeled_children(**kwargs)
 
     def show(self, **kwargs):
         return f"{self.cond.show(**kwargs)}.select({self.when1.show(**kwargs)}, {self.when0.show(**kwargs)})"
 
     def instantiate(self, **kwargs):
         return self.cond.execute(**kwargs).select(self.when1.execute(**kwargs), self.when0.execute(**kwargs))
 
@@ -664,45 +728,41 @@
         return 3
 
     def reduce(self, **kwargs):
         expand_select_xor = kwargs.get("expand_select_xor", False)
         expand_select_and_or = kwargs.get("expand_select_and_or", False)
 
         if self.when1 == self.ONE and self.when0 == self.ZERO:
-            return self.cond.simplify(**kwargs)
+            return self.cond
         elif self.when1 == self.ZERO and self.when0 == self.ONE:
-            return (~self.cond).simplify(**kwargs)
+            return ~self.cond
         elif self.when0 == self.when1:
-            return self.when0.simplify(**kwargs)
+            return self.when0
         elif self.when1 == self.ONE:
-            return self.cond.simplify(**kwargs) | self.when0.simplify(**kwargs)
+            return self.cond | self.when0
         elif self.when1 == self.ZERO:
-            return (~self.cond).simplify(**kwargs) & self.when0.simplify(**kwargs)
+            return ~self.cond & self.when0
         elif self.when0 == self.ONE:
-            return (~self.cond).simplify(**kwargs) | self.when1.simplify(**kwargs)
+            return ~self.cond | self.when1
         elif self.when0 == self.ZERO:
-            return self.cond.simplify(**kwargs) & self.when1.simplify(**kwargs)
+            return self.cond & self.when1
         else:
-            when1_ = self.when1.simplify(**kwargs)
-            when0_ = self.when0.simplify(**kwargs)
-            cond_ = self.cond.simplify(**kwargs)
-
-            if when1_ == ~when0_:
-                return cond_ ^ when0_
-            elif when0_ == ~when1_:
-                return cond_ ^ when0_
-            elif isinstance(when0_, Invert) and isinstance(when1_, Invert):
-                return ~Select(cond_, when1_.v, when0_.v)
+            if self.when1 == ~self.when0:
+                return self.cond ^ self.when0
+            elif self.when0 == ~self.when1:
+                return self.cond ^ self.when0
+            elif isinstance(self.when0, Invert) and isinstance(self.when1, Invert):
+                return ~Select(self.cond, self.when1.v, self.when0.v)
             else:
                 if expand_select_xor:
-                    return when0_ ^ (cond_ & (when0_ ^ when1_))
+                    return self.when0 ^ (self.cond & (self.when0 ^ self.when1))
                 elif expand_select_and_or:
-                    return (cond_ & when1_) | ((~cond_).simplify(**kwargs) & when0_)
+                    return (self.cond & self.when1) | (~self.cond & self.when0)
                 else:
-                    return Select(cond_, when1_, when0_)
+                    return Select(self.cond.simplify(**kwargs), self.when1.simplify(**kwargs), self.when0.simplify(**kwargs))
 
     def expected_active_fraction(self, **kwargs):
         afc = self.cond.expected_active_fraction(**kwargs)
         af1 = self.when1.expected_active_fraction(**kwargs)
         af0 = self.when0.expected_active_fraction(**kwargs)
         return afc*af1 + (1. - afc)*af0
 @dataclass
```

### Comparing `bhv-0.3.1/bhv/vanilla.py` & `bhv-0.4.2/bhv/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,16 @@
         self.data: bytes = data
 
     @classmethod
     def rand(cls) -> 'VanillaBHV':
         return VanillaBHV(random.randbytes(DIMENSION//8))
 
     @classmethod
-    def random(cls, active=0.5) -> 'VanillaBHV':
+    def random(cls, active: float) -> 'VanillaBHV':
+        assert 0. <= active <= 1.
         return VanillaBHV(bytes([
             (random.random() < active) | (random.random() < active) << 1 | (random.random() < active) << 2 | (random.random() < active) << 3 |
             (random.random() < active) << 4 | (random.random() < active) << 5 | (random.random() < active) << 6 | (random.random() < active) << 7
             for _ in range(DIMENSION//8)]))
 
     def roll_bytes(self, n: int) -> 'VanillaBHV':
         assert abs(n) < DIMENSION//8, "only supports DIMENSION/8 rolls"
@@ -67,29 +68,26 @@
 
     def __and__(self, other: 'VanillaBHV') -> 'VanillaBHV':
         return self.from_int(self.to_int() & other.to_int())
 
     def __or__(self, other: 'VanillaBHV') -> 'VanillaBHV':
         return self.from_int(self.to_int() | other.to_int())
 
-    def __invert__(self) -> 'VanillaBHV':
-        return self.from_int(~self.to_int())
-
     if version_info[2] >= 10:
         def active(self) -> int:
             return self.to_int().bit_count()
     else:
         def active(self) -> int:
             return bin(self.to_int()).count("1")
 
     def to_int(self) -> int:
-        return int.from_bytes(self.data, byteorder, signed=True)
+        return int.from_bytes(self.data, byteorder, signed=False)
 
     @classmethod
     def from_int(cls, i: int):
-        return VanillaBHV(i.to_bytes(DIMENSION//8, byteorder, signed=True))
+        return VanillaBHV(i.to_bytes(DIMENSION//8, byteorder, signed=False))
 
 
 VanillaBHV.ZERO = VanillaBHV(bytes([0 for _ in range(DIMENSION//8)]))
 VanillaBHV.ONE = VanillaBHV(bytes([0xff for _ in range(DIMENSION//8)]))
 VanillaBHV._FEISTAL_SUBKEYS = VanillaBHV.nrand2(VanillaBHV._FEISTAL_ROUNDS, 4)
 VanillaBHV.HALF = VanillaBHV(bytes([0 for _ in range(DIMENSION//16)] + [0xff for _ in range(DIMENSION//16)]))
```

### Comparing `bhv-0.3.1/bhv/visualization.py` & `bhv-0.4.2/bhv/visualization.py`

 * *Files identical despite different names*

### Comparing `bhv-0.3.1/bhv.egg-info/PKG-INFO` & `bhv-0.4.2/bhv.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bhv
-Version: 0.3.1
+Version: 0.4.2
 Summary: Boolean Hypervectors
 Author: Adam Vandervorst
 Author-email: contact@adamv.be
 Keywords: ai binary hypervector hdc bsc
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `bhv-0.3.1/setup.py` & `bhv-0.4.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.3.1'
+VERSION = '0.4.2'
 DESCRIPTION = 'Boolean Hypervectors'
 LONG_DESCRIPTION = 'Boolean Hypervectors with various operators for experiments in hyperdimensional computing (HDC).'
 
 setup(
     name="bhv",
     version=VERSION,
     author="Adam Vandervorst",
```

