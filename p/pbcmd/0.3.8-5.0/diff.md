# Comparing `tmp/pbcmd-0.3.8.tar.gz` & `tmp/pbcmd-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pbcmd-0.3.8.tar", last modified: Thu Sep  2 21:09:28 2021, max compression
+gzip compressed data, was "pbcmd-5.0.tar", last modified: Tue Dec  6 03:05:39 2022, max compression
```

## Comparing `pbcmd-0.3.8.tar` & `pbcmd-5.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2021-09-02 21:09:28.136238 pbcmd-0.3.8/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-0.3.8/.gitignore
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      846 2021-09-02 21:09:28.136238 pbcmd-0.3.8/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-0.3.8/README.rst
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      142 2021-07-29 14:42:18.000000 pbcmd-0.3.8/pyproject.toml
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      650 2021-09-02 21:09:28.136238 pbcmd-0.3.8/setup.cfg
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2021-07-29 14:46:15.000000 pbcmd-0.3.8/setup.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2021-09-02 21:09:28.136238 pbcmd-0.3.8/src/
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2021-09-02 21:09:28.136238 pbcmd-0.3.8/src/pbcmd/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-0.3.8/src/pbcmd/__init__.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      284 2021-07-29 14:50:23.000000 pbcmd-0.3.8/src/pbcmd/calc.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      766 2021-09-02 20:09:18.000000 pbcmd-0.3.8/src/pbcmd/cli.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5336 2021-09-02 20:19:33.000000 pbcmd-0.3.8/src/pbcmd/cpush.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2976 2021-07-29 14:58:44.000000 pbcmd-0.3.8/src/pbcmd/csplit.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2021-07-29 15:08:55.000000 pbcmd-0.3.8/src/pbcmd/git.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-0.3.8/src/pbcmd/hello.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2021-07-29 15:10:29.000000 pbcmd-0.3.8/src/pbcmd/mail.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2021-07-29 15:11:20.000000 pbcmd-0.3.8/src/pbcmd/obscure.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      927 2021-07-29 15:13:01.000000 pbcmd-0.3.8/src/pbcmd/proxy.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2021-07-29 15:14:55.000000 pbcmd-0.3.8/src/pbcmd/pyon2json.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-0.3.8/src/pbcmd/rm_timestamped.py
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2021-07-29 15:17:45.000000 pbcmd-0.3.8/src/pbcmd/timefmt.py
-drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2021-09-02 21:09:28.136238 pbcmd-0.3.8/src/pbcmd.egg-info/
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      846 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/PKG-INFO
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)      517 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/SOURCES.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/dependency_links.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/entry_points.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)       49 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/requires.txt
--rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2021-09-02 21:09:28.000000 pbcmd-0.3.8/src/pbcmd.egg-info/top_level.txt
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2022-12-06 03:05:39.743583 pbcmd-5.0/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2035 2020-12-15 02:52:07.000000 pbcmd-5.0/.gitignore
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2022-12-06 03:05:39.743583 pbcmd-5.0/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      245 2021-08-03 13:23:21.000000 pbcmd-5.0/README.rst
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      729 2022-12-06 03:00:21.000000 pbcmd-5.0/pyproject.toml
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       38 2022-12-06 03:05:39.743583 pbcmd-5.0/setup.cfg
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2022-12-06 02:55:21.000000 pbcmd-5.0/setup.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2022-12-06 03:05:39.743583 pbcmd-5.0/src/
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2022-12-06 03:05:39.743583 pbcmd-5.0/src/pbcmd/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        0 2021-07-29 14:48:36.000000 pbcmd-5.0/src/pbcmd/__init__.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      284 2022-12-06 02:39:31.000000 pbcmd-5.0/src/pbcmd/calc.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      766 2021-09-02 20:09:18.000000 pbcmd-5.0/src/pbcmd/cli.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     5649 2022-09-30 15:21:25.000000 pbcmd-5.0/src/pbcmd/cpush.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     2729 2022-12-06 02:43:41.000000 pbcmd-5.0/src/pbcmd/csplit.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     6585 2022-12-06 02:43:49.000000 pbcmd-5.0/src/pbcmd/git.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      208 2021-07-29 15:09:35.000000 pbcmd-5.0/src/pbcmd/hello.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1783 2022-12-06 02:43:54.000000 pbcmd-5.0/src/pbcmd/mail.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1773 2022-12-06 02:45:17.000000 pbcmd-5.0/src/pbcmd/obscure.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1069 2021-09-07 16:30:06.000000 pbcmd-5.0/src/pbcmd/proxy.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1688 2022-12-06 02:47:02.000000 pbcmd-5.0/src/pbcmd/pyon2json.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)     1891 2021-07-29 15:15:52.000000 pbcmd-5.0/src/pbcmd/rm_timestamped.py
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      746 2022-12-06 02:47:15.000000 pbcmd-5.0/src/pbcmd/timefmt.py
+drwxr-xr-x   0 parantapa  (1000) parantapa  (1000)        0 2022-12-06 03:05:39.743583 pbcmd-5.0/src/pbcmd.egg-info/
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      667 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/PKG-INFO
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)      507 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/SOURCES.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        1 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/dependency_links.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       37 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/entry_points.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)       49 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/requires.txt
+-rw-r--r--   0 parantapa  (1000) parantapa  (1000)        6 2022-12-06 03:05:39.000000 pbcmd-5.0/src/pbcmd.egg-info/top_level.txt
```

### Comparing `pbcmd-0.3.8/.gitignore` & `pbcmd-5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/cli.py` & `pbcmd-5.0/src/pbcmd/cli.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/cpush.py` & `pbcmd-5.0/src/pbcmd/cpush.py`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from subprocess import run, CalledProcessError
 
 import json5
 import click
 from pydantic import BaseModel, ValidationError
 from pydantic.types import DirectoryPath
 
-LOCAL_CONFIG_FILE = ".cpush.json"
+LOCAL_CONFIG_FILE = ".cpush.json5"
 GLOBAL_CONFIG_FILE = Path("~/.config/cpush/cpush.json").expanduser()
 ROOT = Path("/")
 
 
 RemotePath = NewType("RemotePath", str)
 BorgRepo = NewType("BorgRepo", Path)
 
@@ -130,62 +130,78 @@
 
 class GlobalConfig(BaseModel):
     """Global configuration."""
 
     backup_dir: DirectoryPath
 
 
+def do_cpush(
+    gconfig: GlobalConfig, lconfig: LocalConfig, remote: str, project_dir: Path
+):
+    click.secho(f"Using remote: {remote}", fg="yellow")
+
+    remote_dir = lconfig.remotes[remote]
+    backup_dir = gconfig.backup_dir / lconfig.project / remote / "remote_backup"
+    borg_repo = gconfig.backup_dir / lconfig.project / "borg_repo"
+
+    borg_repo = cast(BorgRepo, borg_repo)
+
+    if not backup_dir.is_dir():
+        backup_dir.mkdir(0o700, parents=True, exist_ok=True)
+    if not borg_repo.is_dir():
+        borg_init(borg_repo)
+
+    now = datetime.now().replace(microsecond=0).isoformat()
+
+    borg_create(f"local-{now}", project_dir, borg_repo)
+    rsync_pull(remote_dir, backup_dir)
+    borg_create(f"{remote}-{now}", backup_dir, borg_repo)
+    borg_prune(borg_repo)
+    rsync_push(remote_dir, project_dir)
+
+
 @click.command()
-@click.argument("to", type=str, default="")
+@click.argument("to", type=str, default="ALL")
 def cpush(to: str):
-    """Push code to remote directory."""
+    """Push code to remote directory.
+
+    pb cpush <remote>
+    """
     try:
         gconfig = GLOBAL_CONFIG_FILE.read_text()
         gconfig = json5.loads(gconfig)
         gconfig = GlobalConfig.parse_obj(gconfig)
 
         lconfig = find_config(Path.cwd())
         project_dir = lconfig.parent
 
         lconfig = lconfig.read_text()
         lconfig = json5.loads(lconfig)
         lconfig = LocalConfig.parse_obj(lconfig)
 
-        if to == "":
-            if len(lconfig.remotes) == 1:
-                remote = list(lconfig.remotes.keys())[0]
-            else:
-                raise click.UsageError("Multiple remotes available; must specify one.")
+        if to == "ALL":
+            for remote in list(lconfig.remotes.keys()):
+                do_cpush(
+                    gconfig=gconfig,
+                    lconfig=lconfig,
+                    remote=remote,
+                    project_dir=project_dir,
+                )
         else:
             if to in lconfig.remotes:
                 remote = to
+                do_cpush(
+                    gconfig=gconfig,
+                    lconfig=lconfig,
+                    remote=remote,
+                    project_dir=project_dir,
+                )
             else:
                 raise click.UsageError(f"Remote {to} not defined in local config.")
 
-        click.secho(f"Using remote: {remote}", fg="yellow")
-
-        remote_dir = lconfig.remotes[remote]
-        backup_dir = gconfig.backup_dir / lconfig.project / remote / "remote_backup"
-        borg_repo = gconfig.backup_dir / lconfig.project / remote / "borg_repo"
-
-        borg_repo = cast(BorgRepo, borg_repo)
-
-        if not backup_dir.is_dir():
-            backup_dir.mkdir(0o700, parents=True, exist_ok=True)
-        if not borg_repo.is_dir():
-            borg_init(borg_repo)
-
-        now = datetime.now().replace(microsecond=0).isoformat()
-
-        borg_create(f"local-{now}", project_dir, borg_repo)
-        rsync_pull(remote_dir, backup_dir)
-        borg_create(f"remote-{now}", backup_dir, borg_repo)
-        borg_prune(borg_repo)
-        rsync_push(remote_dir, project_dir)
-
         click.secho("Code push finished completed successfully", fg="green")
     except (RuntimeError, FileNotFoundError, ValidationError) as e:
         click.secho(e, fg="red")
         sys.exit(1)
 
 
 if __name__ == "__main__":
```

