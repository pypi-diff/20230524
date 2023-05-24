# Comparing `tmp/listupy-0.0.0.tar.gz` & `tmp/listupy-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "listupy-0.0.0.tar", last modified: Wed May 24 10:41:00 2023, max compression
+gzip compressed data, was "listupy-0.1.0.tar", last modified: Wed May 24 10:54:54 2023, max compression
```

## Comparing `listupy-0.0.0.tar` & `listupy-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-24 10:41:00.025202 listupy-0.0.0/
--rw-rw-rw-   0        0        0     1175 2023-05-24 10:41:00.024132 listupy-0.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      450 2023-05-24 10:10:20.000000 listupy-0.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-24 10:40:59.991404 listupy-0.0.0/listupy/
--rw-rw-rw-   0        0        0     1565 2023-05-24 10:40:08.000000 listupy-0.0.0/listupy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:41:00.022954 listupy-0.0.0/listupy/parts/
--rw-rw-rw-   0        0        0       41 2023-05-24 10:14:06.000000 listupy-0.0.0/listupy/parts/test_python_file.py
--rw-rw-rw-   0        0        0      284 2023-05-24 10:39:39.000000 listupy-0.0.0/listupy/test.py
-drwxrwxrwx   0        0        0        0 2023-05-24 10:41:00.020952 listupy-0.0.0/listupy.egg-info/
--rw-rw-rw-   0        0        0     1175 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      276 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       24 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/requires.txt
--rw-rw-rw-   0        0        0       22 2023-05-24 10:40:59.000000 listupy-0.0.0/listupy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-24 10:41:00.025202 listupy-0.0.0/setup.cfg
--rw-rw-rw-   0        0        0      984 2023-05-24 10:11:58.000000 listupy-0.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:54:54.074769 listupy-0.1.0/
+-rw-rw-rw-   0        0        0     4871 2023-05-24 10:54:54.073763 listupy-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3606 2023-05-24 10:54:15.000000 listupy-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-24 10:54:54.043623 listupy-0.1.0/listupy/
+-rw-rw-rw-   0        0        0     1638 2023-05-24 10:45:17.000000 listupy-0.1.0/listupy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:54:54.072112 listupy-0.1.0/listupy/parts/
+-rw-rw-rw-   0        0        0       41 2023-05-24 10:14:06.000000 listupy-0.1.0/listupy/parts/test_python_file.py
+-rw-rw-rw-   0        0        0      284 2023-05-24 10:39:39.000000 listupy-0.1.0/listupy/test.py
+drwxrwxrwx   0        0        0        0 2023-05-24 10:54:54.070153 listupy-0.1.0/listupy.egg-info/
+-rw-rw-rw-   0        0        0     4871 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      276 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       24 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       22 2023-05-24 10:54:53.000000 listupy-0.1.0/listupy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-24 10:54:54.074769 listupy-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      984 2023-05-24 10:54:50.000000 listupy-0.1.0/setup.py
```

### Comparing `listupy-0.0.0/listupy/__init__.py` & `listupy-0.1.0/listupy/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,25 +27,25 @@
 	return ret_n
 
 # pythonファイルのリストアップ [listupy]
 def listup(dir_name):
 	# 再帰的にpythonファイルをすべて列挙
 	file_ls = r_listup(dir_name)
 	# 統計情報
-	res = f"# listupy レポート\n\n## サマリ\n合計{line_n(file_ls)}行; {len(file_ls)}ファイル\n\n"
+	res = f"# listupy report\n\n## summary\n- {line_n(file_ls)} lines\n- {len(file_ls)} files\n\n"
 	# 各ファイルの内容を足していく
 	for filename, content in file_ls:
 		res += f"## {filename}\n```python\n{content}\n```\n\n"
 	return res
 
 # コンソールから利用
 def console_command():
 	# コンソール引数
 	parser = argparse.ArgumentParser()
 	parser.add_argument("-i", "--input", required = True, help = "Target directory name.")
 	parser.add_argument("-o", "--output", required = False, help = "Output text filepath.")
 	args_dic = vars(parser.parse_args())
-	# debug
-	print(args_dic)
-	sys.exit()
 	# pythonファイルのリストアップ [listupy]
 	res = listup(args_dic["input"])
+	# 出力
+	if args_dic["output"] is None: args_dic["output"] = "./listup_result.md"
+	fies[args_dic["output"], "text"] = res
```

### Comparing `listupy-0.0.0/setup.py` & `listupy-0.1.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # 公開用パッケージの作成 [ezpip]
 import ezpip
 
 # 公開用パッケージの作成 [ezpip]
 with ezpip.packager(develop_dir = "./_develop_listupy/") as p:
 	setup(
 		name = "listupy",
-		version = "0.0.0",
+		version = "0.1.0",
 		description = "A tool that recursively enumerates Python files within a folder, calculates the total number of lines, and compiles them into a single Markdown text.",
 		author = "bib_inf",
 		author_email = "contact.bibinf@gmail.com",
 		url = "https://github.co.jp/",
 		packages = p.packages,
 		install_requires = ["relpath", "ezpip", "sout", "fies"],
 		long_description = p.long_description,
```

