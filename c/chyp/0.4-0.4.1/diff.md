# Comparing `tmp/chyp-0.4.tar.gz` & `tmp/chyp-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chyp-0.4.tar", last modified: Mon May 22 22:25:42 2023, max compression
+gzip compressed data, was "chyp-0.4.1.tar", last modified: Wed May 24 08:34:01 2023, max compression
```

## Comparing `chyp-0.4.tar` & `chyp-0.4.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 22:25:42.039116 chyp-0.4/
--rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.4/LICENSE
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    14272 2023-05-22 22:25:42.039116 chyp-0.4/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13737 2023-05-22 21:50:22.000000 chyp-0.4/README.md
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 22:25:42.035117 chyp-0.4/chyp/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.4/chyp/__init__.py
--rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.4/chyp/__main__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    17152 2023-05-22 22:21:29.000000 chyp-0.4/chyp/graph.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 22:25:42.039116 chyp-0.4/chyp/gui/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.4/chyp/gui/__init__.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.4/chyp/gui/app.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.4/chyp/gui/codeview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.4/chyp/gui/colors.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.4/chyp/gui/completion.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.4/chyp/gui/document.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11645 2023-05-22 22:23:03.000000 chyp-0.4/chyp/gui/editor.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.4/chyp/gui/errorlist.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     7251 2023-05-22 22:20:03.000000 chyp-0.4/chyp/gui/graphscene.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1258 2023-05-22 22:23:12.000000 chyp-0.4/chyp/gui/graphview.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-22 22:23:14.000000 chyp-0.4/chyp/gui/highlighter.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.4/chyp/gui/mainwindow.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    10470 2023-05-22 22:21:33.000000 chyp-0.4/chyp/layout.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.4/chyp/matcher.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    14794 2023-05-22 22:21:41.000000 chyp-0.4/chyp/parser.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.4/chyp/rewrite.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1791 2023-05-22 22:21:48.000000 chyp-0.4/chyp/rule.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.4/chyp/scraps.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4650 2023-05-22 22:21:58.000000 chyp-0.4/chyp/state.py
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     4780 2023-05-22 22:22:17.000000 chyp-0.4/chyp/term.py
-drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-22 22:25:42.035117 chyp-0.4/chyp.egg-info/
--rw-rw-r--   0 aleger    (1000) aleger    (1000)    14272 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/PKG-INFO
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/SOURCES.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/dependency_links.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/entry_points.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/requires.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-22 22:25:42.000000 chyp-0.4/chyp.egg-info/top_level.txt
--rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.4/pyproject.toml
--rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-22 22:25:42.039116 chyp-0.4/setup.cfg
--rw-rw-r--   0 aleger    (1000) aleger    (1000)     1059 2023-05-22 22:17:39.000000 chyp-0.4/setup.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 08:34:01.522154 chyp-0.4.1/
+-rw-r--r--   0 aleger    (1000) aleger    (1000)    11357 2022-09-06 15:50:03.000000 chyp-0.4.1/LICENSE
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-24 08:34:01.522154 chyp-0.4.1/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    15651 2023-05-24 08:31:14.000000 chyp-0.4.1/README.md
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 08:34:01.522154 chyp-0.4.1/chyp/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      653 2023-05-22 22:21:15.000000 chyp-0.4.1/chyp/__init__.py
+-rw-r--r--   0 aleger    (1000) aleger    (1000)      715 2023-05-22 22:21:24.000000 chyp-0.4.1/chyp/__main__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    17152 2023-05-22 22:21:29.000000 chyp-0.4.1/chyp/graph.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 08:34:01.522154 chyp-0.4.1/chyp/gui/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      651 2023-05-22 22:23:21.000000 chyp-0.4.1/chyp/gui/__init__.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2537 2023-05-22 22:22:46.000000 chyp-0.4.1/chyp/gui/app.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4911 2023-05-22 22:22:48.000000 chyp-0.4.1/chyp/gui/codeview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4824 2023-05-22 22:20:22.000000 chyp-0.4.1/chyp/gui/colors.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     2060 2023-05-22 22:22:54.000000 chyp-0.4.1/chyp/gui/completion.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4774 2023-05-22 22:23:00.000000 chyp-0.4.1/chyp/gui/document.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11651 2023-05-24 07:44:21.000000 chyp-0.4.1/chyp/gui/editor.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3285 2023-05-22 22:23:06.000000 chyp-0.4.1/chyp/gui/errorlist.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     8136 2023-05-23 21:03:29.000000 chyp-0.4.1/chyp/gui/graphscene.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1258 2023-05-22 22:23:12.000000 chyp-0.4.1/chyp/gui/graphview.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3307 2023-05-22 22:23:14.000000 chyp-0.4.1/chyp/gui/highlighter.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    13424 2023-05-22 22:23:18.000000 chyp-0.4.1/chyp/gui/mainwindow.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    10786 2023-05-23 21:40:13.000000 chyp-0.4.1/chyp/layout.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    11350 2023-05-22 22:20:49.000000 chyp-0.4.1/chyp/matcher.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    14794 2023-05-22 22:21:41.000000 chyp-0.4.1/chyp/parser.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3804 2023-05-22 22:21:44.000000 chyp-0.4.1/chyp/rewrite.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1791 2023-05-22 22:21:48.000000 chyp-0.4.1/chyp/rule.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     3068 2023-03-30 12:34:42.000000 chyp-0.4.1/chyp/scraps.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     4650 2023-05-22 22:21:58.000000 chyp-0.4.1/chyp/state.py
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     6018 2023-05-23 23:17:32.000000 chyp-0.4.1/chyp/term.py
+drwxrwxr-x   0 aleger    (1000) aleger    (1000)        0 2023-05-24 08:34:01.522154 chyp-0.4.1/chyp.egg-info/
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)    16188 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/PKG-INFO
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      630 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/SOURCES.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        1 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/dependency_links.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       43 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/entry_points.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       40 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/requires.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)        5 2023-05-24 08:34:01.000000 chyp-0.4.1/chyp.egg-info/top_level.txt
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)      161 2023-05-05 09:44:28.000000 chyp-0.4.1/pyproject.toml
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)       38 2023-05-24 08:34:01.522154 chyp-0.4.1/setup.cfg
+-rw-rw-r--   0 aleger    (1000) aleger    (1000)     1061 2023-05-24 08:33:25.000000 chyp-0.4.1/setup.py
```

### Comparing `chyp-0.4/LICENSE` & `chyp-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chyp-0.4/PKG-INFO` & `chyp-0.4.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: chyp
-Version: 0.4
-Summary: An interactive theorem prover for string diagrams
-Home-page: https://github.com/akissinger/chyp
-Author: Aleks Kissinger
-Author-email: aleks0@gmail.com
-License: Apache2
-Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 Chyp (pronounced "chip") is an interactive theorem prover for symmetric monoidal categories (SMCs), a.k.a. process theories. Symmetric monoidal categories are a very general way to reason about processes that can be composed in sequence or in parallel. String diagrams are a convenient notation for maps in an SMC, where processes are represented as boxes connected to each other by wires.
 
 ![Chyp screenshot](https://github.com/akissinger/chyp/raw/master/chyp-screen.png)
 
 Chyp is short for _Cospans of HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching from terms to this combinatoric structure, we obtain a convenient rewrite theory for string diagrams that automatically handles the extra "bureaucracy" that comes from working with sequential and parallel composition together. There is a lot of theory behind this, which has been developed over a series of papers:
 
 * [String Diagram Rewrite Theory I: Rewriting with Frobenius Structure](https://arxiv.org/abs/2012.01847)
@@ -124,27 +108,27 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
 
 Now, when we place the cursor over any step of this rule, it is highlighted in green, and it shows where that rule is applied. The green highlighting is indicating that Chyp has successfully checked this step. Namely, it has matched the LHS of the given rule on the previous term, rewritten the LHS to the RHS, and checked the result is the same as the term given. If we make a mistake in the example above (e.g. try to replace `assoc` with `bialg` or `sw` with `id * id`), that line will turn red. This means Chyp was _not_ able to find a matching for the rule given which implies the given equality.
 
 By default, Chyp tries to apply rules from left to right. We can apply a rule in the other direction by prefixing the rule name with `-`. For example, the proof above can be done backwards as follows:
 
     rewrite ba1_backwards :
-      f * id ; f ; g ; g * id
-      = id * f ; f ; g ; g * id by assoc
-      = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
+      g * f ; id * id * g ; id * sw * id ; f * f ; g * id
+      = id * f ; f ; g ; g * id by -bialg
+      = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
 Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d) by refl
 
-In fact, we can omit the `by refl`. The following is equivalent:
+Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -187,15 +171,15 @@
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
 
 # Modules and importing
 
-As structures and proofs get more complicated, we may want to split them into multiple files. Every `*.chyp` file defines a module, which can be imported in other `*.chyp` file. Suppose for example we define the following file `monoid.chyp`:
+As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
     rule assoc : m * id ; m = id * m ; m
     rule unitL : u * id ; m = id
     rule unitR : id * u ; m = id
 
@@ -228,30 +212,67 @@
     import cmonoid as M2(m = m2, u = u2)
 
     gen cp : 1 -> 2
     rule dist :
       m1 * id ; m2 = 
       = id * m1 ; m2 = cp * id * id ; id * sw * id ; m2 * m2 ; m1
 
+Even though we now have short aliases for generators, the rules still live in their respective namespaces. For example, `M1.assoc` can be used to rewrite `m1 * id ; m1` to `id * m1 ; m1` and `M2.assoc` will rewrite `m2 * id ; m2` to `id * m2 ; m2`.
+
 This is especially convenient if modules share generators in non-trivial ways. For example, a pair of Frobenius algebras interacting as a bialgebra could be defined this way, assuming `frobenius.chyp` and `bialg.chyp` have already been defined:
 
     gen m1 : 2 -> 1
     gen u1 : 0 -> 1
     gen n1 : 1 -> 2
     gen v1 : 1 -> 0
 
     gen m2 : 2 -> 1
     gen u2 : 0 -> 1
     gen n2 : 1 -> 2
     gen v2 : 1 -> 0
 
-    import frobenius(m = m1, u = u1, n = n1, v = v1) as F1
-    import frobenius(m = m2, u = u2, n = n2, v = v2) as F2
-    import bialg(m = m1, u = u1, n = n2, v = v2) as B1
-    import bialg(m = m2, u = u2, n = n1, v = v1) as B2
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+    import frobenius as F2(m = m2, u = u2, n = n2, v = v2)
+    import bialg as B1(m = m1, u = u1, n = n2, v = v2)
+    import bialg as B2(m = m2, u = u2, n = n1, v = v1)
+
+We can even set the generators in an imported module equal to arbitrary terms, as long as the types match.
+
+To understand how this works, it is useful to know that this is just some syntactic sugar that takes advantage of the behaviour of the `gen` statement. Normally, the `gen` statement will add a new generator to the current namespace. However, if a term with that name already exists, it will simply check the already existing term has the right arity and coarity. This allows us to alias generators in a module using `let` statements _before_ it is imported. So, in fact, the line:
+
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+
+is exactly equivalent to:
+
+    let F1.m = m1
+    let F1.u = u1
+    let F1.n = n1
+    let F1.v = v1
+    import frobenius as F1
+
+Whenever an `m` is encountered in `frobenius.chyp` (which will be interpreted as `F1.m`), it will automatically get replaced by `m1` thanks to the `let` statement.
+
+If we alias generators to some more complicated terms, these just end up the RHS of the `let` statements. For example, we could get the "almost" Frobenius algebra laws of the [ZW calculus](https://arxiv.org/abs/1501.07082) with a statement like this:
+
+
+    gen m : 2 -> 1
+    gen u : 0 -> 1
+    gen n : 1 -> 2
+    gen v : 1 -> 0
+    gen d : 1 -> 1
+
+    import frobenius as W(m = d * d ; m, u = u, n = d ; n, v = d ; v)
+
+where the last line is equivalent to:
+
+    let W.m = d * d ; m
+    let W.u = u
+    let W.n = d ; n
+    let W.v = d ; v
+    import frobenius as W
 
 
 ## Finding modules
 
 The `import` statement always looks for `*.chyp` files in the same directory of the current file. Chyp doesn't have a notion of "search paths" for modules, but this might be added in the future.
 
 Files can be imported from subdirectories by adding dots:
```

### Comparing `chyp-0.4/README.md` & `chyp-0.4.1/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: chyp
+Version: 0.4.1
+Summary: An interactive theorem prover for string diagrams
+Home-page: https://github.com/akissinger/chyp
+Author: Aleks Kissinger
+Author-email: aleks0@gmail.com
+License: Apache2
+Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 Chyp (pronounced "chip") is an interactive theorem prover for symmetric monoidal categories (SMCs), a.k.a. process theories. Symmetric monoidal categories are a very general way to reason about processes that can be composed in sequence or in parallel. String diagrams are a convenient notation for maps in an SMC, where processes are represented as boxes connected to each other by wires.
 
 ![Chyp screenshot](https://github.com/akissinger/chyp/raw/master/chyp-screen.png)
 
 Chyp is short for _Cospans of HYPergraphs_, which refers to how string diagrams are represented and plugged together formally in the tool. By switching from terms to this combinatoric structure, we obtain a convenient rewrite theory for string diagrams that automatically handles the extra "bureaucracy" that comes from working with sequential and parallel composition together. There is a lot of theory behind this, which has been developed over a series of papers:
 
 * [String Diagram Rewrite Theory I: Rewriting with Frobenius Structure](https://arxiv.org/abs/2012.01847)
@@ -108,27 +124,27 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
 
 Now, when we place the cursor over any step of this rule, it is highlighted in green, and it shows where that rule is applied. The green highlighting is indicating that Chyp has successfully checked this step. Namely, it has matched the LHS of the given rule on the previous term, rewritten the LHS to the RHS, and checked the result is the same as the term given. If we make a mistake in the example above (e.g. try to replace `assoc` with `bialg` or `sw` with `id * id`), that line will turn red. This means Chyp was _not_ able to find a matching for the rule given which implies the given equality.
 
 By default, Chyp tries to apply rules from left to right. We can apply a rule in the other direction by prefixing the rule name with `-`. For example, the proof above can be done backwards as follows:
 
     rewrite ba1_backwards :
-      f * id ; f ; g ; g * id
-      = id * f ; f ; g ; g * id by assoc
-      = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
+      g * f ; id * id * g ; id * sw * id ; f * f ; g * id
+      = id * f ; f ; g ; g * id by -bialg
+      = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
 Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d) by refl
 
-In fact, we can omit the `by refl`. The following is equivalent:
+Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -171,15 +187,15 @@
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
 
 # Modules and importing
 
-As structures and proofs get more complicated, we may want to split them into multiple files. Every `*.chyp` file defines a module, which can be imported in other `*.chyp` file. Suppose for example we define the following file `monoid.chyp`:
+As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
     rule assoc : m * id ; m = id * m ; m
     rule unitL : u * id ; m = id
     rule unitR : id * u ; m = id
 
@@ -212,30 +228,67 @@
     import cmonoid as M2(m = m2, u = u2)
 
     gen cp : 1 -> 2
     rule dist :
       m1 * id ; m2 = 
       = id * m1 ; m2 = cp * id * id ; id * sw * id ; m2 * m2 ; m1
 
+Even though we now have short aliases for generators, the rules still live in their respective namespaces. For example, `M1.assoc` can be used to rewrite `m1 * id ; m1` to `id * m1 ; m1` and `M2.assoc` will rewrite `m2 * id ; m2` to `id * m2 ; m2`.
+
 This is especially convenient if modules share generators in non-trivial ways. For example, a pair of Frobenius algebras interacting as a bialgebra could be defined this way, assuming `frobenius.chyp` and `bialg.chyp` have already been defined:
 
     gen m1 : 2 -> 1
     gen u1 : 0 -> 1
     gen n1 : 1 -> 2
     gen v1 : 1 -> 0
 
     gen m2 : 2 -> 1
     gen u2 : 0 -> 1
     gen n2 : 1 -> 2
     gen v2 : 1 -> 0
 
-    import frobenius(m = m1, u = u1, n = n1, v = v1) as F1
-    import frobenius(m = m2, u = u2, n = n2, v = v2) as F2
-    import bialg(m = m1, u = u1, n = n2, v = v2) as B1
-    import bialg(m = m2, u = u2, n = n1, v = v1) as B2
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+    import frobenius as F2(m = m2, u = u2, n = n2, v = v2)
+    import bialg as B1(m = m1, u = u1, n = n2, v = v2)
+    import bialg as B2(m = m2, u = u2, n = n1, v = v1)
+
+We can even set the generators in an imported module equal to arbitrary terms, as long as the types match.
+
+To understand how this works, it is useful to know that this is just some syntactic sugar that takes advantage of the behaviour of the `gen` statement. Normally, the `gen` statement will add a new generator to the current namespace. However, if a term with that name already exists, it will simply check the already existing term has the right arity and coarity. This allows us to alias generators in a module using `let` statements _before_ it is imported. So, in fact, the line:
+
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+
+is exactly equivalent to:
+
+    let F1.m = m1
+    let F1.u = u1
+    let F1.n = n1
+    let F1.v = v1
+    import frobenius as F1
+
+Whenever an `m` is encountered in `frobenius.chyp` (which will be interpreted as `F1.m`), it will automatically get replaced by `m1` thanks to the `let` statement.
+
+If we alias generators to some more complicated terms, these just end up the RHS of the `let` statements. For example, we could get the "almost" Frobenius algebra laws of the [ZW calculus](https://arxiv.org/abs/1501.07082) with a statement like this:
+
+
+    gen m : 2 -> 1
+    gen u : 0 -> 1
+    gen n : 1 -> 2
+    gen v : 1 -> 0
+    gen d : 1 -> 1
+
+    import frobenius as W(m = d * d ; m, u = u, n = d ; n, v = d ; v)
+
+where the last line is equivalent to:
+
+    let W.m = d * d ; m
+    let W.u = u
+    let W.n = d ; n
+    let W.v = d ; v
+    import frobenius as W
 
 
 ## Finding modules
 
 The `import` statement always looks for `*.chyp` files in the same directory of the current file. Chyp doesn't have a notion of "search paths" for modules, but this might be added in the future.
 
 Files can be imported from subdirectories by adding dots:
```

### Comparing `chyp-0.4/chyp/__init__.py` & `chyp-0.4.1/chyp/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/__main__.py` & `chyp-0.4.1/chyp/__main__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/graph.py` & `chyp-0.4.1/chyp/graph.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/__init__.py` & `chyp-0.4.1/chyp/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/app.py` & `chyp-0.4.1/chyp/gui/app.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/codeview.py` & `chyp-0.4.1/chyp/gui/codeview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/colors.py` & `chyp-0.4.1/chyp/gui/colors.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/completion.py` & `chyp-0.4.1/chyp/gui/completion.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/document.py` & `chyp-0.4.1/chyp/gui/document.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/editor.py` & `chyp-0.4.1/chyp/gui/editor.py`

 * *Files 0% similar despite different names*

```diff
@@ -257,19 +257,19 @@
 
                 if rw_term:
                     cursor = self.code_view.textCursor()
                     cursor.clearSelection()
                     cursor.setPosition(start)
                     cursor.setPosition(end, mode=QTextCursor.MoveMode.KeepAnchor)
 
-                    self.blockSignals(True)
+                    # self.blockSignals(True)
                     cursor.insertText(rw_term)
                     self.code_view.setTextCursor(cursor)
-                    self.blockSignals(False)
-                    self.update_state()
+                    # self.blockSignals(False)
+                    # self.update_state()
 
     def repeat_step_at_cursor(self) -> None:
         self.update_state()
         pos = self.code_view.textCursor().position()
         part = self.state.part_at(pos)
         if part and part[2] == 'rewrite' and part[3] in self.state.rewrites:
             rule = self.state.rewrites[part[3]].rule
```

### Comparing `chyp-0.4/chyp/gui/errorlist.py` & `chyp-0.4.1/chyp/gui/errorlist.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/graphscene.py` & `chyp-0.4.1/chyp/gui/graphscene.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 from __future__ import annotations
+import itertools
 from typing import Optional, List, Tuple
 
 from PySide6.QtCore import Qt, QPointF
 from PySide6.QtGui import QBrush, QColor, QFont, QPainter, QPainterPath, QPen, QTransform, QUndoStack
 from PySide6.QtWidgets import (QGraphicsEllipseItem, QGraphicsItem,
                                QGraphicsPathItem, QGraphicsRectItem, QGraphicsScene,
                                QGraphicsSceneMouseEvent, QStyleOptionGraphicsItem, QWidget)
@@ -67,23 +68,35 @@
 
         if self.fg != '':
             painter.setPen(QPen(QColor(self.fg)))
         painter.setFont(QFont("sans", 11))
         painter.drawText(self.boundingRect(), Qt.AlignmentFlag.AlignCenter, str(self.value)) # type:ignore
 
 class VItem(QGraphicsEllipseItem):
-    def __init__(self, g: Graph, v: int) -> None:
+    def __init__(self, g: Graph, v: int, eitem: Optional[EItem]=None, i: int=-1) -> None:
         super().__init__(-0.0625 * SCALE, -0.0625 * SCALE, 0.125 * SCALE, 0.125 * SCALE)
         self.setVisible(False)
         self.g = g
         self.v = v
+        self.eitem = eitem
+        self.i = i
         vd = g.vertex_data(v)
         self.setPos(vd.x * SCALE, vd.y * SCALE)
         self.setBrush(QBrush(QColor(0,0,0)))
 
+    def refresh(self):
+        if self.eitem and self.i != -1:
+            x_shift = 0.7 * SCALE
+            if self.eitem.num_t == 1:
+                y_shift = 0
+            else:
+                y_shift = ((self.i / (self.eitem.num_t - 1)) - 0.5) * SCALE
+            p = self.eitem.pos()
+            self.setPos(p.x() + x_shift, p.y() + y_shift)
+
 class TItem(QGraphicsPathItem):
     def __init__(self, vitem: VItem, eitem: EItem, i: int, src: bool) -> None:
         super().__init__()
         g = vitem.g
         self.vitem = vitem
         self.eitem = eitem
         if (g.vertex_data(vitem.v).highlight or
@@ -148,20 +161,27 @@
     def add_items(self) -> None:
         vi = {}
         ei = {}
         for e in self.g.edges():
             ei[e] = EItem(self.g, e)
             self.addItem(ei[e])
 
-        for v in self.g.vertices():
+        for v in itertools.chain(self.g.inputs(), self.g.outputs()):
             vi[v] = VItem(self.g, v)
             self.addItem(vi[v])
 
         for e in self.g.edges():
             ed = self.g.edge_data(e)
+            for i, v in enumerate(ed.t):
+                if not v in vi:
+                    vi[v] = VItem(self.g, v, ei[e], i)
+                    self.addItem(vi[v])
+
+        for e in self.g.edges():
+            ed = self.g.edge_data(e)
             for i, v in enumerate(ed.s):
                 ti = TItem(vi[v], ei[e], i, src=True)
                 self.addItem(ti)
             for i, v in enumerate(ed.t):
                 ti = TItem(vi[v], ei[e], i, src=False)
                 self.addItem(ti)
 
@@ -181,22 +201,25 @@
         dx = round((p.x() - self.drag_start.x())/grid_size) * grid_size
         dy = round((p.y() - self.drag_start.y())/grid_size) * grid_size
 
         # move the items that have been dragged
         for it,pos in self.drag_items:
             it.setPos(QPointF(pos.x() + dx, pos.y() + dy))
 
-        # update positions for any tentacles attached to dragged items
         for it in self.items():
+            # update positions for any vertices and tentacles attached to dragged items
             if isinstance(it, TItem):
                 for it1,_ in self.drag_items:
-                    if it.vitem == it1 or it.eitem == it1:
+                    if it.vitem == it1 or it.eitem == it1 or it.vitem.eitem == it1:
+                        it.vitem.refresh()
                         it.refresh()
                         break
-            elif isinstance(it, VItem) or (isinstance(it, EItem) and it.is_id):
+
+            # if the mouse is near a vertex or identity box, make it visible
+            if isinstance(it, VItem) or (isinstance(it, EItem) and it.is_id):
                 if abs(it.pos().x() - p.x()) < 10 and abs(it.pos().y() - p.y()) < 10:
                     it.setVisible(True)
                 else:
                     it.setVisible(False)
 
 
     def mouseReleaseEvent(self, _: QGraphicsSceneMouseEvent) -> None:
```

### Comparing `chyp-0.4/chyp/gui/graphview.py` & `chyp-0.4.1/chyp/gui/graphview.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/highlighter.py` & `chyp-0.4.1/chyp/gui/highlighter.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/gui/mainwindow.py` & `chyp-0.4.1/chyp/gui/mainwindow.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/layout.py` & `chyp-0.4.1/chyp/layout.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,30 +29,46 @@
 
     Vertices and edges are placed in layers according to `layer_decomp`. Their
     y-coordinates are chosen by convex optimation to try to make connections as
     straight as possible subject to the constraints:
       1. inputs and outputs must be in order and at least 1.0 apart
       2. edges must be in order and not overlapping
     """
-    v_layers, e_layers = layer_decomp(g)
+    e_layers = layer_decomp(g)
 
     # initialise x-coordinates and rough y-coordinates
-    x = -(len(v_layers) - 1) * 1.5
-    for layer in range(len(v_layers)):
-        for i, v in enumerate(v_layers[layer]):
-            vd = g.vertex_data(v)
-            vd.x = x if layer == 0 or layer == len(v_layers)-1 else x - 0.8
-            vd.y = i - (len(v_layers[layer])-1)/2
-        if layer >= len(e_layers): break
-        for i, e in enumerate(e_layers[layer]):
+    x = -(len(e_layers) + 1) * 1.5
+    inp = list(g.inputs())
+    for i, v in enumerate(inp):
+        vd = g.vertex_data(v)
+        vd.x = x + 1.5
+        vd.y = i - (len(inp)-1)/2
+
+    x += 3.0
+
+    for e_layer in e_layers:
+        v_layer = []
+        for i, e in enumerate(e_layer):
             ed = g.edge_data(e)
-            ed.x = x + 1.5
-            ed.y = 2 * i - (len(e_layers[layer])-1)
+            ed.x = x
+            ed.y = 2 * i - (len(e_layer)-1)
+            v_layer += ed.t
+
+        for i, v in enumerate(v_layer):
+            vd = g.vertex_data(v)
+            vd.x = x + 0.7
+            vd.y = i - (len(v_layer)-1)/2
         x += 3.0
 
+    outp = list(g.outputs())
+    for i, v in enumerate(outp):
+        vd = g.vertex_data(v)
+        vd.x = x - 1.5
+        vd.y = i - (len(outp)-1)/2
+
     if g.num_vertices() == 0 or g.num_edges() == 0: return
 
     # solve for better y-coordinates using convex optimisation
     
     # variables for the y-coordinates of vertices/edges
     vy = Variable(g.num_vertices(), 'vy')
     ey = Variable(g.num_edges(), 'ey')
@@ -124,74 +140,74 @@
         ed.y = y - yshift
         for j,v in enumerate(ed.t):
             if not g.is_boundary(v):
                 yshift_v = 0 if len(ed.t) <= 1 else ((j / (len(ed.t) - 1)) - 0.5)
                 g.vertex_data(v).y = ed.y + yshift_v
 
 
-def layer_layout(g: Graph) -> None:
-    """A simple layout using `layer_decomp`.
-
-    Vertices are evenly spaced around the x-axis and edges are placed
-    as close to the average y-coordinate of their inputs as possible.
-    """
-    v_layers, e_layers = layer_decomp(g)
-    x = -(len(v_layers) - 1) * 1.5
-    for l in range(len(e_layers)):
-        v_layer = v_layers[l]
-        e_layer = e_layers[l]
-        for i, v in enumerate(v_layer):
-            vd = g.vertex_data(v)
-            vd.x = x
-            vd.y = i - ((len(v_layer) - 1) * 0.5)
+# def layer_layout(g: Graph) -> None:
+#     """A simple layout using `layer_decomp`.
 
-        # place edges, starting from the middle and working outward
-        end = len(e_layer)
-        start = math.ceil(end/2)
-
-        max_y = 0.0 # max y-coordinate for edges above the middle
-        min_y = 0.0 # min y-coordinate for edges below the middle
-
-        # for an odd number of edges, place the middle edge first
-        if start > end/2:
-            i = start-1
-            ed = g.edge_data(e_layer[i])
-            ed.x = x + 1.5
-            ed.y = sum(g.vertex_data(v).y for v in ed.s)/len(ed.s) if len(ed.s) != 0 else 0
-            pad = ed.box_size() * 0.5
-            min_y = pad
-            max_y = -pad
-
-        for i1 in range(start, end):
-            i0 = end - i1 - 1
-
-            # place one edge above max_y
-            ed = g.edge_data(e_layer[i0])
-            pad = ed.box_size() * 0.5
-            ed.x = x + 1.5
-            ed.y = min(max_y - pad,
-                       sum(g.vertex_data(v).y for v in ed.s)/len(ed.s)
-                           if len(ed.s) != 0 else 0)
-            max_y = ed.y - pad
-
-            # place one edge below min_y
-            ed = g.edge_data(e_layer[i1])
-            pad = ed.box_size() * 0.5
-            ed.x = x + 1.5
-            ed.y = max(min_y + pad,
-                       sum(g.vertex_data(v).y for v in ed.s)/len(ed.s)
-                           if len(ed.s) != 0 else 0)
-            min_y = ed.y + pad
-
-        x += 3.0
-
-    for i, v in enumerate(v_layers[-1]):
-        vd = g.vertex_data(v)
-        vd.x = x
-        vd.y = i - ((len(v_layers[-1]) - 1) * 0.5)
+#     Vertices are evenly spaced around the x-axis and edges are placed
+#     as close to the average y-coordinate of their inputs as possible.
+#     """
+#     v_layers, e_layers = layer_decomp(g)
+#     x = -(len(v_layers) - 1) * 1.5
+#     for l in range(len(e_layers)):
+#         v_layer = v_layers[l]
+#         e_layer = e_layers[l]
+#         for i, v in enumerate(v_layer):
+#             vd = g.vertex_data(v)
+#             vd.x = x
+#             vd.y = i - ((len(v_layer) - 1) * 0.5)
+
+#         # place edges, starting from the middle and working outward
+#         end = len(e_layer)
+#         start = math.ceil(end/2)
+
+#         max_y = 0.0 # max y-coordinate for edges above the middle
+#         min_y = 0.0 # min y-coordinate for edges below the middle
+
+#         # for an odd number of edges, place the middle edge first
+#         if start > end/2:
+#             i = start-1
+#             ed = g.edge_data(e_layer[i])
+#             ed.x = x + 1.5
+#             ed.y = sum(g.vertex_data(v).y for v in ed.s)/len(ed.s) if len(ed.s) != 0 else 0
+#             pad = ed.box_size() * 0.5
+#             min_y = pad
+#             max_y = -pad
+
+#         for i1 in range(start, end):
+#             i0 = end - i1 - 1
+
+#             # place one edge above max_y
+#             ed = g.edge_data(e_layer[i0])
+#             pad = ed.box_size() * 0.5
+#             ed.x = x + 1.5
+#             ed.y = min(max_y - pad,
+#                        sum(g.vertex_data(v).y for v in ed.s)/len(ed.s)
+#                            if len(ed.s) != 0 else 0)
+#             max_y = ed.y - pad
+
+#             # place one edge below min_y
+#             ed = g.edge_data(e_layer[i1])
+#             pad = ed.box_size() * 0.5
+#             ed.x = x + 1.5
+#             ed.y = max(min_y + pad,
+#                        sum(g.vertex_data(v).y for v in ed.s)/len(ed.s)
+#                            if len(ed.s) != 0 else 0)
+#             min_y = ed.y + pad
+
+#         x += 3.0
+
+#     for i, v in enumerate(v_layers[-1]):
+#         vd = g.vertex_data(v)
+#         vd.x = x
+#         vd.y = i - ((len(v_layers[-1]) - 1) * 0.5)
 
 
 
 
 # def ready_edges(g: Graph, edges: Set[int], v_done: Set[int]) -> Set[int]:
 #     ready = set()
 #     for e in edges:
```

### Comparing `chyp-0.4/chyp/matcher.py` & `chyp-0.4.1/chyp/matcher.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/parser.py` & `chyp-0.4.1/chyp/parser.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/rewrite.py` & `chyp-0.4.1/chyp/rewrite.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/rule.py` & `chyp-0.4.1/chyp/rule.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/scraps.py` & `chyp-0.4.1/chyp/scraps.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp/state.py` & `chyp-0.4.1/chyp/state.py`

 * *Files identical despite different names*

### Comparing `chyp-0.4/chyp.egg-info/PKG-INFO` & `chyp-0.4.1/chyp.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chyp
-Version: 0.4
+Version: 0.4.1
 Summary: An interactive theorem prover for string diagrams
 Home-page: https://github.com/akissinger/chyp
 Author: Aleks Kissinger
 Author-email: aleks0@gmail.com
 License: Apache2
 Project-URL: Bug Tracker, https://github.com/akissinger/chyp/issues
 Classifier: Programming Language :: Python :: 3
@@ -124,27 +124,27 @@
       = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
 
 Now, when we place the cursor over any step of this rule, it is highlighted in green, and it shows where that rule is applied. The green highlighting is indicating that Chyp has successfully checked this step. Namely, it has matched the LHS of the given rule on the previous term, rewritten the LHS to the RHS, and checked the result is the same as the term given. If we make a mistake in the example above (e.g. try to replace `assoc` with `bialg` or `sw` with `id * id`), that line will turn red. This means Chyp was _not_ able to find a matching for the rule given which implies the given equality.
 
 By default, Chyp tries to apply rules from left to right. We can apply a rule in the other direction by prefixing the rule name with `-`. For example, the proof above can be done backwards as follows:
 
     rewrite ba1_backwards :
-      f * id ; f ; g ; g * id
-      = id * f ; f ; g ; g * id by assoc
-      = g * f ; id * id * g ; id * sw * id ; f * f ; g * id by bialg
+      g * f ; id * id * g ; id * sw * id ; f * f ; g * id
+      = id * f ; f ; g ; g * id by -bialg
+      = f * id ; f ; g ; g * id by -assoc
 
 The golden rule of Chyp is that _only connectivity matters_. So, if two terms give the same diagram, like `a * b ; c * d` and `(a ; c) * (b ; d)`, Chyp treats them as identical. Since under the hood, Chyp does everything with graph rewriting and not term rewriting, the prover handles all of this extra book-keeping for you.
 
 Sometimes it can be helpful for readability to do a trivial proof step that does nothing but write the same string diagram differently. There is a special rule called `refl` (for reflexivity) for this. For example:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d) by refl
 
-In fact, we can omit the `by refl`. The following is equivalent:
+Formally, `refl` is defined as `id0 = id0`, i.e. the empty graph equals itself, which always matches exactly once on any graph. If we drop the `by` clause, Chyp automatically assumes `by refl`, so the following is equivalent:
 
     rewrite foo :
       a * b ; c * d
       = (a ; c) * (b ; d)
 
 
 The `def` statement introduced in the previous section is just syntactic sugar for a `gen` followed by a rule. That is:
@@ -187,15 +187,15 @@
       = g * g * g ; id * id * id * sw * id ; id * g * f * g * g ; sw * sw * id * sw * id ; id * f * id * f * f ; sw * sw * id ; id * f * f by bialg
 
 How to we know it's a normal form? Pressing `CTRL+SHIFT+Enter` one more time will result in a red line that reads `  = ? by bialg`, which means Chyp wasn't able to find any more matchings of the `bialg` rule.
 
 
 # Modules and importing
 
-As structures and proofs get more complicated, we may want to split them into multiple files. Every `*.chyp` file defines a module, which can be imported in other `*.chyp` file. Suppose for example we define the following file `monoid.chyp`:
+As structures and proofs get more complicated, we may want to split them into multiple files. Every chyp file defines a module, which can be imported in other chyp files. Suppose for example we define the following file `monoid.chyp`:
 
     gen m : 2 -> 1
     gen u : 0 -> 1
     rule assoc : m * id ; m = id * m ; m
     rule unitL : u * id ; m = id
     rule unitR : id * u ; m = id
 
@@ -228,30 +228,67 @@
     import cmonoid as M2(m = m2, u = u2)
 
     gen cp : 1 -> 2
     rule dist :
       m1 * id ; m2 = 
       = id * m1 ; m2 = cp * id * id ; id * sw * id ; m2 * m2 ; m1
 
+Even though we now have short aliases for generators, the rules still live in their respective namespaces. For example, `M1.assoc` can be used to rewrite `m1 * id ; m1` to `id * m1 ; m1` and `M2.assoc` will rewrite `m2 * id ; m2` to `id * m2 ; m2`.
+
 This is especially convenient if modules share generators in non-trivial ways. For example, a pair of Frobenius algebras interacting as a bialgebra could be defined this way, assuming `frobenius.chyp` and `bialg.chyp` have already been defined:
 
     gen m1 : 2 -> 1
     gen u1 : 0 -> 1
     gen n1 : 1 -> 2
     gen v1 : 1 -> 0
 
     gen m2 : 2 -> 1
     gen u2 : 0 -> 1
     gen n2 : 1 -> 2
     gen v2 : 1 -> 0
 
-    import frobenius(m = m1, u = u1, n = n1, v = v1) as F1
-    import frobenius(m = m2, u = u2, n = n2, v = v2) as F2
-    import bialg(m = m1, u = u1, n = n2, v = v2) as B1
-    import bialg(m = m2, u = u2, n = n1, v = v1) as B2
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+    import frobenius as F2(m = m2, u = u2, n = n2, v = v2)
+    import bialg as B1(m = m1, u = u1, n = n2, v = v2)
+    import bialg as B2(m = m2, u = u2, n = n1, v = v1)
+
+We can even set the generators in an imported module equal to arbitrary terms, as long as the types match.
+
+To understand how this works, it is useful to know that this is just some syntactic sugar that takes advantage of the behaviour of the `gen` statement. Normally, the `gen` statement will add a new generator to the current namespace. However, if a term with that name already exists, it will simply check the already existing term has the right arity and coarity. This allows us to alias generators in a module using `let` statements _before_ it is imported. So, in fact, the line:
+
+    import frobenius as F1(m = m1, u = u1, n = n1, v = v1)
+
+is exactly equivalent to:
+
+    let F1.m = m1
+    let F1.u = u1
+    let F1.n = n1
+    let F1.v = v1
+    import frobenius as F1
+
+Whenever an `m` is encountered in `frobenius.chyp` (which will be interpreted as `F1.m`), it will automatically get replaced by `m1` thanks to the `let` statement.
+
+If we alias generators to some more complicated terms, these just end up the RHS of the `let` statements. For example, we could get the "almost" Frobenius algebra laws of the [ZW calculus](https://arxiv.org/abs/1501.07082) with a statement like this:
+
+
+    gen m : 2 -> 1
+    gen u : 0 -> 1
+    gen n : 1 -> 2
+    gen v : 1 -> 0
+    gen d : 1 -> 1
+
+    import frobenius as W(m = d * d ; m, u = u, n = d ; n, v = d ; v)
+
+where the last line is equivalent to:
+
+    let W.m = d * d ; m
+    let W.u = u
+    let W.n = d ; n
+    let W.v = d ; v
+    import frobenius as W
 
 
 ## Finding modules
 
 The `import` statement always looks for `*.chyp` files in the same directory of the current file. Chyp doesn't have a notion of "search paths" for modules, but this might be added in the future.
 
 Files can be imported from subdirectories by adding dots:
```

### Comparing `chyp-0.4/chyp.egg-info/SOURCES.txt` & `chyp-0.4.1/chyp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `chyp-0.4/setup.py` & `chyp-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     long_description = fh.read()
 
 
 data_files = []
 
 setuptools.setup(
     name="chyp",
-    version="0.4",
+    version="0.4.1",
     author="Aleks Kissinger",
     author_email="aleks0@gmail.com",
     description="An interactive theorem prover for string diagrams",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akissinger/chyp",
     project_urls={
```

