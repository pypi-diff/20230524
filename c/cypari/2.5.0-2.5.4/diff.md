# Comparing `tmp/cypari-2.5.0.tar.gz` & `tmp/cypari-2.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, last modified: Wed Nov 23 18:58:03 2022, from Unix
+gzip compressed data, was "cypari-2.5.4.tar", last modified: Sun Apr  2 20:59:17 2023, max compression
```

## Comparing `cypari-2.5.0.tar` & `cypari-2.5.4.tar`

### file list

```diff
@@ -1,73 +1,4653 @@
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:57:26.000000 cypari-2.5.0/
--rw-r--r--   0 nmd        (502) wheel        (0)      177 2022-11-23 18:57:26.000000 cypari-2.5.0/._PKG-INFO
--rw-r--r--   0 nmd        (502) wheel        (0)     1142 2022-11-23 18:57:26.854455 cypari-2.5.0/PKG-INFO
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/macOS/
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/patches/
--rw-r--r--   0 nmd        (502) wheel        (0)     6455 2022-11-23 18:03:46.000000 cypari-2.5.0/build_pari.sh
--rw-r--r--   0 nmd        (502) wheel        (0)      370 2022-11-23 18:03:46.000000 cypari-2.5.0/MANIFEST.in
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/
--rw-r--r--   0 nmd        (502) wheel        (0)    15364 2022-11-23 18:03:46.000000 cypari-2.5.0/setup.py
--rw-r--r--   0 nmd        (502) wheel        (0)     5062 2022-11-23 18:03:46.000000 cypari-2.5.0/appveyor.py
--rw-r--r--   0 nmd        (502) wheel        (0)     1713 2022-11-23 18:03:46.000000 cypari-2.5.0/README.rst
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/
--rw-r--r--   0 nmd        (502) wheel        (0)     2050 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/paths.py
--rw-r--r--   0 nmd        (502) wheel        (0)      733 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/__init__.py
--rw-r--r--   0 nmd        (502) wheel        (0)     5922 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/parser.py
--rw-r--r--   0 nmd        (502) wheel        (0)    13994 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/generator.py
--rw-r--r--   0 nmd        (502) wheel        (0)    10867 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/doc.py
--rw-r--r--   0 nmd        (502) wheel        (0)    11803 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/args.py
--rw-r--r--   0 nmd        (502) wheel        (0)     2358 2022-11-23 18:03:46.000000 cypari-2.5.0/autogen/ret.py
--rw-r--r--   0 nmd        (502) wheel        (0)      392 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/mingw_c.patch
--rw-r--r--   0 nmd        (502) wheel        (0)    10045 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/README.Windows
--rw-r--r--   0 nmd        (502) wheel        (0)     1629 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/pari_config.patch
--rw-r--r--   0 nmd        (502) wheel        (0)      930 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/get_toolchain.py
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/gcc/
--rw-r--r--   0 nmd        (502) wheel        (0)      132 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/clear_cache.txt
-drwxr-xr-x   0 nmd        (502) wheel        (0)        0 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/
--rw-r--r--   0 nmd        (502) wheel        (0)       48 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/get_output_format.c
--rw-r--r--   0 nmd        (502) wheel        (0)    65988 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/libparicrt32.a
--rw-r--r--   0 nmd        (502) wheel        (0)     2359 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/Makefile
--rw-r--r--   0 nmd        (502) wheel        (0)      700 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/get_output_format32.o
--rw-r--r--   0 nmd        (502) wheel        (0)    36670 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/libparicrt64.a
--rw-r--r--   0 nmd        (502) wheel        (0)    41345 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/stdio.h
--rw-r--r--   0 nmd        (502) wheel        (0)      743 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/crt/get_output_format64.o
--rw-r--r--   0 nmd        (502) wheel        (0)  3275122 2022-11-23 18:03:46.000000 cypari-2.5.0/Windows/gcc/libgcc.a
--rw-r--r--   0 nmd        (502) wheel        (0)     3886 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/types.pxd
--rw-r--r--   0 nmd        (502) wheel        (0)     6601 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/closure.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      594 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/parisage.h
--rw-r--r--   0 nmd        (502) wheel        (0)     4745 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/memory.pxd
--rw-r--r--   0 nmd        (502) wheel        (0)    20590 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/implementation.c
--rw-r--r--   0 nmd        (502) wheel        (0)      247 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/version.py
--rw-r--r--   0 nmd        (502) wheel        (0)       16 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/sage.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)     7941 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/signals.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      458 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/cypari.h
--rw-r--r--   0 nmd        (502) wheel        (0)     1086 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/memory.py
--rw-r--r--   0 nmd        (502) wheel        (0)    44877 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/pari_instance.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)     5761 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/handle_error.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)     4664 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/_pari.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      517 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/__init__.py
--rw-r--r--   0 nmd        (502) wheel        (0)     4082 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/test.py
--rw-r--r--   0 nmd        (502) wheel        (0)     1421 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/string_utils.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      223 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/Py_SET_SIZE.h
--rw-r--r--   0 nmd        (502) wheel        (0)     8123 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/stack.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)    20140 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/declinl.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)       79 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/long_win64py3.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)       77 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/long_win64py2.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)      541 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/long_hack.h
--rw-r--r--   0 nmd        (502) wheel        (0)     1473 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/_pari.pxd
--rw-r--r--   0 nmd        (502) wheel        (0)      181 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/memory.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)    10822 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/macros.h
--rw-r--r--   0 nmd        (502) wheel        (0)   203279 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/paridecl.pxd
--rw-r--r--   0 nmd        (502) wheel        (0)     3644 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/struct_signals.h
--rw-r--r--   0 nmd        (502) wheel        (0)       68 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/long_generic.pxi
--rw-r--r--   0 nmd        (502) wheel        (0)    44610 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/tests.py
--rw-r--r--   0 nmd        (502) wheel        (0)    18937 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/convert.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      524 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/py3tests.py
--rw-r--r--   0 nmd        (502) wheel        (0)      839 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/paripriv.pxd
--rw-r--r--   0 nmd        (502) wheel        (0)      555 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/py2tests.py
--rw-r--r--   0 nmd        (502) wheel        (0)   133526 2022-11-23 18:03:46.000000 cypari-2.5.0/cypari/gen.pyx
--rw-r--r--   0 nmd        (502) wheel        (0)      449 2022-11-23 18:03:46.000000 cypari-2.5.0/patches/paristio.patch
--rw-r--r--   0 nmd        (502) wheel        (0)      278 2022-11-23 18:03:46.000000 cypari-2.5.0/macOS/mac_paricfg.patch
--rw-r--r--   0 nmd        (502) wheel        (0)      605 2022-11-23 18:03:46.000000 cypari-2.5.0/macOS/rename_wheels.py
--rw-r--r--   0 nmd        (502) wheel        (0)      132 2022-11-23 18:03:46.000000 cypari-2.5.0/macOS/clear_cache.txt
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:17.005144 cypari-2.5.4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1131 2023-04-02 20:59:17.005370 cypari-2.5.4/PKG-INFO
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2569 2023-04-01 22:38:25.000000 cypari-2.5.4/README.rst
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6580 2023-04-01 22:38:25.000000 cypari-2.5.4/build_pari.sh
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.355687 cypari-2.5.4/cypari/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      223 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/Py_SET_SIZE.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      357 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/__init__.py
+-rw-r--r--   0 nmd      (444129884) staff       (20) 17865477 2023-04-02 18:32:14.748119 cypari-2.5.4/cypari/_pari.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      767 2023-04-02 18:32:14.748802 cypari-2.5.4/cypari/_pari.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      458 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/cypari.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20425 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/implementation.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      541 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/long_hack.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10849 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/macros.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1086 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/memory.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      594 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/parisage.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      555 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/py2tests.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      524 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/py3tests.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3644 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/struct_signals.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3924 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/test.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)    44457 2023-04-01 22:38:25.000000 cypari-2.5.4/cypari/tests.py
+-rw-r--r--   0 nmd      (444129884) staff       (20)      247 2023-04-02 18:34:23.321072 cypari-2.5.4/cypari/version.py
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.371635 cypari-2.5.4/gmp_src/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1200 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/.gdbinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3945 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/AUTHORS
+-rw-r--r--   0 nmd      (444129884) staff       (20)    35147 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/COPYING
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7639 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/COPYING.LESSERv3
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18092 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/COPYINGv2
+-rw-r--r--   0 nmd      (444129884) staff       (20)    35150 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/COPYINGv3
+-rw-r--r--   0 nmd      (444129884) staff       (20)  1182652 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/ChangeLog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2489 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/INSTALL
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9220 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/INSTALL.autoconf
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20170 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    57139 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    39315 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/NEWS
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4051 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)   124127 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/acinclude.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)   363087 2020-11-14 18:45:12.000000 cypari-2.5.4/gmp_src/aclocal.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3681 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/asl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1718 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/assert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/bootstrap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1846 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/compat.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     7333 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/compile
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    37968 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/config.guess
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20161 2020-11-14 18:45:15.000000 cypari-2.5.4/gmp_src/config.in
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     4973 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/config.sub
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    48921 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/configfsf.guess
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    34193 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/configfsf.sub
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)   939139 2020-11-14 18:45:15.000000 cypari-2.5.4/gmp_src/configure
+-rw-r--r--   0 nmd      (444129884) staff       (20)   140444 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/configure.ac
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.375287 cypari-2.5.4/gmp_src/cxx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18813 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/cxx/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1129 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/dummy.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2458 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/isfuns.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3580 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/ismpf.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1641 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/ismpq.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1710 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/ismpz.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2056 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/ismpznw.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2339 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/limits.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2088 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/osdoprnti.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3791 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/osfuns.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1986 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/osmpf.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/osmpq.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/cxx/osmpz.cc
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.377672 cypari-2.5.4/gmp_src/demos/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1610 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24221 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/demos/Makefile.in
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.380792 cypari-2.5.4/gmp_src/demos/calc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1570 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20273 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/demos/calc/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2110 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1103 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/calc-common.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      855 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/calc-config-h.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    69898 2020-11-14 18:45:31.000000 cypari-2.5.4/gmp_src/demos/calc/calc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4459 2020-11-14 18:45:31.000000 cypari-2.5.4/gmp_src/demos/calc/calc.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11479 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/calc.y
+-rw-r--r--   0 nmd      (444129884) staff       (20)    49571 2020-11-14 18:45:31.000000 cypari-2.5.4/gmp_src/demos/calc/calclex.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2858 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/calclex.l
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3872 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/calc/calcread.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.384858 cypari-2.5.4/gmp_src/demos/expr/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1919 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19841 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/demos/expr/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19269 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4434 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/expr-impl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    27124 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/expr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5203 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/expr.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4677 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4642 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprfa.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5104 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2747 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprqa.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1438 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8172 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprz.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2924 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/exprza.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5993 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/run-expr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12947 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/expr/t-expr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8370 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/factorize.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/isprime.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.386857 cypari-2.5.4/gmp_src/demos/perl/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.387858 cypari-2.5.4/gmp_src/demos/perl/GMP/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3085 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP/Mpf.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2652 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP/Mpq.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3350 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP/Mpz.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1375 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP/Rand.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    22070 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    72638 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/GMP.xs
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2435 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/INSTALL
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/Makefile.PL
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1599 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/sample.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)    59242 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/test.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1896 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/test2.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3254 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/perl/typemap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1641 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/pexpr-config-h.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    30797 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/pexpr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9905 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/primes.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33356 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/primes.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4041 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/demos/qcn.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.391590 cypari-2.5.4/gmp_src/doc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1235 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    27251 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/doc/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/configuration
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23559 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/fdl-1.3.texi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5931 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/doc/gmp.info
+-rw-r--r--   0 nmd      (444129884) staff       (20)   302874 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/doc/gmp.info-1
+-rw-r--r--   0 nmd      (444129884) staff       (20)   216314 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/doc/gmp.info-2
+-rw-r--r--   0 nmd      (444129884) staff       (20)   452111 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/gmp.texi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4945 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/isa_abi_headache
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     6047 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/doc/mdate-sh
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23522 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/projects.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)      101 2020-11-14 18:45:31.000000 cypari-2.5.4/gmp_src/doc/stamp-vti
+-rw-r--r--   0 nmd      (444129884) staff       (20)    51799 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/doc/tasks.html
+-rw-r--r--   0 nmd      (444129884) staff       (20)   323102 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/doc/texinfo.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      101 2020-11-14 18:45:31.000000 cypari-2.5.4/gmp_src/doc/version.texi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2114 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/errno.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7399 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/extract-dbl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6508 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-bases.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7519 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-fac.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3778 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-fib.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2845 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-jacobitab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-psqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6885 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gen-trialdivtab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    84000 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gmp-h.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)   181296 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gmp-impl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gmp.pc.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)   129113 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gmpxx.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/gmpxx.pc.in
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    14675 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/install-sh
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2600 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/invalid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    83238 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/longlong.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)   324089 2015-09-05 19:10:02.000000 cypari-2.5.4/gmp_src/ltmain.sh
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3693 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/memory.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.393188 cypari-2.5.4/gmp_src/mini-gmp/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21683 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/ChangeLog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3344 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)    89688 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/mini-gmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11548 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/mini-gmp.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11683 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/mini-mpq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4014 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/mini-mpq.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.403392 cypari-2.5.4/gmp_src/mini-gmp/tests/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1919 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/Makefile
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11502 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/hex-random.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2177 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/hex-random.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3148 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/mini-random.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1574 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/mini-random.h
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2947 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/run-tests
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1389 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1911 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-aorsmul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2596 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-bitops.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6609 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-cmp_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4465 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-comb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4777 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-cong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6344 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2018 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-div_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4850 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-double.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3833 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2970 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-import.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2939 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1677 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-lcm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2706 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-limbs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2638 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-logops.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2433 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-lucm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4503 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mpq_addsub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4535 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mpq_double.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4172 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mpq_muldiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3463 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mpq_muldiv_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6981 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mpq_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2656 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1471 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-powm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3688 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-pprime_p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17526 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-reuse.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2243 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-root.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2367 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-scan.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4496 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-signed.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3998 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-sqrt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8652 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1717 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/t-sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4557 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/testutils.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1290 2020-11-14 18:45:35.000000 cypari-2.5.4/gmp_src/mini-gmp/tests/testutils.h
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     6872 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/missing
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1099 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_bpl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1595 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_clz_tab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3049 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_dv_tab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1499 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_get_fns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2171 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_minv_tab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1617 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mp_set_fns.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.423262 cypari-2.5.4/gmp_src/mpf/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1908 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19856 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/mpf/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1509 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/abs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3717 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/add_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/ceilfloor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1201 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/clear.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1308 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/clears.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2676 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1688 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/cmp_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2909 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/cmp_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/cmp_z.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3849 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4705 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/div_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2532 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/div_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1603 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/dump.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3587 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/eq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1800 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_s.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1157 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_sint.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1161 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_slong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1164 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_sshort.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1816 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_u.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1138 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_uint.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1148 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_ulong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1145 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/fits_ushort.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1371 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1567 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_d_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1198 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_dfl_prec.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1185 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_prc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2437 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8558 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3175 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/get_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1297 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/init.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1337 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/init2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1292 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/inits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2318 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1499 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/int_p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1646 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/iset.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/iset_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1617 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/iset_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1369 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/iset_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1539 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/iset_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2741 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4419 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/mul_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6120 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/mul_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1575 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/neg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2908 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/out_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2271 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/pow_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1741 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/random2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1838 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/reldiff.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1519 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1589 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_dfl_prec.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2107 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_prc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1322 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_prc_raw.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3647 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1467 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9239 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1366 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1443 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/set_z.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1200 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/size.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3660 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/sqrt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3391 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/sqrt_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8919 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1352 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/sub_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1421 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/swap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1845 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/trunc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3350 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/ui_div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6143 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/ui_sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpf/urandomb.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.426321 cypari-2.5.4/gmp_src/mpn/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4727 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/Makeasm.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1960 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23976 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/mpn/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1702 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/README
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.436452 cypari-2.5.4/gmp_src/mpn/alpha/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7922 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5047 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2791 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3112 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/alpha-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3706 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3710 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/aorslsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5775 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1653 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/cntlz.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4276 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2328 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2249 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2983 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/default.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2921 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/dive_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4527 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/divrem_2.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.437061 cypari-2.5.4/gmp_src/mpn/alpha/ev5/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6855 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev5/diveby3.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8724 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev5/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.439903 cypari-2.5.4/gmp_src/mpn/alpha/ev6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8021 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3783 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10272 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9843 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6881 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13616 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.444900 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1922 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8117 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3491 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3978 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/addmul_3.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4872 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/addmul_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5108 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2873 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7443 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8117 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/nails/submul_1.asm
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     7664 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/slot.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8112 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev6/sub_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.446617 cypari-2.5.4/gmp_src/mpn/alpha/ev67/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2448 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev67/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2888 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev67/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2577 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/ev67/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3169 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2381 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3555 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3581 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5481 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2966 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3411 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2936 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2570 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/sqr_diag_addlsh1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5275 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2802 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1399 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/umul.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3145 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/alpha/unicos.m4
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.459355 cypari-2.5.4/gmp_src/mpn/arm/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1228 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2806 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4087 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3011 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2546 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/arm-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2487 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2975 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1918 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2109 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5227 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3854 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3672 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2124 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2223 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2698 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2116 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.462323 cypari-2.5.4/gmp_src/mpn/arm/neon/
+-rw-r--r--   0 nmd      (444129884) staff       (20)       98 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5272 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6726 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/lorrshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5801 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4468 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3261 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/neon/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2807 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2075 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2789 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3040 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/udiv.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.463865 cypari-2.5.4/gmp_src/mpn/arm/v5/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1982 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v5/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2782 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v5/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3433 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v5/mod_1_2.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.469560 cypari-2.5.4/gmp_src/mpn/arm/v6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2468 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2652 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4146 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/addmul_3.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3078 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8539 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2158 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2453 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2892 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3556 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11115 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2694 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.471057 cypari-2.5.4/gmp_src/mpn/arm/v6t2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4560 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6t2/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1731 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6t2/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2437 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v6t2/gcd_22.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.327102 cypari-2.5.4/gmp_src/mpn/arm/v7a/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.475542 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3274 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3685 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1368 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3531 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3597 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10074 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5583 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2464 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.478160 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1517 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/aorsorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1517 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/aorsorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3522 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/aorsorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2342 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2658 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2261 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4203 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/neon/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3432 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora15/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.480507 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1216 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11374 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2666 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1207 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1216 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora17/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.481010 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora5/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9656 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora5/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.481623 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9413 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora7/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.482702 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora8/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3404 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora8/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9814 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora8/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.483862 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora9/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1368 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora9/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9893 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm/v7a/cora9/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.497948 cypari-2.5.4/gmp_src/mpn/arm64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2911 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3368 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1464 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/aorsorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1464 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/aorsorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3351 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/aorsorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1713 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/arm64-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2425 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2766 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2915 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2107 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2236 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1984 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.498941 cypari-2.5.4/gmp_src/mpn/arm64/cora53/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cora53/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11777 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cora53/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.499446 cypari-2.5.4/gmp_src/mpn/arm64/cora57/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8394 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cora57/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.499973 cypari-2.5.4/gmp_src/mpn/arm64/cora72/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11804 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cora72/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.500445 cypari-2.5.4/gmp_src/mpn/arm64/cora73/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10680 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/cora73/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1746 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/darwin.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1896 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2559 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8766 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5297 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2149 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3492 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2716 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2752 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4416 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3746 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3176 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2996 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2419 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/sqr_diag_addlsh1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.500921 cypari-2.5.4/gmp_src/mpn/arm64/xgene1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8130 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/arm64/xgene1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    55792 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/asm-defs.m4
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     3014 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cpp-ccas
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.504811 cypari-2.5.4/gmp_src/mpn/cray/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3879 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2514 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/add_n.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.506938 cypari-2.5.4/gmp_src/mpn/cray/cfp/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1399 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/cfp/addmul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1346 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/cfp/mul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8721 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/cfp/mulwwc90.s
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8704 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/cfp/mulwwj90.s
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1399 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/cfp/submul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2792 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1290 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/hamdist.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.510259 cypari-2.5.4/gmp_src/mpn/cray/ieee/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3224 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/addmul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2796 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4230 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/invert_limb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2959 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/mul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2600 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/mul_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2488 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/sqr_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3248 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/ieee/submul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1626 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/lshift.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2253 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/mulww.f
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1262 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/popcount.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1631 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/rshift.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2621 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/cray/sub_n.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.583721 cypari-2.5.4/gmp_src/mpn/generic/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1078 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2744 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_err1_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3251 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_err2_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3693 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_err3_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2001 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5552 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/add_n_sub_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/addmul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1801 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bdiv_dbm1c.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2175 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2760 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bdiv_q_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2440 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2997 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/binvert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4689 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/broot.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4058 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/brootinv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bsqrt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2567 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/bsqrtinv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1135 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1973 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/cnd_add_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1979 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/cnd_sub_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1428 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/cnd_swap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/com.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1780 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/comb_tables.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/compute_powtab.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1151 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/copyd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1170 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/copyi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3803 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dcpi1_bdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dcpi1_bdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dcpi1_div_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6317 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dcpi1_div_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6807 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dcpi1_divappr_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10333 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3166 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7731 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_1n_pi1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5418 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_1n_pi2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6166 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_1u_pi2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9270 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2176 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_2n_pi1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2244 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/div_qr_2u_pi1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dive_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5423 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/diveby3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8034 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/divexact.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5425 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/divis.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2647 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/divrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7158 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/divrem_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3296 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/divrem_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2393 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/dump.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5237 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/fib2_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6414 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/fib2m.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6635 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2914 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcd_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2028 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcd_11.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3209 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcd_22.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4742 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcd_subdiv_step.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13124 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcdext.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5513 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcdext_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gcdext_lehmer.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11300 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13992 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/get_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1172 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5087 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21410 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7445 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd2_jacobi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6574 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd_appr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6725 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd_jacobi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7440 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd_matrix.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6246 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd_reduce.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3722 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/hgcd_step.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3005 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10632 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/invertappr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6932 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/jacbase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7740 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/jacobi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7212 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/jacobi_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1816 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/logops_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2050 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/lshift.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2080 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/lshiftc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8216 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/matrix22_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1988 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/matrix22_mul1_inverse_vector.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7535 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9069 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_1_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3701 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_1_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4199 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_1_3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4470 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_1_4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3853 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mod_34lsub1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7111 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mode1o.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7690 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mu_bdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8193 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mu_bdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5197 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mu_div_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mu_div_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9963 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mu_divappr_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15189 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2179 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mul_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    28888 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mul_fft.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2812 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mul_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2105 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mullo_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mullo_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6010 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mulmid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2362 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mulmid_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1814 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mulmid_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9983 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/mulmod_bnm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1078 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/neg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/nussbaumer_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/perfpow.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8418 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/perfsqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3421 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/popham.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3084 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/pow_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4701 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/powlo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17267 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/powm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4098 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/pre_divrem_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1756 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/pre_mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1446 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/random.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3262 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/random2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1667 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/redc_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3045 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/redc_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2235 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/redc_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4867 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/remove.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18444 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/rootrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2017 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/rshift.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2518 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_bdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2364 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_bdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2254 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_bdiv_r.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6371 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_div_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2697 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_div_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4189 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sbpi1_divappr_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1786 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/scan0.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1740 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/scan1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1620 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_aors_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3623 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4311 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1320 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5372 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_pi1_div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11759 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_powm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1645 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sec_tabselect.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7327 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/set_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1579 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sizeinbase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2831 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8557 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqr_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7914 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqrlo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5273 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqrlo_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8498 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqrmod_bnm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18364 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sqrtrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5797 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/strongfibo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1080 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1085 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2750 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub_err1_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3257 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub_err2_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3699 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub_err3_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2012 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/sub_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3326 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/submul_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10981 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/tdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5673 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom22_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3811 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom2_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8624 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom32_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8292 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom33_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5842 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom3_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6031 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom42_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7102 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom42_mulmid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6376 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom43_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7945 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom44_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5188 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom4_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6673 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom52_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom53_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom54_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8611 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom62_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6286 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom63_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5826 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom6_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8490 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom6h_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom8_sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10218 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom8h_mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2366 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_couple_handling.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_dgr3_pm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2753 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_dgr3_pm2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2569 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_pm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3659 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_pm2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3858 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_pm2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3025 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_eval_pm2rexp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11817 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_12pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18427 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_16pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6784 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_5pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7026 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_6pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8237 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_7pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6620 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/toom_interpolate_8pts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3984 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/trialdiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3299 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/udiv_w_sdiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1139 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/zero.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1118 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/generic/zero_p.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.599925 cypari-2.5.4/gmp_src/mpn/ia64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9372 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8349 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/add_n_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17852 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20943 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1587 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/aorsorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1587 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/aorsorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9925 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/aorsorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9313 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6598 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3568 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3404 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6782 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10809 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6524 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/divrem_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2615 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10076 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4167 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/ia64-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3055 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7174 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7110 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/lorrshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8416 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5115 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11349 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11545 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15213 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11463 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3389 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4738 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/sqr_diag_addlsh1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12629 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/ia64/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.600353 cypari-2.5.4/gmp_src/mpn/lisp/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13748 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/lisp/gmpasm-mode.el
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2665 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m4-ccas
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.603692 cypari-2.5.4/gmp_src/mpn/m68k/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4795 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2427 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2714 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4074 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6069 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/m68k-defs.m4
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.605589 cypari-2.5.4/gmp_src/mpn/m68k/mc68020/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2508 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/mc68020/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2246 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/mc68020/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1471 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/mc68020/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1428 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/mc68020/umul.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2696 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m68k/t-m68k-defs.pl
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.607535 cypari-2.5.4/gmp_src/mpn/m88k/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1577 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2928 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/add_n.s
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.609493 cypari-2.5.4/gmp_src/mpn/m88k/mc88110/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/mc88110/add_n.S
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1794 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/mc88110/addmul_1.s
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1823 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/mc88110/mul_1.s
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6740 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/mc88110/sub_n.S
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4316 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/mul_1.s
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2998 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/m88k/sub_n.s
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.610016 cypari-2.5.4/gmp_src/mpn/minithres/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4353 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/minithres/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.615290 cypari-2.5.4/gmp_src/mpn/mips32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2520 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2508 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2580 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2238 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2042 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/mips-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2017 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/mips.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2327 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2130 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2531 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2515 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1343 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips32/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.618652 cypari-2.5.4/gmp_src/mpn/mips64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2019 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2762 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2580 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.621195 cypari-2.5.4/gmp_src/mpn/mips64/hilo/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/hilo/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/hilo/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1722 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/hilo/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2536 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/hilo/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1338 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/hilo/umul.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2264 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2152 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2778 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/mips64/sub_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.625134 cypari-2.5.4/gmp_src/mpn/pa32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3526 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1926 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1731 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.628781 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2852 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2632 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3091 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.631472 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2237 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4729 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2412 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2329 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2273 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4961 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/pa7100/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1789 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3116 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2742 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1473 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa1_1/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.633531 cypari-2.5.4/gmp_src/mpn/pa32/hppa2_0/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2558 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa2_0/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7586 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa2_0/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2662 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa2_0/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2570 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/hppa2_0/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1972 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/pa-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1897 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1962 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6896 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa32/udiv.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.639600 cypari-2.5.4/gmp_src/mpn/pa64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3125 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18604 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3430 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5341 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12482 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2878 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17439 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2793 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18778 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3208 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2703 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/pa64/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.644813 cypari-2.5.4/gmp_src/mpn/power/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2823 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3237 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2587 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2016 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3030 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2035 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1245 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/sdiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2894 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1299 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/power/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.657723 cypari-2.5.4/gmp_src/mpn/powerpc32/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.659784 cypari-2.5.4/gmp_src/mpn/powerpc32/750/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1878 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/750/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9105 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/750/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2897 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/750/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2827 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/750/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5132 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2722 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/addlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3459 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1908 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/aix.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3620 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2785 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2093 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/darwin.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2555 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/diveby3.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/divrem_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2124 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/eabi.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2375 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/elf.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10466 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3596 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3643 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3314 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4154 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2393 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.660332 cypari-2.5.4/gmp_src/mpn/powerpc32/p3/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6940 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p3/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.660863 cypari-2.5.4/gmp_src/mpn/powerpc32/p3-p7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4434 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p3-p7/aors_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.661360 cypari-2.5.4/gmp_src/mpn/powerpc32/p4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9831 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p4/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.661892 cypari-2.5.4/gmp_src/mpn/powerpc32/p5/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6815 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p5/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.662389 cypari-2.5.4/gmp_src/mpn/powerpc32/p6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7401 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p6/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.662900 cypari-2.5.4/gmp_src/mpn/powerpc32/p7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7341 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/p7/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3847 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/powerpc-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3484 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3047 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1962 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/sqr_diag_addlsh1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2731 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3240 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1427 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.665354 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4848 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4749 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8231 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9395 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1235 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc32/vmx/popcount.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.671778 cypari-2.5.4/gmp_src/mpn/powerpc64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5844 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2214 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/aix.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2811 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2183 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2021 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2837 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/darwin.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2534 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/elf.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3890 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4322 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4383 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/lshiftc.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.674941 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2715 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2119 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1979 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.675498 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/p4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8153 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/p4/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2630 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2722 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2196 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode32/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.686840 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4582 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4871 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1504 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/aorsorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1504 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/aorsorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5014 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/aorsorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2834 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3076 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4576 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2829 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5473 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3735 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/divrem_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2060 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3006 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2769 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5312 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2893 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2571 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3674 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12664 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/mul_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.687364 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p3/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8255 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p3/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.687891 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10134 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p4/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.688427 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p5/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10708 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p5/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.690039 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4389 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p6/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7061 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p6/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11216 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p6/mul_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.694197 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3097 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/aormul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2874 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1507 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/aorsorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1507 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/aorsorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3182 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/aorsorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1861 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3379 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7682 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p7/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.695209 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p8/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7456 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p8/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1666 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p8/invert_limb.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.700266 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2494 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/add_n_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2991 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4630 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3912 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1762 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3271 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12492 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2784 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4324 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11403 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/p9/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3729 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16328 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/mode64/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.701410 cypari-2.5.4/gmp_src/mpn/powerpc64/p6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3078 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p6/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3168 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p6/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3008 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p6/rshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.702913 cypari-2.5.4/gmp_src/mpn/powerpc64/p7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2740 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p7/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2791 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p7/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2345 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p7/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2072 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/p7/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3126 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1482 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.703292 cypari-2.5.4/gmp_src/mpn/powerpc64/vmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5886 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/powerpc64/vmx/popcount.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.332604 cypari-2.5.4/gmp_src/mpn/riscv/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.704494 cypari-2.5.4/gmp_src/mpn/riscv/64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2307 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/riscv/64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2037 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/riscv/64/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1633 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/riscv/64/mul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.709927 cypari-2.5.4/gmp_src/mpn/s390_32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      899 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2507 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2940 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1812 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.714526 cypari-2.5.4/gmp_src/mpn/s390_32/esame/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1828 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3111 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3284 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1688 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7950 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1756 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2787 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4312 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1760 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/esame/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5940 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5506 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2764 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2943 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2603 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2514 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_32/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.724065 cypari-2.5.4/gmp_src/mpn/s390_64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2772 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1813 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3314 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3096 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1664 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3043 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1814 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8159 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2143 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5577 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4144 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4016 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2345 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1736 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2824 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3808 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4409 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3219 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1743 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.724595 cypari-2.5.4/gmp_src/mpn/s390_64/z10/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11305 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/s390_64/z10/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.725674 cypari-2.5.4/gmp_src/mpn/sh/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1653 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sh/add_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.726983 cypari-2.5.4/gmp_src/mpn/sh/sh2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1789 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sh/sh2/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1696 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sh/sh2/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1796 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sh/sh2/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1665 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sh/sub_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.733508 cypari-2.5.4/gmp_src/mpn/sparc32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2586 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5753 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3443 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2462 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2400 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3353 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2284 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2924 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/sparc-defs.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7779 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3450 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3337 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3992 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/udiv_nfp.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.737048 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1773 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2132 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6741 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1971 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1513 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1773 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2169 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/ultrasparct1/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2105 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.740059 cypari-2.5.4/gmp_src/mpn/sparc32/v8/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2866 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2582 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2610 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1780 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.741104 cypari-2.5.4/gmp_src/mpn/sparc32/v8/supersparc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2639 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/supersparc/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2661 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/supersparc/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2661 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1317 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v8/umul.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.746657 cypari-2.5.4/gmp_src/mpn/sparc32/v9/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2838 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7411 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6867 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9130 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2850 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7827 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1646 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc32/v9/udiv.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.754850 cypari-2.5.4/gmp_src/mpn/sparc64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5284 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2129 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4349 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/dive_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/divrem_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2411 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5902 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2985 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3075 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6789 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5856 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/mod_1_4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/mode1o.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3009 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3405 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9250 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/sparc64.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.758762 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4495 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17309 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13564 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3227 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16253 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7420 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/sqr_diagonal.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4530 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1858 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc1234/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.759307 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc34/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10781 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparc34/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.767381 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1751 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/addlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/addlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1746 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/addlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2119 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6564 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2033 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/rsblsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/rsblsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1746 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/rsblshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1751 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/sublsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1746 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/sublshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2119 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct1/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.778198 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2598 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3847 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5496 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/aormul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4919 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/aormul_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3520 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/aorslsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3261 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2973 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3704 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2848 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1943 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2279 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1987 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/missing.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2324 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/missing.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4857 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2649 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2063 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3766 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1794 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2207 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/sqr_diag_addlsh1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2952 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3640 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct3/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.778730 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct45/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7608 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/sparc64/ultrasparct45/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.779686 cypari-2.5.4/gmp_src/mpn/thumb/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1770 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/thumb/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1766 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/thumb/sub_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.783652 cypari-2.5.4/gmp_src/mpn/vax/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1752 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2593 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1559 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/elf.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2194 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1547 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2502 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1516 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2600 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/vax/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.797036 cypari-2.5.4/gmp_src/mpn/x86/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19080 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5028 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3457 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/aorsmul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.806176 cypari-2.5.4/gmp_src/mpn/x86/atom/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1798 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1817 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3638 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/aorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3805 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5380 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/aorslshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1342 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2437 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/cnd_add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2636 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/cnd_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1261 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10150 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3232 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/lshiftc.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.807738 cypari-2.5.4/gmp_src/mpn/x86/atom/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1253 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/mmx/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1253 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/mmx/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1244 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/mmx/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1260 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3092 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/rshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.812343 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3713 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1241 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1244 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1245 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2771 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9373 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11859 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sse2/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1970 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/atom/sublsh2_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.812893 cypari-2.5.4/gmp_src/mpn/x86/bd1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10024 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bd1/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.813419 cypari-2.5.4/gmp_src/mpn/x86/bd2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10138 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bd2/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.813917 cypari-2.5.4/gmp_src/mpn/x86/bd4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10846 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bd4/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2617 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4263 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bdiv_q_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.814459 cypari-2.5.4/gmp_src/mpn/x86/bt1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10347 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bt1/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.814946 cypari-2.5.4/gmp_src/mpn/x86/bt2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10086 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/bt2/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2735 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2061 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2716 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.815451 cypari-2.5.4/gmp_src/mpn/x86/core2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9930 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/core2/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.815960 cypari-2.5.4/gmp_src/mpn/x86/coreibwl/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10271 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/coreibwl/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.816471 cypari-2.5.4/gmp_src/mpn/x86/coreihwl/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10213 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/coreihwl/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.816961 cypari-2.5.4/gmp_src/mpn/x86/coreinhm/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10718 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/coreinhm/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.817448 cypari-2.5.4/gmp_src/mpn/x86/coreisbr/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10225 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/coreisbr/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2568 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/darwin.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3767 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5449 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4132 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/divrem_2.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.824064 cypari-2.5.4/gmp_src/mpn/x86/fat/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1065 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/com.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15355 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/fat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6408 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/fat_entry.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2798 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/lshiftc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1063 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1139 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mod_1_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1141 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mod_1_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1141 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mod_1_4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1068 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mode1o.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1075 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/mullo_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/redc_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/fat/redc_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2977 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/gcd_11.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.824578 cypari-2.5.4/gmp_src/mpn/x86/geode/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6108 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/geode/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1354 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.825048 cypari-2.5.4/gmp_src/mpn/x86/goldmont/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10483 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/goldmont/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.825484 cypari-2.5.4/gmp_src/mpn/x86/i486/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2352 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/i486/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.825942 cypari-2.5.4/gmp_src/mpn/x86/k10/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10390 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k10/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.831773 cypari-2.5.4/gmp_src/mpn/x86/k6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8639 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6385 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9827 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/aorsmul_1.asm
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     5944 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/cross.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4504 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7537 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.833437 cypari-2.5.4/gmp_src/mpn/x86/k6/k62mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3070 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/k62mmx/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5647 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/k62mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5687 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/k62mmx/rshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.836481 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2318 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5466 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2701 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4481 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2717 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mmx/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3928 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4030 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5161 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12512 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3379 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/pre_mod_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14082 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k6/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.844828 cypari-2.5.4/gmp_src/mpn/x86/k7/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5871 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4748 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/addlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5817 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3474 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5242 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4406 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2508 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13099 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/invert_limb.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.848367 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3225 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3027 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3713 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19083 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9633 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9601 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mmx/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4285 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4889 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3806 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4051 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4375 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11828 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12277 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4028 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k7/sublsh1_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.848887 cypari-2.5.4/gmp_src/mpn/x86/k8/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/k8/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2494 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/lshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.849393 cypari-2.5.4/gmp_src/mpn/x86/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3214 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/mmx/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3442 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2981 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4783 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/mul_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.849892 cypari-2.5.4/gmp_src/mpn/x86/nano/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7205 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/nano/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.856631 cypari-2.5.4/gmp_src/mpn/x86/p6/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3445 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3154 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6688 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5612 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4321 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5113 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2419 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8944 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3663 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/lshsub_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.859554 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14996 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10191 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1389 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mmx/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4270 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3736 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11664 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/mul_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.860116 cypari-2.5.4/gmp_src/mpn/x86/p6/p3mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1439 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/p3mmx/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12287 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.864750 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9240 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1242 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1243 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1251 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1251 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1239 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/p6/sse2/submul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.874502 cypari-2.5.4/gmp_src/mpn/x86/pentium/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4120 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3246 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5255 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3778 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3075 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3957 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5149 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2599 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3459 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4030 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4940 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/lshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.876922 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7141 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1425 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8702 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8228 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9481 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mmx/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5513 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3159 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3303 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3267 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3068 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4915 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8986 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.878860 cypari-2.5.4/gmp_src/mpn/x86/pentium4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4101 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1973 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2282 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.880433 cypari-2.5.4/gmp_src/mpn/x86/pentium4/mmx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/mmx/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4389 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/mmx/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1337 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/mmx/rshift.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.890884 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2368 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2672 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/addlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3030 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4862 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2228 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/cnd_add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2474 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/cnd_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4601 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13140 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10061 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3846 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5311 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3554 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3563 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18835 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7156 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3251 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/rsh1add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18889 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2598 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5324 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/pentium4/sse2/submul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2633 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/sec_tabselect.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.891344 cypari-2.5.4/gmp_src/mpn/x86/silvermont/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10694 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/silvermont/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.891879 cypari-2.5.4/gmp_src/mpn/x86/skylake/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9971 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/skylake/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7073 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/sqr_basecase.asm
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2113 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/t-zdisp.sh
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     4025 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/t-zdisp2.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1611 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/udiv.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1518 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/umul.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    30392 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/x86-defs.m4
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.892383 cypari-2.5.4/gmp_src/mpn/x86/zn1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10522 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/zn1/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.892912 cypari-2.5.4/gmp_src/mpn/x86/zn2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10852 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86/zn2/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.918397 cypari-2.5.4/gmp_src/mpn/x86_64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2697 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3203 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/addaddmul_1msb0.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3831 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3613 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3870 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4218 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aors_err1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3348 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aors_err2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3080 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aors_err3_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3690 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4146 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/aorsmul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.929031 cypari-2.5.4/gmp_src/mpn/x86_64/atom/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3437 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5102 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4042 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2860 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3877 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1272 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/cnd_add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1272 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/cnd_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1301 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10522 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2590 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2657 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3180 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3631 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1238 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10466 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5538 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2526 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4847 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/atom/sublsh1_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.937743 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      478 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4224 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1328 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4137 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1282 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13359 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5084 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4107 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3685 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7587 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4992 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd1/sublsh1_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.939367 cypari-2.5.4/gmp_src/mpn/x86_64/bd2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2254 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd2/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2926 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd2/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13152 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd2/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.941338 cypari-2.5.4/gmp_src/mpn/x86_64/bd4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd4/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2262 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd4/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd4/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13319 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bd4/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bdiv_dbm1c.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4479 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bdiv_q_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.946760 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3478 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4297 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2101 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2143 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2600 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1293 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4833 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8739 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8902 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9865 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt1/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.949828 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1252 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1297 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11659 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/bt2/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4309 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/cnd_aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2128 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2120 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2104 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.964239 cypari-2.5.4/gmp_src/mpn/x86_64/core2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4176 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aors_err1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3234 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3964 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1260 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5007 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2233 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2766 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10626 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4658 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5425 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2943 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3182 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16719 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7748 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4334 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8230 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3767 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2884 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17381 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1472 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1472 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/sublsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3322 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/core2/sublshC_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.967180 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/addmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12016 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7099 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8284 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17160 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreibwl/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.973204 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5072 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4152 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2838 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12539 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3421 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3578 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7507 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7368 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9057 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9556 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreihwl/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.976817 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4825 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4033 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11641 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4301 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4892 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10069 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreinhm/sec_tabselect.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.988252 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4433 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1778 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1857 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3880 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aorrlshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4933 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4328 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4444 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3669 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/cnd_add_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4309 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/cnd_sub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1278 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11819 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1305 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3977 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7403 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6768 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10034 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4083 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8965 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/coreisbr/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/darwin.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4500 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/div_qr_1n_pi1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3264 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/div_qr_2n_pi1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4074 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/div_qr_2u_pi1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3506 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6455 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/divrem_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3926 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/divrem_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2348 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/dos64.m4
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.989154 cypari-2.5.4/gmp_src/mpn/x86_64/fastavx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3795 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastavx/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3673 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastavx/copyi.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.994665 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      603 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6861 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/com-palignr.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4326 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5762 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/copyd-palignr.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4114 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6786 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/copyi-palignr.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4577 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/lshift-movdqu2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4428 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4524 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/lshiftc-movdqu2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4716 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4561 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/rshift-movdqu2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4826 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fastsse/sec_tabselect.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.999638 cypari-2.5.4/gmp_src/mpn/x86_64/fat/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1234 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/addmul_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13693 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/fat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5828 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/fat_entry.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2807 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1063 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1071 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/mul_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1075 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/mullo_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/redc_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1059 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/redc_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1071 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/fat/sqr_basecase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2553 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3423 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10572 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.002507 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1320 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1333 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13191 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1299 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1285 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/goldmont/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2953 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/invert_limb.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1539 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/invert_limb_table.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.006942 cypari-2.5.4/gmp_src/mpn/x86_64/k10/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2825 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12033 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2533 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1294 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k10/sec_tabselect.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.010596 cypari-2.5.4/gmp_src/mpn/x86_64/k8/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4045 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4611 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3971 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/bdiv_q_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4606 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/div_qr_1n_pi1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11332 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8707 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8007 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9575 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/mulmid_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10545 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14488 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/k8/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5309 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/logops_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3881 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3923 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/lshsub_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1414 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/missing-call.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2224 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/missing-inline.m4
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3177 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/missing.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5043 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mod_1_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4576 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mod_1_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5132 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mod_1_4.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4390 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3974 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mode1o.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4157 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3996 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mul_2.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.341439 cypari-2.5.4/gmp_src/mpn/x86_64/mulx/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.010901 cypari-2.5.4/gmp_src/mpn/x86_64/mulx/adx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3519 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/mulx/adx/addmul_1.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.012739 cypari-2.5.4/gmp_src/mpn/x86_64/nano/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1299 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1299 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3830 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/dive_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11861 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1238 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/nano/popcount.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.019722 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1290 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/addmul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4172 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/aorslsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/aorslsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4146 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/aorslshC_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1321 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12645 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1285 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3369 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/mod_34lsub1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1292 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1281 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/mul_2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1310 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1284 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/redc_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6608 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3580 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/sec_tabselect.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1304 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/pentium4/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3671 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/popham.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4120 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/rsh1aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3834 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3666 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/sec_tabselect.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.024893 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1564 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1564 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/aorrlsh2_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1335 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/aors_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1351 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12503 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1266 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1300 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1303 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1296 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1305 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1311 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1269 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1300 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1305 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/silvermont/sqr_basecase.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.025333 cypari-2.5.4/gmp_src/mpn/x86_64/skylake/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12439 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/skylake/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2487 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/sqr_diag_addlsh1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3500 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/sublsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11222 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/x86_64-defs.m4
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.034921 cypari-2.5.4/gmp_src/mpn/x86_64/zen/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1359 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/aorrlsh1_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4589 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/aorrlsh_n.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4113 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/aorsmul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1274 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/com.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/copyd.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1280 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/copyi.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/gcd_11.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1302 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/gcd_22.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14138 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/gmp-mparam.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1285 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/hamdist.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/lshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1294 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/lshiftc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3850 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/mul_1.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11435 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/mul_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/mullo_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/popcount.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/rshift.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11367 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/sbpi1_bdiv_r.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11493 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/sqr_basecase.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1298 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen/sublsh1_n.asm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.035337 cypari-2.5.4/gmp_src/mpn/x86_64/zen2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14407 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpn/x86_64/zen2/gmp-mparam.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.051457 cypari-2.5.4/gmp_src/mpq/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1539 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19078 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/mpq/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1544 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/abs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3348 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/aors.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1683 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/canonicalize.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/clear.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1421 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/clears.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1817 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3043 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/cmp_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3289 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1961 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/equal.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5852 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1297 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/get_den.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/get_num.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2403 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/get_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1366 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/init.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1292 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/inits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1689 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2018 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/inv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2800 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/md_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2872 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1532 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/neg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1452 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/out_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1531 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4105 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1352 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_den.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2960 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_f.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1345 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_num.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1750 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1905 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1710 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1429 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/set_z.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1401 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpq/swap.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.118783 cypari-2.5.4/gmp_src/mpz/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3103 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/2fac_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2983 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    22050 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/mpz/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1378 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/abs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1060 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1102 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/add_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6885 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/and.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3032 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/aors.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3050 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/aors_ui.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3995 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/aorsmul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7246 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/aorsmul_i.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1484 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/array_init.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11371 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/bin_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19841 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/bin_uiui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1569 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2604 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_q_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2028 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2982 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_qr_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1868 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_r.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2660 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_r_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2499 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cdiv_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2959 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cfdiv_q_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3805 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cfdiv_r_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1242 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/clear.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/clears.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2959 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/clrbit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1571 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3708 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmp_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1876 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1808 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmp_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1478 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmpabs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3450 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmpabs_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1768 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cmpabs_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2395 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/com.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3137 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/combit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5120 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3515 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cong_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2880 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/cong_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1927 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/dive_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3640 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/divegcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2141 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/divexact.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1303 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/divis.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1690 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/divis_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2209 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/divis_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1485 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/dump.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5163 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/export.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2851 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fac_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1563 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2488 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_q_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2022 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2863 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_qr_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1861 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_r.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2543 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_r_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2384 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fdiv_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1699 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fib2_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4520 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fib_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1585 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_s.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1175 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_sint.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1179 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_slong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1182 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_sshort.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1123 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_uint.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1126 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_ulong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1129 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/fits_ushort.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4029 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2203 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/gcd_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3422 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/gcdext.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1276 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1484 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/get_d_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1574 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/get_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3314 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/get_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1139 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/get_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1125 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/getlimbn.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3718 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/hamdist.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4800 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/import.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1270 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/init.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1584 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/init2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1409 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/inits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4863 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/inp_raw.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4189 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1918 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4534 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/ior.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1448 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/iset.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1327 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/iset_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1620 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/iset_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1620 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/iset_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/iset_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5914 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/jacobi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3637 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/kronsz.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3411 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/kronuz.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2538 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/kronzs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2287 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/kronzu.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2030 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/lcm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1987 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/lcm_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1221 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/limbs_finish.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1189 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/limbs_modify.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1137 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/limbs_read.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1178 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/limbs_write.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4372 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/lucmod.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2484 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/lucnum2_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5583 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/lucnum_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3446 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mfac_uiui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6141 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/millerrabin.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1817 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mod.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3696 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1824 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mul_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2876 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mul_i.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1153 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mul_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1153 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/mul_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16635 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/n_pow_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1428 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/neg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3301 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/nextprime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11845 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/oddfac_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4187 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/out_raw.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/out_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1222 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/perfpow.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1182 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/perfsqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1196 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/popcount.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1490 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/pow_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6158 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/powm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2319 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/powm_sec.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6961 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/powm_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4432 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/pprime_p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4265 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/primorial_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3061 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/prodlimbs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1248 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/random.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1477 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/random2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2026 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/realloc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1859 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/realloc2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3588 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/remove.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1281 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/roinit_n.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2286 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/root.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2454 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/rootrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3039 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/rrandomb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3831 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/scan0.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3699 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/scan1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1344 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2824 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1777 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_f.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1139 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1522 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3633 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1505 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/set_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2752 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/setbit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1151 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/size.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1383 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/sizeinbase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2014 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/sqrt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2389 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/sqrtrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5235 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/stronglucas.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1065 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1107 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/sub_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/swap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2124 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1663 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_q_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2270 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_q_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2699 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_qr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_qr_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2388 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_r.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2096 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_r_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2458 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_r_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2173 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tdiv_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2565 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/tstbit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1688 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/ui_pow_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2180 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/ui_sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1487 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/urandomb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2686 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/urandomm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3886 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/mpz/xor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4257 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/nextprime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11871 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/primesieve.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.126476 cypari-2.5.4/gmp_src/printf/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1505 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19052 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/printf/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1279 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/asprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1957 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/asprntffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17660 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/doprnt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10979 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/doprntf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3943 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/doprnti.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1285 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/fprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1605 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/obprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2067 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/obprntffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1531 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/obvprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1277 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/printf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2252 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/printffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10199 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/repl-vsnprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1467 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/snprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3953 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/snprntffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1457 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/sprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2558 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/sprintffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3735 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/vasprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1211 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/vfprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1203 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/vprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1394 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/vsnprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1405 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/printf/vsprintf.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.131256 cypari-2.5.4/gmp_src/rand/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1380 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18793 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/rand/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1481 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/rand.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randbui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1206 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randclr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1182 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randdef.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1233 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randiset.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2958 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randlc2s.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9435 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randlc2x.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15715 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randmt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1662 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randmt.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4482 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randmts.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2567 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randmui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1387 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/rands.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1244 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randsd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1317 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/rand/randsdui.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.135033 cypari-2.5.4/gmp_src/scanf/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1321 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18681 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/scanf/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20899 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/doscan.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1292 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/fscanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1730 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/fscanffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1282 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/scanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1424 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/sscanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/sscanffuns.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1219 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/vfscanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1210 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/vscanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1804 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/scanf/vsscanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4519 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tal-debug.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3871 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tal-notreent.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2432 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tal-reent.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     4640 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/test-driver
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.145441 cypari-2.5.4/gmp_src/tests/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1545 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    47368 2020-11-14 18:45:16.000000 cypari-2.5.4/gmp_src/tests/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4413 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/amd64call.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3025 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/amd64check.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2524 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/arm32call.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2669 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/arm32check.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.156238 cypari-2.5.4/gmp_src/tests/cxx/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3267 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    51952 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/cxx/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1809 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/clocale.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11210 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-assign.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12639 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-binary.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1570 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-cast.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16180 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-constr.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7305 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-cxx11.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1020 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-do-exceptions-work-at-all-with-this-compiler.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      867 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-headers.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2168 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-iostream.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19072 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-istream.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4467 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-locale.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12741 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-misc.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2923 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-mix.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13655 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2719 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops2.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2917 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops2f.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2679 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops2qf.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5065 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops2z.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3020 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ops3.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13949 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ostream.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-prec.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3227 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-rand.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17797 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-ternary.cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2749 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/cxx/t-unary.cc
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.158946 cypari-2.5.4/gmp_src/tests/devel/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1880 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20584 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/devel/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1173 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4056 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/gen-test-longlong_h.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8387 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/primes.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9671 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/sqrtrem_1_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    88571 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/devel/try.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6429 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/memory.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.160582 cypari-2.5.4/gmp_src/tests/misc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1316 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/misc/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33804 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/misc/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5016 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/misc/t-locale.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    25148 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/misc/t-printf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    49572 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/misc/t-scanf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13974 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/misc.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.171088 cypari-2.5.4/gmp_src/tests/mpf/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1397 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50810 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/mpf/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4955 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/reuse.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2440 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2492 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-cmp_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3976 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7366 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-conv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4320 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2840 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-dm2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5653 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-eq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8550 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-fits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2342 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3458 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-get_d_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6211 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-get_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3650 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-get_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1490 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-gsprec.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5691 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1785 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-int_p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3877 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-mul_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3561 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-muldiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1609 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-pow_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2640 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-set.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2809 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-set_q.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2512 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-set_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2440 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-set_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4832 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-sqrt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3470 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-sqrt_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8419 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7029 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-trunc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3404 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpf/t-ui_div.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.191755 cypari-2.5.4/gmp_src/tests/mpn/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1718 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    67379 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/mpn/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3611 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/logic.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9286 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-aors_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2047 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-asmtype.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8858 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-bdiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2557 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-broot.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-brootinv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13184 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3805 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-divrem_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9315 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-fat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9436 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-fib2m.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2008 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-gcd_11.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2161 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-gcd_22.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3125 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-gcdext_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13329 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9665 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-hgcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13599 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-hgcd_appr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8716 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-instrument.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3680 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6885 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-iord_u.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5168 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-matrix22.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3846 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-minvert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2921 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mod_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3044 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mp_bases.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2204 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3360 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mullo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2258 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mulmid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6049 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-mulmod_bnm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3137 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-perfsqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3000 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-scan.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2197 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-sizeinbase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3270 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-sqrlo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4926 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-sqrmod_bnm1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      184 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom2-sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      291 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom22.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      209 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom3-sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      205 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom32.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      323 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom33.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      234 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom4-sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      213 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom42.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      202 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom43.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      329 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom44.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      213 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom52.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      224 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom53.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      254 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom54.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      278 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom6-sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      224 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom62.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      250 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom63.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      357 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom6h.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      301 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom8-sqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      519 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/t-toom8h.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3934 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/toom-shared.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3034 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpn/toom-sqr-shared.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.197126 cypari-2.5.4/gmp_src/tests/mpq/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1429 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    41970 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/mpq/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3034 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/io.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5329 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/reuse.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4138 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-aors.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2163 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2677 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2651 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-cmp_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3003 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-cmp_z.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3560 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-equal.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6012 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3617 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-get_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3958 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1611 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-inv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7483 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-md_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5426 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-set_f.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2306 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpq/t-set_str.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.214738 cypari-2.5.4/gmp_src/tests/mpz/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1928 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    76574 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/mpz/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4717 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/convert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2361 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/dive.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1971 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/dive_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3315 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/io.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4340 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/logic.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20369 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/reuse.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3018 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-addsub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8852 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-aorsmul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7341 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-bin.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8834 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-bit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4723 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cdiv_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3670 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6667 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cmp_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2504 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cmp_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5175 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cong.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4406 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-cong_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4652 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-div_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3758 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-divis.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3031 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-divis_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7050 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-export.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3100 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-fac_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4053 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-fdiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4717 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-fdiv_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4639 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-fib_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5028 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-fits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13097 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3710 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-gcd_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1811 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-get_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5963 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-get_d_2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3066 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-get_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3017 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-hamdist.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6446 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-import.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4879 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-inp_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2980 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-invert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6675 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-io_raw.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23490 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-jac.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4171 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-lcm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5478 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-limbs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3529 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-lucm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2651 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-lucnum_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4158 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-mfac_uiui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5702 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-mul.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2663 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-mul_i.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6548 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-nextprime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-oddeven.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5829 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-perfpow.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3892 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-perfsqr.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3552 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-popcount.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4783 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-pow.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5101 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-powm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3352 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-powm_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4945 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-pprime_p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3574 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-primorial_ui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3658 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-remove.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-root.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3547 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-scan.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3586 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-set_d.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2453 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-set_f.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2562 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-set_si.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2677 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-set_str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2499 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-sizeinbase.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2910 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-sqrtrem.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4042 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-tdiv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4731 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/mpz/t-tdiv_ui.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.218976 cypari-2.5.4/gmp_src/tests/rand/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3619 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    40954 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tests/rand/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5741 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/findlc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10743 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/gen.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1918 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/gmpstat.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3135 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/spect.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9899 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/stat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20584 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/statlib.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1752 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-iset.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4417 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-lc2exp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1877 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-mt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10836 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-rand.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1831 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-urbui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1903 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-urmui.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3530 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/t-urndmm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1178 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/rand/zdiv_round.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10712 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/refmpf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    64458 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/refmpn.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1372 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/refmpq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6966 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/refmpz.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2918 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/spinner.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1755 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-bswap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12661 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-constants.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2041 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-count_zeros.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1532 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-hightomask.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1711 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-modlinv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1534 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-parity.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1824 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-popc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2954 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/t-sub.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18786 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/tests.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7406 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/trace.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3834 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/x86call.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3232 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tests/x86check.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.234692 cypari-2.5.4/gmp_src/tune/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6953 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/Makefile.am
+-rw-r--r--   0 nmd      (444129884) staff       (20)    32780 2020-11-14 18:45:17.000000 cypari-2.5.4/gmp_src/tune/Makefile.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19572 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2046 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/alpha.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    66325 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/common.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1536 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/div_qr_1_tune.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1217 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/div_qr_1n_pi1_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1217 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/div_qr_1n_pi1_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1345 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/divrem1div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1337 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/divrem1inv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1259 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/divrem2div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1248 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/divrem2inv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24392 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/freq.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1213 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/gcdext_double.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1225 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/gcdext_single.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1240 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/gcdextod.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1252 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/gcdextos.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2-1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2-2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2-3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2-4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2-5.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1388 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1309 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd_appr_lehmer.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1263 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd_lehmer.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1287 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd_reduce_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1277 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hgcd_reduce_2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1401 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hppa.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1464 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hppa2.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1465 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/hppa2w.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1416 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/ia64.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1183 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/jacbase1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1183 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/jacbase2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1183 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/jacbase3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1189 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/jacbase4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    40450 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/many.pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/mod_1_1-1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1256 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/mod_1_1-2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1488 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/mod_1_div.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1474 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/mod_1_inv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7612 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/modlinv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1468 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/noop.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1740 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/pentium.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1391 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/powerpc.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1367 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/powerpc64.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1166 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/powm_mod.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1283 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/powm_redc.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1197 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/pre_divrem_1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1514 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/set_strb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1408 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/set_strp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1422 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/set_strs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1438 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/sparcv9.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7150 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/speed-ext.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    44861 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/speed.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   124166 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/speed.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    48417 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/time.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4690 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/tune-gcd-p.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    83217 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/tuneup.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1676 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/tune/x86_64.asm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1127 2020-11-14 18:45:09.000000 cypari-2.5.4/gmp_src/version.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     6858 2015-09-05 19:09:34.000000 cypari-2.5.4/gmp_src/ylwrap
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.234955 cypari-2.5.4/macOS/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      278 2023-04-01 22:38:25.000000 cypari-2.5.4/macOS/mac_paricfg.patch
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.239258 cypari-2.5.4/pari_src/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7075 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/AUTHORS
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21040 2022-12-23 18:36:15.000000 cypari-2.5.4/pari_src/CHANGES
+-rw-r--r--   0 nmd      (444129884) staff       (20)    38270 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/CHANGES-2.10
+-rw-r--r--   0 nmd      (444129884) staff       (20)    36011 2021-04-18 15:48:51.000000 cypari-2.5.4/pari_src/CHANGES-2.12
+-rw-r--r--   0 nmd      (444129884) staff       (20)   213505 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/CHANGES-2.2
+-rw-r--r--   0 nmd      (444129884) staff       (20)    88634 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/CHANGES-2.4
+-rw-r--r--   0 nmd      (444129884) staff       (20)    51287 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/CHANGES-2.6
+-rw-r--r--   0 nmd      (444129884) staff       (20)    45107 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/CHANGES-2.8
+-rw-r--r--   0 nmd      (444129884) staff       (20)    57465 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/COMPAT
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18092 2013-05-03 23:00:49.000000 cypari-2.5.4/pari_src/COPYING
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     6200 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/Configure
+-rw-r--r--   0 nmd      (444129884) staff       (20)      864 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/INSTALL
+-rw-r--r--   0 nmd      (444129884) staff       (20)      672 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/LICENSE
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10529 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/NEW
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3526 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4304 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/README-git
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.272688 cypari-2.5.4/pari_src/config/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4894 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/DOC_Make.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1521 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/GEN_Make.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)      115 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/Imakefile
+-rw-r--r--   0 nmd      (444129884) staff       (20)    22386 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/Makefile.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4496 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/config/TOP_Make.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)       45 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/ansi.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2911 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/arch-osname
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      726 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/checkspaces
+-rw-r--r--   0 nmd      (444129884) staff       (20)       43 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/cleanup_exe
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     1810 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/convertllp64
+-rw-r--r--   0 nmd      (444129884) staff       (20)      123 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/cygwin-gprc
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     6788 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/cygwin-pari.nsi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      254 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/cygwin-postinst
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      309 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/display
+-rw-r--r--   0 nmd      (444129884) staff       (20)      519 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/endian.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      780 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/extract_files
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      337 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/genfunclist
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      385 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/genkernel
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      274 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_MANIFEST
+-rw-r--r--   0 nmd      (444129884) staff       (20)      751 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/get_PATH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1604 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_Qt
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1520 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_X11
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1083 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_archos
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4668 2022-12-23 16:02:05.000000 cypari-2.5.4/pari_src/config/get_cc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9177 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_config_options
+-rw-r--r--   0 nmd      (444129884) staff       (20)      406 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/get_dlcflags
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3898 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_dlld
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1605 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_double_format
+-rw-r--r--   0 nmd      (444129884) staff       (20)      422 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_fltk
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2609 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_gmp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2252 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_graphic_lib
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/get_head
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2049 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/config/get_install
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4338 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_kernel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1800 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_ld
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1962 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/get_libc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      905 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/get_modld
+-rw-r--r--   0 nmd      (444129884) staff       (20)      709 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/get_mt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      287 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/get_nl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      923 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/config/get_objdir
+-rw-r--r--   0 nmd      (444129884) staff       (20)      542 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_perl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      442 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/config/get_pretty
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2501 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/get_readline
+-rw-r--r--   0 nmd      (444129884) staff       (20)      988 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/get_static
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1091 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/get_tests
+-rw-r--r--   0 nmd      (444129884) staff       (20)      187 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/gmp_mismatch.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      239 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/gmp_version.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       73 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/gnu.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      159 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/gprc.mingw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      797 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/has_Qt4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      292 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/has_TIOCGWINSZ.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      116 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_X11.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       94 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_alarm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      734 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/has_avx.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      144 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_clock_gettime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      162 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/has_dlopen.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       78 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_exp2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      114 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/has_fltk.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      100 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/config/has_ftime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       62 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_getenv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      186 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_getrlimit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      221 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_getrusage.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      144 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/has_gettimeofday.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       55 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_isatty.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       78 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_log2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      380 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/has_mmap.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      380 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/has_neon.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       77 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_opendir.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       78 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/has_rint.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      100 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_setsid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      204 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_sigaction.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      438 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/has_sse2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      228 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_stat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       85 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_strftime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       86 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/has_system.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      188 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_times.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      162 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_vsnprintf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       86 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/has_wait.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      108 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/has_waitpid.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      384 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/install
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      601 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/kernel-name
+-rw-r--r--   0 nmd      (444129884) staff       (20)      316 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/kernel.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      125 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/ldflags
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      210 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/locate
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      122 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/locatedir
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      956 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/locatelib
+-rw-r--r--   0 nmd      (444129884) staff       (20)       33 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/log_cmd
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      438 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/look
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2109 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/make_tags
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     4473 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/mingw-pari.nsi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      256 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/config/mpi.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      490 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/myread
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      182 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/config/objdir
+-rw-r--r--   0 nmd      (444129884) staff       (20)      229 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/config/pari.nsi.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4232 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/config/paricfg.h.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)      364 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/config/pthread.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      110 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/rl_version.c
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      816 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/config/settar
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      478 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/config/setversion
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1159 2022-12-24 10:21:07.000000 cypari-2.5.4/pari_src/config/version
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.284727 cypari-2.5.4/pari_src/doc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29958 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/INSTALL.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1101 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/doc/appb.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3467 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/doc/appd.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34964 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/doc/develop.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10072 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/doc/gp.1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5566 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/doc/gphelp.1
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    37206 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/doc/gphelp.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3352 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/doc/index.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      793 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/doc/libpari.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14999 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/doc/parallel.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      203 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/doc/paricfg.tex.in
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13348 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/parimacro.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5214 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/doc/pdfmacs.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10435 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/refcard-ell.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5973 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/refcard-lfun.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12521 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/refcard-mf.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    27085 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/doc/refcard-nf.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    39102 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/refcard.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6626 2022-11-05 13:54:18.000000 cypari-2.5.4/pari_src/doc/refmacro.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2003 2017-01-14 12:26:41.000000 cypari-2.5.4/pari_src/doc/tex2mail.1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6585 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/translations
+-rw-r--r--   0 nmd      (444129884) staff       (20)    85506 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/doc/tutorial-mf.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)   183273 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/tutorial.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      787 2022-12-01 09:37:20.000000 cypari-2.5.4/pari_src/doc/users.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6915 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/doc/usersFUNCS.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21930 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/usersch1.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)   143063 2022-12-05 19:59:52.000000 cypari-2.5.4/pari_src/doc/usersch2.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)  1439773 2022-12-24 10:20:38.000000 cypari-2.5.4/pari_src/doc/usersch3.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)   109169 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/doc/usersch4.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)   657454 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/doc/usersch5.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)   156706 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/usersch6.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    39476 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/usersch7.tex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18369 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/doc/usersch8.tex
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.290057 cypari-2.5.4/pari_src/examples/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4789 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/EXPLAIN
+-rw-r--r--   0 nmd      (444129884) staff       (20)      525 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/examples/Inputrc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      146 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/examples/bench.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2733 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/examples/cl.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      939 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/examples/classno.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      247 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/contfrac.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      913 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/examples/extgcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)       85 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/examples/lucas.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1746 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/minigp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1285 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/openmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1174 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/pari-mt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3086 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/examples/pari.f90
+-rw-r--r--   0 nmd      (444129884) staff       (20)      396 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/examples/parigp.sty
+-rw-r--r--   0 nmd      (444129884) staff       (20)      801 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/examples/rho.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1062 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/examples/squfof.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1798 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/examples/taylor.gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2005 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/examples/thread.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.292721 cypari-2.5.4/pari_src/misc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      522 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/misc/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)      731 2020-04-08 20:04:14.000000 cypari-2.5.4/pari_src/misc/color.dft
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6122 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/misc/cook.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      793 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/misc/gpalias
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      126 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/misc/gpflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3618 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/misc/gprc.dft
+-rw-r--r--   0 nmd      (444129884) staff       (20)      713 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/misc/gprc.dos
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)       65 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/misc/mpigp
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)    73177 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/misc/tex2mail.in
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      773 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/misc/xgp
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.292997 cypari-2.5.4/pari_src/src/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.325601 cypari-2.5.4/pari_src/src/basemath/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24232 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/F2v.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    72388 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/F2x.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24295 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/basemath/F2xqE.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6887 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/F3v.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50899 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FF.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23602 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Fle.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    32207 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Flv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   111698 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Flx.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    63629 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FlxX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    43497 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FlxqE.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20580 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Flxq_log.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    56857 2022-12-21 17:55:15.000000 cypari-2.5.4/pari_src/src/basemath/FpE.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    43233 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FpV.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    68543 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FpX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    85230 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FpXQX_factor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50601 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FpXX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    64067 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/FpX_factor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    38127 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/QX_factor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    46387 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Qfb.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23971 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/RgV.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    80250 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/RgX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8448 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/Ser.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3825 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/basemath/ZG.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    38320 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ZV.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33645 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ZX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    43208 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/Zp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   142197 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/alglin1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    51539 2022-10-26 11:46:05.000000 cypari-2.5.4/pari_src/src/basemath/alglin2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    25248 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/alglin3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    32294 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/aprcl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    97271 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/arith1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24087 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/arith2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    81336 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/base1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   109215 2022-11-08 13:27:13.000000 cypari-2.5.4/pari_src/src/basemath/base2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   100479 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/base3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    84158 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/base4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50302 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/base5.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    28720 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/bb_group.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33254 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/bb_hnf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17723 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/bern.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    56872 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/bibli1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    62863 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/bibli2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17160 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/basemath/bit.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14031 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/bnflog.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11166 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/bnfunits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    31115 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/buch1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   117416 2022-10-31 15:34:23.000000 cypari-2.5.4/pari_src/src/basemath/buch2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    83384 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/buch3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7219 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/buch4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    38479 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/char.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14021 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/concat.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   165587 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/crvwtors.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11236 2022-12-05 19:59:16.000000 cypari-2.5.4/pari_src/src/basemath/digits.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16848 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/dirichlet.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    48455 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ecpp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    40039 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/ellanal.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   205684 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/elliptic.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    47450 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ellisog.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    30138 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/ellpadic.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6216 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/basemath/ellpadiclambdamu.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    59384 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ellrank.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    64246 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ellsea.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21991 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/elltors.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    59053 2022-09-20 09:39:17.000000 cypari-2.5.4/pari_src/src/basemath/factcyclo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   105448 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/galconj.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    93638 2022-12-21 17:55:47.000000 cypari-2.5.4/pari_src/src/basemath/gen1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    74450 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/gen2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   113023 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/gen3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    58768 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/grossenchar.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    61244 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/hgm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    78332 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/basemath/hnf_snf.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    36041 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/hyperell.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    35587 2022-11-16 09:32:38.000000 cypari-2.5.4/pari_src/src/basemath/hypergeom.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   138263 2022-12-05 20:28:57.000000 cypari-2.5.4/pari_src/src/basemath/ifactor1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    32359 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/ispower.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    44757 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/kummer.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14190 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/basemath/lambert.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17846 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/lerch.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    76617 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/lfun.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18572 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/lfunquad.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    85353 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/basemath/lfunutils.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    66862 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/lll.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9046 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/basemath/map.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4200 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/basemath/matperm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19841 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/mellininv.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   373499 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/mftrace.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   148417 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/modsym.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8737 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/msfarey.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    69718 2022-12-05 20:29:05.000000 cypari-2.5.4/pari_src/src/basemath/nffactor.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   166966 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/nflist.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9383 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/nflistQT.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   119159 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/pclgp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    42745 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/perm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17762 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/polarit1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   107267 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/polarit2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    89998 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/polarit3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    69627 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/polclass.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   123442 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/polmodular.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    37341 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/prime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    50285 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/qfisom.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33256 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/qfsolve.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33691 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/quad.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6629 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/ramanujantau.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9547 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/random.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    72845 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/basemath/rootpol.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33081 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/subcyclo.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    45165 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/subfield.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16756 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/subgroup.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   106687 2022-12-21 17:55:47.000000 cypari-2.5.4/pari_src/src/basemath/trans1.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    65028 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/trans2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    90190 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/basemath/trans3.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23084 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/volcano.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29659 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/basemath/zetamult.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.327091 cypari-2.5.4/pari_src/src/desc/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.327423 cypari-2.5.4/pari_src/src/desc/PARI/
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     3787 2022-09-24 14:34:16.000000 cypari-2.5.4/pari_src/src/desc/PARI/822.pm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4599 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/desc/deftune
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     4612 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/desc/doc_make
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2221 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/desc/gen_proto
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     2276 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/desc/gen_tune
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)      298 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/desc/merge_822
+-rw-r--r--   0 nmd      (444129884) staff       (20)    68770 2022-12-21 20:26:47.000000 cypari-2.5.4/pari_src/src/funclist
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.347161 cypari-2.5.4/pari_src/src/functions/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.347705 cypari-2.5.4/pari_src/src/functions/algebras/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6554 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/algebras/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      352 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algadd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      615 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algalgtobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      462 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algaut
+-rw-r--r--   0 nmd      (444129884) staff       (20)      434 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algb
+-rw-r--r--   0 nmd      (444129884) staff       (20)      507 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      637 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algbasistoalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      942 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algcenter
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1037 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algcentralproj
+-rw-r--r--   0 nmd      (444129884) staff       (20)      371 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1288 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algcharpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      329 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algdegree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      527 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algdim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      728 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algdisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      495 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algdivl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      231 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algdivr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      651 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alggroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1799 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alggroupcenter
+-rw-r--r--   0 nmd      (444129884) staff       (20)      610 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alghasse
+-rw-r--r--   0 nmd      (444129884) staff       (20)      802 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alghassef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      543 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alghassei
+-rw-r--r--   0 nmd      (444129884) staff       (20)      930 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algindex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6463 2022-10-05 23:53:45.000000 cypari-2.5.4/pari_src/src/functions/algebras/alginit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      385 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alginv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      499 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alginvbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      851 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algisassociative
+-rw-r--r--   0 nmd      (444129884) staff       (20)      583 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algiscommutative
+-rw-r--r--   0 nmd      (444129884) staff       (20)      937 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algisdivision
+-rw-r--r--   0 nmd      (444129884) staff       (20)      622 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algisdivl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      513 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algisinv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1008 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algisramified
+-rw-r--r--   0 nmd      (444129884) staff       (20)      705 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algissemisimple
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1020 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algissimple
+-rw-r--r--   0 nmd      (444129884) staff       (20)      964 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algissplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      670 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatadd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      650 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatcontains
+-rw-r--r--   0 nmd      (444129884) staff       (20)      589 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatelement
+-rw-r--r--   0 nmd      (444129884) staff       (20)      917 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglathnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      555 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatindex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      673 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatinter
+-rw-r--r--   0 nmd      (444129884) staff       (20)      760 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatlefttransporter
+-rw-r--r--   0 nmd      (444129884) staff       (20)      872 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      786 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatrighttransporter
+-rw-r--r--   0 nmd      (444129884) staff       (20)      737 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/alglatsubset
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1077 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/algebras/algmakeintegral
+-rw-r--r--   0 nmd      (444129884) staff       (20)      372 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      802 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algmultable
+-rw-r--r--   0 nmd      (444129884) staff       (20)      347 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algneg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      895 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      545 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algpoleval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      376 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      685 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algprimesubalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      721 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algquotient
+-rw-r--r--   0 nmd      (444129884) staff       (20)      822 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algradical
+-rw-r--r--   0 nmd      (444129884) staff       (20)      638 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algramifiedplaces
+-rw-r--r--   0 nmd      (444129884) staff       (20)      267 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algrandom
+-rw-r--r--   0 nmd      (444129884) staff       (20)      832 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algrelmultable
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1198 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsimpledec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1802 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1390 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsplittingdata
+-rw-r--r--   0 nmd      (444129884) staff       (20)      768 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsplittingfield
+-rw-r--r--   0 nmd      (444129884) staff       (20)      353 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsqr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      376 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsub
+-rw-r--r--   0 nmd      (444129884) staff       (20)      898 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algsubalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1745 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algtableinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      446 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algtensor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1232 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algtomatrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)      896 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algtrace
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1174 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/algebras/algtype
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.354913 cypari-2.5.4/pari_src/src/functions/combinatorics/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      706 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      613 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/bernfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)      282 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/bernpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      562 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/bernreal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1170 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/bernvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      708 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/binomial
+-rw-r--r--   0 nmd      (444129884) staff       (20)      502 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/eulerfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)      314 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/eulerianpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      277 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/eulerpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      550 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/eulerreal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      908 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/eulervec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      157 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/fibonacci
+-rw-r--r--   0 nmd      (444129884) staff       (20)      551 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/hammingweight
+-rw-r--r--   0 nmd      (444129884) staff       (20)      937 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/harmonic
+-rw-r--r--   0 nmd      (444129884) staff       (20)      519 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/numbpart
+-rw-r--r--   0 nmd      (444129884) staff       (20)      536 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/numtoperm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2246 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/partitions
+-rw-r--r--   0 nmd      (444129884) staff       (20)      475 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/permcycles
+-rw-r--r--   0 nmd      (444129884) staff       (20)      326 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/permorder
+-rw-r--r--   0 nmd      (444129884) staff       (20)      287 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/permsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)      364 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/permtonum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1565 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/combinatorics/stirling
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.374597 cypari-2.5.4/pari_src/src/functions/conversions/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1513 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Col
+-rw-r--r--   0 nmd      (444129884) staff       (20)      591 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Colrev
+-rw-r--r--   0 nmd      (444129884) staff       (20)      506 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      528 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/List
+-rw-r--r--   0 nmd      (444129884) staff       (20)      853 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/Map
+-rw-r--r--   0 nmd      (444129884) staff       (20)      990 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Mat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1660 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/Mod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1771 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/Pol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      914 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Polrev
+-rw-r--r--   0 nmd      (444129884) staff       (20)      351 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/Qfb
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2221 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Ser
+-rw-r--r--   0 nmd      (444129884) staff       (20)      745 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Set
+-rw-r--r--   0 nmd      (444129884) staff       (20)      993 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Str
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2361 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Vec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      553 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/Vecrev
+-rw-r--r--   0 nmd      (444129884) staff       (20)      729 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/Vecsmall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      664 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/binary
+-rw-r--r--   0 nmd      (444129884) staff       (20)      882 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitand
+-rw-r--r--   0 nmd      (444129884) staff       (20)      613 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitneg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      706 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitnegimply
+-rw-r--r--   0 nmd      (444129884) staff       (20)      616 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1688 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitprecision
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1050 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/bittest
+-rw-r--r--   0 nmd      (444129884) staff       (20)      633 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/bitxor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      513 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/ceil
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1029 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/centerlift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      478 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/characteristic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1748 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/component
+-rw-r--r--   0 nmd      (444129884) staff       (20)      401 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/conj
+-rw-r--r--   0 nmd      (444129884) staff       (20)      838 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/conjvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1817 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/denominator
+-rw-r--r--   0 nmd      (444129884) staff       (20)      935 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/digits
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1476 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/exponent
+-rw-r--r--   0 nmd      (444129884) staff       (20)      514 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/floor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      220 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/frac
+-rw-r--r--   0 nmd      (444129884) staff       (20)      528 2022-12-05 19:59:16.000000 cypari-2.5.4/pari_src/src/functions/conversions/fromdigits
+-rw-r--r--   0 nmd      (444129884) staff       (20)      439 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/imag
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1129 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/length
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1934 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/lift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      773 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/liftall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      762 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/liftint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      718 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/liftpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      433 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/norm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1036 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/numerator
+-rw-r--r--   0 nmd      (444129884) staff       (20)      385 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/oo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1101 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/padicprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1497 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/precision
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3505 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/random
+-rw-r--r--   0 nmd      (444129884) staff       (20)      424 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/conversions/real
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1559 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/round
+-rw-r--r--   0 nmd      (444129884) staff       (20)      458 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/serchop
+-rw-r--r--   0 nmd      (444129884) staff       (20)      678 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/serprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1010 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/simplify
+-rw-r--r--   0 nmd      (444129884) staff       (20)      343 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/sizebyte
+-rw-r--r--   0 nmd      (444129884) staff       (20)      725 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/sizedigit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1709 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/truncate
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1185 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/conversions/valuation
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2556 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/varhigher
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1865 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/variable
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1066 2020-04-08 20:04:14.000000 cypari-2.5.4/pari_src/src/functions/conversions/variables
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3296 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/conversions/varlower
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.387902 cypari-2.5.4/pari_src/src/functions/default/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      284 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      665 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/TeXstyle
+-rw-r--r--   0 nmd      (444129884) staff       (20)      288 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/breakloop
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2179 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/colors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      162 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/compatible
+-rw-r--r--   0 nmd      (444129884) staff       (20)      552 2020-12-12 18:37:29.000000 cypari-2.5.4/pari_src/src/functions/default/datadir
+-rw-r--r--   0 nmd      (444129884) staff       (20)      376 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/default/debug
+-rw-r--r--   0 nmd      (444129884) staff       (20)      339 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/default/debugfiles
+-rw-r--r--   0 nmd      (444129884) staff       (20)      967 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/debugmem
+-rw-r--r--   0 nmd      (444129884) staff       (20)      673 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/echo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      776 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/factor_add_primes
+-rw-r--r--   0 nmd      (444129884) staff       (20)      672 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/factor_proven
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1410 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/format
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1014 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/graphcolormap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      400 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/graphcolors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      581 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/help
+-rw-r--r--   0 nmd      (444129884) staff       (20)      713 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/histfile
+-rw-r--r--   0 nmd      (444129884) staff       (20)      443 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/histsize
+-rw-r--r--   0 nmd      (444129884) staff       (20)      553 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/lines
+-rw-r--r--   0 nmd      (444129884) staff       (20)      237 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/linewrap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1193 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/log
+-rw-r--r--   0 nmd      (444129884) staff       (20)      249 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/logfile
+-rw-r--r--   0 nmd      (444129884) staff       (20)      739 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/nbthreads
+-rw-r--r--   0 nmd      (444129884) staff       (20)      468 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/new_galois_format
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1403 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/output
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1040 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/default/parisize
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1223 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/parisizemax
+-rw-r--r--   0 nmd      (444129884) staff       (20)      712 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/path
+-rw-r--r--   0 nmd      (444129884) staff       (20)      226 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/plothsizes
+-rw-r--r--   0 nmd      (444129884) staff       (20)      395 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/prettyprinter
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1738 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/primelimit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1449 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/prompt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      347 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/prompt_cont
+-rw-r--r--   0 nmd      (444129884) staff       (20)      235 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/psfile
+-rw-r--r--   0 nmd      (444129884) staff       (20)      435 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/readline
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1733 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/realbitprecision
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1305 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/realprecision
+-rw-r--r--   0 nmd      (444129884) staff       (20)      309 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/recover
+-rw-r--r--   0 nmd      (444129884) staff       (20)      456 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/secure
+-rw-r--r--   0 nmd      (444129884) staff       (20)      257 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/seriesprecision
+-rw-r--r--   0 nmd      (444129884) staff       (20)      868 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/simplify
+-rw-r--r--   0 nmd      (444129884) staff       (20)      826 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/sopath
+-rw-r--r--   0 nmd      (444129884) staff       (20)      832 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/strictargs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      163 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/strictmatch
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1157 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/threadsize
+-rw-r--r--   0 nmd      (444129884) staff       (20)      890 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/default/threadsizemax
+-rw-r--r--   0 nmd      (444129884) staff       (20)      929 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/default/timer
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.417367 cypari-2.5.4/pari_src/src/functions/elliptic_curves/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10220 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1251 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ell2cover
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1333 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellL1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      227 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elladd
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1311 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellak
+-rw-r--r--   0 nmd      (444129884) staff       (20)      888 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellan
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1275 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellanalyticrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3935 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      207 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellbil
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1138 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellbsd
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1762 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellcard
+-rw-r--r--   0 nmd      (444129884) staff       (20)      599 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellchangecurve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      745 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellchangepoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      725 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellchangepointinv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      620 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellconvertname
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1161 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elldivpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1434 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elleisnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      595 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elleta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      940 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellformaldifferential
+-rw-r--r--   0 nmd      (444129884) staff       (20)      722 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellformalexp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      675 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellformallog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      980 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellformalpoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      745 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellformalw
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1831 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellfromeqn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1211 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellfromj
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1509 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellgenerators
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1969 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellglobalred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3601 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1081 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellheegner
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1084 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellheight
+-rw-r--r--   0 nmd      (444129884) staff       (20)      813 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellheightmatrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)      717 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellidentify
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4924 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      722 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellintegralmodel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1213 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisdivisible
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1044 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisogeny
+-rw-r--r--   0 nmd      (444129884) staff       (20)      964 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisogenyapply
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2357 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisomat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      602 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisoncurve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1419 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellisotree
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1280 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellissupersingular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      281 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellj
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1351 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elllocalred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1165 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elllog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      742 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elllseries
+-rw-r--r--   0 nmd      (444129884) staff       (20)      362 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellminimaldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2091 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellminimalmodel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1432 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellminimaltwist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1308 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellmoddegree
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2256 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellmodulareqn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1054 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      190 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellneg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      874 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellnonsingularmultiple
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1873 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellorder
+-rw-r--r--   0 nmd      (444129884) staff       (20)      307 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellordinate
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4554 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicL
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3370 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicbsd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      906 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicfrobenius
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3366 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicheight
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1066 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicheightmatrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2326 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadiclambdamu
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1033 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadiclog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2053 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadicregulator
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1365 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpadics2
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1462 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellperiods
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3144 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpointtoz
+-rw-r--r--   0 nmd      (444129884) staff       (20)      183 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3799 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)      587 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellrankinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      842 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)      901 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellrootno
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1671 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellsaturation
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3178 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellsea
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1818 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellsearch
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1140 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellsigma
+-rw-r--r--   0 nmd      (444129884) staff       (20)      241 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellsub
+-rw-r--r--   0 nmd      (444129884) staff       (20)      599 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltamagawa
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1085 2020-11-14 12:26:52.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltaniyama
+-rw-r--r--   0 nmd      (444129884) staff       (20)      594 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltatepairing
+-rw-r--r--   0 nmd      (444129884) staff       (20)      807 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltors
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1140 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltrace
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1549 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/elltwist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2678 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellweilcurve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      846 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellweilpairing
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1908 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellwp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      932 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellxn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1480 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellzeta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2017 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/ellztopoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6016 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/genus2red
+-rw-r--r--   0 nmd      (444129884) staff       (20)      858 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellchangecurve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      729 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellcharpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      683 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperelldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      822 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellisoncurve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1108 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellminimaldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1516 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellminimalmodel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2203 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellpadicfrobenius
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1349 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1413 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/elliptic_curves/hyperellred
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.418506 cypari-2.5.4/pari_src/src/functions/gp2c/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      123 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c/DEBUGLEVEL
+-rw-r--r--   0 nmd      (444129884) staff       (20)      528 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c/clone
+-rw-r--r--   0 nmd      (444129884) staff       (20)      432 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c/copy
+-rw-r--r--   0 nmd      (444129884) staff       (20)      108 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c/unclone
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.424049 cypari-2.5.4/pari_src/src/functions/gp2c_internal/
+-rw-r--r--   0 nmd      (444129884) staff       (20)       82 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_avma
+-rw-r--r--   0 nmd      (444129884) staff       (20)      809 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_badtype
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3362 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_cast
+-rw-r--r--   0 nmd      (444129884) staff       (20)      160 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_cgetg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      521 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_const
+-rw-r--r--   0 nmd      (444129884) staff       (20)      281 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_formatcode
+-rw-r--r--   0 nmd      (444129884) staff       (20)      103 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_gc_needed
+-rw-r--r--   0 nmd      (444129884) staff       (20)      193 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_gerepileall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      344 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_gerepileupto
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_maxprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)       76 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_norange
+-rw-r--r--   0 nmd      (444129884) staff       (20)      181 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_prec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      227 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_stack_lim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      171 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_strtoclosure
+-rw-r--r--   0 nmd      (444129884) staff       (20)      894 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_tovec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2655 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_typedef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      521 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/gp2c_internal/_wrap
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.433584 cypari-2.5.4/pari_src/src/functions/graphic/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3979 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      804 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/plot
+-rw-r--r--   0 nmd      (444129884) staff       (20)      594 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotbox
+-rw-r--r--   0 nmd      (444129884) staff       (20)      434 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotclip
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1346 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotcolor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      862 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotcopy
+-rw-r--r--   0 nmd      (444129884) staff       (20)      259 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotcursor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      906 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotdraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      747 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5548 2022-09-24 12:30:28.000000 cypari-2.5.4/pari_src/src/functions/graphic/ploth
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1157 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plothexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      697 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/plothraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      977 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/plothrawexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      948 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plothsizes
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1254 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      413 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotkill
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1230 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotlines
+-rw-r--r--   0 nmd      (444129884) staff       (20)      463 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotlinetype
+-rw-r--r--   0 nmd      (444129884) staff       (20)      209 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotmove
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1181 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)      374 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotpointsize
+-rw-r--r--   0 nmd      (444129884) staff       (20)      454 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotpointtype
+-rw-r--r--   0 nmd      (444129884) staff       (20)      588 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrbox
+-rw-r--r--   0 nmd      (444129884) staff       (20)      711 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrecth
+-rw-r--r--   0 nmd      (444129884) staff       (20)      941 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrecthraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      462 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrline
+-rw-r--r--   0 nmd      (444129884) staff       (20)      381 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrmove
+-rw-r--r--   0 nmd      (444129884) staff       (20)      792 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotrpoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      726 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotscale
+-rw-r--r--   0 nmd      (444129884) staff       (20)      902 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/plotstring
+-rw-r--r--   0 nmd      (444129884) staff       (20)      215 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/psdraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      553 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/psploth
+-rw-r--r--   0 nmd      (444129884) staff       (20)      237 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/graphic/psplothraw
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.437867 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6491 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      406 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmalpha
+-rw-r--r--   0 nmd      (444129884) staff       (20)      423 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmbydegree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      386 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmcoef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      829 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmcoefs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      507 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1821 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmeulerfactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      327 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmgamma
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1653 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgminit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      680 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmissymmetrical
+-rw-r--r--   0 nmd      (444129884) staff       (20)      661 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmparams
+-rw-r--r--   0 nmd      (444129884) staff       (20)      535 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/hgmtwist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1736 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/hypergeometric_motives/lfunhgm
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.446256 cypari-2.5.4/pari_src/src/functions/l_functions/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16423 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/functions/l_functions/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1939 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1445 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunabelianrelinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      545 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunan
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3173 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunartin
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2466 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuncheckfeq
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3448 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4615 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuncost
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7994 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuncreate
+-rw-r--r--   0 nmd      (444129884) staff       (20)      543 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfundiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      757 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfundual
+-rw-r--r--   0 nmd      (444129884) staff       (20)      826 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunetaquo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      542 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuneuler
+-rw-r--r--   0 nmd      (444129884) staff       (20)      664 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfungenus2
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1782 2021-04-30 16:51:10.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunhardy
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2215 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuninit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      708 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunlambda
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1475 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunmfspec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      375 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      959 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunorderzero
+-rw-r--r--   0 nmd      (444129884) staff       (20)      678 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunparams
+-rw-r--r--   0 nmd      (444129884) staff       (20)      845 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunqf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1518 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunrootres
+-rw-r--r--   0 nmd      (444129884) staff       (20)      985 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunshift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      535 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunsympow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1268 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuntheta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1565 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunthetacost
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1622 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunthetainit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      609 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfuntwist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1722 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/l_functions/lfunzeros
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.472947 cypari-2.5.4/pari_src/src/functions/linear_algebra/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      913 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2985 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/algdep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2908 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/charpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2578 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/concat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      450 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/dirpowers
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1399 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/forqfvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2163 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/lindep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1134 2020-11-01 10:29:59.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matadjoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      201 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matcompanion
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2100 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matconcat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1300 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matdet
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1046 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matdetint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      690 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matdetmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      594 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matdiagonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1466 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mateigen
+-rw-r--r--   0 nmd      (444129884) staff       (20)      710 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matfrobenius
+-rw-r--r--   0 nmd      (444129884) staff       (20)      243 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathess
+-rw-r--r--   0 nmd      (444129884) staff       (20)      263 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3969 2022-03-11 11:29:37.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      792 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathnfmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      637 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathnfmodid
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1552 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mathouseholder
+-rw-r--r--   0 nmd      (444129884) staff       (20)      196 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matid
+-rw-r--r--   0 nmd      (444129884) staff       (20)      716 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matimage
+-rw-r--r--   0 nmd      (444129884) staff       (20)      551 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matimagecompl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1013 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matimagemod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      623 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matindexrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)      672 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matintersect
+-rw-r--r--   0 nmd      (444129884) staff       (20)      820 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matinverseimage
+-rw-r--r--   0 nmd      (444129884) staff       (20)      580 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matinvmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      230 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matisdiagonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1028 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matker
+-rw-r--r--   0 nmd      (444129884) staff       (20)      628 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matkerint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      654 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matkermod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      424 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matmuldiagonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      432 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matmultodiagonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      453 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matpascal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      478 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matpermanent
+-rw-r--r--   0 nmd      (444129884) staff       (20)      952 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matqr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      138 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1267 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matreduce
+-rw-r--r--   0 nmd      (444129884) staff       (20)      689 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1594 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matrixqz
+-rw-r--r--   0 nmd      (444129884) staff       (20)      349 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matsize
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2073 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matsnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1603 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1648 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matsolvemod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      866 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/matsupplement
+-rw-r--r--   0 nmd      (444129884) staff       (20)      207 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/mattranspose
+-rw-r--r--   0 nmd      (444129884) staff       (20)      444 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/minpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      858 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/norml2
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1448 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/normlp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      811 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/powers
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1295 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfauto
+-rw-r--r--   0 nmd      (444129884) staff       (20)      783 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfautoexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      202 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfbil
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2659 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfeval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1227 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfgaussred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1265 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1332 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfisominit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      878 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfjacobi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3834 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qflll
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1825 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qflllgram
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6451 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfminim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      840 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfminimize
+-rw-r--r--   0 nmd      (444129884) staff       (20)      202 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      819 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qforbits
+-rw-r--r--   0 nmd      (444129884) staff       (20)      907 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfparam
+-rw-r--r--   0 nmd      (444129884) staff       (20)      638 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfperfection
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1110 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfrep
+-rw-r--r--   0 nmd      (444129884) staff       (20)      361 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1028 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/qfsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      634 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setbinop
+-rw-r--r--   0 nmd      (444129884) staff       (20)      320 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setdelta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      320 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setintersect
+-rw-r--r--   0 nmd      (444129884) staff       (20)      574 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setisset
+-rw-r--r--   0 nmd      (444129884) staff       (20)      366 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setminus
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1668 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setsearch
+-rw-r--r--   0 nmd      (444129884) staff       (20)      290 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/setunion
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1238 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/snfrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)      396 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/trace
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2823 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vecextract
+-rw-r--r--   0 nmd      (444129884) staff       (20)      303 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vecprod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1949 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vecsearch
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4876 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vecsort
+-rw-r--r--   0 nmd      (444129884) staff       (20)      290 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vecsum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1141 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vector
+-rw-r--r--   0 nmd      (444129884) staff       (20)      444 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vectorsmall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      288 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/linear_algebra/vectorv
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.484768 cypari-2.5.4/pari_src/src/functions/member_functions/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/a1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/a2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/a3
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/a4
+-rw-r--r--   0 nmd      (444129884) staff       (20)      137 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/a6
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/area
+-rw-r--r--   0 nmd      (444129884) staff       (20)      137 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/b2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/b4
+-rw-r--r--   0 nmd      (444129884) staff       (20)      143 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/b6
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/b8
+-rw-r--r--   0 nmd      (444129884) staff       (20)      195 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/bid
+-rw-r--r--   0 nmd      (444129884) staff       (20)      221 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/bnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/c4
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/c6
+-rw-r--r--   0 nmd      (444129884) staff       (20)      266 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/clgp
+-rw-r--r--   0 nmd      (444129884) staff       (20)       96 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/codiff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      286 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/cyc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      199 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/diff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      249 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/disc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      128 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/e
+-rw-r--r--   0 nmd      (444129884) staff       (20)       87 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/eta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      127 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/f
+-rw-r--r--   0 nmd      (444129884) staff       (20)      360 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/member_functions/fu
+-rw-r--r--   0 nmd      (444129884) staff       (20)      335 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/member_functions/gen
+-rw-r--r--   0 nmd      (444129884) staff       (20)      203 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/member_functions/group
+-rw-r--r--   0 nmd      (444129884) staff       (20)      204 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/index
+-rw-r--r--   0 nmd      (444129884) staff       (20)      132 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/j
+-rw-r--r--   0 nmd      (444129884) staff       (20)       87 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/mod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      176 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/nf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      280 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/no
+-rw-r--r--   0 nmd      (444129884) staff       (20)       93 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/omega
+-rw-r--r--   0 nmd      (444129884) staff       (20)      151 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/orders
+-rw-r--r--   0 nmd      (444129884) staff       (20)      230 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/p
+-rw-r--r--   0 nmd      (444129884) staff       (20)      242 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/pol
+-rw-r--r--   0 nmd      (444129884) staff       (20)       96 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/polabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      189 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/r1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      189 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/r2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      236 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/reg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      254 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/roots
+-rw-r--r--   0 nmd      (444129884) staff       (20)      194 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/sign
+-rw-r--r--   0 nmd      (444129884) staff       (20)      142 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/t2
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/tate
+-rw-r--r--   0 nmd      (444129884) staff       (20)      133 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/tu
+-rw-r--r--   0 nmd      (444129884) staff       (20)      171 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/zk
+-rw-r--r--   0 nmd      (444129884) staff       (20)      142 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/member_functions/zkst
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.504035 cypari-2.5.4/pari_src/src/functions/modular_forms/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3563 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1739 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/getcache
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1387 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/lfunmf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      279 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfDelta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      755 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfEH
+-rw-r--r--   0 nmd      (444129884) staff       (20)      368 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfEk
+-rw-r--r--   0 nmd      (444129884) staff       (20)      825 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfTheta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1123 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfatkin
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1571 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfatkineigenvalues
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2578 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfatkininit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1283 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      396 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfbd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      500 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfbracket
+-rw-r--r--   0 nmd      (444129884) staff       (20)      441 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcoef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      949 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcoefs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      699 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1041 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcosets
+-rw-r--r--   0 nmd      (444129884) staff       (20)      486 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcuspisregular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      540 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcusps
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1440 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcuspval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      546 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfcuspwidth
+-rw-r--r--   0 nmd      (444129884) staff       (20)      563 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfderiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      648 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfderivE2
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1160 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfdescribe
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2803 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfdim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      764 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2628 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfeigenbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1954 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfeigensearch
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2370 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfeisenstein
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3947 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfembed
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1623 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfeval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1140 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mffields
+-rw-r--r--   0 nmd      (444129884) staff       (20)      872 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mffromell
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1419 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mffrometaquo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1866 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mffromlfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1625 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mffromqf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1538 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfgaloisprojrep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1582 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfgaloistype
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1824 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfhecke
+-rw-r--r--   0 nmd      (444129884) staff       (20)      651 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfheckemat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2822 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      944 2020-04-08 20:04:14.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfisCM
+-rw-r--r--   0 nmd      (444129884) staff       (20)      564 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfisequal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      855 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfisetaquo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1167 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfkohnenbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3107 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfkohnenbijection
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1355 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfkohneneigenbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1729 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mflinear
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1392 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfmanin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      371 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      270 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfnumcusps
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2145 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfparams
+-rw-r--r--   0 nmd      (444129884) staff       (20)      990 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfperiodpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      498 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfperiodpolbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2950 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfpetersson
+-rw-r--r--   0 nmd      (444129884) staff       (20)      293 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2256 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfsearch
+-rw-r--r--   0 nmd      (444129884) staff       (20)      502 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfshift
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1403 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfshimura
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4009 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfslashexpansion
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1076 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfspace
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2622 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfsplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      792 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfsturm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1896 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfsymbol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2922 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mfsymboleval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      875 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftaylor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2956 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      655 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftocoset
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1028 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftonew
+-rw-r--r--   0 nmd      (444129884) staff       (20)      801 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftraceform
+-rw-r--r--   0 nmd      (444129884) staff       (20)      893 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_forms/mftwist
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.512426 cypari-2.5.4/pari_src/src/functions/modular_symbols/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1555 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      854 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msatkinlehner
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1683 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mscosets
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1017 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mscuspidal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      748 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msdim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      786 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mseisenstein
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2263 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mseval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2160 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msfarey
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1585 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msfromcusp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2819 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msfromell
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1197 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msfromhecke
+-rw-r--r--   0 nmd      (444129884) staff       (20)      270 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msgetlevel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      389 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msgetsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)      338 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msgetweight
+-rw-r--r--   0 nmd      (444129884) staff       (20)      984 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mshecke
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1745 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      877 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msissymbol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mslattice
+-rw-r--r--   0 nmd      (444129884) staff       (20)      623 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msnew
+-rw-r--r--   0 nmd      (444129884) staff       (20)      564 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msomseval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4138 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspadicL
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1963 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspadicinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1719 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspadicmoments
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3179 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspadicseries
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2064 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspathgens
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1359 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspathlog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1974 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspetersson
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5840 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mspolygon
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1522 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msqexpansion
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1482 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mssplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      571 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/msstar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2509 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/modular_symbols/mstooms
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.580032 cypari-2.5.4/pari_src/src/functions/number_fields/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    23469 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/functions/number_fields/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1479 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfcertify
+-rw-r--r--   0 nmd      (444129884) staff       (20)      591 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfdecodemodule
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6940 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      944 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfisintnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1534 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfisnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3727 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfisprincipal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      223 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfissunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3372 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfisunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1356 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1149 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnflogdegree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      968 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnflogef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      841 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfnarrow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1012 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfsignunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1173 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfsunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2513 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnfunits
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2866 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrL1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1557 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2470 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrclassfield
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1213 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrclassno
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1183 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrclassnolist
+-rw-r--r--   0 nmd      (444129884) staff       (20)      917 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrcompositum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2970 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      250 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrconductorofchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1493 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrdisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2592 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrdisclist
+-rw-r--r--   0 nmd      (444129884) staff       (20)      454 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrgaloisapply
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1929 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrgaloismatrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3532 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      643 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrisconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1418 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrisgalois
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3830 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrisprincipal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2221 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrmap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1396 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrrootnumber
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2248 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/bnrstark
+-rw-r--r--   0 nmd      (444129884) staff       (20)      346 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/dirzetak
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1345 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/factornf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1166 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoischardet
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1213 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoischarpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2423 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoischartable
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1088 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisconjclasses
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1335 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2005 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisfixedfield
+-rw-r--r--   0 nmd      (444129884) staff       (20)      852 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisgetgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1067 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisgetname
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1600 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisgetpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1105 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisidentify
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4067 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      596 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisisabelian
+-rw-r--r--   0 nmd      (444129884) staff       (20)      559 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoisisnormal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      865 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoispermtopol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      856 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoissplittinginit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2851 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoissubcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      423 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoissubfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)      814 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/galoissubgroups
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1549 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharalgebraic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1110 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1838 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharduallog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      824 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gchareval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2562 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharidentify
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3080 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1051 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharisalgebraic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2263 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharlocal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2036 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharlog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      481 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/gcharnewprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1327 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealadd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      868 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealaddtoone
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1159 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2766 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealchinese
+-rw-r--r--   0 nmd      (444129884) staff       (20)      457 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealcoprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1108 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      617 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealdown
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1180 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealfactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1829 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealfactorback
+-rw-r--r--   0 nmd      (444129884) staff       (20)      963 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealfrobenius
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2125 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealhnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      753 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealintersect
+-rw-r--r--   0 nmd      (444129884) staff       (20)      414 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealinv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1274 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealismaximal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      662 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealispower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2832 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/ideallist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1736 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/ideallistarch
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1601 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/ideallog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      385 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealmin
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1274 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      214 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      393 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealnumden
+-rw-r--r--   0 nmd      (444129884) staff       (20)      895 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2173 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealprimedec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      778 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealprincipalunits
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1715 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealramgroups
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2823 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1504 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealredmodpower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3478 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealstar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2019 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealtwoelt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      542 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/idealval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      399 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/matalgtobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      399 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/matbasistoalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1543 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/modreverse
+-rw-r--r--   0 nmd      (444129884) staff       (20)      478 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/newtonpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      580 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfalgtobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6844 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      569 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfbasistoalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      996 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfcertify
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3367 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfcompositum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      341 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfdetint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1871 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfdisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1517 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfdiscfactors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      307 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltadd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      226 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      406 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltdiveuc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      556 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltdivmodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      345 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltdivrem
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1168 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltembed
+-rw-r--r--   0 nmd      (444129884) staff       (20)      420 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltispower
+-rw-r--r--   0 nmd      (444129884) staff       (20)      405 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltissquare
+-rw-r--r--   0 nmd      (444129884) staff       (20)      423 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      225 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      553 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltmulmodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      145 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      354 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      544 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltpowmodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      359 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltreduce
+-rw-r--r--   0 nmd      (444129884) staff       (20)      553 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltreducemodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1196 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)      150 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfelttrace
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1846 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfeltval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1986 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nffactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      818 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nffactorback
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1191 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nffactormod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2202 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfgaloisapply
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2291 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfgaloisconj
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1921 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfgrunwaldwang
+-rw-r--r--   0 nmd      (444129884) staff       (20)      779 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfhilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      798 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfhnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      539 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfhnfmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9961 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      243 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfisideal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3758 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfisincl
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1623 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfisisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)      857 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfislocalpower
+-rw-r--r--   0 nmd      (444129884) staff       (20)      475 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfkermodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12555 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nflist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1235 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfmodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1298 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfmodprinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1024 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfmodprlift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      859 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfnewprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1429 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfpolsturm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2018 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfresolvent
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1691 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfroots
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1234 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfrootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1419 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      825 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsolvemodpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3019 2022-11-30 13:34:53.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsplitting
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1937 2021-06-09 10:39:44.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsubfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1243 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsubfieldscm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      511 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/nfsubfieldsmax
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4332 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polcompositum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4265 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polgalois
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1850 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5385 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polredabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2276 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polredbest
+-rw-r--r--   0 nmd      (444129884) staff       (20)      206 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/polredord
+-rw-r--r--   0 nmd      (444129884) staff       (20)      465 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/poltschirnhaus
+-rw-r--r--   0 nmd      (444129884) staff       (20)      481 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfalgtobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1089 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)      422 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfbasistoalg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      577 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfcharpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2430 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3512 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfdedekind
+-rw-r--r--   0 nmd      (444129884) staff       (20)      235 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfdet
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1068 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfdisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1246 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfeltabstorel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1545 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfeltdown
+-rw-r--r--   0 nmd      (444129884) staff       (20)      538 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfeltnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      757 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfeltreltoabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      519 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfelttrace
+-rw-r--r--   0 nmd      (444129884) staff       (20)      951 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfeltup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2279 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfequation
+-rw-r--r--   0 nmd      (444129884) staff       (20)      690 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfhnfbasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1825 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealabstorel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      482 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealdown
+-rw-r--r--   0 nmd      (444129884) staff       (20)      999 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealfactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      469 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealhnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      410 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      572 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealnormabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      445 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealnormrel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1366 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealprimedec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1647 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealreltoabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      463 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealtwoelt
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1421 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfidealup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5623 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      440 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfisabelian
+-rw-r--r--   0 nmd      (444129884) staff       (20)      540 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfisfree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      852 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfislocalcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2347 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfisnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1060 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfisnorminit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      235 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfkummer
+-rw-r--r--   0 nmd      (444129884) staff       (20)      648 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnflllgram
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1247 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfnormgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)      794 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfpolred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2082 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfpolredabs
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1967 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfpolredbest
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1940 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfpseudobasis
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1086 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/rnfsteinitz
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3890 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/subcyclohminus
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9576 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/subcycloiwasawa
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8592 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_fields/subcyclopclgp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2601 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_fields/subgrouplist
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.626041 cypari-2.5.4/pari_src/src/functions/number_theoretical/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6989 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1118 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/addprimes
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2148 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/bestappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2389 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/bestapprPade
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1565 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/bestapprnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      183 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/bezout
+-rw-r--r--   0 nmd      (444129884) staff       (20)      371 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/bigomega
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1561 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/charconj
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1802 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/chardiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3260 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/chareval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1380 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/chargalois
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1616 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/charker
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1800 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/charmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1399 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/charorder
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1710 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/charpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2323 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/chinese
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1774 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/content
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2932 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/contfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1491 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/contfracpnqn
+-rw-r--r--   0 nmd      (444129884) staff       (20)      659 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/core
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1126 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/coredisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      334 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/dirdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1594 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/direuler
+-rw-r--r--   0 nmd      (444129884) staff       (20)      688 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/dirmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1547 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/dirpowerssum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2013 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/divisors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      912 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/divisorslenstra
+-rw-r--r--   0 nmd      (444129884) staff       (20)      525 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/eulerphi
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11662 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1156 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factorback
+-rw-r--r--   0 nmd      (444129884) staff       (20)      216 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factorcantor
+-rw-r--r--   0 nmd      (444129884) staff       (20)      217 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factorff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      347 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factorial
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2084 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factorint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2509 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factormod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1940 2022-11-30 13:35:28.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factormodDDF
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1709 2022-11-30 13:35:28.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factormodSQF
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2456 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/factormodcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      707 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffcompomap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      551 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffembed
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1142 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffextend
+-rw-r--r--   0 nmd      (444129884) staff       (20)      486 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/fffrobenius
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1870 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffgen
+-rw-r--r--   0 nmd      (444129884) staff       (20)      703 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      546 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffinvmap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1851 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/fflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      740 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffmap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      973 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffmaprel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      652 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffnbirred
+-rw-r--r--   0 nmd      (444129884) staff       (20)      860 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/fforder
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1120 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ffprimroot
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2420 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/gcd
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1123 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/gcdext
+-rw-r--r--   0 nmd      (444129884) staff       (20)      996 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/halfgcd
+-rw-r--r--   0 nmd      (444129884) staff       (20)      536 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/hilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      751 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/isfundamental
+-rw-r--r--   0 nmd      (444129884) staff       (20)      479 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ispolygonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1303 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ispower
+-rw-r--r--   0 nmd      (444129884) staff       (20)      484 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ispowerful
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2465 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/isprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      471 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/isprimepower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1776 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ispseudoprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      888 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ispseudoprimepower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1850 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/issquare
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1505 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/issquarefree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      442 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/istotient
+-rw-r--r--   0 nmd      (444129884) staff       (20)      758 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/kronecker
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1521 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/lcm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1024 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/logint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      192 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/moebius
+-rw-r--r--   0 nmd      (444129884) staff       (20)      893 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/nextprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      221 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/numdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      362 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/omega
+-rw-r--r--   0 nmd      (444129884) staff       (20)      914 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/precprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      464 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/prime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5402 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/primecert
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1687 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/primecertexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      994 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/primecertisvalid
+-rw-r--r--   0 nmd      (444129884) staff       (20)      508 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/primepi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      619 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/primes
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2868 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbclassno
+-rw-r--r--   0 nmd      (444129884) staff       (20)      275 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbcomp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      431 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbcompraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1323 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbcornacchia
+-rw-r--r--   0 nmd      (444129884) staff       (20)      508 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbhclassno
+-rw-r--r--   0 nmd      (444129884) staff       (20)      868 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbnucomp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      559 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbnupow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      263 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbpow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      337 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbpowraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      515 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbprimeform
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1039 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbred
+-rw-r--r--   0 nmd      (444129884) staff       (20)      578 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbredsl2
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2562 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/qfbsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2938 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadclassunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      540 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quaddisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      927 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadgen
+-rw-r--r--   0 nmd      (444129884) staff       (20)      577 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadhilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      630 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      612 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadray
+-rw-r--r--   0 nmd      (444129884) staff       (20)      527 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadregulator
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1507 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1236 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadunitindex
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1226 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/quadunitnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1855 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/ramanujantau
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1791 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/randomprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      476 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/removeprimes
+-rw-r--r--   0 nmd      (444129884) staff       (20)      467 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/sigma
+-rw-r--r--   0 nmd      (444129884) staff       (20)      859 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/sqrtint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      545 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/sqrtnint
+-rw-r--r--   0 nmd      (444129884) staff       (20)      329 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/sumdedekind
+-rw-r--r--   0 nmd      (444129884) staff       (20)      617 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/sumdigits
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1776 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)      668 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/zncharconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1217 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znchardecompose
+-rw-r--r--   0 nmd      (444129884) staff       (20)      856 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znchargauss
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1767 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/zncharinduce
+-rw-r--r--   0 nmd      (444129884) staff       (20)      794 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/zncharisodd
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1261 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znchartokronecker
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1095 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znchartoprimitive
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2882 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znconreychar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1651 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znconreyconductor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1148 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znconreyexp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3025 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znconreylog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3323 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/zncoppersmith
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2804 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znlog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      651 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znorder
+-rw-r--r--   0 nmd      (444129884) staff       (20)      703 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znprimroot
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1479 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znstar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3232 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/number_theoretical/znsubgroupgenerators
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.631585 cypari-2.5.4/pari_src/src/functions/operators/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14124 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/functions/operators/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1381 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/cmp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1121 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/divrem
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1060 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/operators/lex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      549 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/max
+-rw-r--r--   0 nmd      (444129884) staff       (20)      549 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/min
+-rw-r--r--   0 nmd      (444129884) staff       (20)      550 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/shift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      425 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/shiftmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      371 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/sign
+-rw-r--r--   0 nmd      (444129884) staff       (20)      903 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/vecmax
+-rw-r--r--   0 nmd      (444129884) staff       (20)      905 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/operators/vecmin
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.662455 cypari-2.5.4/pari_src/src/functions/polynomials/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      364 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      864 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/O
+-rw-r--r--   0 nmd      (444129884) staff       (20)      215 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/bezoutres
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1543 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/deriv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1528 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/derivn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1968 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/diffop
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1572 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/eval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1492 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/factorpadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)      854 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/fft
+-rw-r--r--   0 nmd      (444129884) staff       (20)      935 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/fftinv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1397 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/intformal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      993 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/padicappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1839 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/padicfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1227 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polchebyshev
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4403 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polclass
+-rw-r--r--   0 nmd      (444129884) staff       (20)      953 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polcoef
+-rw-r--r--   0 nmd      (444129884) staff       (20)      415 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polcoeff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      896 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      912 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polcyclofactors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      739 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poldegree
+-rw-r--r--   0 nmd      (444129884) staff       (20)      761 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1388 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poldiscfactors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      528 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poldiscreduced
+-rw-r--r--   0 nmd      (444129884) staff       (20)      251 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polgraeffe
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1133 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polhensellift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      948 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polhermite
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4330 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polinterpolate
+-rw-r--r--   0 nmd      (444129884) staff       (20)      437 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poliscyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      497 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poliscycloprod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      461 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polisirreducible
+-rw-r--r--   0 nmd      (444129884) staff       (20)      749 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/pollaguerre
+-rw-r--r--   0 nmd      (444129884) staff       (20)      610 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/pollead
+-rw-r--r--   0 nmd      (444129884) staff       (20)      714 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/pollegendre
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1716 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polmodular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      389 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrecip
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2275 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polresultant
+-rw-r--r--   0 nmd      (444129884) staff       (20)      827 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polresultantext
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1168 2021-04-30 16:18:22.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polroots
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1173 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrootsbound
+-rw-r--r--   0 nmd      (444129884) staff       (20)      218 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrootsff
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1148 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrootsmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1731 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrootspadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1835 2021-04-30 16:18:22.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polrootsreal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1651 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polsturm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1358 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polsubcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2312 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polsubcyclofast
+-rw-r--r--   0 nmd      (444129884) staff       (20)      654 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polsylvestermatrix
+-rw-r--r--   0 nmd      (444129884) staff       (20)      285 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polsym
+-rw-r--r--   0 nmd      (444129884) staff       (20)      206 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poltchebi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1123 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polteichmuller
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1233 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/poltomonic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1020 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/polzagier
+-rw-r--r--   0 nmd      (444129884) staff       (20)      817 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/seralgdep
+-rw-r--r--   0 nmd      (444129884) staff       (20)      333 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/serconvol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1033 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/serdiffdep
+-rw-r--r--   0 nmd      (444129884) staff       (20)      346 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/serlaplace
+-rw-r--r--   0 nmd      (444129884) staff       (20)      398 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/serreverse
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1156 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/subst
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1103 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/substpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      946 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/polynomials/substvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1040 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/sumformal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      702 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/polynomials/taylor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3201 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/thue
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3720 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/polynomials/thueinit
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.699641 cypari-2.5.4/pari_src/src/functions/programming/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2352 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      136 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/_eval_mnemonic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1110 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/addhelp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2255 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/alarm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1839 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/alias
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4578 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/allocatemem
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1787 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/apply
+-rw-r--r--   0 nmd      (444129884) staff       (20)      414 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/arity
+-rw-r--r--   0 nmd      (444129884) staff       (20)      490 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/break
+-rw-r--r--   0 nmd      (444129884) staff       (20)      685 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/breakpoint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1541 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/call
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1469 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/dbg_down
+-rw-r--r--   0 nmd      (444129884) staff       (20)      697 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/dbg_err
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1499 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/dbg_up
+-rw-r--r--   0 nmd      (444129884) staff       (20)      470 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/dbg_x
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1795 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/default
+-rw-r--r--   0 nmd      (444129884) staff       (20)      399 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/errname
+-rw-r--r--   0 nmd      (444129884) staff       (20)      674 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/error
+-rw-r--r--   0 nmd      (444129884) staff       (20)      705 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/export
+-rw-r--r--   0 nmd      (444129884) staff       (20)      484 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/exportall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      391 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/extern
+-rw-r--r--   0 nmd      (444129884) staff       (20)      448 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/externstr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2156 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fileclose
+-rw-r--r--   0 nmd      (444129884) staff       (20)      670 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fileextern
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1174 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fileflush
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1512 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fileopen
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1126 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fileread
+-rw-r--r--   0 nmd      (444129884) staff       (20)      643 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/filereadstr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1931 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/filewrite
+-rw-r--r--   0 nmd      (444129884) staff       (20)      435 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/filewrite1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      722 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fold
+-rw-r--r--   0 nmd      (444129884) staff       (20)      499 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/for
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1492 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/forcomposite
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1115 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/fordiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1398 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/fordivfactored
+-rw-r--r--   0 nmd      (444129884) staff       (20)      410 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/foreach
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1239 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/forell
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2097 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/forfactored
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2625 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/forpart
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1355 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/forperm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2443 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/forprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2143 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/forprimestep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3453 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/forsquarefree
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1251 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/forstep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2061 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/forsubgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1900 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/forsubset
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1780 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/forvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      424 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/getabstime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      252 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/getenv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      377 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/getheap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      221 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/getlocalbitprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      243 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/getlocalprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      442 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/getrand
+-rw-r--r--   0 nmd      (444129884) staff       (20)      285 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/getstack
+-rw-r--r--   0 nmd      (444129884) staff       (20)      460 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/gettime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      352 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/getwalltime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      186 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/global
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2391 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/if
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10240 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/iferr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      542 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/inline
+-rw-r--r--   0 nmd      (444129884) staff       (20)      746 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/input
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3591 2021-05-01 10:22:00.000000 cypari-2.5.4/pari_src/src/functions/programming/install
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1461 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/kill
+-rw-r--r--   0 nmd      (444129884) staff       (20)      400 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/listcreate
+-rw-r--r--   0 nmd      (444129884) staff       (20)      987 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/listinsert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      396 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/listkill
+-rw-r--r--   0 nmd      (444129884) staff       (20)      835 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/listpop
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1495 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/listput
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1200 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/listsort
+-rw-r--r--   0 nmd      (444129884) staff       (20)      125 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/local
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2712 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/localbitprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2248 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/localprec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      296 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/mapdelete
+-rw-r--r--   0 nmd      (444129884) staff       (20)      515 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/mapget
+-rw-r--r--   0 nmd      (444129884) staff       (20)      914 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/mapisdefined
+-rw-r--r--   0 nmd      (444129884) staff       (20)      460 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/mapput
+-rw-r--r--   0 nmd      (444129884) staff       (20)      115 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/my
+-rw-r--r--   0 nmd      (444129884) staff       (20)      521 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/next
+-rw-r--r--   0 nmd      (444129884) staff       (20)      805 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parapply
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1647 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/pareval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3338 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parfor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1421 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parforeach
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1756 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parforprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1650 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parforprimestep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1369 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parforvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2709 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parploth
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1551 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parplothexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      759 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/parselect
+-rw-r--r--   0 nmd      (444129884) staff       (20)      720 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/parsum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      744 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/parvector
+-rw-r--r--   0 nmd      (444129884) staff       (20)      534 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/print
+-rw-r--r--   0 nmd      (444129884) staff       (20)      513 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/print1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7804 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/printf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      556 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/printp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      459 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/printsep
+-rw-r--r--   0 nmd      (444129884) staff       (20)      491 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/printsep1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      709 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/printtex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      446 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/quit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1071 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/read
+-rw-r--r--   0 nmd      (444129884) staff       (20)      384 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/readstr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      967 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/readvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      287 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/return
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2793 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/select
+-rw-r--r--   0 nmd      (444129884) staff       (20)      464 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/self
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1235 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/setdebug
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1179 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/setrand
+-rw-r--r--   0 nmd      (444129884) staff       (20)      720 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strchr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      907 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strexpand
+-rw-r--r--   0 nmd      (444129884) staff       (20)      404 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strjoin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      751 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/strprintf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      746 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strsplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1704 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strtex
+-rw-r--r--   0 nmd      (444129884) staff       (20)      507 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/strtime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      708 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/programming/system
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2339 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/trap
+-rw-r--r--   0 nmd      (444129884) staff       (20)      608 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/type
+-rw-r--r--   0 nmd      (444129884) staff       (20)      254 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/unexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)      232 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/unexportall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      248 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/uninline
+-rw-r--r--   0 nmd      (444129884) staff       (20)      421 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/until
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2381 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/version
+-rw-r--r--   0 nmd      (444129884) staff       (20)      510 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/warning
+-rw-r--r--   0 nmd      (444129884) staff       (20)      932 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/whatnow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      394 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/while
+-rw-r--r--   0 nmd      (444129884) staff       (20)      618 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/write
+-rw-r--r--   0 nmd      (444129884) staff       (20)      313 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/write1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1973 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/programming/writebin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      393 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/programming/writetex
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.711513 cypari-2.5.4/pari_src/src/functions/sums/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5655 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/sums/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3274 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/asympnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2034 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/asympnumraw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      538 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/contfraceval
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1098 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/contfracinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2415 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/derivnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      853 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/intcirc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3368 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/intfuncinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14164 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/sums/intnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1452 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/intnumgauss
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2012 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/intnumgaussinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2505 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/intnuminit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7144 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/sums/intnumosc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3109 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/intnumromb
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1901 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/laurentseries
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6611 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/limitnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1432 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/prod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1164 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/prodeuler
+-rw-r--r--   0 nmd      (444129884) staff       (20)      458 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/prodeulerrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      958 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/prodinf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      390 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/prodnumrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1166 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/sums/solve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1254 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/solvestep
+-rw-r--r--   0 nmd      (444129884) staff       (20)      612 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3323 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumalt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      447 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      557 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumdivmult
+-rw-r--r--   0 nmd      (444129884) staff       (20)      447 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumeulerrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2260 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/suminf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5956 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5281 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1056 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumapinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      999 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnuminit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1970 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumlagrange
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2330 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumlagrangeinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      959 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnummonien
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3184 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnummonieninit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      830 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1443 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/sums/sumnumsidi
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2981 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/sums/sumpos
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.727368 cypari-2.5.4/pari_src/src/functions/symbolic_operators/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1286 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/add
+-rw-r--r--   0 nmd      (444129884) staff       (20)      892 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/adde
+-rw-r--r--   0 nmd      (444129884) staff       (20)      175 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/and
+-rw-r--r--   0 nmd      (444129884) staff       (20)      312 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/call
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1213 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/coeff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      720 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/compr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      330 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/concat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      433 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/deriv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1134 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/div
+-rw-r--r--   0 nmd      (444129884) staff       (20)      742 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/dive
+-rw-r--r--   0 nmd      (444129884) staff       (20)      530 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/divent
+-rw-r--r--   0 nmd      (444129884) staff       (20)      385 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/divente
+-rw-r--r--   0 nmd      (444129884) staff       (20)      253 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/divround
+-rw-r--r--   0 nmd      (444129884) staff       (20)      337 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/divrounde
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1404 2021-01-04 12:48:54.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/eq
+-rw-r--r--   0 nmd      (444129884) staff       (20)      155 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/fact
+-rw-r--r--   0 nmd      (444129884) staff       (20)      790 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/ge
+-rw-r--r--   0 nmd      (444129884) staff       (20)      781 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/gt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      226 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/hist
+-rw-r--r--   0 nmd      (444129884) staff       (20)      139 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/id
+-rw-r--r--   0 nmd      (444129884) staff       (20)      846 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/le
+-rw-r--r--   0 nmd      (444129884) staff       (20)      778 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/lt
+-rw-r--r--   0 nmd      (444129884) staff       (20)      531 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/mm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      566 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/mod
+-rw-r--r--   0 nmd      (444129884) staff       (20)      476 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/mode
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2111 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/mul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      839 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/mule
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1183 2021-01-04 12:48:54.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/ne
+-rw-r--r--   0 nmd      (444129884) staff       (20)      426 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/neg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      196 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/not
+-rw-r--r--   0 nmd      (444129884) staff       (20)      185 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/or
+-rw-r--r--   0 nmd      (444129884) staff       (20)      323 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/pl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      276 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/pound
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1647 2021-05-01 10:20:18.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/pow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      547 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/pp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      195 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/range
+-rw-r--r--   0 nmd      (444129884) staff       (20)      259 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/shiftl
+-rw-r--r--   0 nmd      (444129884) staff       (20)      363 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/shiftle
+-rw-r--r--   0 nmd      (444129884) staff       (20)      322 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/shiftr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      372 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/shiftre
+-rw-r--r--   0 nmd      (444129884) staff       (20)      440 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/slice
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1152 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/sub
+-rw-r--r--   0 nmd      (444129884) staff       (20)      892 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/sube
+-rw-r--r--   0 nmd      (444129884) staff       (20)      198 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/symbolic_operators/trans
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.763968 cypari-2.5.4/pari_src/src/functions/transcendental/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      371 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/Catalan
+-rw-r--r--   0 nmd      (444129884) staff       (20)      324 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/Euler
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5610 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/HEADER
+-rw-r--r--   0 nmd      (444129884) staff       (20)      143 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/I
+-rw-r--r--   0 nmd      (444129884) staff       (20)      302 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/Pi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      842 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/abs
+-rw-r--r--   0 nmd      (444129884) staff       (20)      477 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/acos
+-rw-r--r--   0 nmd      (444129884) staff       (20)      351 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/acosh
+-rw-r--r--   0 nmd      (444129884) staff       (20)      526 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/agm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      313 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/airy
+-rw-r--r--   0 nmd      (444129884) staff       (20)      197 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/arg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      479 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/asin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      373 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/asinh
+-rw-r--r--   0 nmd      (444129884) staff       (20)      470 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/atan
+-rw-r--r--   0 nmd      (444129884) staff       (20)      336 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/atanh
+-rw-r--r--   0 nmd      (444129884) staff       (20)      208 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besselh1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      208 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besselh2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      364 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besseli
+-rw-r--r--   0 nmd      (444129884) staff       (20)      364 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besselj
+-rw-r--r--   0 nmd      (444129884) staff       (20)      445 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besseljh
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1097 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besseljzero
+-rw-r--r--   0 nmd      (444129884) staff       (20)      201 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besselk
+-rw-r--r--   0 nmd      (444129884) staff       (20)      186 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besseln
+-rw-r--r--   0 nmd      (444129884) staff       (20)      201 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/bessely
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1081 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/besselyzero
+-rw-r--r--   0 nmd      (444129884) staff       (20)      568 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/cos
+-rw-r--r--   0 nmd      (444129884) staff       (20)      226 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/cosh
+-rw-r--r--   0 nmd      (444129884) staff       (20)      215 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/cotan
+-rw-r--r--   0 nmd      (444129884) staff       (20)      242 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/cotanh
+-rw-r--r--   0 nmd      (444129884) staff       (20)      238 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/dilog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1233 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/eint1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      514 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/ellE
+-rw-r--r--   0 nmd      (444129884) staff       (20)      318 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/ellK
+-rw-r--r--   0 nmd      (444129884) staff       (20)      795 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/functions/transcendental/erfc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1104 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/eta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      389 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/exp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      994 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/expm1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1234 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/gamma
+-rw-r--r--   0 nmd      (444129884) staff       (20)      171 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/gammah
+-rw-r--r--   0 nmd      (444129884) staff       (20)      693 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/gammamellininv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1152 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/gammamellininvasymp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1636 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/gammamellininvinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3372 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/hypergeom
+-rw-r--r--   0 nmd      (444129884) staff       (20)      407 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/hyperu
+-rw-r--r--   0 nmd      (444129884) staff       (20)      626 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/incgam
+-rw-r--r--   0 nmd      (444129884) staff       (20)      409 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/incgamc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      940 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/lambertw
+-rw-r--r--   0 nmd      (444129884) staff       (20)      335 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/lerchphi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      532 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/lerchzeta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1577 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/functions/transcendental/lngamma
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1086 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/log
+-rw-r--r--   0 nmd      (444129884) staff       (20)      881 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/log1p
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1600 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/polylog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1965 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/polylogmult
+-rw-r--r--   0 nmd      (444129884) staff       (20)      188 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/psi
+-rw-r--r--   0 nmd      (444129884) staff       (20)      540 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/rootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      564 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      385 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sinc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      222 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sinh
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1017 2021-05-01 10:20:18.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sqr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      820 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sqrt
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1523 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/sqrtn
+-rw-r--r--   0 nmd      (444129884) staff       (20)      201 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/tan
+-rw-r--r--   0 nmd      (444129884) staff       (20)      228 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/tanh
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2369 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/teichmuller
+-rw-r--r--   0 nmd      (444129884) staff       (20)      227 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/theta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      476 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/thetanullk
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1064 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/weber
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1325 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zeta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1573 2020-03-27 14:32:39.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zetahurwitz
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1750 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zetamult
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2985 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zetamultall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      946 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zetamultconvert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      839 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/functions/transcendental/zetamultdual
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.767153 cypari-2.5.4/pari_src/src/gp/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1124 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/gp/emacs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18283 2022-11-05 17:44:17.000000 cypari-2.5.4/pari_src/src/gp/gp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1525 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/gp/gp.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      937 2022-12-21 20:26:52.000000 cypari-2.5.4/pari_src/src/gp/gp_init.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12831 2022-03-01 15:27:29.000000 cypari-2.5.4/pari_src/src/gp/gp_rl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6075 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/gp/texmacs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2307 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/gp/whatnow.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21306 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/gp/whatnow.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.772214 cypari-2.5.4/pari_src/src/graph/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10300 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/plotQt4.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3719 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/plotWin32.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8303 2022-03-01 15:12:50.000000 cypari-2.5.4/pari_src/src/graph/plotX.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4561 2022-03-01 15:12:50.000000 cypari-2.5.4/pari_src/src/graph/plotfltk.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1037 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/plotnone.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    85805 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/graph/plotport.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1320 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/plotps.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1230 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/graph/plotsvg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4473 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/plottty.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5598 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/graph/rect.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.779081 cypari-2.5.4/pari_src/src/headers/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1464 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/pari.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1431 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/headers/paricast.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5430 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/paricom.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1845 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/paridbglvl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)   255702 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/headers/paridecl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1163 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/headers/parierr.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6069 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/headers/parigen.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    87108 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/headers/pariinl.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3260 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/parinf.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13558 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/pariold.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34396 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/paripriv.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9060 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/headers/paristio.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1797 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/headers/parisys.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6915 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/headers/paritune.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.779566 cypari-2.5.4/pari_src/src/kernel/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1470 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/kernel/README
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.780127 cypari-2.5.4/pari_src/src/kernel/aarch64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4839 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/aarch64/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.781151 cypari-2.5.4/pari_src/src/kernel/alpha/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2611 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/alpha/asm0.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3666 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/alpha/asm1.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.781608 cypari-2.5.4/pari_src/src/kernel/arm/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2590 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/arm/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.784609 cypari-2.5.4/pari_src/src/kernel/gmp/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      544 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/gmp/MakeLVL1.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2234 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/gmp/gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5181 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/gmp/gcdext.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1469 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/gmp/int.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34831 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/gmp/mp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6406 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/kernel/gmp/tune.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.785106 cypari-2.5.4/pari_src/src/kernel/hppa/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2885 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/hppa/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.785547 cypari-2.5.4/pari_src/src/kernel/hppa64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4152 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/hppa64/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.786485 cypari-2.5.4/pari_src/src/kernel/ia64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2761 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/ia64/asm0.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2079 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/ia64/asm1.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.786963 cypari-2.5.4/pari_src/src/kernel/ix86/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5284 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/ix86/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.787469 cypari-2.5.4/pari_src/src/kernel/m68k/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5183 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/m68k/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.787923 cypari-2.5.4/pari_src/src/kernel/mips/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3108 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/mips/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.788412 cypari-2.5.4/pari_src/src/kernel/mips64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3130 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/mips64/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.799860 cypari-2.5.4/pari_src/src/kernel/none/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      528 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/MakeLVL1.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8120 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/add.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3259 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/addll.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)      681 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/asm0.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2079 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/bfffo.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3695 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/cmp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7002 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/divll.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4002 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/divll_pre.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3697 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/gcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7117 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/gcdext.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    33858 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/gcdll.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8359 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/halfgcd.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1487 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/int.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4169 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/invmod.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    39338 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/kernel/none/level1.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    54318 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/mp.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    24223 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/mp_indep.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      787 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/mpinl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4119 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/none/mulll.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10794 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/ratlift.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4393 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/tune-gen.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6452 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/none/tune.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.800383 cypari-2.5.4/pari_src/src/kernel/ppc/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2635 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/ppc/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.800919 cypari-2.5.4/pari_src/src/kernel/ppc64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2635 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/ppc64/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.802549 cypari-2.5.4/pari_src/src/kernel/sparcv8_micro/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      132 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/kernel/sparcv8_micro/MakeLVL0.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2619 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/sparcv8_micro/asm0-common.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1037 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/kernel/sparcv8_micro/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.803600 cypari-2.5.4/pari_src/src/kernel/sparcv8_super/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      170 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/kernel/sparcv8_super/MakeLVL0.SH
+-rw-r--r--   0 nmd      (444129884) staff       (20)       18 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/kernel/sparcv8_super/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.804104 cypari-2.5.4/pari_src/src/kernel/x86_64/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5019 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/kernel/x86_64/asm0.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.816568 cypari-2.5.4/pari_src/src/language/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    30388 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/language/anal.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1797 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/anal.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    63219 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/compile.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    25693 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/default.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2277 2022-12-21 20:26:50.000000 cypari-2.5.4/pari_src/src/language/default.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)   132270 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/language/es.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    70453 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/eval.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34105 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/forprime.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    54341 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/gplib.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9331 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/hash.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    79490 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/init.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   250970 2022-12-21 20:26:50.000000 cypari-2.5.4/pari_src/src/language/init.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    79417 2022-12-21 17:53:50.000000 cypari-2.5.4/pari_src/src/language/intnum.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13207 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/members.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1804 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/opcode.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1022 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/paricfg.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      756 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/pariinl.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)   105509 2022-09-19 15:45:34.000000 cypari-2.5.4/pari_src/src/language/parse.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4510 2022-09-19 15:45:34.000000 cypari-2.5.4/pari_src/src/language/parse.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9234 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/parse.y
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5095 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/parsec.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11991 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/readline.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5327 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/language/str.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    58050 2022-11-01 08:37:35.000000 cypari-2.5.4/pari_src/src/language/sumiter.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1764 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/language/tree.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.825323 cypari-2.5.4/pari_src/src/modules/
+-rw-r--r--   0 nmd      (444129884) staff       (20)   133829 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/algebras.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7254 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/elldata.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9909 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/modules/ellfromeqn.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1960 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/modules/forperm.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2335 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/modules/forsubset.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    74091 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/galois.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3309 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/galpol.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    68348 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/genus2red.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21015 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/groupid.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    26208 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/krasner.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    63742 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/mpqs.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17279 2022-03-03 16:35:26.000000 cypari-2.5.4/pari_src/src/modules/mpqs.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11349 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/modules/part.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    57680 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/ratpoints.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    93399 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/modules/stark.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    49423 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/modules/thue.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.829454 cypari-2.5.4/pari_src/src/mt/
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11595 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/mt/mpi.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      709 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/mt/mpi.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3421 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/mt/mt.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      912 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/mt/mt.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     9227 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/mt/pthread.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      805 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/mt/pthread.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1626 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/mt/single.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      709 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/mt/single.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:15.350394 cypari-2.5.4/pari_src/src/systems/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.829945 cypari-2.5.4/pari_src/src/systems/cygwin/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      949 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/cygwin/cygwin.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.830911 cypari-2.5.4/pari_src/src/systems/darwin/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6269 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/systems/darwin/darwin.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2295 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/systems/darwin/dlfcn.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.831869 cypari-2.5.4/pari_src/src/systems/emscripten/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2661 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/emscripten/emscripten.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      808 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/emscripten/emscripten.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.833284 cypari-2.5.4/pari_src/src/systems/mingw/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5181 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/mingw/mingw.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      967 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/mingw/mingw.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)       21 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/systems/mingw/pwinver.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.835298 cypari-2.5.4/pari_src/src/systems/os2/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2163 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/systems/os2/README
+-rw-r--r--   0 nmd      (444129884) staff       (20)      140 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/systems/os2/dlfcn.h
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4747 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/systems/os2/os2.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)      257 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/systems/os2/pari.def.base
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.836309 cypari-2.5.4/pari_src/src/systems/win32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3169 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/systems/win32/README.MSVC
+-rw-r--r--   0 nmd      (444129884) staff       (20)      173 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/systems/win32/pariinl.h
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.838263 cypari-2.5.4/pari_src/src/test/
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:16.938439 cypari-2.5.4/pari_src/src/test/32/
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1310 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/addprimes
+-rw-r--r--   0 nmd      (444129884) staff       (20)      425 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/agm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    81351 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/algebras
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3722 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/alggroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4758 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/alghasse
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5072 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/alglattices
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1612 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/algsplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      221 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/analyz
+-rw-r--r--   0 nmd      (444129884) staff       (20)      350 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/apply
+-rw-r--r--   0 nmd      (444129884) staff       (20)       36 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/test/32/arith
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2110 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/asymp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      203 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/test/32/aurifeuille
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5617 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/bbhnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3611 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bern
+-rw-r--r--   0 nmd      (444129884) staff       (20)    49342 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bessel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      411 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/bestappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      593 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/binomial
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7658 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/bit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6278 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/test/32/bnfinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5028 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/bnfisintnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      734 2021-04-28 15:06:30.000000 cypari-2.5.4/pari_src/src/test/32/bnflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1465 2021-05-23 11:12:30.000000 cypari-2.5.4/pari_src/src/test/32/bnfsunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2793 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bnr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3903 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/bnrL1
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15594 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bnrclassfield
+-rw-r--r--   0 nmd      (444129884) staff       (20)      802 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bnrisgalois
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1512 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/bnrmap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1438 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/character
+-rw-r--r--   0 nmd      (444129884) staff       (20)      416 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/characteristic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8161 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/charpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      296 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/chinese
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/classpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      611 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/cmp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4807 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/combinat
+-rw-r--r--   0 nmd      (444129884) staff       (20)   162655 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/compat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1388 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/concat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1279 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/content
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1039 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/contfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)      546 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/cxtrigo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1821 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/cyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4056 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/debugger
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4595 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/deriv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      432 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/32/det
+-rw-r--r--   0 nmd      (444129884) staff       (20)      510 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/diffop
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2122 2022-12-05 19:59:16.000000 cypari-2.5.4/pari_src/src/test/32/digits
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1041 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/dirmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      520 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/dirpowers
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2333 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/disc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29156 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/div
+-rw-r--r--   0 nmd      (444129884) staff       (20)      571 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/divisors
+-rw-r--r--   0 nmd      (444129884) staff       (20)    36653 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/ell
+-rw-r--r--   0 nmd      (444129884) staff       (20)      983 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellanal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      253 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/ellff
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1120 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellglobalred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5136 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/elliptic
+-rw-r--r--   0 nmd      (444129884) staff       (20)      414 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/ellisogeny
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8652 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellisomat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      130 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/ellissupersingular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      789 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/ellmodulareqn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8488 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3128 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellpadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1590 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellpadiclambdamu
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5006 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1200 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)      889 2020-04-08 20:04:14.000000 cypari-2.5.4/pari_src/src/test/32/ellsea
+-rw-r--r--   0 nmd      (444129884) staff       (20)      126 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ellseaJ
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4446 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/elltors
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7022 2020-02-12 10:36:35.000000 cypari-2.5.4/pari_src/src/test/32/ellweilpairing
+-rw-r--r--   0 nmd      (444129884) staff       (20)       54 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/env
+-rw-r--r--   0 nmd      (444129884) staff       (20)      732 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/equal
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29124 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/err
+-rw-r--r--   0 nmd      (444129884) staff       (20)       40 2020-06-22 16:11:40.000000 cypari-2.5.4/pari_src/src/test/32/eval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      679 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/test/32/exact0
+-rw-r--r--   0 nmd      (444129884) staff       (20)      594 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/export
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10641 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/extract
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7264 2022-12-05 20:28:57.000000 cypari-2.5.4/pari_src/src/test/32/factor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5296 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/factorff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      701 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/factorint
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16191 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/factormod
+-rw-r--r--   0 nmd      (444129884) staff       (20)    19616 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      243 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/ffisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)      684 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/fflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      445 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/fft
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4539 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/forperm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      444 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/forsubset
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1607 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/forvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6499 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/galois
+-rw-r--r--   0 nmd      (444129884) staff       (20)      964 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/galoischartable
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7517 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/galoisinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1371 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/galpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8433 2021-01-04 12:28:09.000000 cypari-2.5.4/pari_src/src/test/32/gamma
+-rw-r--r--   0 nmd      (444129884) staff       (20)      736 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/gammamellininv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6717 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/gcdext
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10724 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/gchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)      263 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/gchar-large
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2676 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/gchar-lfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)    42879 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/genus2red
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/gp
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2849 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/graph
+-rw-r--r--   0 nmd      (444129884) staff       (20)      321 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/harmonic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6429 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/help
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8291 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/hgm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      378 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/history
+-rw-r--r--   0 nmd      (444129884) staff       (20)    41221 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/hyperell
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1349 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/hyperelldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4765 2022-11-16 09:36:04.000000 cypari-2.5.4/pari_src/src/test/32/hypergeom
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5531 2022-12-23 16:01:53.000000 cypari-2.5.4/pari_src/src/test/32/ideal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      214 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/idealappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      888 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/idealramgroups
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2510 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/incgam
+-rw-r--r--   0 nmd      (444129884) staff       (20)      311 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/install
+-rw-r--r--   0 nmd      (444129884) staff       (20)      423 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/interpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6789 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/intnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      324 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/intnumosc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2273 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/io
+-rw-r--r--   0 nmd      (444129884) staff       (20)    11816 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/ispower
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20788 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/isprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3693 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/32/iterator
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1418 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/kernel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8251 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/krasner
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7519 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/test/32/lambert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      247 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/32/language
+-rw-r--r--   0 nmd      (444129884) staff       (20)      586 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/lerch
+-rw-r--r--   0 nmd      (444129884) staff       (20)      442 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/lex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16900 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/lfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/lfunartin
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29667 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/lfunquad
+-rw-r--r--   0 nmd      (444129884) staff       (20)    38201 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/lfuntype
+-rw-r--r--   0 nmd      (444129884) staff       (20)      792 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/lift
+-rw-r--r--   0 nmd      (444129884) staff       (20)      908 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/32/lindep
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16338 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/linear
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1376 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/32/list
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2241 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/lll
+-rw-r--r--   0 nmd      (444129884) staff       (20)      162 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/log
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1152 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/logint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2239 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/map
+-rw-r--r--   0 nmd      (444129884) staff       (20)    17615 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/mat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3898 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/32/mathnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      836 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/matpermanent
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8059 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/matsnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12788 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/member
+-rw-r--r--   0 nmd      (444129884) staff       (20)      301 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/memory
+-rw-r--r--   0 nmd      (444129884) staff       (20)    79616 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/mf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      635 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/mfgaloisrep
+-rw-r--r--   0 nmd      (444129884) staff       (20)       35 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/minim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      100 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/test/32/minmax
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3298 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/32/modfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/modpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4281 2022-03-03 14:05:24.000000 cypari-2.5.4/pari_src/src/test/32/modpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18197 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/modsym
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3943 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/modular
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7202 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/mscosets
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15317 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/mspadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5896 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/mspolygon
+-rw-r--r--   0 nmd      (444129884) staff       (20)       96 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/multiif
+-rw-r--r--   0 nmd      (444129884) staff       (20)       23 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/multivar-mul
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12500 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6623 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/nfcompositum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      153 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/nfdiscfactors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      825 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/nfeltembed
+-rw-r--r--   0 nmd      (444129884) staff       (20)      576 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/nfeltsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)    52116 2022-03-03 14:06:11.000000 cypari-2.5.4/pari_src/src/test/32/nffactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3961 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/nfhilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)    29673 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)      360 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/nfislocalpower
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20523 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nflist
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5707 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nflistA5
+-rw-r--r--   0 nmd      (444129884) staff       (20)      756 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nflistQT
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2124 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nflistQTall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      687 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/nfpolsturm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      123 2022-12-05 20:29:05.000000 cypari-2.5.4/pari_src/src/test/32/nfrootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/nfsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4718 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/nfsplitting
+-rw-r--r--   0 nmd      (444129884) staff       (20)      976 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/norm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5997 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/number
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2165 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/objets
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/op
+-rw-r--r--   0 nmd      (444129884) staff       (20)      895 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/orthopol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5462 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/padic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2557 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/parallel
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4361 2018-05-01 12:01:20.000000 cypari-2.5.4/pari_src/src/test/32/partition
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2022 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/perm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      457 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/plotexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12436 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/32/ploth
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6094 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/32/pol
+-rw-r--r--   0 nmd      (444129884) staff       (20)      111 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/polclass
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3959 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/polmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)       84 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/polmodular
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4796 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/test/32/polred
+-rw-r--r--   0 nmd      (444129884) staff       (20)        0 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/test/32/polygonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1374 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/polylog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6320 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/polyser
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3062 2022-12-21 17:56:02.000000 cypari-2.5.4/pari_src/src/test/32/pow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      787 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/prec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1411 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/prime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      145 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/print
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12115 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/printf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2366 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/program
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6031 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/programming
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1951 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/qf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3304 2022-10-31 21:05:51.000000 cypari-2.5.4/pari_src/src/test/32/qfb
+-rw-r--r--   0 nmd      (444129884) staff       (20)      420 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/qfbclassno
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8314 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/qfbsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      667 2021-05-21 11:46:52.000000 cypari-2.5.4/pari_src/src/test/32/qfisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1636 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/qfsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1259 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/32/quad
+-rw-r--r--   0 nmd      (444129884) staff       (20)    20542 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/quadclassunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      747 2020-03-25 11:58:26.000000 cypari-2.5.4/pari_src/src/test/32/quaddisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)    84435 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/quadray
+-rw-r--r--   0 nmd      (444129884) staff       (20)      421 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ramanujantau
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1740 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/random
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2408 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/ranges
+-rw-r--r--   0 nmd      (444129884) staff       (20)    21219 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)      401 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/real
+-rw-r--r--   0 nmd      (444129884) staff       (20)    31613 2022-03-01 15:12:50.000000 cypari-2.5.4/pari_src/src/test/32/resultant
+-rw-r--r--   0 nmd      (444129884) staff       (20)      278 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/32/rfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)    34702 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/rnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      767 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/rnfkummer
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1043 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/rootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2962 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/32/rootsreal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1511 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/round
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16903 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/round4
+-rw-r--r--   0 nmd      (444129884) staff       (20)      425 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/select
+-rw-r--r--   0 nmd      (444129884) staff       (20)       24 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/self
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6481 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/ser
+-rw-r--r--   0 nmd      (444129884) staff       (20)      535 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/set
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1500 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/setdebug
+-rw-r--r--   0 nmd      (444129884) staff       (20)      180 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/size
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1862 2022-11-01 08:37:35.000000 cypari-2.5.4/pari_src/src/test/32/solve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1157 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/32/sort
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3402 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/sqrtn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7030 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/stark
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1333 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/str
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5104 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/subcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3819 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/subcyclopclgp
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15060 2021-06-09 10:39:44.000000 cypari-2.5.4/pari_src/src/test/32/subfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1078 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/subgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1724 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/subst
+-rw-r--r--   0 nmd      (444129884) staff       (20)      108 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/32/sumdedekind
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1832 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/32/sumdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      261 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/test/32/sumformal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1233 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/sumiter
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3162 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/sumnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2800 2022-12-21 17:53:36.000000 cypari-2.5.4/pari_src/src/test/32/sumnumrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1456 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/thue
+-rw-r--r--   0 nmd      (444129884) staff       (20)       28 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/time
+-rw-r--r--   0 nmd      (444129884) staff       (20)    27913 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/32/trans
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6476 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/trans2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      950 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/valuation
+-rw-r--r--   0 nmd      (444129884) staff       (20)      889 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/vararg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      369 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/32/variable
+-rw-r--r--   0 nmd      (444129884) staff       (20)       31 2022-11-05 13:53:53.000000 cypari-2.5.4/pari_src/src/test/32/version
+-rw-r--r--   0 nmd      (444129884) staff       (20)      659 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/32/whatnow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2168 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/zeta
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4476 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/zetahurwitz
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13588 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/zetamult
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6917 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/32/zn
+-rw-r--r--   0 nmd      (444129884) staff       (20)      653 2020-02-13 13:00:46.000000 cypari-2.5.4/pari_src/src/test/32/zncoppersmith
+-rwxr-xr-x   0 nmd      (444129884) staff       (20)     3835 2022-11-18 15:22:22.000000 cypari-2.5.4/pari_src/src/test/dotest
+-rw-r--r--   0 nmd      (444129884) staff       (20)      492 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/dummy.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:17.004817 cypari-2.5.4/pari_src/src/test/in/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      607 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/addprimes
+-rw-r--r--   0 nmd      (444129884) staff       (20)      477 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/agm
+-rw-r--r--   0 nmd      (444129884) staff       (20)    84267 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/algebras
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3034 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/alggroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8006 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/alghasse
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8987 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/alglattices
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5039 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/algsplit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      211 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/analyz
+-rw-r--r--   0 nmd      (444129884) staff       (20)      633 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/apply
+-rw-r--r--   0 nmd      (444129884) staff       (20)      200 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/arith
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1500 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/asymp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      376 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/test/in/aurifeuille
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5108 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/bbhnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      986 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bern
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1762 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bessel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      639 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/bestappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      204 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/in/binomial
+-rw-r--r--   0 nmd      (444129884) staff       (20)      667 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/bit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4195 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      421 2014-03-25 08:59:21.000000 cypari-2.5.4/pari_src/src/test/in/bnfisintnorm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1480 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bnflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1334 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/bnfsunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3817 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bnr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      709 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/bnrL1
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10193 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/bnrclassfield
+-rw-r--r--   0 nmd      (444129884) staff       (20)      262 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/bnrisgalois
+-rw-r--r--   0 nmd      (444129884) staff       (20)      426 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/bnrmap
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1351 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/character
+-rw-r--r--   0 nmd      (444129884) staff       (20)      306 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/characteristic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4054 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/charpoly
+-rw-r--r--   0 nmd      (444129884) staff       (20)      300 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/chinese
+-rw-r--r--   0 nmd      (444129884) staff       (20)      599 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/cmp
+-rw-r--r--   0 nmd      (444129884) staff       (20)      370 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/combinat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4308 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/compat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      658 2021-06-09 11:37:13.000000 cypari-2.5.4/pari_src/src/test/in/concat
+-rw-r--r--   0 nmd      (444129884) staff       (20)      522 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/content
+-rw-r--r--   0 nmd      (444129884) staff       (20)      620 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/contfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1038 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/cxtrigo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      866 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/cyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)      611 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/debugger
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1210 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/deriv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1102 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/in/det
+-rw-r--r--   0 nmd      (444129884) staff       (20)      274 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/diffop
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1030 2022-12-05 19:59:16.000000 cypari-2.5.4/pari_src/src/test/in/digits
+-rw-r--r--   0 nmd      (444129884) staff       (20)      705 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/dirmul
+-rw-r--r--   0 nmd      (444129884) staff       (20)      344 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/dirpowers
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2808 2020-02-10 19:50:52.000000 cypari-2.5.4/pari_src/src/test/in/disc
+-rw-r--r--   0 nmd      (444129884) staff       (20)      898 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/in/div
+-rw-r--r--   0 nmd      (444129884) staff       (20)      465 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/divisors
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14055 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ell
+-rw-r--r--   0 nmd      (444129884) staff       (20)      994 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellanal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3458 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellff
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1038 2020-02-14 09:59:12.000000 cypari-2.5.4/pari_src/src/test/in/ellglobalred
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1220 2021-04-28 13:36:36.000000 cypari-2.5.4/pari_src/src/test/in/elliptic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8412 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/ellisogeny
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2173 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellisomat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1312 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellissupersingular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      123 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/ellmodulareqn
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6296 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2132 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/ellpadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2326 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellpadiclambdamu
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7279 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellrank
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1333 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2711 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellsea
+-rw-r--r--   0 nmd      (444129884) staff       (20)      185 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ellseaJ
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2663 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/elltors
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3928 2020-02-12 10:36:35.000000 cypari-2.5.4/pari_src/src/test/in/ellweilpairing
+-rw-r--r--   0 nmd      (444129884) staff       (20)      112 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/env
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1754 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/equal
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5804 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/err
+-rw-r--r--   0 nmd      (444129884) staff       (20)       47 2020-06-22 16:11:40.000000 cypari-2.5.4/pari_src/src/test/in/eval
+-rw-r--r--   0 nmd      (444129884) staff       (20)      596 2011-09-22 20:02:11.000000 cypari-2.5.4/pari_src/src/test/in/exact0
+-rw-r--r--   0 nmd      (444129884) staff       (20)      855 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/export
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1336 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/extract
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2398 2022-12-05 20:28:57.000000 cypari-2.5.4/pari_src/src/test/in/factor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2040 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/factorff
+-rw-r--r--   0 nmd      (444129884) staff       (20)      314 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/factorint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1801 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/factormod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4674 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ff
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5095 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/ffisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1038 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/fflog
+-rw-r--r--   0 nmd      (444129884) staff       (20)      508 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/fft
+-rw-r--r--   0 nmd      (444129884) staff       (20)      522 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/forperm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      618 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/forsubset
+-rw-r--r--   0 nmd      (444129884) staff       (20)      501 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/forvec
+-rw-r--r--   0 nmd      (444129884) staff       (20)     8591 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/galois
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1977 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/galoischartable
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5261 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/galoisinit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      620 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/galpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1198 2021-01-04 12:28:09.000000 cypari-2.5.4/pari_src/src/test/in/gamma
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2169 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/gammamellininv
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5503 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/gcdext
+-rw-r--r--   0 nmd      (444129884) staff       (20)    18415 2022-10-30 16:07:08.000000 cypari-2.5.4/pari_src/src/test/in/gchar
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1241 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/gchar-large
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10060 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/gchar-lfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16389 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/genus2red
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1027 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/graph
+-rw-r--r--   0 nmd      (444129884) staff       (20)      130 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/harmonic
+-rw-r--r--   0 nmd      (444129884) staff       (20)      279 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/help
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5213 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/hgm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      102 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/history
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2377 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/hyperell
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2865 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/hyperelldisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4810 2022-11-16 09:32:38.000000 cypari-2.5.4/pari_src/src/test/in/hypergeom
+-rw-r--r--   0 nmd      (444129884) staff       (20)    10612 2022-12-23 16:01:53.000000 cypari-2.5.4/pari_src/src/test/in/ideal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      197 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/idealappr
+-rw-r--r--   0 nmd      (444129884) staff       (20)      941 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/idealramgroups
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1000 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/incgam
+-rw-r--r--   0 nmd      (444129884) staff       (20)      199 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/install
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1691 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/interpol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4891 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/intnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      484 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/intnumosc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1252 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/io
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3603 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ispower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2400 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/isprime
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3045 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/in/iterator
+-rw-r--r--   0 nmd      (444129884) staff       (20)      569 2017-12-05 22:49:55.000000 cypari-2.5.4/pari_src/src/test/in/krasner
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1520 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/test/in/lambert
+-rw-r--r--   0 nmd      (444129884) staff       (20)      535 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/in/language
+-rw-r--r--   0 nmd      (444129884) staff       (20)      345 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/lerch
+-rw-r--r--   0 nmd      (444129884) staff       (20)      795 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/lex
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15084 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/test/in/lfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)      679 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/lfunartin
+-rw-r--r--   0 nmd      (444129884) staff       (20)      420 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/lfunquad
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3210 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/lfuntype
+-rw-r--r--   0 nmd      (444129884) staff       (20)      346 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/lift
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1128 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/in/lindep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2653 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/linear
+-rw-r--r--   0 nmd      (444129884) staff       (20)      916 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/list
+-rw-r--r--   0 nmd      (444129884) staff       (20)      786 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/lll
+-rw-r--r--   0 nmd      (444129884) staff       (20)       99 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/log
+-rw-r--r--   0 nmd      (444129884) staff       (20)      381 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/logint
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1629 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/map
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7749 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/mat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2525 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/in/mathnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)      505 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/matpermanent
+-rw-r--r--   0 nmd      (444129884) staff       (20)    14161 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/matsnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1621 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/member
+-rw-r--r--   0 nmd      (444129884) staff       (20)       63 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/memory
+-rw-r--r--   0 nmd      (444129884) staff       (20)    22570 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/mf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1063 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/mfgaloisrep
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4101 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/minim
+-rw-r--r--   0 nmd      (444129884) staff       (20)      191 2014-03-25 08:59:22.000000 cypari-2.5.4/pari_src/src/test/in/minmax
+-rw-r--r--   0 nmd      (444129884) staff       (20)      218 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/in/modfun
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1567 2022-03-03 14:05:24.000000 cypari-2.5.4/pari_src/src/test/in/modpr
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5785 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/modsym
+-rw-r--r--   0 nmd      (444129884) staff       (20)      842 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/modular
+-rw-r--r--   0 nmd      (444129884) staff       (20)      855 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/mscosets
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3571 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/mspadic
+-rw-r--r--   0 nmd      (444129884) staff       (20)      750 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/mspolygon
+-rw-r--r--   0 nmd      (444129884) staff       (20)      395 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/multiif
+-rw-r--r--   0 nmd      (444129884) staff       (20)      506 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/multivar-mul
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4595 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2373 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/nfcompositum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      102 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/nfdiscfactors
+-rw-r--r--   0 nmd      (444129884) staff       (20)      234 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/nfeltembed
+-rw-r--r--   0 nmd      (444129884) staff       (20)      978 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nfeltsign
+-rw-r--r--   0 nmd      (444129884) staff       (20)    15004 2022-03-03 14:06:11.000000 cypari-2.5.4/pari_src/src/test/in/nffactor
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1697 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/nfhilbert
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3583 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)      673 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/nfislocalpower
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3370 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nflist
+-rw-r--r--   0 nmd      (444129884) staff       (20)      498 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nflistA5
+-rw-r--r--   0 nmd      (444129884) staff       (20)      555 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nflistQT
+-rw-r--r--   0 nmd      (444129884) staff       (20)      428 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nflistQTall
+-rw-r--r--   0 nmd      (444129884) staff       (20)      545 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nfpolsturm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      506 2022-12-05 20:29:05.000000 cypari-2.5.4/pari_src/src/test/in/nfrootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)      548 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/nfsplitting
+-rw-r--r--   0 nmd      (444129884) staff       (20)      466 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/norm
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2237 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/number
+-rw-r--r--   0 nmd      (444129884) staff       (20)      883 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/objets
+-rw-r--r--   0 nmd      (444129884) staff       (20)      123 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/op
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1440 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/orthopol
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3013 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/padic
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2303 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/parallel
+-rw-r--r--   0 nmd      (444129884) staff       (20)      922 2018-05-01 12:01:20.000000 cypari-2.5.4/pari_src/src/test/in/partition
+-rw-r--r--   0 nmd      (444129884) staff       (20)      358 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/perm
+-rw-r--r--   0 nmd      (444129884) staff       (20)      836 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/plotexport
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2750 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/in/ploth
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2460 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/in/pol
+-rw-r--r--   0 nmd      (444129884) staff       (20)    13548 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/polclass
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1105 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/polmod
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7117 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/polmodular
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3761 2022-12-21 20:26:45.000000 cypari-2.5.4/pari_src/src/test/in/polred
+-rw-r--r--   0 nmd      (444129884) staff       (20)      162 2014-03-25 08:59:22.000000 cypari-2.5.4/pari_src/src/test/in/polygonal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      365 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/in/polylog
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1294 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/polyser
+-rw-r--r--   0 nmd      (444129884) staff       (20)      883 2022-12-21 17:55:47.000000 cypari-2.5.4/pari_src/src/test/in/pow
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1015 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/prec
+-rw-r--r--   0 nmd      (444129884) staff       (20)      682 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/prime
+-rw-r--r--   0 nmd      (444129884) staff       (20)      508 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/print
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2504 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/printf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1039 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/program
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3919 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/programming
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1581 2020-12-12 18:45:59.000000 cypari-2.5.4/pari_src/src/test/in/qf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1250 2022-10-31 21:05:51.000000 cypari-2.5.4/pari_src/src/test/in/qfb
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1061 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/qfbclassno
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1628 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/qfbsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2931 2021-05-21 11:46:52.000000 cypari-2.5.4/pari_src/src/test/in/qfisom
+-rw-r--r--   0 nmd      (444129884) staff       (20)    88096 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/qfsolve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      734 2022-10-05 22:56:00.000000 cypari-2.5.4/pari_src/src/test/in/quad
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1378 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/quadclassunit
+-rw-r--r--   0 nmd      (444129884) staff       (20)      126 2020-03-25 11:58:27.000000 cypari-2.5.4/pari_src/src/test/in/quaddisc
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1174 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/quadray
+-rw-r--r--   0 nmd      (444129884) staff       (20)      358 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ramanujantau
+-rw-r--r--   0 nmd      (444129884) staff       (20)      849 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/random
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1232 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/ranges
+-rw-r--r--   0 nmd      (444129884) staff       (20)    22240 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ratpoints
+-rw-r--r--   0 nmd      (444129884) staff       (20)      651 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/real
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2937 2022-03-01 15:12:50.000000 cypari-2.5.4/pari_src/src/test/in/resultant
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1081 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/in/rfrac
+-rw-r--r--   0 nmd      (444129884) staff       (20)     7153 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/rnf
+-rw-r--r--   0 nmd      (444129884) staff       (20)     6101 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/rnfkummer
+-rw-r--r--   0 nmd      (444129884) staff       (20)      135 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/rootsof1
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1825 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/in/rootsreal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      363 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/round
+-rw-r--r--   0 nmd      (444129884) staff       (20)    87603 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/round4
+-rw-r--r--   0 nmd      (444129884) staff       (20)      286 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/select
+-rw-r--r--   0 nmd      (444129884) staff       (20)       33 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/self
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3391 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/ser
+-rw-r--r--   0 nmd      (444129884) staff       (20)      438 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/set
+-rw-r--r--   0 nmd      (444129884) staff       (20)      277 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/setdebug
+-rw-r--r--   0 nmd      (444129884) staff       (20)      395 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/size
+-rw-r--r--   0 nmd      (444129884) staff       (20)      497 2022-11-01 08:37:35.000000 cypari-2.5.4/pari_src/src/test/in/solve
+-rw-r--r--   0 nmd      (444129884) staff       (20)      792 2018-07-25 18:00:21.000000 cypari-2.5.4/pari_src/src/test/in/sort
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1712 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/sqrtn
+-rw-r--r--   0 nmd      (444129884) staff       (20)      962 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/stark
+-rw-r--r--   0 nmd      (444129884) staff       (20)      756 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/str
+-rw-r--r--   0 nmd      (444129884) staff       (20)      732 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/subcyclo
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2082 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/subcyclopclgp
+-rw-r--r--   0 nmd      (444129884) staff       (20)    12710 2021-06-09 10:39:44.000000 cypari-2.5.4/pari_src/src/test/in/subfields
+-rw-r--r--   0 nmd      (444129884) staff       (20)      511 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/subgroup
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2687 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/subst
+-rw-r--r--   0 nmd      (444129884) staff       (20)       92 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/sumdedekind
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1286 2019-12-09 13:25:12.000000 cypari-2.5.4/pari_src/src/test/in/sumdiv
+-rw-r--r--   0 nmd      (444129884) staff       (20)      109 2014-03-25 08:59:22.000000 cypari-2.5.4/pari_src/src/test/in/sumformal
+-rw-r--r--   0 nmd      (444129884) staff       (20)      560 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/sumiter
+-rw-r--r--   0 nmd      (444129884) staff       (20)     3783 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/sumnum
+-rw-r--r--   0 nmd      (444129884) staff       (20)      764 2022-12-21 17:52:55.000000 cypari-2.5.4/pari_src/src/test/in/sumnumrat
+-rw-r--r--   0 nmd      (444129884) staff       (20)     4722 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/thue
+-rw-r--r--   0 nmd      (444129884) staff       (20)      289 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/time
+-rw-r--r--   0 nmd      (444129884) staff       (20)      913 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/trans
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2541 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/trans2
+-rw-r--r--   0 nmd      (444129884) staff       (20)      805 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/valuation
+-rw-r--r--   0 nmd      (444129884) staff       (20)      692 2020-10-26 12:43:04.000000 cypari-2.5.4/pari_src/src/test/in/vararg
+-rw-r--r--   0 nmd      (444129884) staff       (20)      413 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/variable
+-rw-r--r--   0 nmd      (444129884) staff       (20)       16 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/in/version
+-rw-r--r--   0 nmd      (444129884) staff       (20)       90 2017-01-14 12:26:42.000000 cypari-2.5.4/pari_src/src/test/in/whatnow
+-rw-r--r--   0 nmd      (444129884) staff       (20)      499 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/zeta
+-rw-r--r--   0 nmd      (444129884) staff       (20)      970 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/zetahurwitz
+-rw-r--r--   0 nmd      (444129884) staff       (20)     1828 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/zetamult
+-rw-r--r--   0 nmd      (444129884) staff       (20)     5517 2022-09-19 15:42:30.000000 cypari-2.5.4/pari_src/src/test/in/zn
+-rw-r--r--   0 nmd      (444129884) staff       (20)      546 2020-02-13 13:00:46.000000 cypari-2.5.4/pari_src/src/test/in/zncoppersmith
+-rw-r--r--   0 nmd      (444129884) staff       (20)     2239 2017-11-09 09:26:14.000000 cypari-2.5.4/pari_src/src/test/kerntest.c
+-rw-r--r--   0 nmd      (444129884) staff       (20)    28176 2022-02-25 22:10:32.000000 cypari-2.5.4/pari_src/src/test/tune.c
+drwxr-xr-x   0 nmd      (444129884) staff       (20)        0 2023-04-02 20:59:17.005063 cypari-2.5.4/patches/
+-rw-r--r--   0 nmd      (444129884) staff       (20)      396 2023-04-01 22:38:25.000000 cypari-2.5.4/patches/pari_2.15.patch
+-rw-r--r--   0 nmd      (444129884) staff       (20)    16800 2023-04-02 18:31:38.113520 cypari-2.5.4/setup.py
```

### Comparing `cypari-2.5.0/PKG-INFO` & `cypari-2.5.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: cypari
-Version: 2.5.0
+Version: 2.5.4
 Summary: Sage's PARI extension, modified to stand alone.