### Comparing `pbcmd-0.3.8/src/pbcmd/csplit.py` & `pbcmd-5.0/src/pbcmd/csplit.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,14 +8,25 @@
 import click
 from tqdm import tqdm
 
 COMP_OPEN = {"gzip": gzip.open, "bz2": bz2.open, "xz": lzma.open, "text": open}
 COMP_OPTION_TYPE = click.Choice(list(COMP_OPEN) + ["infer"])
 
 
+def infer_compression(fname: str) -> str:
+    if fname.endswith(".gz"):
+        return "gzip"
+    elif fname.endswith(".bz2"):
+        return "bz2"
+    elif fname.endswith(".xz"):
+        return "xz"
+    else:
+        return "text"
+
+
 @click.command()
 @click.option(
     "-n",
     "--lines-per-file",
     default=1000,
     show_default=True,
     help="Maximum number of lines per output file",
@@ -55,32 +66,18 @@
 ):
     """Split a large compressed text file into multiple smaller (compressed) text files.
 
     {index} in output_file_format will be replaced by index of the output file.
     index of output files start from 0
     """
     if input_compression == "infer":
-        if input_file.endswith(".gz"):
-            input_compression = "gzip"
-        elif input_file.endswith(".bz2"):
-            input_compression = "bz2"
-        elif input_file.endswith(".xz"):
-            input_compression = "xz"
-        else:
-            input_compression = "text"
+        input_compression = infer_compression(input_file)
 
     if output_compression == "infer":
