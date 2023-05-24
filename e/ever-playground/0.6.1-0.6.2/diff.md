# Comparing `tmp/ever_playground-0.6.1.tar.gz` & `tmp/ever_playground-0.6.2.tar.gz`

## Comparing `ever_playground-0.6.1.tar` & `ever_playground-0.6.2.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 ever_playground-0.6.1/Cargo.toml
--rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.1/.gitignore
--rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.6.1/.vscode/settings.json
--rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.1/README.md
--rw-rw-r--   0     1000     1000     4831 2023-05-22 11:02:08.000000 ever_playground-0.6.1/ever_playground/__init__.py
--rw-rw-r--   0     1000     1000     5944 2023-05-22 15:35:59.000000 ever_playground-0.6.1/ever_playground/ever_playground.pyi
--rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.1/examples/basics.py
--rw-rw-r--   0     1000     1000      836 2023-05-22 14:54:56.000000 ever_playground-0.6.1/examples/highload/generate.fif
--rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.1/examples/highload/highload-wallet-v2.fif
--rw-rw-r--   0     1000     1000     4689 2023-05-22 16:05:26.000000 ever_playground-0.6.1/examples/highload/highload-wallet-v2.py
--rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/order-list-fift
--rw-------   0     1000     1000      234 2023-05-22 14:54:59.000000 ever_playground-0.6.1/examples/highload/order-list-py
--rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/sample.pk
--rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.1/examples/highload/sample27172.addr
--rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.1/examples/recover-stake.fif
--rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.1/examples/recover-stake.py
--rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.1/examples/runvm.py
--rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.1/examples/testgiver.fif
--rw-rw-r--   0     1000     1000     2902 2023-05-22 11:25:27.000000 ever_playground-0.6.1/examples/testgiver.py
--rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.1/examples/validator-elect-req.fif
--rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.1/examples/validator-elect-req.py
--rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.1/pyproject.toml
--rwxrwxr-x   0     1000     1000     2879 2023-05-22 16:19:13.000000 ever_playground-0.6.1/run-examples.py
--rw-rw-r--   0     1000     1000    18118 2023-05-22 15:37:09.000000 ever_playground-0.6.1/src/lib.rs
--rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.6.1/src/tests.rs
--rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.1/src/utils.rs
--rw-rw-r--   0     1000     1000    24730 2023-05-22 16:18:35.000000 ever_playground-0.6.1/Cargo.lock
--rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      604 1970-01-01 00:00:00.000000 ever_playground-0.6.2/Cargo.toml
+-rw-rw-r--   0     1000     1000       78 2023-05-15 13:10:44.000000 ever_playground-0.6.2/.gitignore
+-rw-rw-r--   0     1000     1000      181 2023-05-12 14:44:59.000000 ever_playground-0.6.2/.vscode/settings.json
+-rw-rw-r--   0     1000     1000      566 2023-05-17 11:44:03.000000 ever_playground-0.6.2/README.md
+-rw-rw-r--   0     1000     1000     4831 2023-05-22 11:02:08.000000 ever_playground-0.6.2/ever_playground/__init__.py
+-rw-rw-r--   0     1000     1000     5944 2023-05-22 15:35:59.000000 ever_playground-0.6.2/ever_playground/ever_playground.pyi
+-rw-rw-r--   0     1000     1000     2245 2023-05-22 13:02:10.000000 ever_playground-0.6.2/examples/basics.py
+-rw-rw-r--   0     1000     1000      821 2023-05-22 21:04:47.000000 ever_playground-0.6.2/examples/highload/generate.fif
+-rwxrwxr-x   0     1000     1000     3399 2023-05-22 16:05:31.000000 ever_playground-0.6.2/examples/highload/highload-wallet-v2.fif
+-rw-rw-r--   0     1000     1000     4688 2023-05-22 21:07:18.000000 ever_playground-0.6.2/examples/highload/highload-wallet-v2.py
+-rw-------   0     1000     1000      180 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/order-list-fift
+-rw-------   0     1000     1000      240 2023-05-22 21:04:58.000000 ever_playground-0.6.2/examples/highload/order-list-py
+-rw-------   0     1000     1000       32 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/sample.pk
+-rw-------   0     1000     1000       36 2023-05-22 14:37:50.000000 ever_playground-0.6.2/examples/highload/sample27172.addr
+-rw-rw-r--   0     1000     1000     1487 2023-05-24 13:11:36.000000 ever_playground-0.6.2/examples/ifjmp-perf-eval.py
+-rwxrwxr-x   0     1000     1000      870 2023-05-22 16:19:06.000000 ever_playground-0.6.2/examples/recover-stake.fif
+-rw-rw-r--   0     1000     1000     1889 2023-05-22 16:19:27.000000 ever_playground-0.6.2/examples/recover-stake.py
+-rw-rw-r--   0     1000     1000     2327 2023-05-22 13:04:32.000000 ever_playground-0.6.2/examples/runvm.py
+-rwxrwxr-x   0     1000     1000     1187 2023-05-22 11:04:24.000000 ever_playground-0.6.2/examples/testgiver.fif
+-rw-rw-r--   0     1000     1000     2864 2023-05-23 09:21:52.000000 ever_playground-0.6.2/examples/testgiver.py
+-rwxrwxr-x   0     1000     1000     1645 2023-05-22 12:49:48.000000 ever_playground-0.6.2/examples/validator-elect-req.fif
+-rw-rw-r--   0     1000     1000     3607 2023-05-20 15:28:34.000000 ever_playground-0.6.2/examples/validator-elect-req.py
+-rw-rw-r--   0     1000     1000      946 2023-05-17 10:02:52.000000 ever_playground-0.6.2/pyproject.toml
+-rwxrwxr-x   0     1000     1000     3030 2023-05-24 13:21:40.000000 ever_playground-0.6.2/run-examples.py
+-rw-rw-r--   0     1000     1000    18118 2023-05-22 15:37:09.000000 ever_playground-0.6.2/src/lib.rs
+-rw-rw-r--   0     1000     1000     1064 2023-05-11 14:01:16.000000 ever_playground-0.6.2/src/tests.rs
+-rw-rw-r--   0     1000     1000     3689 2023-05-15 14:26:56.000000 ever_playground-0.6.2/src/utils.rs
+-rw-rw-r--   0     1000     1000    24730 2023-05-24 13:19:21.000000 ever_playground-0.6.2/Cargo.lock
+-rw-r--r--   0        0        0      718 1970-01-01 00:00:00.000000 ever_playground-0.6.2/PKG-INFO
```

### Comparing `ever_playground-0.6.1/Cargo.toml` & `ever_playground-0.6.2/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "ever-playground"
-version = "0.6.1"
+version = "0.6.2"
 edition = "2021"
 
 [lib]
 name = "ever_playground"
 crate-type = ["cdylib"]
 
 [dependencies]