-Home-page: https://github.com/3-manifolds/cypari
+Home-page: https://bitbucket.org/t3m/cypari
 Author: Marc Culler and Nathan M. Dunfield
 Author-email: culler@uic.edu, nathan@dunfield.info
 License: GPLv2+
-Description: The package *cypari* is a Python wrapper for the `PARI library
-        <http://pari.math.u-bordeaux.fr/>`_, a computer algebra system for
-        number theory computations.  It is derived from the `corresponding
-        component <https://github.com/sagemath/cypari2>`_
-        of `SageMath <http://www.sagemath.org>`_, but is independent of the rest of
-        SageMath and can be used with any recent version of Python 3.
-        
 Keywords: Pari,SageMath,SnapPy
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Topic :: Scientific/Engineering :: Mathematics
+
+The package *cypari* is a Python wrapper for the `PARI library
+<http://pari.math.u-bordeaux.fr/>`_, a computer algebra system for
+number theory computations.  It is derived from the `corresponding
+component
+<https://github.com/sagemath/sage/blob/797dd7b4c273556d9677fadffa2ef6dd7f113857/src/sage/libs/cypari2/gen.pyx>`_
+of `SageMath <http://www.sagemath.org>`_, but is independent of the rest of
+SageMath and can be used with any recent version of Python 3.
```

### Comparing `cypari-2.5.0/build_pari.sh` & `cypari-2.5.4/build_pari.sh`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     echo "For macOS use pari and gmp as arguments to build universal binaries."
     exit
 fi
 
 #PARIURL=https://pari.math.u-bordeaux.fr/pub/pari/OLD/2.11/
 #PARIVERSION=pari-2.11.4
 PARIURL=http://pari.math.u-bordeaux.fr/pub/pari/unix/
-PARIVERSION=pari-2.15.1
+PARIVERSION=pari-2.15.2
 GMPURL=https://ftp.gnu.org/gnu/gmp/
 GMPVERSION=gmp-6.2.1
 
 if [[ $(pwd) =~ " " ]]; then
     echo "Fatal Error: Sorry, the path:"
     echo "             $(pwd)"
     echo "             has a space in it, preventing GMP from building"
@@ -125,26 +125,28 @@
     if [ ! -d "build" ] ; then
 	mkdir build ;
     fi
     cd build
     tar xzf ../${PARIVERSION}.tar.gz
     mv ${PARIVERSION} pari_src
     cd pari_src
-    # Add a guard against multiple includes of paristio.h
-    patch -p0 < ../../patches/paristio.patch
+    # Add a guard against multiple includes of paristio.h and fix uispsp.
+    patch -p0 < ../../patches/pari_2.15.patch
 else
     cd build/pari_src
-    # Add a guard against multiple includes of paristio.h
-    patch -p0 < ../../patches/paristio.patch
+    # Add a guard against multiple includes of paristio.h and fix uispsp.
+    patch -p0 < ../../patches/pari_2.15.patch
 fi
 
 export DESTDIR=
 if [ $(uname) = "Darwin" ] ; then
     rm -rf Odarwin*
     export CFLAGS="-arch x86_64 -arch arm64 -mmacosx-version-min=10.9"
+# For debugging:
+#   export CFLAGS="-g -arch x86_64 -arch arm64 -mmacosx-version-min=10.9"
     ./Configure --host=universal-darwin --prefix=${PARIPREFIX} --with-gmp=${GMPPREFIX}
     cd Odarwin-universal
     make install
     make install-lib-sta
     make clean
 elif [ `python -c "import sys; print(sys.platform)"` = 'win32' ] ; then
 #Windows
```

