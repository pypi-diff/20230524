# Comparing `tmp/sqlite_vss-0.1.1a5-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip` & `tmp/sqlite_vss-0.1.1a6-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 1545974 bytes, number of entries: 9
--rwxr-xr-x  2.0 unx    15784 b- defN 23-May-23 17:03 noop.cpython-311-x86_64-linux-gnu.so
--rw-r--r--  2.0 unx      572 b- defN 23-May-23 17:03 sqlite_vss/__init__.py
--rw-r--r--  2.0 unx   186896 b- defN 23-May-23 17:03 sqlite_vss/vector0.so
--rw-r--r--  2.0 unx       79 b- defN 23-May-23 17:03 sqlite_vss/version.py
--rw-r--r--  2.0 unx  5124248 b- defN 23-May-23 17:03 sqlite_vss/vss0.so
--rw-r--r--  2.0 unx      496 b- defN 23-May-23 17:03 sqlite_vss-0.1.1a5.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 23-May-23 17:03 sqlite_vss-0.1.1a5.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 23-May-23 17:03 sqlite_vss-0.1.1a5.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      724 b- defN 23-May-23 17:03 sqlite_vss-0.1.1a5.dist-info/RECORD
-9 files, 5328920 bytes uncompressed, 1544736 bytes compressed:  71.0%
+Zip file size: 1545980 bytes, number of entries: 9
+-rwxr-xr-x  2.0 unx    15792 b- defN 23-May-23 21:07 noop.cpython-311-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      572 b- defN 23-May-23 21:07 sqlite_vss/__init__.py
+-rw-r--r--  2.0 unx   186896 b- defN 23-May-23 21:07 sqlite_vss/vector0.so
+-rw-r--r--  2.0 unx       79 b- defN 23-May-23 21:07 sqlite_vss/version.py
+-rw-r--r--  2.0 unx  5124248 b- defN 23-May-23 21:07 sqlite_vss/vss0.so
+-rw-r--r--  2.0 unx      496 b- defN 23-May-23 21:07 sqlite_vss-0.1.1a6.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 23-May-23 21:07 sqlite_vss-0.1.1a6.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 23-May-23 21:07 sqlite_vss-0.1.1a6.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      724 b- defN 23-May-23 21:07 sqlite_vss-0.1.1a6.dist-info/RECORD
+9 files, 5328928 bytes uncompressed, 1544742 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -9,20 +9,20 @@
 
 Filename: sqlite_vss/version.py
 Comment: 
 
 Filename: sqlite_vss/vss0.so
 Comment: 
 
-Filename: sqlite_vss-0.1.1a5.dist-info/METADATA
+Filename: sqlite_vss-0.1.1a6.dist-info/METADATA
 Comment: 
 
-Filename: sqlite_vss-0.1.1a5.dist-info/WHEEL
+Filename: sqlite_vss-0.1.1a6.dist-info/WHEEL
 Comment: 
 
-Filename: sqlite_vss-0.1.1a5.dist-info/top_level.txt
+Filename: sqlite_vss-0.1.1a6.dist-info/top_level.txt
 Comment: 
 
-Filename: sqlite_vss-0.1.1a5.dist-info/RECORD
+Filename: sqlite_vss-0.1.1a6.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## noop.cpython-311-x86_64-linux-gnu.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              DYN (Shared object file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x1040
   Start of program headers:          64 (bytes into file)
-  Start of section headers:          14184 (bytes into file)
+  Start of section headers:          14192 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           56 (bytes)
   Number of program headers:         10
   Size of section headers:           64 (bytes)
   Number of section headers:         25
   Section header string table index: 24
```

### readelf --wide --sections {}

```diff
@@ -1,8 +1,8 @@
-There are 25 section headers, starting at offset 0x3768:
+There are 25 section headers, starting at offset 0x3770:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .note.gnu.property NOTE            0000000000000270 000270 000020 00   A  0   0  8
   [ 2] .note.gnu.build-id NOTE            0000000000000290 000290 000024 00   A  0   0  4
   [ 3] .gnu.hash         GNU_HASH        00000000000002b8 0002b8 00001c 00   A  4   0  8
@@ -19,16 +19,16 @@
   [14] .fini_array       FINI_ARRAY      0000000000003e78 002e78 000008 08  WA  0   0  8
   [15] .dynamic          DYNAMIC         0000000000003e80 002e80 000160 10  WA  5   0  8
   [16] .got              PROGBITS        0000000000003fe0 002fe0 000020 08  WA  0   0  8
   [17] .got.plt          PROGBITS        0000000000004000 003000 000018 08  WA  0   0  8
   [18] .data             PROGBITS        0000000000004018 003018 000008 00  WA  0   0  8
   [19] .bss              NOBITS          0000000000004020 003020 000008 00  WA  0   0  1
   [20] .comment          PROGBITS        0000000000000000 003020 00002b 01  MS  0   0  1