```

### Comparing `ever_playground-0.6.1/README.md` & `ever_playground-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/ever_playground/__init__.py` & `ever_playground-0.6.2/ever_playground/__init__.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/ever_playground/ever_playground.pyi` & `ever_playground-0.6.2/ever_playground/ever_playground.pyi`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/basics.py` & `ever_playground-0.6.2/examples/basics.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/highload/generate.fif` & `ever_playground-0.6.2/examples/highload/generate.fif`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 #!/usr/bin/fift -s
 "TonUtil.fif" include
-"GetOpt.fif" include
 
 0 0x0000000000000000000000000000000000000000000000000000000000000000 "sample27172.addr" save-address
 newkeypair drop "sample.pk" B>file
 
 "SEND " 1 0x1111111111111111111111111111111111111111111111111111111111111111 0 smca>$ $+ " 1.111" $+ +cr
 "SEND " 2 0x2222222222222222222222222222222222222222222222222222222222222222 0 smca>$ $+ " 2.222" $+ +cr $+
 "SEND " 3 0x3333333333333333333333333333333333333333333333333333333333333333 0 smca>$ $+ " 3.333" $+ +cr $+
 $>B "order-list-fift" B>file
 
-"SEND 1:1111111111111111111111111111111111111111111111111111111111111111 1.111" +cr
-"SEND 2:2222222222222222222222222222222222222222222222222222222222222222 2.222" +cr $+
-"SEND 3:3333333333333333333333333333333333333333333333333333333333333333 3.333" +cr $+
+"SEND 1:1111111111111111111111111111111111111111111111111111111111111111 1 1.111" +cr
+"SEND 2:2222222222222222222222222222222222222222222222222222222222222222 1 2.222" +cr $+
+"SEND 3:3333333333333333333333333333333333333333333333333333333333333333 1 3.333" +cr $+
 $>B "order-list-py" B>file
```

### Comparing `ever_playground-0.6.1/examples/highload/highload-wallet-v2.fif` & `ever_playground-0.6.2/examples/highload/highload-wallet-v2.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/highload/highload-wallet-v2.py` & `ever_playground-0.6.2/examples/highload/highload-wallet-v2.py`

 * *Files 4% similar despite different names*

```diff
@@ -83,19 +83,20 @@
     t = create_simple_transfer(address, ng, bounce)
     order = create_order(t, send_mode)
     add_order(Slice(order))
 
 with open(order_file, "r") as file:
     for line in file:
         chunks = line.split(" ")
-        assert(len(chunks) == 3)
+        assert(len(chunks) == 4)
         assert(chunks[0] == "SEND")
         address = chunks[1]
-        ng = Currency.from_str(chunks[2])
-        send(address, ng, True) # TODO read bounce from order list?
+        bounce = bool(chunks[2])
+        ng = Currency.from_str(chunks[3])
+        send(address, ng, bounce)
 
 now = 1684770872 # int(time.time())
 orders_cell = orders.serialize().finalize()
 query_id = ((now + timeout) << 32) + (orders_cell.repr_hash() & 0xffffffff)
 
 signing_message = Builder().i(32, subwallet_id).i(64, query_id).s(Slice(orders_cell)).finalize()
 print(f"signing message: {signing_message}")