### Comparing `cypari-2.5.0/setup.py` & `cypari-2.5.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,44 +1,37 @@
 long_description =  """\
 The package *cypari* is a Python wrapper for the `PARI library
 <http://pari.math.u-bordeaux.fr/>`_, a computer algebra system for
 number theory computations.  It is derived from the `corresponding
-component <https://github.com/sagemath/cypari2>`_
+component
+<https://github.com/sagemath/sage/blob/797dd7b4c273556d9677fadffa2ef6dd7f113857/src/sage/libs/cypari2/gen.pyx>`_
 of `SageMath <http://www.sagemath.org>`_, but is independent of the rest of
 SageMath and can be used with any recent version of Python 3.
 """
 
 no_cython_message = """
-You need to have Cython (>= 0.29) installed to build the CyPari
+You need to have Cython (>= 0.28) installed to build the snappy
 module since you're missing the autogenerated C/C++ files, e.g.
 
-  sudo python -m pip install "cython>=0.29"
+  sudo python -m pip install "cython>=0.28"
 
 """
+
 import os, sys, re, sysconfig, subprocess, shutil, site, platform, time
-try:
-    assert sys.version_info.major == 3
-except:
+if sys.version_info.major == 2:
     print("Python 2 is not supported")
     sys.exit()
 from glob import glob
 from setuptools import setup, Command
 from distutils.extension import Extension
 from distutils.command.build_ext import build_ext
 from distutils.command.sdist import sdist
 from distutils.util import get_platform
 from subprocess import Popen, PIPE
 