-  [21] .debug_str        PROGBITS        0000000000000000 00304b 0000e0 01  MS  0   0  1
-  [22] .symtab           SYMTAB          0000000000000000 003130 000420 18     23  40  8
-  [23] .strtab           STRTAB          0000000000000000 003550 000145 00      0   0  1
-  [24] .shstrtab         STRTAB          0000000000000000 003695 0000d3 00      0   0  1
+  [21] .debug_str        PROGBITS        0000000000000000 00304b 0000e9 01  MS  0   0  1
+  [22] .symtab           SYMTAB          0000000000000000 003138 000420 18     23  40  8
+  [23] .strtab           STRTAB          0000000000000000 003558 000145 00      0   0  1
+  [24] .shstrtab         STRTAB          0000000000000000 00369d 0000d3 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 9e7a35e71b0e12fd51a00bc508eda2f0e3f84fd0
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ba6f77c8ad8704485ea190dfd58003e21f1bd93f
```

### strings --all --bytes=8 {}

```diff
@@ -1,15 +1,15 @@
 __gmon_start__
 _ITM_deregisterTMCloneTable
 _ITM_registerTMCloneTable
 __cxa_finalize
 /opt/hostedtoolcache/Python/3.11.3/x64/lib
 GCC: (Ubuntu 9.4.0-1ubuntu1~20.04.1) 9.4.0
+/home/runner/work/sqlite-vss/sqlite-vss/bindings/python/sqlite_vss
 GNU C17 9.4.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
-/home/runner/work/sqlite-vss/sqlite-vss/python/sqlite_vss
 crtstuff.c
 deregister_tm_clones
 __do_global_dtors_aux
 completed.8061
 __do_global_dtors_aux_fini_array_entry
 frame_dummy
 __frame_dummy_init_array_entry
```

### readelf --wide --decompress --string-dump=.debug_str {}

```diff
@@ -1,6 +1,6 @@
 
 String dump of section '.debug_str':
-  [     0]  GNU C17 9.4.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
-  [    9f]  /home/runner/work/sqlite-vss/sqlite-vss/python/sqlite_vss
-  [    d9]  noop.c
+  [     0]  /home/runner/work/sqlite-vss/sqlite-vss/bindings/python/sqlite_vss
+  [    43]  GNU C17 9.4.0 -mtune=generic -march=x86-64 -g -O3 -fwrapv -fPIC -fasynchronous-unwind-tables -fstack-protector-strong -fstack-clash-protection -fcf-protection
+  [    e2]  noop.c
```

## sqlite_vss/vector0.so

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 5475a31d0aefb57a23b8a212d4042aae17f9f35e
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: ea715c162a9e08aee4b3ced7ad43325cff0cc04f
```

### strings --all --bytes=8 {}

```diff
@@ -331,15 +331,15 @@
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATL
 []A\A]A^A_
 AVAUATUH
 []A\A]A^A_
-v0.1.1-alpha.5
+v0.1.1-alpha.6
 vector0_api_ptr
 Blob type not right
 vector_fvecs_each
 vector::_M_range_insert
 %d out of range: %s
 value not a vector
 size: %lld [
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x0001f000 76302e31 2e312d61 6c706861 2e350076 v0.1.1-alpha.5.v
+  0x0001f000 76302e31 2e312d61 6c706861 2e360076 v0.1.1-alpha.6.v
   0x0001f010 6563746f 72305f61 70695f70 74720042 ector0_api_ptr.B
   0x0001f020 6c6f6220 74797065 206e6f74 20726967 lob type not rig
   0x0001f030 68740076 6563746f 72300025 733a2025 ht.vector0.%s: %
   0x0001f040 73007665 63746f72 5f667665 63735f65 s.vector_fvecs_e
   0x0001f050 61636800 76656374 6f723a3a 5f4d5f72 ach.vector::_M_r
   0x0001f060 616e6765 5f696e73 65727400 2564206f ange_insert.%d o
   0x0001f070 7574206f 66207261 6e67653a 20257300 ut of range: %s.
```

## sqlite_vss/version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "0.1.1-alpha.5"
+__version__ = "0.1.1-alpha.6"
 __version_info__ = tuple(__version__.split("."))