```

### Comparing `ever_playground-0.6.1/examples/recover-stake.fif` & `ever_playground-0.6.2/examples/recover-stake.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/recover-stake.py` & `ever_playground-0.6.2/examples/recover-stake.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/runvm.py` & `ever_playground-0.6.2/examples/runvm.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/testgiver.fif` & `ever_playground-0.6.2/examples/testgiver.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/testgiver.py` & `ever_playground-0.6.2/examples/testgiver.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 # #!/usr/bin/fift -s
 # "TonUtil.fif" include
 
 import sys
-from fractions import Fraction
-
 from ever_playground import Builder as B, Slice as S, Currency, parse_smc_addr, parse_load_address
 
 # { ."usage: " @' $0 type ." <dest-addr> <seqno> <amount> [<savefile>]" cr
 #   ."Creates a request to TestGiver and saves it into <savefile>.boc" cr
 #   ."('testgiver-query.boc' by default)" cr 1 halt
 # } : usage
 def usage():
@@ -48,17 +46,17 @@
 print(f"Requesting {amount} to account {dest_address} seqno {hex(seqno)} bounce {bounce}")
 
 # // create a message (NB: 01b00.., b = bounce)
 # <b b{01} s, bounce 1 i, b{000100} s, dest_addr addr, 
 #    amount Gram, 0 9 64 32 + + 1+ 1+ u, 0 32 u, "GIFT" $, b>
 # <b seqno 32 u, 1 8 u, swap ref, b>
 # dup ."enveloping message: " <s csr. cr
-hint = bytes("GIFT", "utf8").hex()
+hint = bytes("GIFT", "utf8")
 c1 = B().ib("01").i(1, bounce).ib("000100").i(8, dest_wc).i(256, dest_addr) \
-    .b(amount.serialize()).i(9 + 64 + 32 + 1 + 1, 0).i(32, 0).x(hint) \
+    .b(amount.serialize()).i(9 + 64 + 32 + 1 + 1, 0).i(32, 0).y(hint) \
     .finalize()
 message = B().i(32, seqno).i(8, 1).r(c1).finalize()
 print(f"enveloping message: {message}")
 
 # <b b{1000100} s, giver_addr addr, 0 Gram, b{00} s,
 #    swap <s s, b>
 # dup ."resulting external message: " <s csr. cr
```

### Comparing `ever_playground-0.6.1/examples/validator-elect-req.fif` & `ever_playground-0.6.2/examples/validator-elect-req.fif`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/examples/validator-elect-req.py` & `ever_playground-0.6.2/examples/validator-elect-req.py`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/pyproject.toml` & `ever_playground-0.6.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/run-examples.py` & `ever_playground-0.6.2/run-examples.py`

 * *Files 8% similar despite different names*

```diff
@@ -66,14 +66,15 @@
     
     run(["python3", script + ".py"] + common + [py_output])
     run(fift + [script + ".fif"] + common + [fift_output])
 
     assert_identical_files(py_output, fift_output)
 
 def test_highload_wallet_v2():
+    curdir = os.getcwd()
     os.chdir("examples/highload")
 
     script = "highload-wallet-v2"
     base = "wallet-query"
     py_output = "py-" + base
     fift_output = "fift-" + base
 
@@ -84,13 +85,19 @@
     # assert_identical_files(py_output + ".boc", fift_output + ".boc")
     p = Cell.read(open(py_output + ".boc", "rb").read())
     f = Cell.read(open(fift_output + ".boc", "rb").read())
     remove(py_output + ".boc")
     remove(fift_output + ".boc")
     assert(p == f)
 
+    os.chdir(curdir)
+
+def test_ifjmp_perf_eval():
+    run(["python3", "examples/ifjmp-perf-eval.py"])
+
 run_basics()
 run_runvm()
 test_recover_stake()
 test_testgiver()
 test_validator_elect_req()
 test_highload_wallet_v2()
+test_ifjmp_perf_eval()
```

### Comparing `ever_playground-0.6.1/src/lib.rs` & `ever_playground-0.6.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/src/tests.rs` & `ever_playground-0.6.2/src/tests.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/src/utils.rs` & `ever_playground-0.6.2/src/utils.rs`

 * *Files identical despite different names*

### Comparing `ever_playground-0.6.1/Cargo.lock` & `ever_playground-0.6.2/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -223,15 +223,15 @@
  "serde",
  "sha2 0.9.9",
  "zeroize",
 ]
 
 [[package]]
 name = "ever-playground"
-version = "0.6.1"
+version = "0.6.2"
 dependencies = [
  "ed25519-dalek",
  "num-bigint",
  "pyo3",
  "rand",
  "ton_block",
  "ton_labs_assembler",
```

### Comparing `ever_playground-0.6.1/PKG-INFO` & `ever_playground-0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ever-playground
-Version: 0.6.1
+Version: 0.6.2
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # ever-playground
 
 A tool alternative to Fift: play with Cells, Slices, Builders, and Dictionaries — native types of TVM; assemble and run TVM code.
```