-MSYS64_W = os.environ.get('MSYS64_DIR', r'C:\msys64')
-MSYS64_U = os.environ.get('MSYS64_DIR', '/c/msys64')
-
-if sys.version_info < (3,5):
-    ('CyPari requires Python 3.5 or newer')
-    sys.exit()
-
 cpu_width = '64bit' if sys.maxsize > 2**32 else '32bit'
 
 if sys.platform == 'win32':
     compiler_set = False
     ext_compiler = 'msvc'
     for n, arg in enumerate(sys.argv):
         if arg == '-c':
@@ -62,41 +55,59 @@
 if sys.platform == 'win32':
     # We always build the Pari library with mingw, no matter which compiler
     # is used for the CyPari extension.
     # Make sure that our C compiler matches our python and that we can run bash
     # and other needed utilities such as find.
     bash_proc = Popen(['bash', '-c', 'echo $PATH'], stdout=PIPE, stderr=PIPE)
     BASHPATH, _ = bash_proc.communicate()
-    if cpu_width == '64bit':
-        TOOLCHAIN_W = MSYS64_W + r'\ucrt64\bin'
-        TOOLCHAIN_U = MSYS64_U + '/ucrt64/bin'
+    BASHPATH = BASHPATH.decode('utf8')
+    if sys.version_info >= (3,5):
+        if cpu_width == '64bit':
+            TOOLCHAIN_W = r'C:\mingw-w64\x86_64-8.1.0-posix-seh-rt_v6-rev0\mingw64'
+            TOOLCHAIN_U = '/c/mingw-w64/x86_64-8.1.0-posix-seh-rt_v6-rev0/mingw64'
+        else:
+            TOOLCHAIN_W = r'C:\mingw-w64\i686-8.1.0-posix-dwarf-rt_v6-rev0\mingw32'
+            TOOLCHAIN_U = '/c/mingw-w64/i686-8.1.0-posix-dwarf-rt_v6-rev0/mingw32'
     else:
-        TOOLCHAIN_W = MSYS64_W + r'\ucrt32\bin'
-        TOOLCHAIN_U = MSYS64_U + '/ucrt32/bin'
-
-    WINPATH=r'{0};{1}\bin;%{1}\usr\local\bin;{1}\usr\bin;'.format(
-        TOOLCHAIN_W, MSYS64_W)
-    BASHPATH='{0}:{1}'.format(TOOLCHAIN_U,BASHPATH.decode('utf-8'))
-    KIT_PATH=r'/c/Program Files (x86)/Windows Kits/10/bin/10.0.22000.0/x64'
-    BASH = r'%s\usr\bin\bash'%MSYS64_W
+        if cpu_width == '64bit':
+            TOOLCHAIN_W = r'C:\mingw-w64\x86_64-6.3.0-posix-seh-rt_v5-rev1\mingw64'
+            TOOLCHAIN_U = '/c/mingw-w64/x86_64-6.3.0-posix-seh-rt_v5-rev1/mingw64'
+        else:
+            TOOLCHAIN_W = r'C:\mingw-w64\i686-6.3.0-posix-dwarf-rt_v5-rev1\mingw32'
+            TOOLCHAIN_U = '/c/mingw-w64/i686-6.3.0-posix-dwarf-rt_v5-rev1/mingw32'
+        
+    WINPATH=r'%s\bin;C:\msys64\usr\local\bin;C:\msys64\usr\bin;'%TOOLCHAIN_W
+    BASHPATH='%s/bin:/c/msys64/usr/bin:'%TOOLCHAIN_U + BASHPATH
+    os.environ['PATH'] = ';'.join([WINPATH, os.environ['PATH']])
+    BASH = r'C:\msys64\usr\bin\bash'
 else:
     BASHPATH = os.environ['PATH']
     BASH = '/bin/bash'
 