```

## sqlite_vss/vss0.so

 * *File has been modified after NT_GNU_BUILD_ID has been applied.*

### readelf --wide --notes {}

```diff
@@ -1,8 +1,8 @@
 
 Displaying notes found in: .note.gnu.property
   Owner                Data size 	Description
   GNU                  0x00000010	NT_GNU_PROPERTY_TYPE_0	      Properties: x86 feature: IBT, SHSTK
 
 Displaying notes found in: .note.gnu.build-id
   Owner                Data size 	Description
-  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 13554f54e40985e630247ac86af3f18648cacd1a
+  GNU                  0x00000014	NT_GNU_BUILD_ID (unique build ID bitstring)	    Build ID: 3c8dc8ecab6dabe033a119ef05b5319dee5fa70f
```

### strings --all --bytes=8 {}

```diff
@@ -7381,15 +7381,15 @@
 AWAVAUATUSH
 L$ H9L$8
 []A\A]A^A_
 AWAVAUATUSH
 []A\A]A^A_
 AWAVAUATI
 [A\A]A^A_]
-v0.1.1-alpha.5
+v0.1.1-alpha.6
 fullscan
 vss_search
 vss_range_search
 1st argument is not a vector
 vss0_rangesearchparams
 vss0_searchparams
 drop table "%w_index";
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -1,10 +1,10 @@
 
 Hex dump of section '.rodata':
-  0x00380000 76302e31 2e312d61 6c706861 2e350066 v0.1.1-alpha.5.f
+  0x00380000 76302e31 2e312d61 6c706861 2e360066 v0.1.1-alpha.6.f
   0x00380010 756c6c73 63616e00 7673735f 73656172 ullscan.vss_sear
   0x00380020 63680076 73735f72 616e6765 5f736561 ch.vss_range_sea
   0x00380030 72636800 31737420 61726775 6d656e74 rch.1st argument
   0x00380040 20697320 6e6f7420 61207665 63746f72  is not a vector
   0x00380050 00767373 305f7261 6e676573 65617263 .vss0_rangesearc
   0x00380060 68706172 616d7300 76737330 5f736561 hparams.vss0_sea
   0x00380070 72636870 6172616d 73006472 6f702074 rchparams.drop t
```

## Comparing `sqlite_vss-0.1.1a5.dist-info/RECORD` & `sqlite_vss-0.1.1a6.dist-info/RECORD`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-noop.cpython-311-x86_64-linux-gnu.so,sha256=4swCe5ZHJGjSyqveLIyVe-H5qqHAIdWOwZb7Gpobwx8,15784
+noop.cpython-311-x86_64-linux-gnu.so,sha256=BRTnmVFT9picFaWyD-cpgnn1xNLs3H2ZzcRnD5qtJKo,15792
 sqlite_vss/__init__.py,sha256=5PIhAIaJ1cVKtzSV9eZaymWS4CjRHUjkJ6y8VXyaG8Y,572
-sqlite_vss/vector0.so,sha256=a0C0pcqCknkigNNspgG6jGYCRGtRiuM15rj9GL3ejKU,186896
-sqlite_vss/version.py,sha256=7SWo6eI8cbEh9e5b7e-MdX_qqyAp2ykfykFLrfuFpw4,79
-sqlite_vss/vss0.so,sha256=FEa3A-uRmmhUQNRB2lHyf1kTGI2onQySlX9QE-ZlUBA,5124248
-sqlite_vss-0.1.1a5.dist-info/METADATA,sha256=tAkOmDjR2310s54UK4lUqgd4Ndj-7G5hSAfUpjhg1hE,496
-sqlite_vss-0.1.1a5.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
-sqlite_vss-0.1.1a5.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
-sqlite_vss-0.1.1a5.dist-info/RECORD,,
+sqlite_vss/vector0.so,sha256=8TM1MPJiyHADj4pW4Gq4gV2M7MkUUSV2SUUQBxR-q6I,186896
+sqlite_vss/version.py,sha256=ooqUZBE6g7FxGP1UvOO1ulQ5CbCgNEUrjNU1BBhXWqM,79
+sqlite_vss/vss0.so,sha256=J_vfQ0PbSpRCK96C4AkHwj6kW27azPf_GKEMEXTn9RU,5124248
+sqlite_vss-0.1.1a6.dist-info/METADATA,sha256=rYuQBb9B-7Ud1Pc_gotPyc3U5M2jDuvxciJBViP8A48,496
+sqlite_vss-0.1.1a6.dist-info/WHEEL,sha256=A8X7wachHegSPoWuFmtYiHrJoCGdZ0KzfYp5hU1FoC8,105
+sqlite_vss-0.1.1a6.dist-info/top_level.txt,sha256=Z2PPuSp9qvLljXNaO4Jwv8wSXtVhLIU2qBu5OEgZxGQ,16
+sqlite_vss-0.1.1a6.dist-info/RECORD,,
```