-        if output_file_format.endswith(".gz"):
-            output_compression = "gzip"
-        elif output_file_format.endswith(".bz2"):
-            output_compression = "bz2"
-        elif output_file_format.endswith(".xz"):
-            output_compression = "xz"
-        else:
-            output_compression = "text"
+        output_compression = infer_compression(output_file_format)
 
     if "{index}" not in output_file_format:
         raise click.UsageError("Output file format string doesn't contain '{index}'")
 
     in_open = COMP_OPEN[input_compression]
     out_open = COMP_OPEN[output_compression]
```

### Comparing `pbcmd-0.3.8/src/pbcmd/git.py` & `pbcmd-5.0/src/pbcmd/git.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/mail.py` & `pbcmd-5.0/src/pbcmd/mail.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/obscure.py` & `pbcmd-5.0/src/pbcmd/obscure.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/proxy.py` & `pbcmd-5.0/src/pbcmd/proxy.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,38 +1,42 @@
 """Start a ssh based socks proxy using autossh."""
 
+import shlex
+
 import click
-from subprocess import run
+from subprocess import run, CalledProcessError
 
 
 @click.command()
 @click.option(
     "-p", "--port", default=12001, show_default=True, help="Local port to listen on."
 )
 @click.option("-v", "--verbose", count=True, help="Verbosity level.")
 @click.argument("host", type=str, nargs=1)
 def proxy(port, verbose, host):
     """Start a ssh proxy on local port to remove host."""
     click.secho(f"Starting proxy to {host} on port {port}", fg="green")
 
-    # fmt: off
-    options = [
-        "-M", "0",
-        "-o", "ServerAliveInterval 10",
-        "-o", "ServerAliveCountMax 3",
-        "-o", "ExitOnForwardFailure=yes",
-        "-N",
-        "-S", "none",
-        "-D",
-        f"127.0.0.1:{port}",
-    ]
-    # fmt: on
+    options = f"""
+        -M 0
+        -S none
+        -o ServerAliveInterval=10
+        -o ServerAliveCountMax=3
+        -o ExitOnForwardFailure=yes
+        -o BatchMode=yes
+        -N
+        -D
+        127.0.0.1:{port}
+        """
+    options = shlex.split(options)
 
     for _ in range(verbose):
         options.append("-v")
 
     cmd = ["autossh"] + options + [host]
-    run(cmd, check=True)
-
+    try:
+        run(cmd, check=True)
+    except CalledProcessError as e:
+        click.secho(f"Proxy command failed\n{e}", fg="red")
 
 if __name__ == "__main__":
     proxy()
```

### Comparing `pbcmd-0.3.8/src/pbcmd/pyon2json.py` & `pbcmd-5.0/src/pbcmd/pyon2json.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/rm_timestamped.py` & `pbcmd-5.0/src/pbcmd/rm_timestamped.py`

 * *Files identical despite different names*

### Comparing `pbcmd-0.3.8/src/pbcmd/timefmt.py` & `pbcmd-5.0/src/pbcmd/timefmt.py`

 * *Files identical despite different names*