+# We build the 32 bit and 64 bit versions of the Pari library in separate
+# directories, but in macOS we use lipo to combine them into a fat library.
+# On Windows we also build separately for the Universal CRT on Python >= 3.5
 if sys.platform == 'darwin':
-    GMPDIR = 'gmp'
     PARIDIR = 'pari'
+    GMPDIR = 'gmp'
+elif sys.platform == 'win32':
+    if cpu_width == '64bit':
+        PARIDIR = 'pari64'
+        GMPDIR = 'gmp64'
+    else:
+        PARIDIR = 'pari32'
+        GMPDIR = 'gmp32'
 else:
     if cpu_width  == '64bit':
         GMPDIR = 'gmp64'
         PARIDIR = 'pari64'
     else:
         GMPDIR = 'gmp32'
         PARIDIR = 'pari32'
-
+    
 pari_include_dir = os.path.join('libcache', PARIDIR, 'include')
 pari_library_dir = os.path.join('libcache', PARIDIR, 'lib')
 pari_static_library = os.path.join(pari_library_dir, 'libpari.a')
 gmp_library_dir = os.path.join('libcache', GMPDIR, 'lib')
 gmp_static_library = os.path.join(gmp_library_dir, 'libgmp.a')
 
 MSVC_include_dirs = [
@@ -114,19 +125,19 @@
 else:
     MSVC_extra_objects = [
     r'C:\Program Files (x86)\Windows Kits\10\Lib\10.0.22000.0\um\x86\Uuid.lib',
     r'C:\Program Files (x86)\Windows Kits\10\Lib\10.0.22000.0\um\x86\kernel32.lib',
     r'C:\Program Files (x86)\Windows Kits\10\Lib\10.0.22000.0\ucrt\x86\ucrt.lib',
     os.path.abspath(os.path.join('Windows', 'gcc', 'libgcc.a')),
     ]
-    
+
 class CyPariClean(Command):
     user_options = []
     def initialize_options(self):
-        pass
+        pass 
     def finalize_options(self):
         pass
     def run(self):
         junkdirs = (glob('build/lib*') +
                     glob('build/bdist*') +
                     glob('build/temp*') +
                     glob('cypari*.egg-info')
@@ -149,24 +160,25 @@
                 os.remove(file)
             except OSError:
                 pass
 
 class CyPariTest(Command):
     user_options = []
     def initialize_options(self):
-        pass
+        pass 
     def finalize_options(self):
         pass
     def run(self):
         build_lib_dir = os.path.join(
             'build',
-            'lib.{platform}-{version_info[0]}.{version_info[1]}'.format(
+            'lib.{platform}-cpython-{version_info[0]}{version_info[1]}'.format(
                 platform=sysconfig.get_platform(),
                 version_info=sys.version_info)
         )
+        print(build_lib_dir)
         sys.path.insert(0, os.path.abspath(build_lib_dir))
         from cypari.test import runtests
         sys.exit(runtests())
 
 def check_call(args):
     try:
         subprocess.check_call(args)
@@ -188,22 +200,28 @@
     def finalize_options(self):
         pass
     def run(self):
         if os.path.exists('build'):
             shutil.rmtree('build')
         if os.path.exists('dist'):
             shutil.rmtree('dist')
-        os.remove('cypari/_pari.c')
+        for filename in glob('cypari/_pari*.c'):
+            os.remove(filename)
 
         pythons = os.environ.get('RELEASE_PYTHONS', sys.executable).split(',')
         print('releasing for: %s'%(', '.join(pythons)))
         for python in pythons:
             check_call([python, 'setup.py', 'clean'])
             check_call([python, 'setup.py', 'build'])
             check_call([python, 'setup.py', 'test'])
+            # Save a copy of the _pari.c file for each major version of Python.
+            _pari_c_name = '_pari_py%s.c'%python_major(python)
+            _pari_c_path = os.path.join('cypari', _pari_c_name)
+            if not os.path.exists(_pari_c_path):
+                os.rename(os.path.join('cypari', '_pari.c'), _pari_c_path)
             if sys.platform.startswith('linux'):
                 plat = get_platform().replace('linux', 'manylinux1')
                 plat = plat.replace('-', '_')
                 check_call([python, 'setup.py', 'bdist_wheel', '-p', plat])
                 check_call([python, 'setup.py', 'bdist_egg'])
             else:
                 check_call([python, 'setup.py', 'bdist_wheel'])
@@ -227,50 +245,48 @@
 win64_py2_decls = b'''
 '''
 
 decls = b'''
 '''
 
 class CyPariBuildExt(build_ext):
-
+        
     def run(self):
         building_sdist = False
-
+        
         if os.path.exists('pari_src'):
             # We are building an sdist.  Move the Pari source code into build.
             if not os.path.exists('build'):
                 os.mkdir('build')
             os.rename('pari_src', os.path.join('build', 'pari_src'))
             os.rename('gmp_src', os.path.join('build', 'gmp_src'))
             building_sdist = True
-
+        
         if (not os.path.exists(os.path.join('libcache', PARIDIR))
             or not os.path.exists(os.path.join('libcache', GMPDIR))):
             if sys.platform == 'win32':
                 # This is meant to work even in a Windows Command Prompt
                 if cpu_width == 64:
-                    cmd = r'export PATH="%s" ; export MSYSTEM=MINGW64 ; bash build_pari.sh %s %s'%(
-                        BASHPATH, PARIDIR, GMPDIR)
+                    cmd = r'export PATH="%s" ; export MSYSTEM=MINGW64 ; bash build_pari.sh %s %s'%(BASHPATH, PARIDIR, GMPDIR)
                 else:
-                    cmd = r'export PATH="%s" ; export MSYSTEM=MINGW32 ; bash build_pari.sh %s %s'%(
-                        BASHPATH, PARIDIR, GMPDIR)
+                    cmd = r'export PATH="%s" ; export MSYSTEM=MINGW32 ; bash build_pari.sh %s %s'%(BASHPATH, PARIDIR, GMPDIR)
             else:
                 cmd = r'export PATH="%s" ; bash build_pari.sh %s %s'%(BASHPATH, PARIDIR, GMPDIR)
             if subprocess.call([BASH, '-c', cmd]):
                 sys.exit("***Failed to build PARI library***")
 
         if building_sdist:
             build_ext.run(self)
             return
 
         if (not os.path.exists(os.path.join('cypari', 'auto_gen.pxi')) or
             not os.path.exists(os.path.join('cypari', 'auto_instance.pxi'))):
             import autogen
             autogen.rebuild()
-
+            
         # Provide declarations in an included .pxi file which indicate
         # whether we are building for 64 bit Python on Windows, and
         # which version of Python we are using.  We need to handle 64
         # bit Windows differently because (a) it is the only 64 bit
         # system with 32 bit longs and (b) Pari deals with this by:
         # #define long long long thereby breaking lots of stuff in the
         # Python headers.
@@ -292,34 +308,34 @@
         else:
             old_code = b''
         if old_code != code:
             with open(long_include, 'wb') as output:
                 output.write(code)
 
         # If we have Cython, check that .c files are up to date
-        try:
+        try: 
             from Cython.Build import cythonize
             cythonize([os.path.join('cypari', '_pari.pyx')],
-                      compiler_directives = {'language_level':3})
+                      compiler_directives = {'language_level':2})
         except ImportError:
             if not os.path.exists(os.path.join('cypari', '_pari.c')):
                 sys.exit(no_cython_message)
 
         build_ext.run(self)
 
 class CyPariSourceDist(sdist):
-
+    
     def _tarball_info(self, lib):
         lib_re = re.compile('(%s-[0-9\.]+)\.tar\.[bg]z2*'%lib)
         for f in os.listdir('.'):
             lib_match = lib_re.search(f)
             if lib_match:
                 break
         return lib_match.group(), lib_match.groups()[0]
-
+    
     def run(self):
         tarball, dir = self._tarball_info('pari')
         check_call(['tar', 'xfz', tarball])
         os.rename(dir, 'pari_src')
         tarball, dir = self._tarball_info('gmp')
         check_call(['tar', 'xfj', tarball])
         os.rename(dir, 'gmp_src')
@@ -349,28 +365,30 @@
     # Ignore the assembly language inlines when building the extension.
     compile_args += ['/DDISABLE_INLINE']
     if False:  # Toggle for debugging symbols
         compile_args += ['/Zi']
         link_args += ['/DEBUG']
     # Add the mingw crt objects needed by libpari.
     if cpu_width == '64bit':
-         link_args += [
-             os.path.join('Windows', 'crt', 'libparicrt64.a'),
-             'legacy_stdio_definitions.lib',
-             os.path.join('Windows', 'crt', 'get_output_format64.o'),
-         ]
+        link_args += [os.path.join('Windows', 'crt', 'libparicrt64.a'),
+                      'advapi32.lib']
+        if sys.version_info >= (3, 5):
+            link_args += [
+                'legacy_stdio_definitions.lib',
+                os.path.join('Windows', 'crt', 'get_output_format64.o')]
     else:
-         link_args += [
-             os.path.join('Windows', 'crt', 'libparicrt32.a'),
-             'legacy_stdio_definitions.lib',
-             os.path.join('Windows', 'crt', 'get_output_format32.o')
-         ]
+        link_args += [os.path.join('Windows', 'crt', 'libparicrt32.a'),
+                      'advapi32.lib']
+        if sys.version_info >= (3, 5):
+            link_args += [
+                'legacy_stdio_definitions.lib', 'advapi32.lib',
+                os.path.join('Windows', 'crt', 'get_output_format32.o')]
 
 link_args += [pari_static_library, gmp_static_library]
-
+    
 if sys.platform.startswith('linux'):
     link_args += ['-Wl,-Bsymbolic-functions', '-Wl,-Bsymbolic']
 
 include_dirs = [pari_include_dir]
 extra_objects = []
 if sys.platform == 'win32':
     include_dirs += MSVC_include_dirs
@@ -400,15 +418,15 @@
         'test': CyPariTest,
         'release': CyPariRelease,
         'sdist': CyPariSourceDist,
     },
     ext_modules = [_pari],
     zip_safe = False,
     long_description = long_description,
-    url = 'https://github.com/3-manifolds/cypari',
+    url = 'https://bitbucket.org/t3m/cypari',
     author = 'Marc Culler and Nathan M. Dunfield',
     author_email = 'culler@uic.edu, nathan@dunfield.info',
     license='GPLv2+',
     classifiers = [
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Science/Research',
         'License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)',
```

### Comparing `cypari-2.5.0/README.rst` & `cypari-2.5.4/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 CyPari
 ======
 
 CyPari is a standalone version of Sage's pari module which is largely
 consistent with the Sage cypari2 package that it inspired, but which
 can be distributed in binary form as a pip wheel and also works on
 Windows.  In particular, CyPari uses the automated build scripts
-written by Jeroen DeMeyer for cypari2.  Currently it uses Pari 2.15,
+written by Jeroen DeMeyer for cypari2.  Currently it uses Pari 2.11,
 which is several releases newer than the PARI used in the original
 version of CyPari.  The fact that the build process continues to work
 with each new release of PARI is a strong validation of Jeroen's
 flexible build scheme.
 
 CyPari handles critical signals such as SIGSEGV when sent from within
 a sig_on - sig_off block. Long computations in sig_on - sig_off blocks
@@ -38,7 +38,31 @@
 
 All tests should pass on all platforms.
 
 To clean up the build area (but not remove PARI) use::
 
     python setup.py clean
 
+Note that the ``future`` module is required for Python 2.
+Install if necessary with::
+
+    pip install future
+
+For building on Windows we expect an msys64 system with the
+toolchains::
+
+    mingw-w64\i686-6.3.0-posix-dwarf-rt_v5-rev1 (for 32-bit builds)
+    mingw-w64\x86_64-8.1.0-posix-seh-rt_v6-rev0 (for 64-bit builds)
+
+These toolchains support Microsoft's Universal C Runtime, which means
+that CyPari no longer requires installation of any special C runtime
+dll files.  The build process uses the mingw toolchains to build libpari.a
+but the Python extension is built with an appropriate version of
+MSVC.
+
+It is also possible to build the Windows Python extension entirely
+with MinGW for Python versions less than 3.5.  To do this, run::
+
+    setup.py build -cmingw32
+
+Currently we support 32 and 64 bit Python 2.7, 3.6-3.10 on linux,
+macOS and Windows.
```

### Comparing `cypari-2.5.0/Windows/README.Windows` & `cypari-2.5.4/pari_src/doc/gp.1`

 * *Files 27% similar despite different names*

```diff
@@ -1,186 +1,378 @@
-Introduction
-------------
-
-Version 2 of CyPari for Windows is built using MSys2 and the mingw32
-gcc toolchain.  It passes the doctests at essentially the same rate as
-the linux and macOS versions, and supports SIGINT interrupts via
-control-C.  However, there are some caveats:
-
-1) The mingw32 toolchain must be modified to produce a Python
-extension module which does not segfault while being loaded.  (See the
-explanation in "About Segfaults" below.)  To deal with this issue, the
-script install_files_32.sh in the toolchain directory adds the needed
-files to your mingw32 toolchain.  (The mingw64 version has not been
-tested, but may work.)
-
-2) To be able to interrupt a long computation by typing control-C
-requires two non-trivial things: (i) the module must have appropriate
-SIGINT handlers and (see "About longjmp" below); and (ii) the terminal
-must send a SIGINT signal (see "About SIGINT" below).  The caveat here
-is that the Cygwin Mintty terminal provided with MSys2 does not handle
-sending a SIGINT in the same way as the Windows console, which causes
-different behavior. More importantly, it is not possible to run python
-interactively in Mintty at all, unless you run the python process
-within a winpty wrapper:
-$ winpty python
-
-One way to handle this is to add something like the following to the
-end of the .bash_profile in your msys2 home directory:
-
-export PATH="/c/Python27:/c/Python27/Scripts:/c/emacs-2.4.v/bin:/c/Program Files (x86)/Common Files/Microsoft/Visual C++ for Python/9.0/VC/bin:$PATH"
-winpty bash; exit
-
-(The second line runs bash in a winpty wrapper and exits when that shell
-is killed.)
-
-About Segfaults
----------------
-
-When I first built this package and tested it, Python segfaulted while
-loading the module.  With great effort I finally identified the point
-where the crash occurred.  It was crashing when calling realloc in the
-function initprimes (src/language/forprimes.c.  This routine first
-calls malloc to allocate a block of memory which is provably large
-enough to hold a table with the desired number of primes, then writes
-the primes into the table, and finally calls realloc to reduce the
-size of the block to the size of the table.  How could this fail?
-
-The answer is that the malloc function was coming from the C runtime
-in msvcr90.dll while the realloc function was coming from the older
-C runtime msvcrt.dll.  The Python executable was linked against the
-former while mingw2 uses the latter as its default runtime.  The two
-runtimes are not compatible.  When Python loads, it needs malloc so
-it resolves the malloc symbol against msvcr90.dll.  However, it does
-not immediately use realloc, so that symbol remains unresolved.  When
-the cypari extension module is loaded it inherits the malloc from
-Python, but it does not inherit realloc since that is still
-unresolved.  When realloc is needed in initprimes, the symbol is
-resolved against the msvcrt.dll.  The two runtimes do not allocate
-memory in compatible ways - hence the segfault.
-
-There is a reason why mingw32 uses the out-of-date msvcrt runtime, and
-it has to do with Microsoft's attempt to deal with the "DLL Hell"
-caused by having many incompatible DLL's on the same system, all with
-the same name.  Their solution was called "Side by Side Assemblies"
-which consist of a DLL, which has been assigned a cryprographic key
-uniquely identifying its precise version, and an xml "Manifest file"
-which specifies the key.  These must appear in the same subdirectory
-of the C:\Windows\winsxs directory.  In order for a third party DLL or
-EXE to call functions from a dll in a side-by-side assemply, the
-library must have its own manifest file which matches the one in
-winsxs.  This user manifest file must either appear in the same
-directory as the DLL or EXE, or else be embedded in it as a Windows
-"Resource".  The gcc linker is able to embed these resource files, if
-they are supplied on the command line.
-
-So, to ensure that our cypari extension module gets its C runtime
-functions from the same DLL as the Python executable we need to do two
-things (and possible a third, even more technical one).  First, we
-need to prevent gcc from linking against its default msvcrt runtime.
-This is done by providing gcc with a "specs" file which specifies
-things such as which "hidden" link libraries (e.g. C runtimes) are
-linked before the user-supplied libraries.  Our specs file specifies
-that gcc should link agains the msvcr90 runtime. Second, we need to
-provide a resource file that matches the msvcr90 runtime so that the
-OS will allow the extension module to access the runtime.  The final
-technical item is that one of the hidden libraries, called
-libmoldname, which has the job of mapping names of runtime functions
-to the older name which has an underscore prepended, probably has to
-be replaced with one that has symbols matching msvcr90 instead of
-msvcrt.  To accomplish all this we need to add three files to the
-mingw32 toolchain.  Thes files are named specs90, mscvr90.res and
-libmoldname90.a. In addition, to make gcc use the specs file, we need
-to pass the option specs=specs90 to the mingw32 linker.  Our spec
-file is a modified version of the one developed by the mingwpy
-project (https://mingwpy.github.io/).  Instructions for using the
-gnu dlltool to build libmoldname90.a can be found on the pygame
-website (http://www.pygame.org/wiki/PreparingMinGW).  The tool used
-to convert an xml file to a windows resource is called windres
-(see http://www.mingw.org/wiki/MS_resource_compiler).  The structure
-of a manifest file is described on the Microsoft developer site
-(https://msdn.microsoft.com/en-us/library/windows/desktop/aa375365(v=vs.85).aspx).
-
-About longjmp
--------------
-
-Sage's sig_on and sig_off macros are based on the setjmp/longjmp
-paradigm (or, on posix systems, sigsetjmp/siglongjmp).  This low level
-paradigm is an early precursor of the try - except blocks in high
-level languages.  It is commonly used in combination with signal
-handlers.  The basic construction looks like this:
-
-if (setjmp(env) == 0) {
-   ... long running interruptible code
-   }
-... go on from here ...   
-
-The setjmp function saves a copy of the current stack frame in the
-global struct env and returns 0.  If one wants to be able to interrupt
-the long running code one needs a signal handler like this:
-
-void handler(int signum) {
-  ... do something ...
-  longjmp(env, signum); /* never returns */
-}
-
-The effect of the call to longjmp is to use the saved frame to
-reconstruct the stack so it is in the same state that it would have
-been in if the function setjmp had returned the value signum instead
-of 0, and then coninue execution at the next instruction past the
-longjmp.  Thus when the signal handler returns, the program executes as
-if it had simply skipped the entire block of long running code.  The
-return value of setjmp can be used to determine how to recover from
-the interrupt.
-
-There are many things that can go wrong with this.  The typical error
-is to call setjmp from a function which returns before the call to
-longjmp.  This inserts a stack frame at a random point in the stack,
-resulting is a totally trashed stack and a big crash.
-
-One thing to notice about this paradigm is that it assumes that the
-signal handler is running on the same stack as the main program.
-While this is not a posix requirement, it is true for most posix
-systems including linux and macOS.  But it is NOT true for Windows.
-In Windows, the signal handler runs in a separate thread with its own
-stack and has no way of accessing the stack of its parent
-process. However, it turns out that there is (exactly) one special
-signal for which Windows supports using longjmp in the handler, namely
-SIGFPE.  This is explicitly stated in the Windows documentation:
-https://msdn.microsoft.com/en-us/library/xdkz3x12.aspx
-https://msdn.microsoft.com/en-us/library/aa246458(v=vs.60).aspx
-
-We take advantage of this quirk to port the cysignals package to
-Windows.  When our handler is called with a different signal than
-SIGFPE, it stores the signal number in the global cysigs structure and
-raises SIGFPE. (This means we are raising a signal within a signal
-handler, which would be a no-no in posix but appears to be OK in
-Windows.)  When the handler is called with SIGFPE it chacks the cysigs
-structure and responds appropriately (no stored signal means that it
-is a real SIGFPE).
-
-About SIGINT
-------------
-
-In Windows it is not supported for one process to use signals to
-communicate with another.  In posix the "kill" function does not
-necessarily terminate the target process, it just sends it a signal.
-But Windows takes "kill" very literally.  The target process will be
-terminated after receiving the signal, no matter what.  The only use
-of the signal number when a process gets "killed" by another is for
-deciding which cleanup routine to call before termination.
-
-However, there is another class of things which behave similarly to
-signals.  Perhaps they should be called "events" since there only two
-that I know of: CTRL_C_EVENT and CTRL_BREAK_EVENT.  These events can
-have handlers, just like signals.  Windows has two distinct types of
-proecesses, "Console" processes and "Gui" processes, and only Console
-processes support these events.  The Windows Command Prompt knows how
-to deliver these eponymous "events" in response to the keystokes in
-their name.  As far as I can tell, other consoles cannot do this,
-MinTTY being the prime example.  This is why it is not a trivial
-matter to arrange for delivery of a SIGINT signal when you want to
-interrupt a long-running computation.  (I believe that the original
-MSys terminal was actually a subclass of the same object as the CONS:
-Command Prompt, and that is why it was able to supply the SIGINT.  If
-a terminal can initiate a CTRL_C_EVENT, then one can create a
-CTRL-C-EVENT handler which raises SIGINT.
+.TH GP 1 "11 September 2017"
+.SH NAME
+gp \- The PARI calculator
+.SH SYNOPSIS
+.B gp
+.RB [ -s
+.IR stacksize ]
+.RB [ -p
+.IR primelimit ]
+.RB [ --emacs ]
+.RB [ -f | --fast ]
+.RB [ -q | --quiet ]
+.RB [ -D | --default
+.IR key=val ]
+.RB [ --help ]
+.RB [ --test ]
+.RB [ --texmacs ]
+.RB [ --version ]
+.RB [ --version-short ]
+[ file1 file2 ...]
+
+.SH DESCRIPTION
+Invokes the PARI-GP calculator
+\&\fBgp\fR; gp is an advanced programmable calculator, specializing in number
+theory, which computes symbolically as long as possible, numerically where
+needed, and contains a wealth of arithmetic functions: factorizations,
+elliptic curves, Galois theory, class field theory, modular forms, etc.
+Commands, written in the GP scripting language, are input interactively or
+loaded from files.
+
+If present at the end of the command line, files 'file1', 'file2', ...
+are loaded on startup; they must be written in the GP language.
+
+.SH OPTIONS
+Command line options are available in both short form (-f) and POSIX-like
+(--fast). Numeric arguments can be followed by a modifier
+.B k
+,
+.B M
+or
+.B G
+at the user's convenience; in that case the argument is multiplied by 10^3,
+10^6, or 10^9 respectively.
+
+.TP
+.B \-f, \--fast
+Fast start (or factory settings). Do not read
+.B .gprc
+(see below) upon startup.
+.TP
+.B \-p limit
+[DEPRECATED]
+Upon startup, gp computes a table of small primes used in
+number-theoretic applications. If
+.I primelimit
+is set, the table include primes up to that bound instead of the default
+(= 500000). It is now mostly useless to change this value.
+.TP
+.B \-q, \--quiet
+Quiet mode. Do not print headers or history numbers and do not say goodbye.
+
+.TP
+.B \-D, \--default key=val
+performs
+.BR default(key,
+.BR val) ";"
+on startup, overriding values from the
+.B gprc
+preferences file. 'val' must be a constant value and is not allowed to
+involve any computation (e.g. 1+1 is forbidden). Any number of such
+default-setting statements may appear on the command line. A key may be set
+multiple times, the last setting taking precedence
+
+.TP
+.B \-s limit
+Size of gp internal stack allocated on startup. When gp runs out of space, it
+interrupts the current computation and raises a
+.BI "stack overflow"
+exception. If this occurs frequently, start with a bigger stack. The stack
+size can also be
+increased from within gp, using
+.BR default(parisize, limit) ";"
+it is convenient to set
+.B parisize
+from your
+.B .gprc
+to that the setting is persistent across sessions; a value of 80MB is sensible.
+We strongly advise to also set
+.B parisizemax
+to a positive, much larger, value in your
+.B .gprc
+(about what you believe your machine can stand, usually half the available
+RAM or so): this strives to fit computation in the parisize range but allows
+it to temporarily go beyond it (up to parisizemax).
+Note that computations with a
+.B smaller
+stack may be more efficient due to better data locality. Finally,
+.B threadsize
+and
+.B threadsizemax
+play analogous roles in the parallel version of gp.
+
+.TP
+.B \--emacs
+gp can be run in an
+.I Emacs
+shell (see GP User's manual for details). This flag is then required for
+smooth interaction with the
+.I PariEmacs
+package (pari.el). It is set automatically by the pari.el package, and will
+produce display oddities if you set it outside of an
+.I Emacs
+session.
+.TP
+.B \--help
+print a summary of available command-line options.
+.TP
+.B \--test
+run gp in test mode: suppress printing of history numbers and wrap long
+output lines (to get readable diff output). For benches only.
+.TP
+.B \--texmacs
+gp can be run from a
+.I TeXmacs
+frontend. This flag is set by TeXmacs, to enable special purpose
+communication channels. Do not set it yourself.
+
+.TP
+.B \--version
+output version info (banner) then exit.
+
+.TP
+.B \--version-short
+output version number then exit.
+
+.SH USE
+.TP
+.B ?
+to get online help.
+.TP
+.B ??
+to get extended online help (more precisely, to call the external help
+program,
+.B gphelp
+by default)
+.TP
+.B quit
+(or \\q), or
+.B EOF
+(Ctrl-D) to quit
+.BR gp .
+.PP
+The following works only when gp was linked with GNU
+.IR readline
+library:
+.TP
+arrow keys
+for editing and viewing the input history.
+.TP
+.B TAB
+ for automatic completion
+
+.SH MANUALS
+The following material is included in the standard distribution (originally
+in TeX format) and can also be downloaded at
+.RS
+.I http://pari.math.u-bordeaux.fr/doc.html
+.RE
+or viewed online at
+.RS
+.I http://pari.math.u-bordeaux.fr/dochtml/html/
+.RE
+
+.TP
+.I The User's Guide to PARI/GP
+(users.dvi)
+.TP
+.I The User's Guide to the PARI library
+(library.dvi)
+.TP
+.I The Developer's Guide to the PARI library
+(develop.dvi)
+.TP
+.I PARI/GP, a tutorial
+(tutorial.dvi)
+.TP
+.I PARI/GP reference cards
+(refcard*.dvi)
+
+.SH FILES
+.TP
+.I gp
+main executable
+.TP
+.I $HOME/.gprc
+(or $GPRC if set) user preference file, read at beginning of execution by
+each
+.B gp
+shell. A default gprc
+.I gprc.dft
+is provided with the distribution. If this file cannot be found,
+.I /etc/gprc
+is checked instead.
+
+.TP
+.I <logfile>
+a file used to log in all commands and results; default:
+.B pari.log
+(you need to set the
+.B log
+default in your gprc or interactively)
+
+.TP
+.I <psfile>
+a file used to dump PostScript drawings; default:
+.B pari.ps
+
+.TP
+.I <histfile>
+a file where gp will keep a history of all input commands (you need to set
+the
+.B histfile
+default in the gprc file)
+
+.TP
+.I gphelp
+default external help program (as above)
+.TP
+.I *.gp
+GP programs
+
+.SH ENVIRONMENT
+.TP
+.I $GPRC
+place to look for the user's preference file (gprc); if the file does not exist,
+we then check in $HOME/.gprc, /etc/gprc, and finally for a file named 'gprc'
+in PARI's
+.B datadir.
+
+.TP
+.I $GP_DATA_DIR
+directory containing data installed by optional PARI packages.
+For example, the Galois resolvents files in directory
+.I galdata/
+needed by the
+.B polgalois
+function, in degrees 8 to 11; or the modular polynomials in
+.I seadata/
+used by the
+.B ellap
+function for large base fields. This environment variable
+overrides PARI's 'datadir', defined at Configure time.
+
+.TP
+.I $GP_POSTSCRIPT_VIEWER
+an application able to display PostScript files, used by the
+.I plotps
+graphic engine. This engine is a fallback used to output hi-res plots even
+when no compatible graphical library was available on your platform at
+Configure time. (Dumps the graph to a temporary file, then open the file.)
+
+.TP
+.I $GP_SVG_VIEWER
+an application able to display SVG images files, used by the
+.I plotsvg
+graphic engine. This engine is a fallback used to output hi-res plots even
+when no compatible graphical library was available on your platform at
+Configure time. (Dumps the graph to a temporary file, then open the file.)
+
+.TP
+.I $GPHELP
+name of the external help program invoked by ?? and ??? shortcuts.
+
+.TP
+.I $GPTMPDIR
+name of the directory where temporary files will be generated.
+
+.SH HOME PAGE
+PARI's home page resides at
+.RS
+.I http://pari.math.u-bordeaux.fr/
+.RE
+
+.SH MAILING LISTS
+There are a number of mailing lists devoted to the PARI/GP package, and most
+feedback should be directed to those. See
+.RS
+.I http://pari.math.u-bordeaux.fr/lists.html
+.RE
+for details. The most important ones are:
+
+.PP
+-
+.B pari-announce
+(moderated): for us to announce major version changes.
+.PP
+-
+.B pari-dev:
+for everything related to the development of PARI, including
+suggestions, technical questions, bug reports or patch submissions.
+
+.PP
+-
+.B pari-users:
+for discuss about everything else, in particular ask for help.
+
+To subscribe, send empty messages with a Subject: containing the word
+"subscribe" respectively to
+
+.PP
+   pari-announce-request@pari.math.u-bordeaux.fr
+.PP
+   pari-users-request@pari.math.u-bordeaux.fr
+.PP
+   pari-dev-request@pari.math.u-bordeaux.fr
+
+.SH BUG REPORTS
+Bugs should be submitted online to our Bug Tracking System, available from
+PARI's home page, or directly from the URL
+.RS
+.I http://pari.math.u-bordeaux.fr/Bugs/
+.RE
+Further instructions can be found on that page.
+
+.SH TRIVIA
+Despite the leading G, GP has nothing to do with GNU. The first version was
+originally called GPC, for Great Programmable Calculator. When people started
+calling it "the GPC Calculator", the trailing C was dropped.
+
+PARI has nothing to do with the French capital. The name is a pun about the
+project's early stages when the authors started to implement a library for
+"Pascal ARIthmetic" in the PASCAL programming language. They quickly
+switched to C.
+
+For the benefit of non-native French speakers, here's a slightly expanded
+explanation:
+.B Blaise Pascal
+(1623-1662) was a famous French mathematician and philosopher who was one
+of the founders of probability and devised one of the first "arithmetic
+machines". He once proposed the following "proof" of the existence of God
+for the unbelievers: whether He exists or not I lose nothing by believing
+in Him, whereas if He does and I misbehave... This is the so-called "pari
+de Pascal" (Pascal's Wager).
+
+Note that PARI also means "fairy" in Persian.
+
+.SH AUTHORS
+PARI was originally written by Christian Batut, Dominique Bernardi, Henri
+Cohen, and Michel Olivier in Laboratoire A2X (Universite Bordeaux I, France),
+and was maintained by Henri Cohen up to version 1.39.15 (1995), and by Karim
+Belabas since then.
+
+A great number of people have contributed to the successive improvements
+which eventually resulted in the present version. See the AUTHORS file in
+the distribution.
+
+.SH SEE ALSO
+.IR gap (1),
+.IR gphelp (1),
+.IR perl (1),
+.IR readline (3),
+.IR sage (1),
+.IR tex (1),
+.IR texmacs (1),
+
+.SH COPYING
+
+This program is free software; you can redistribute it and/or modify it under
+the terms of the GNU General Public License as published by the Free Software
+Foundation.
+
+This program is distributed in the hope that it will be useful, but WITHOUT
+ANY WARRANTY; without even the implied warranty of MERCHANTABILITY or FITNESS
+FOR A PARTICULAR PURPOSE. See the GNU General Public License for more details.
+
+You should have received a copy of the GNU General Public License along with
+this program; if not, write to the Free Software Foundation, Inc., 675 Mass
+Ave, Cambridge, MA 02139, USA.
```

### Comparing `cypari-2.5.0/cypari/parisage.h` & `cypari-2.5.4/cypari/parisage.h`

 * *Files identical despite different names*

### Comparing `cypari-2.5.0/cypari/implementation.c` & `cypari-2.5.4/cypari/implementation.c`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,14 @@
  * is embedded in CyPari, rather than being a separate extension module.
  * Some features have been removed for this special use.
  * 
  * You should have received a copy of the GNU Lesser General Public License
  * along with cysignals.  If not, see <http://www.gnu.org/licenses/>.
  *
  ****************************************************************************/
-
 #define ENABLE_DEBUG_CYSIGNALS 0
 #if ENABLE_DEBUG_CYSIGNALS
 #define DEBUG(...) fprintf(stderr, __VA_ARGS__); fflush(stderr);
 #else
 #define DEBUG(...)
 #endif
 
@@ -62,23 +61,14 @@
 static sigset_t sigmask_with_sigint;
 
 
 static void do_raise_exception(int sig);
 static void sigdie(int sig, const char* s);
 static void print_backtrace(void);
 
-static inline void reset_CPU(void)
-{
-#if defined(__x86_64__)
-    /* Clear FPU tag word */
-    asm("emms");
-#endif
-}
-
-
 /* Handler for SIGHUP, SIGINT, SIGALRM
  *
  * Inside sig_on() (i.e. when cysigs.sig_on_count is positive), this
  * raises an exception and jumps back to sig_on().
  * Outside of sig_on(), we set Python's interrupt flag using
  * PyErr_SetInterrupt() */
 static void cysigs_interrupt_handler(int sig)
@@ -88,15 +78,14 @@
     {
       if (!cysigs.block_sigint && !PARI_SIGINT_block)
         {
             /* Raise an exception so Python can see it */
             do_raise_exception(sig);
 
             /* Jump back to sig_on() (the first one if there is a stack) */
-            reset_CPU();
             siglongjmp(cysigs.env, sig);
         }
     }
     else
     {
         /* Set the Python interrupt indicator, which will cause the
          * Python-level interrupt handler in cysignals/signals.pyx to
@@ -130,15 +119,14 @@
     {
         /* We are inside sig_on(), so we can handle the signal! */
         DEBUG("Inside sig_on-sig_off -- calling siglongjmp.\n")
         /* Raise an exception so Python can see it */
         do_raise_exception(sig);
 
         /* Jump back to sig_on() (the first one if there is a stack) */
-        reset_CPU();
         siglongjmp(cysigs.env, sig);
     }
     else
     {
         /* We are outside sig_on() and have no choice but to terminate Python */
         DEBUG("Outside sig-on-sig_off -- terminating Python.\n")
 
@@ -335,15 +323,15 @@
 #include <string.h>
 #include <limits.h>
 #include <sys/types.h>
 #include <Python.h>
 #include <stdlib.h>
 #include <pari/pari.h>
 #include "struct_signals.h"
-#include <Windows.h>
+#include <windows.h>
 #include <float.h>
 
 #ifndef __MINGW32__
 #  define inline __inline
 #endif
 /* The cysigs object (there is a unique copy of this, shared by all
  * Cython modules using cysignals) */
```

### Comparing `cypari-2.5.0/cypari/memory.py` & `cypari-2.5.4/cypari/memory.py`

 * *Files identical despite different names*

### Comparing `cypari-2.5.0/cypari/test.py` & `cypari-2.5.4/cypari/test.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,30 +62,29 @@
         docstring = getattr(cls.__dict__[key], '__doc__')
         if isinstance(docstring, str):
             if docstring.find('sage:') >= 0 and docstring.find('>>>') < 0:
                 _pari.__test__['%s.%s (line 0)'%(cls.__name__, key)] = docstring
 
 # We skip tests for the _close method, which is unused, marked dangerous,
 # and causes segfaults.
-bad_tests = ['Pari._close (line 0)', 'Pari._close']
+bad_tests = (
+    '__test__.Pari._close (line 0)',
+)
 
 def runtests(verbose=False):
     parser = DocTestParser()
     finder = doctest.DocTestFinder(parser=parser)
     failed, attempted = 0, 0
     for module, extra_globals in modules_to_test:
         print('Running doctests in %s:'%module.__name__)
         runner = doctest.DocTestRunner(
             verbose=verbose,
             optionflags=doctest.ELLIPSIS|doctest.IGNORE_EXCEPTION_DETAIL)
         count = 0
         for test in finder.find(module, extraglobs=extra_globals):
-            if any(test.name.endswith(bad_test) for bad_test in bad_tests):
-                print('skipping %s'%test.name.split()[0])
-                continue
             count += 1
             runner.run(test)
         result = runner.summarize()
         failed += result.failed
         attempted += result.attempted
         print(result)
         print()
```

### Comparing `cypari-2.5.0/cypari/long_hack.h` & `cypari-2.5.4/cypari/long_hack.h`

 * *Files identical despite different names*

### Comparing `cypari-2.5.0/cypari/macros.h` & `cypari-2.5.4/cypari/macros.h`

 * *Files 2% similar despite different names*

```diff
@@ -269,16 +269,17 @@
 /* This is called by Pari's cb_pari_err_recover callback.
  * In Posix this sends a SIGABRT.  In Windows this raises SIGFPE
  * with an out-of-range mapped signal.  The signal handler should
  * either do a longjmp back to the last sig_on, or schedule one for later.
  */
 static inline void sig_error(void)
 {
+#if defined(__MINGW32__) || defined(_WIN32)
     void (*old_handler)(int);
-    (void) old_handler;
+#endif
     DEBUG( "sig_error called with count %d\n", cysigs.sig_on_count)
     if (unlikely(cysigs.sig_on_count <= 0))
     {
         fprintf(stderr, "sig_error() without sig_on()\n");
     }
 #if defined(__MINGW32__) || defined(_WIN32)
     /*
```

### Comparing `cypari-2.5.0/cypari/struct_signals.h` & `cypari-2.5.4/cypari/struct_signals.h`

 * *Files identical despite different names*

### Comparing `cypari-2.5.0/cypari/tests.py` & `cypari-2.5.4/cypari/tests.py`

 * *Files 0% similar despite different names*

```diff
@@ -209,15 +209,15 @@
     [2, 4]~*x + [1, 3]~
 
     >>> pari(3).Qfb(7, 1)
     Qfb(3, 7, 1)
     >>> pari(3).Qfb(7, 2)
     Traceback (most recent call last):
     ...
-    PariError: domain error in Qfb: issquare(disc) = 1
+    cypari_pari.PariError: domain error in Qfb: issquare(disc) = 1
 
     >>> pari([1,5,2]).Set()
     [1, 2, 5]
     >>> pari([]).Set()
     []
     >>> pari([1,1,-1,-1,3,3]).Set()
     [-1, 1, 3]
@@ -235,26 +235,26 @@
     >>> _.Strchr()
     "Sage"
     >>> pari([83, 97, 103, 101]).Strchr()
     "Sage"
 
 Basic functions::
 
-    >>> pari(0).binary()
-    []
-    >>> pari(-5).binary()
-    [1, 0, 1]
-    >>> pari(5).binary()
-    [1, 0, 1]
-    >>> pari(2005).binary()
-    [1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1]
-    >>> pari('"2"').binary()
-    Traceback (most recent call last):
-    ...
-    PariError: incorrect type in binary (t_STR)
+     >>> pari(0).binary()
+     []
+     >>> pari(-5).binary()
+     [1, 0, 1]
+     >>> pari(5).binary()
+     [1, 0, 1]
+     >>> pari(2005).binary()
+     [1, 1, 1, 1, 1, 0, 1, 0, 1, 0, 1]
+     >>> pari('"2"').binary()
+     Traceback (most recent call last):
+     ...
+     PariError: incorrect type in binary (t_STR)
 
     >>> pari(1.4).ceil()
     2
     >>> pari(-1.4).ceil()
     -1
     >>> pari('3/4').ceil()
     1
@@ -614,31 +614,26 @@
 
     >>> pari(1.5).cos()
     0.0707372016677029
     >>> pari('1+I').cos()
     0.833730025131149 - 0.988897705762865*I
     >>> pari('x+O(x^8)').cos()
     1 - 1/2*x^2 + 1/24*x^4 - 1/720*x^6 + 1/40320*x^8 + O(x^9)
+
     >>> pari(1.5).cosh()
     2.35240961524325
     >>> pari('1+I').cosh()
     0.833730025131149 + 0.988897705762865*I
     >>> pari('x+O(x^8)').cosh()
     1 + 1/2*x^2 + 1/24*x^4 + 1/720*x^6 + 1/40320*x^8 + O(x^9)
-
-# With some Python versions this does the division and produces
-# 1.99339881490586 E19 as the result.
-#    >>> pari(5).cotan()
-#    -0.295812915532746
-#    >>> x = pari.pi()
-#    >>> pari(x).cotan()
-#    Traceback (most recent call last):
-#    ...
-#    PariError: impossible inverse in divrr: 0.E-18
-
+    >>> pari(5).cotan()
+    -0.295812915532746
+    >>> x = pari.pi()
+    >>> pari(x).cotan()
+    1.99339881490586 E19
     >>> pari(1).dilog()
     1.64493406684823
     >>> pari('1+I').dilog()
     0.616850275068085 + 1.46036211675312*I
 
     >>> pari(1).erfc()
     0.157299207050285
@@ -1382,15 +1377,15 @@
     True
 
     >>> nf = pari('y^2 - 5').nfinit()
     >>> P = nf.idealprimedec(5)[0]
     >>> Q = nf.idealprimedec(2)[0]
     >>> moduli = pari.matrix(2,2,[P,4,Q,4])
     >>> residues = pari.vector(2,[0,1])
-    >>> v = nf.idealchinese(moduli, residues)
+    >>> v = nf.idealchinese(moduli,residues)
     >>> b = v + 0*nf.nfgenerator()
     >>> nf.idealval(b, P)
     4
     >>> nf.idealval(b-1, Q)
     4
 
     >>> nf = pari('x^3 - 2').nfinit()
@@ -1491,18 +1486,16 @@
     >>> I = [Kp.nfalgtobasis(2), Kp.nfalgtobasis(3+b**2), Kp.nfalgtobasis(1), Kp.nfalgtobasis(1)]
     >>> Kp.nfhnf([A,I])
     [[1, [15, 6]~, [0, -54]~, [113, 72]~; 0, 1, [-4, -1]~, [0, -1]~; 0, 0, 1, 0; 0, 0, 0, 1], [[360, 180; 0, 180], [6, 4; 0, 2], [1, 0]~, 1]]
     >>> A = pari('[1,0,0,5*b; 1,2*b,b,57; 0,2,1,b-3; 2,0,b,b]')
     >>> I = [Kp.idealprimedec(2)[0][1],Kp.nfalgtobasis(3+b),Kp.nfalgtobasis(1),Kp.nfalgtobasis(1)]
     >>> Kp.nfhnf([A, I])
     [[1, [7605, 4]~, [-8110, -51]~, [2313, 50]~; 0, 1, 0, -1; 0, 0, 1, 0; 0, 0, 0, 1], [[19320, 2520; 0, 168], [2, 1; 0, 1], 1, 1]]
-
     >>> pari('x^3 - 17').nfinit()
     [x^3 - 17, [1, 1], -867, 3, [[1, 1.68006914259990, 2.57128159065824; 1, -0.340034571299952 - 2.65083754153991*I, -1.28564079532912 + 2.22679517779329*I], [1, 1.68006914259990, 2.57128159065824; 1, -2.99087211283986, 0.941154382464174; 1, 2.31080297023995, -3.51243597312241], [16, 27, 41; 16, -48, 15; 16, 37, -56], [3, 1, 0; 1, -11, 17; 0, 17, 0], [51, 0, 16; 0, 17, 3; 0, 0, 1], [17, 0, -1; 0, 0, 3; -1, 3, 2], [51, [-17, 6, -1; 0, -18, 3; 1, 0, -16]], [3, 17]], [2.57128159065824, -1.28564079532912 + 2.22679517779329*I], [3, x^2 - x + 1, 3*x], [1, 0, -1; 0, 0, 3; 0, 1, 1], [1, 0, 0, 0, -4, 6, 0, 6, -1; 0, 1, 0, 1, 1, -1, 0, -1, 3; 0, 0, 1, 0, 2, 0, 1, 0, 1]]
-
     >>> pari('x^2 + 10^100 + 1').nfinit()
     [...]
     >>> pari('1.0').nfinit()
     Traceback (most recent call last):
     ...
     PariError: incorrect type in checknf [please apply nfinit()] (t_REAL)
     >>> F = pari('y^3-2').nfinit()
@@ -1651,22 +1644,23 @@
 
     >>> f = pari('y^3+y+1')
     >>> K = f.nfinit()
     >>> x = pari('x'); y = pari('y')
     >>> g = x**5 - x**2 + y
     >>> L = K.rnfinit(g)
 
-    >>> pari(-23).quadhilbert()
-    x^3 - x^2 + 1
-    >>> pari(145).quadhilbert()
-    x^4 - x^3 - 5*x^2 - x + 1
-    >>> pari(-12).quadhilbert()   # Not fundamental
-    Traceback (most recent call last):
-    ...
-    PariError: domain error in quadray: isfundamental(D) = 0
+     >>> pari(-23).quadhilbert()
+     x^3 - x^2 + 1
+
+     >>> pari(145).quadhilbert()
+     x^4 - x^3 - 5*x^2 - x + 1
+     >>> pari(-12).quadhilbert()   # Not fundamental
+     Traceback (most recent call last):
+     ...
+     PariError: domain error in quadray: isfundamental(D) = 0
 
     # Closures
 
     >>> def the_answer():
     ...     return 42
     >>> f = pari(the_answer)
     >>> f()
```

### Comparing `cypari-2.5.0/cypari/py3tests.py` & `cypari-2.5.4/cypari/py3tests.py`

 * *Files identical despite different names*

### Comparing `cypari-2.5.0/cypari/py2tests.py` & `cypari-2.5.4/cypari/py2tests.py`

 * *Files identical despite different names*

