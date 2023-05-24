# Comparing `tmp/geovisio_cli-0.1.0.tar.gz` & `tmp/geovisio_cli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geovisio_cli-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "geovisio_cli-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `geovisio_cli-0.1.0.tar` & `geovisio_cli-0.2.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
--rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/.gitignore
--rw-r--r--   0        0        0     1732 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/.gitlab-ci.yml
--rw-r--r--   0        0        0     2558 2023-05-17 11:11:47.310135 geovisio_cli-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/LICENSE
--rw-r--r--   0        0        0      551 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/Makefile
--rw-r--r--   0        0        0     7467 2023-05-15 17:41:10.367730 geovisio_cli-0.1.0/README.md
--rw-r--r--   0        0        0     2502 2023-05-15 08:17:13.338400 geovisio_cli-0.1.0/USAGE.md
--rw-r--r--   0        0        0       53 2023-05-17 11:11:47.310135 geovisio_cli-0.1.0/geovisio_cli/__init__.py
--rw-r--r--   0        0        0     1937 2023-05-16 14:39:06.445129 geovisio_cli-0.1.0/geovisio_cli/auth.py
--rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.1.0/geovisio_cli/exception.py
--rw-r--r--   0        0        0     4182 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/geovisio_cli/main.py
--rw-r--r--   0        0        0      173 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/geovisio_cli/model.py
--rw-r--r--   0        0        0    19722 2023-05-17 11:07:32.865046 geovisio_cli-0.1.0/geovisio_cli/sequence.py
--rw-r--r--   0        0        0      948 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.1.0/tests/fixtures/e1.jpg
--rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/e2.jpg
--rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/e3.jpg
--rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/invalid_pic.jpg
--rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/fixtures/not_a_pic.md
--rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/integration/__init__.py
--rw-r--r--   0        0        0      865 2023-03-14 15:26:20.141986 geovisio_cli-0.1.0/tests/integration/conftest.py
--rw-r--r--   0        0        0      651 2023-05-12 13:36:09.582468 geovisio_cli-0.1.0/tests/integration/docker-compose-geovisio.yml
--rw-r--r--   0        0        0      369 2023-05-15 08:17:13.342400 geovisio_cli-0.1.0/tests/integration/test_status.py
--rw-r--r--   0        0        0     8012 2023-05-15 17:46:58.046466 geovisio_cli-0.1.0/tests/integration/test_upload.py
--rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.1.0/tests/test_process.py
--rw-r--r--   0        0        0     2579 2023-05-15 17:51:20.171581 geovisio_cli-0.1.0/tests/test_sequence.py
--rw-r--r--   0        0        0     8411 1970-01-01 00:00:00.000000 geovisio_cli-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       47 2023-03-24 13:15:13.689899 geovisio_cli-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1371 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     3132 2023-05-24 13:20:49.654423 geovisio_cli-0.2.0/CHANGELOG.md
+-rw-r--r--   0        0        0     5468 2023-03-24 13:15:13.689899 geovisio_cli-0.2.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     1070 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/LICENSE
+-rw-r--r--   0        0        0      590 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/Makefile
+-rw-r--r--   0        0        0     7516 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/README.md
+-rw-r--r--   0        0        0     2792 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/USAGE.md
+-rw-r--r--   0        0        0       53 2023-05-24 13:20:49.654423 geovisio_cli-0.2.0/geovisio_cli/__init__.py
+-rw-r--r--   0        0        0     6173 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/auth.py
+-rw-r--r--   0        0        0      284 2023-04-14 11:12:54.559203 geovisio_cli-0.2.0/geovisio_cli/exception.py
+-rw-r--r--   0        0        0     5455 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/main.py
+-rw-r--r--   0        0        0      136 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/model.py
+-rw-r--r--   0        0        0    18222 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/sequence.py
+-rw-r--r--   0        0        0     1457 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/geovisio_cli/utils.py
+-rw-r--r--   0        0        0      971 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/__init__.py
+-rw-r--r--   0        0        0      191 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/conftest.py
+-rw-r--r--   0        0        0   523332 2023-03-14 15:26:20.137987 geovisio_cli-0.2.0/tests/fixtures/e1.jpg
+-rw-r--r--   0        0        0   483454 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/e2.jpg
+-rw-r--r--   0        0        0   529344 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/e3.jpg
+-rw-r--r--   0        0        0       16 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/invalid_pic.jpg
+-rw-r--r--   0        0        0       27 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/fixtures/not_a_pic.md
+-rw-r--r--   0        0        0        0 2023-03-14 15:26:20.141986 geovisio_cli-0.2.0/tests/integration/__init__.py
+-rw-r--r--   0        0        0     3327 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/conftest.py
+-rw-r--r--   0        0        0     2189 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/tests/integration/docker-compose-geovisio.yml
+-rw-r--r--   0        0        0      584 2023-05-22 08:59:23.607560 geovisio_cli-0.2.0/tests/integration/docker-compose-gitlab-override.yml
+-rw-r--r--   0        0        0    76457 2023-05-22 08:59:23.611560 geovisio_cli-0.2.0/tests/integration/keycloak-realm.json
+-rw-r--r--   0        0        0     3222 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_auth.py
+-rw-r--r--   0        0        0      369 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_status.py
+-rw-r--r--   0        0        0     8178 2023-05-24 13:17:27.558420 geovisio_cli-0.2.0/tests/integration/test_upload.py
+-rw-r--r--   0        0        0      583 2023-05-10 11:47:16.328656 geovisio_cli-0.2.0/tests/test_process.py
+-rw-r--r--   0        0        0     2579 2023-05-15 17:51:20.171581 geovisio_cli-0.2.0/tests/test_sequence.py
+-rw-r--r--   0        0        0     8491 1970-01-01 00:00:00.000000 geovisio_cli-0.2.0/PKG-INFO
```

### Comparing `geovisio_cli-0.1.0/.gitlab-ci.yml` & `geovisio_cli-0.2.0/.gitlab-ci.yml`

 * *Files 17% similar despite different names*

```diff
@@ -25,28 +25,20 @@
     - black --fast --check .
 
 tests:
   image: python:3.8-alpine
   services:
     - docker:dind
   script:
-    - apk add --update --no-cache docker-cli docker-cli-compose curl
-    - pip install .[dev]
-    - docker compose -f tests/integration/docker-compose-geovisio.yml up -d --wait
-      # additional sleep since Postgres start twice as docker and screw all docker healthcheck mechanisms
-    - sleep 5
-    - docker compose -f tests/integration/docker-compose-geovisio.yml ps
-    - GEOVISIO=$(docker compose -f tests/integration/docker-compose-geovisio.yml port geovisio-api 5000)
-    # Since the docker service is run on another container, we need to cheat and change the geovisio host url
-    - OTHER_URL=$(echo $GEOVISIO | sed 's#0.0.0.0:\(.*\)#http://docker:\1#g')
-    - curl $OTHER_URL || true
-    - pytest -s -vv --external-geovisio-url=$OTHER_URL
+    - apk add --update --no-cache docker-cli docker-cli-compose
+    - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml run --rm integration-test-runner
+
   after_script:
-    - docker compose -f tests/integration/docker-compose-geovisio.yml logs || true
-    - docker compose -f tests/integration/docker-compose-geovisio.yml down || true
+    - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml logs || true
+    - PROJECT_DIR=$PWD docker compose -f tests/integration/docker-compose-geovisio.yml -f tests/integration/docker-compose-gitlab-override.yml down || true
 
 deploy_pypi:
   stage: deploy
   image: python:3.8-alpine
   script:
     - apk add --update --no-cache git
     - pip install .[build]
```

### Comparing `geovisio_cli-0.1.0/CHANGELOG.md` & `geovisio_cli-0.2.0/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,14 +2,25 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.2.0] - 2023-05-24
+
+### Added
+- A new `--token` parameter to `geovisio upload` to provide a custom geovisio token for authentication.
+- A new `geovisio login` command to login on a geovisio instance
+
+### Changed
+- If a geovisio instance has a mandatory login for upload, the upload will ask to register the computer in the user's account first, if the user has not done a `geovisio login` first
+
+### Removed
+- Giving a user/password to `geovisio upload` is deprecated, authentication should use a token.
 
 ## [0.1.0] - 2023-05-17
 
 ### Added
 - A new `--title` parameter to `geovisio upload` and `geovisio test_process` to provide a title to the uploaded collection. If no title is given, it will default to the directory name.
 - Broken uploads can now be recovered: if on a first upload try, some pictures fail, you can re-launch a second upload try by running the same `upload` command. The `_geovisio.toml` stores in a sequence folder which pictures were correctly sent, thus skip them on next try.
 
@@ -46,14 +57,15 @@
 
 ## [0.0.1] - 2023-03-14
 
 ### Added
 - Basic scripts for uploading pictures to a GeoVisio API
 
 
-[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...main
+[Unreleased]: https://gitlab.com/geovisio/cli/-/compare/0.2.0...main
+[0.2.0]: https://gitlab.com/geovisio/cli/-/compare/0.1.0...0.2.0
 [0.1.0]: https://gitlab.com/geovisio/cli/-/compare/0.0.5...0.1.0
 [0.0.5]: https://gitlab.com/geovisio/cli/-/compare/0.0.4...0.0.5
 [0.0.4]: https://gitlab.com/geovisio/cli/-/compare/0.0.3...0.0.4
 [0.0.3]: https://gitlab.com/geovisio/cli/-/compare/0.0.2...0.0.3
 [0.0.2]: https://gitlab.com/geovisio/cli/-/compare/0.0.1...0.0.2
 [0.0.1]: https://gitlab.com/PanierAvide/geovisio/-/commits/0.0.1
```

### Comparing `geovisio_cli-0.1.0/CODE_OF_CONDUCT.md` & `geovisio_cli-0.2.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/LICENSE` & `geovisio_cli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/Makefile` & `geovisio_cli-0.2.0/Makefile`

 * *Files 10% similar despite different names*

```diff
@@ -10,11 +10,11 @@
 
 fmt: ## Format code
 	black --fast .
 
 ci: type-check fmt test ## Run all check like the ci
 
 docs:  ## Generates documentation from Typer embedded docs
-	python -m typer_cli ./geovisio_cli/main.py utils docs --name geovisio --output USAGE.md
+	XDG_CONFIG_HOME='/home/a_user/.config' python -m typer_cli ./geovisio_cli/main.py utils docs --name geovisio --output USAGE.md
 
 help: ## Print this help message
 	@grep -E '^[a-zA-Z_-]+:.*## .*$$' $(MAKEFILE_LIST) | awk 'BEGIN {FS = ":.*?## "}; {printf "\033[36m%-30s\033[0m %s\n", $$1, $$2}'
```

### Comparing `geovisio_cli-0.1.0/README.md` & `geovisio_cli-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -118,21 +118,25 @@
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
 Note that you can launch again the same command to recover a partial sequence import, for example if only some pictures failed to upload.
 
 #### Authentication
 
-If the GeoVisio API requires a login for the upload, the user/password can either be set:
-* with command-line arguments (`--user` / `--password`)
-* with environment variables (`GEOVISIO_USER` / `GEOVISIO_PASSWORD`)
+If the GeoVisio API requires a login for the upload, the `upload` command will ask for a login on the instance by visiting a given url with a browser. 
 
-If no information is set but required by the GeoVisio instance, they will be asked interactively. This is the best way to enter the password so it will not be stored in the command-line history.
+You can also login before hand with the command:
 
-Note: the password is not stored, and sent directly to geovisio. If the future, this will be removed in favor of API keys when geovisio will support those.
+```bash
+geovisio login --api-url http://localhost:5000/
+```
+
+Both will store the credentials in a configuration file, located either in a [XDG](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html) defined directory or in a user specific .config, in a subdirectory `geovisio/config.toml`.
+
+If you do not want to use this, you can also provide a geovisio token with the `--token` parameter.
 
 ### Collection status
 
 Prints the status of a collection.
 
 ```bash
 geovisio collection-status --id <some collection id> --api-url http://localhost:5000
```

### Comparing `geovisio_cli-0.1.0/USAGE.md` & `geovisio_cli-0.2.0/USAGE.md`

 * *Files 17% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 * `--install-completion`: Install completion for the current shell.
 * `--show-completion`: Show completion for the current shell, to copy it or customize the installation.
 * `--help`: Show this message and exit.
 
 **Commands**:
 
 * `collection-status`: Print the status of a collection.
+* `login`: Authenticate into the given instance, and...
 * `test-process`: (For testing) Generates a TOML file with...
 * `upload`: Processes and sends a given sequence on...
 
 ## `geovisio collection-status`
 
 Print the status of a collection.
 
@@ -37,14 +38,33 @@
 
 * `--id TEXT`: Id of the collection
 * `--api-url TEXT`: GeoVisio endpoint URL
 * `--location TEXT`: Full url of the collection
 * `--wait / --no-wait`: wait for all pictures to be ready  [default: no-wait]
 * `--help`: Show this message and exit.
 
+## `geovisio login`
+
+Authenticate into the given instance, and save credentials in a configuration file.
+
+This will generate credentials, and ask the user to visit a page to associate those credentials to the user's account.
+
+The credentials will be stored in /home/a_user/.config/geovisio/config.toml
+
+**Usage**:
+
+```console
+$ geovisio login [OPTIONS]
+```
+
+**Options**:
+
+* `--api-url TEXT`: GeoVisio endpoint URL  [required]
+* `--help`: Show this message and exit.
+
 ## `geovisio test-process`
 
 (For testing) Generates a TOML file with metadata used for upload
 
 **Usage**:
 
 ```console
@@ -73,16 +93,15 @@
 **Arguments**:
 
 * `PATH`: Local path to your sequence folder  [required]
 
 **Options**:
 
 * `--api-url TEXT`: GeoVisio endpoint URL  [required]
-* `--user TEXT`: GeoVisio user name if the geovisio instance needs it.
-If none is provided and the geovisio instance requires it, the username will be asked during run.  [env var: GEOVISIO_USER]
-* `--password TEXT`: GeoVisio password if the geovisio instance needs it.
-If none is provided and the geovisio instance requires it, the password will be asked during run.
-Note: is is advised to wait for prompt without using this variable.  [env var: GEOVISIO_PASSWORD]
 * `--wait / --no-wait`: Wait for all pictures to be ready  [default: no-wait]
 * `--is-blurred / --is-not-blurred`: Define if sequence is already blurred or not  [default: is-not-blurred]
 * `--title TEXT`: Collection title. If not provided, the title will be the directory name.
+* `--token TEXT`: GeoVisio token if the geovisio instance needs it.
+
+If none is provided and the geovisio instance requires it, the token will be asked during run.
+Note: is is advised to wait for prompt without using this variable.
 * `--help`: Show this message and exit.
```

### Comparing `geovisio_cli-0.1.0/geovisio_cli/main.py` & `geovisio_cli-0.2.0/geovisio_cli/main.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import typer
 from pathlib import Path
-from geovisio_cli import sequence, exception, model
+from geovisio_cli import sequence, exception, model, auth
 from rich import print
 from rich.panel import Panel
 from typing import Optional
 import os
 
 
 app = typer.Typer(help="GeoVisio command-line client")
@@ -12,22 +12,24 @@
 
 @app.command()
 def upload(
     path: Path = typer.Argument(..., help="Local path to your sequence folder"),
     api_url: str = typer.Option(..., help="GeoVisio endpoint URL"),
     user: str = typer.Option(
         default=None,
-        help="""GeoVisio user name if the geovisio instance needs it.
+        hidden=True,
+        help="""DEPRECATED: GeoVisio user name if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the username will be asked during run.
 """,
         envvar="GEOVISIO_USER",
     ),
     password: str = typer.Option(
         default=None,
-        help="""GeoVisio password if the geovisio instance needs it.
+        hidden=True,
+        help="""DEPRECATED: GeoVisio password if the geovisio instance needs it.
 If none is provided and the geovisio instance requires it, the password will be asked during run.
 Note: is is advised to wait for prompt without using this variable.
 """,
         envvar="GEOVISIO_PASSWORD",
     ),
     wait: bool = typer.Option(default=False, help="Wait for all pictures to be ready"),
     isBlurred: bool = typer.Option(
@@ -35,18 +37,30 @@
         "--is-blurred/--is-not-blurred",
         help="Define if sequence is already blurred or not",
     ),
     title: Optional[str] = typer.Option(
         default=None,
         help="Collection title. If not provided, the title will be the directory name.",
     ),
+    token: Optional[str] = typer.Option(
+        default=None,
+        help="""GeoVisio token if the geovisio instance needs it.
+
+If none is provided and the geovisio instance requires it, the token will be asked during run.
+Note: is is advised to wait for prompt without using this variable.
+""",
+    ),
 ):
     """Processes and sends a given sequence on your GeoVisio API"""
-    geovisio = model.Geovisio(url=api_url, user=user, password=password)
     try:
+        if user or password:
+            raise exception.CliException(
+                "user/password authentication have been deprecated, use a token or `geovisio login` instead"
+            )
+        geovisio = model.Geovisio(url=api_url, token=token)
         sequence.upload(
             path, geovisio, wait=wait, alreadyBlurred=isBlurred, title=title
         )
     except exception.CliException as e:
         print(
             Panel(
                 f"{e}",
@@ -122,7 +136,32 @@
             Panel(
                 f"{e}",
                 title="[red]Error while getting collection status",
                 border_style="red",
             )
         )
         return 1
+
+
+@app.command(
+    help=f"""
+    Authenticate into the given instance, and save credentials in a configuration file.
+
+    This will generate credentials, and ask the user to visit a page to associate those credentials to the user's account.
+
+    The credentials will be stored in {auth.get_config_file_path()}
+    """
+)
+def login(
+    api_url: str = typer.Option(..., help="GeoVisio endpoint URL"),
+):
+    try:
+        auth.create_auth_credentials(model.Geovisio(url=api_url))
+    except exception.CliException as e:
+        print(
+            Panel(
+                f"{e}",
+                title="[red]Error while getting credentials",
+                border_style="red",
+            )
+        )
+        return 1
```

### Comparing `geovisio_cli-0.1.0/geovisio_cli/sequence.py` & `geovisio_cli-0.2.0/geovisio_cli/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,20 +15,20 @@
 )
 from rich.panel import Panel
 from rich.console import Group
 from rich.live import Live
 from geovisio_cli.exception import CliException, raise_for_status
 from geovisio_cli.auth import login
 from geovisio_cli.model import Geovisio
+from geovisio_cli import utils
 from time import sleep
 from datetime import timedelta
 import os
 import toml
 
-REQUESTS_TIMEOUT = 30
 SEQUENCE_TOML_FILE = "_geovisio.toml"
 
 
 @dataclass
 class InteriorOrientation:
     make: str
     model: str
@@ -147,201 +147,201 @@
     path: Path,
     geovisio: Geovisio,
     title: Optional[str],
     wait: bool = False,
     alreadyBlurred: bool = False,
 ) -> UploadReport:
     # early test that the given url is correct
-    _test_geovisio_url(geovisio.url)
+    utils.test_geovisio_url(geovisio.url)
+    with requests.session() as s:
+        # early test login
+        if not _login_if_needed(s, geovisio):
+            raise CliException(
+                "🔁 Computer not authenticated yet, impossible to upload pictures, but you can try again the same upload command after finalizing the login"
+            )
 
-    sequence = process(path, title)
+        sequence = process(path, title)
 
-    return _publish(sequence, geovisio, wait, alreadyBlurred)
+        return _publish(s, sequence, geovisio, wait, alreadyBlurred)
 
 
 def _publish(
-    sequence: Sequence, geovisio: Geovisio, wait: bool, alreadyBlurred: bool
+    session: requests.Session,
+    sequence: Sequence,
+    geovisio: Geovisio,
+    wait: bool,
+    alreadyBlurred: bool,
 ) -> UploadReport:
-    with requests.session() as s:
-        # Check if API needs login
-        apiConf = s.get(f"{geovisio.url}/api/configuration")
-        if apiConf.json().get("auth") and apiConf.json()["auth"].get("enabled", False):
-            login(s, geovisio)
-
-        # Read sequence data
-        if sequence.id:
-            sequence = info(sequence)
-            print(
-                f'🔄 Syncing collection "{sequence.title}" (local folder: {sequence.path}, API ID: {sequence.id})'
-            )
-        else:
-            print(f'📂 Publishing collection "{sequence.title}" ({sequence.path})')
-
-        data = {}
-        if sequence.title:
-            data["title"] = sequence.title
-
-        # List pictures to upload
-        picturesToUpload = {}
-        for i, p in enumerate(sequence.pictures, start=1):
-            if p.id is None or p.status == "broken":
-                picturesToUpload[i] = p
-
-        # Create sequence on initial publishing
-        if not sequence.id:
-            seq = s.post(
-                f"{geovisio.url}/api/collections", data=data, timeout=REQUESTS_TIMEOUT
-            )
-            raise_for_status(seq, "Impossible to query GeoVisio")
+    # Read sequence data
+    if sequence.id:
+        sequence = info(sequence)
+        print(
+            f'🔄 Syncing collection "{sequence.title}" (local folder: {sequence.path}, API ID: {sequence.id})'
+        )
+    else:
+        print(f'📂 Publishing collection "{sequence.title}" ({sequence.path})')
 
-            sequence.id = seq.json()["id"]
-            sequence.location = seq.headers["Location"]
-            _write_sequence_toml(sequence)
+    data = {}
+    if sequence.title:
+        data["title"] = sequence.title
+
+    # List pictures to upload
+    picturesToUpload = {}
+    for i, p in enumerate(sequence.pictures, start=1):
+        if p.id is None or p.status == "broken":
+            picturesToUpload[i] = p
+
+    # Create sequence on initial publishing
+    if not sequence.id:
+        seq = session.post(
+            f"{geovisio.url}/api/collections", data=data, timeout=utils.REQUESTS_TIMEOUT
+        )
+        raise_for_status(seq, "Impossible to query GeoVisio")
+
+        sequence.id = seq.json()["id"]
+        sequence.location = seq.headers["Location"]
+        _write_sequence_toml(sequence)
 
-            print(f"✅ Created collection {sequence.location}")
+        print(f"✅ Created collection {sequence.location}")
 
-        else:
-            print(
-                f"⏭️ Skipping {len(sequence.pictures) - len(picturesToUpload)} already published pictures"
-            )
+    else:
+        print(
+            f"⏭️ Skipping {len(sequence.pictures) - len(picturesToUpload)} already published pictures"
+        )
 
-        if not sequence.location:
-            raise CliException("Sequence has no API location defined")
+    if not sequence.location:
+        raise CliException("Sequence has no API location defined")
 
-        report = UploadReport(location=sequence.location)
+    report = UploadReport(location=sequence.location)
 
-        uploading_progress = Progress(
-            TextColumn("{task.description}"),
-            BarColumn(),
-            TimeElapsedColumn(),
-            TextColumn("[{task.completed}/{task.total}]"),
-        )
-        current_pic_progress = Progress(
-            TextColumn("📷 Processing [bold purple]{task.fields[file]}"),
-            SpinnerColumn("simpleDots"),
-        )
-        error_progress = Progress(TextColumn("{task.description}"))
+    uploading_progress = Progress(
+        TextColumn("{task.description}"),
+        BarColumn(),
+        TimeElapsedColumn(),
+        TextColumn("[{task.completed}/{task.total}]"),
+    )
+    current_pic_progress = Progress(
+        TextColumn("📷 Processing [bold purple]{task.fields[file]}"),
+        SpinnerColumn("simpleDots"),
+    )
+    error_progress = Progress(TextColumn("{task.description}"))
+
+    last_error = Progress(
+        TextColumn("🔎 Last error 🔎\n{task.description}"),
+    )
+    error_panel = Panel(Group(error_progress, last_error), title="Errors")
+    uploading_task = uploading_progress.add_task(
+        f"[green]🚀 Uploading pictures...",
+        total=len(picturesToUpload),
+    )
+    current_pic_task = current_pic_progress.add_task("", file="")
+    progress_group = Group(
+        uploading_progress,
+        current_pic_progress,
+        error_panel,
+    )
+    error_task = error_progress.add_task("[green]No errors")
+    last_error_task = last_error.add_task("", visible=False)
+    with Live(progress_group):
+        for i, p in picturesToUpload.items():
+            if not p.path:
+                raise CliException(f"Missing path for picture {i}")
+
+            uploading_progress.advance(uploading_task)
+            current_pic_progress.update(current_pic_task, file=p.path.split("/")[-1])
+            try:
+                picture_response = session.post(
+                    f"{sequence.location}/items",
+                    files={"picture": open(p.path, "rb")},
+                    data={
+                        "position": i,
+                        "isBlurred": "true" if alreadyBlurred else "false",
+                    },
+                    timeout=utils.REQUESTS_TIMEOUT,
+                )
+            except (requests.Timeout,) as timeout_error:
+                raise CliException(
+                    f"""Timeout while trying to post picture. Maybe the instance is overloaded? Please contact your instance administrator.
 
-        last_error = Progress(
-            TextColumn("🔎 Last error 🔎\n{task.description}"),
-        )
-        error_panel = Panel(Group(error_progress, last_error), title="Errors")
-        uploading_task = uploading_progress.add_task(
-            f"[green]🚀 Uploading pictures...",
-            total=len(picturesToUpload),
-        )
-        current_pic_task = current_pic_progress.add_task("", file="")
-        progress_group = Group(
-            uploading_progress,
-            current_pic_progress,
-            error_panel,
-        )
-        error_task = error_progress.add_task("[green]No errors")
-        last_error_task = last_error.add_task("", visible=False)
-        with Live(progress_group):
-            for i, p in picturesToUpload.items():
-                if not p.path:
-                    raise CliException(f"Missing path for picture {i}")
-
-                uploading_progress.advance(uploading_task)
-                current_pic_progress.update(
-                    current_pic_task, file=p.path.split("/")[-1]
+            [bold]Error:[/bold]
+            {timeout_error}"""
                 )
-                try:
-                    picture_response = s.post(
-                        f"{sequence.location}/items",
-                        files={"picture": open(p.path, "rb")},
-                        data={
-                            "position": i,
-                            "isBlurred": "true" if alreadyBlurred else "false",
-                        },
-                        timeout=REQUESTS_TIMEOUT,
-                    )
-                except (requests.Timeout,) as timeout_error:
-                    raise CliException(
-                        f"""Timeout while trying to post picture. Maybe the instance is overloaded? Please contact your instance administrator.
+            except (
+                requests.ConnectionError,
+                requests.ConnectTimeout,
+                requests.TooManyRedirects,
+            ) as cnx_error:
+                raise CliException(
+                    f"""Impossible to reach GeoVisio while trying to post a picture, connection was lost. Please contact your instance administrator.
 
-                [bold]Error:[/bold]
-                {timeout_error}"""
-                    )
-                except (
-                    requests.ConnectionError,
-                    requests.ConnectTimeout,
-                    requests.TooManyRedirects,
-                ) as cnx_error:
-                    raise CliException(
-                        f"""Impossible to reach GeoVisio while trying to post a picture, connection was lost. Please contact your instance administrator.
+            [bold]Error:[/bold]
+            {cnx_error}"""
+                )
 
-                [bold]Error:[/bold]
-                {cnx_error}"""
+            # Picture at given position exists -> mark it as OK
+            if picture_response.status_code == 409:
+                sequence = status(sequence)
+                _write_sequence_toml(sequence)
+                report.uploaded_pictures.append(p)
+
+            elif picture_response.status_code >= 400:
+                body = (
+                    picture_response.json()
+                    if picture_response.headers.get("Content-Type")
+                    == "application/json"
+                    else picture_response.text
+                )
+                report.errors.append(
+                    UploadError(
+                        position=i,
+                        picture_path=p.path,
+                        status_code=picture_response.status_code,
+                        error=body,
                     )
+                )
 
-                # Picture at given position exists -> mark it as OK
-                if picture_response.status_code == 409:
-                    sequence = status(sequence)
-                    _write_sequence_toml(sequence)
-                    report.uploaded_pictures.append(p)
-
-                elif picture_response.status_code >= 400:
-                    body = (
-                        picture_response.json()
-                        if picture_response.headers.get("Content-Type")
-                        == "application/json"
-                        else picture_response.text
-                    )
-                    report.errors.append(
-                        UploadError(
-                            position=i,
-                            picture_path=p.path,
-                            status_code=picture_response.status_code,
-                            error=body,
-                        )
-                    )
+                error_progress.update(
+                    error_task,
+                    description=f"[bold red]{len(report.errors)} errors",
+                )
+                last_error.update(last_error_task, description=body, visible=True)
+                p.status = "broken"
+                _write_sequence_toml(sequence)
+
+            else:
+                p.location = picture_response.headers["Location"]
+                p.id = picture_response.json()["id"]
+                p.status = None
+                report.uploaded_pictures.append(p)
+                _write_sequence_toml(sequence)
+
+    if not report.uploaded_pictures:
+        print(
+            f"[red]💥 All pictures upload of sequence {sequence.title} failed! 💥[/red]"
+        )
+    else:
+        print(
+            f"🎉 [bold green]{len(report.uploaded_pictures)}[/bold green] pictures uploaded"
+        )
+    if report.errors:
+        print(f"[bold red]{len(report.errors)}[/bold red] pictures not uploaded:")
+        for e in report.errors:
+            msg: Union[str, dict] = e.error
+            if isinstance(e.error, str):
+                msg = escape(e.error.replace("\n", "\\n"))
+            print(f" - {e.picture_path} (status [bold]{e.status_code}[/]): {msg}")
 
-                    error_progress.update(
-                        error_task,
-                        description=f"[bold red]{len(report.errors)} errors",
-                    )
-                    last_error.update(last_error_task, description=body, visible=True)
-                    p.status = "broken"
-                    _write_sequence_toml(sequence)
-
-                else:
-                    p.location = picture_response.headers["Location"]
-                    p.id = picture_response.json()["id"]
-                    p.status = None
-                    report.uploaded_pictures.append(p)
-                    _write_sequence_toml(sequence)
-
-        if not report.uploaded_pictures:
-            print(
-                f"[red]💥 All pictures upload of sequence {sequence.title} failed! 💥[/red]"
-            )
-        else:
-            print(
-                f"🎉 [bold green]{len(report.uploaded_pictures)}[/bold green] pictures uploaded"
-            )
-        if report.errors:
-            print(f"[bold red]{len(report.errors)}[/bold red] pictures not uploaded:")
-            for e in report.errors:
-                msg: Union[str, dict] = e.error
-                if isinstance(e.error, str):
-                    msg = escape(e.error.replace("\n", "\\n"))
-                print(f" - {e.picture_path} (status [bold]{e.status_code}[/]): {msg}")
-
-        if wait:
-            wait_for_sequence(sequence)
-        else:
-            print(f"Note: You can follow the picture processing with the command:")
-            from rich.syntax import Syntax
+    if wait:
+        wait_for_sequence(sequence)
+    else:
+        print(f"Note: You can follow the picture processing with the command:")
+        from rich.syntax import Syntax
 
-            print(
-                f"[bold]geovisio collection-status --wait --location {sequence.location}"
-            )
-        return report
+        print(f"[bold]geovisio collection-status --wait --location {sequence.location}")
+    return report
 
 
 def _check_sequence(sequence: Sequence):
     if not sequence.pictures:
         raise CliException(f"No pictures to upload for sequence {sequence.title}")
 
 
@@ -418,62 +418,28 @@
         tomlFileContent = f.read()
         sequence.from_toml(toml.loads(tomlFileContent))
         f.close()
 
     return sequence
 
 
-def _test_geovisio_url(geovisio: str):
-    full_url = f"{geovisio}/api/collections"
-    try:
-        r = requests.get(full_url, timeout=REQUESTS_TIMEOUT)
-    except (
-        requests.Timeout,
-        requests.ConnectionError,
-        requests.ConnectTimeout,
-        requests.TooManyRedirects,
-    ) as e:
-        raise CliException(
-            f"""The API is not reachable. Please check error and used URL below, and retry later if the URL is correct.
-
-[bold]Used URL:[/bold] {full_url}
-[bold]Error:[/bold]
-{e}"""
-        )
-    except Exception as e:
-        raise CliException(
-            f"""Error while connecting to the API. Please check error and used URL below
-
-[bold]Used URL:[/bold] {full_url}
-[bold]Error:[/bold]
-{e}"""
-        )
-
-    if r.status_code == 404:
-        raise CliException(
-            f"""The API URL is not valid.
-
-Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
-Please make sure you gave the correct URL and retry.
-
-[bold]Used URL:[/bold] {full_url}
-[bold]Error:[/bold]
-{r.text}"""
-        )
-    if r.status_code > 404:
-        raise CliException(
-            f"""The API is unavailable for now. Please check given error and retry later.
-[bold]Used URL:[/bold] {full_url}
-[bold]Error[/bold] (code [cyan]{r.status_code}[/cyan]):
-{r.text}"""
-        )
+def _login_if_needed(session: requests.Session, geovisio: Geovisio) -> bool:
+    # Check if API needs login
+    apiConf = session.get(f"{geovisio.url}/api/configuration")
+    if apiConf.json().get("auth", {}).get("enabled", False):
+        logged_in = login(session, geovisio)
+        if not logged_in:
+            return False
+    return True
 
 
 def status(sequence: Sequence) -> Sequence:
-    s = requests.get(f"{sequence.location}/geovisio_status", timeout=REQUESTS_TIMEOUT)
+    s = requests.get(
+        f"{sequence.location}/geovisio_status", timeout=utils.REQUESTS_TIMEOUT
+    )
     if s.status_code == 404:
         raise CliException(f"Sequence {sequence.location} not found")
     if s.status_code >= 400:
         raise CliException(
             f"Impossible to get sequence {sequence.location} status: {s.text}"
         )
     r = s.json()
@@ -490,15 +456,15 @@
     return sequence
 
 
 def info(sequence: Sequence) -> Sequence:
     if not sequence.location:
         raise CliException(f"Sequence has no location set")
 
-    s = requests.get(sequence.location, timeout=REQUESTS_TIMEOUT)
+    s = requests.get(sequence.location, timeout=utils.REQUESTS_TIMEOUT)
     if s.status_code == 404:
         raise CliException(f"Sequence {sequence.location} not found")
     if s.status_code >= 400:
         raise CliException(
             f"Impossible to get sequence {sequence.location} status: {s.text}"
         )
     r = s.json()
```

### Comparing `geovisio_cli-0.1.0/pyproject.toml` & `geovisio_cli-0.2.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 classifiers = ["License :: OSI Approved :: MIT License"]
 dynamic = ["version", "description"]
 dependencies = [
     "requests ~= 2.28.0",
     "typer ~= 0.7.0",
     "rich[all] ~= 13.3.0",
     "toml ~= 0.10.2",
+    "qrcode ~= 7.4.2",
 ]
 
 [project.urls]
 Home = "https://gitlab.com/geovisio/cli"
 
 [project.scripts]
 geovisio="geovisio_cli.main:app"
```

### Comparing `geovisio_cli-0.1.0/tests/fixtures/e1.jpg` & `geovisio_cli-0.2.0/tests/fixtures/e1.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/tests/fixtures/e2.jpg` & `geovisio_cli-0.2.0/tests/fixtures/e2.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/tests/fixtures/e3.jpg` & `geovisio_cli-0.2.0/tests/fixtures/e3.jpg`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/tests/integration/test_upload.py` & `geovisio_cli-0.2.0/tests/integration/test_upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 import os
 import pytest
 from ..conftest import FIXTURE_DIR
 from pathlib import Path
 import requests
 from geovisio_cli import sequence, exception, model
 from datetime import timedelta
-import re
 import toml
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
 )
-def test_valid_upload(geovisio, datafiles):
+def test_valid_upload(geovisio_with_token, datafiles):
     uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio, title="some title"
+        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
     )
     assert len(uploadReport.uploaded_pictures) == 3
     assert len(uploadReport.errors) == 0
 
     collection = sequence.Sequence(location=uploadReport.location)
     sequence.wait_for_sequence(collection, timeout=timedelta(minutes=1))
     status = sequence.status(collection)
@@ -57,26 +56,26 @@
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
 )
-def test_resume_upload(geovisio, datafiles):
+def test_resume_upload(geovisio_with_token, datafiles):
     # Make e2 not valid to have a partial upload
     picE2 = datafiles / "e2.jpg"
     picE2bak = datafiles / "e2.bak"
     os.rename(picE2, picE2bak)
     with open(picE2, "w") as picE2file:
         picE2file.write("")
         picE2file.close()
 
     # Start upload -> 2 uploaded pics + 1 failure
     uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio, title="some title"
+        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
     )
     assert len(uploadReport.uploaded_pictures) == 2
     assert len(uploadReport.errors) == 1
     assert uploadReport.errors[0].position == 2
 
     # Check TOML file -> e2 has no ID but broken status
     tomlFile = datafiles / sequence.SEQUENCE_TOML_FILE
@@ -89,15 +88,15 @@
 
     # Make e2 valid
     os.remove(picE2)
     os.rename(picE2bak, picE2)
 
     # Launch again upload : 1 uploaded pic + 0 failure
     uploadReport2 = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio, title="some title"
+        path=Path(datafiles), geovisio=geovisio_with_token, title="some title"
     )
     assert uploadReport2.location == uploadReport.location
     assert len(uploadReport2.uploaded_pictures) == 1
     assert len(uploadReport2.errors) == 0
 
     # Check TOML file -> everything has ID and looks like a charm
     with open(tomlFile, "r") as f:
@@ -117,16 +116,18 @@
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
     os.path.join(FIXTURE_DIR, "e2.jpg"),
     os.path.join(FIXTURE_DIR, "e3.jpg"),
     os.path.join(FIXTURE_DIR, "invalid_pic.jpg"),
 )
-def test_upload_with_invalid_file(geovisio, datafiles):
-    uploadReport = sequence.upload(path=Path(datafiles), geovisio=geovisio, title=None)
+def test_upload_with_invalid_file(geovisio_with_token, datafiles):
+    uploadReport = sequence.upload(
+        path=Path(datafiles), geovisio=geovisio_with_token, title=None
+    )
 
     # Only 3 pictures should have been uploaded, 1 is in error
     assert len(uploadReport.uploaded_pictures) == 3
     assert len(uploadReport.errors) == 1
 
     # But the collection status should have 3 items (and be valid)
     collection = sequence.Sequence(location=uploadReport.location)
@@ -147,17 +148,17 @@
         collection.json()["title"] == Path(datafiles).name
     )  # since no title has been set, the directory name has been choosen
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "invalid_pic.jpg"),
 )
-def test_upload_with_no_valid_file(geovisio, datafiles):
+def test_upload_with_no_valid_file(geovisio_with_token, datafiles):
     uploadReport = sequence.upload(
-        path=Path(datafiles), geovisio=geovisio, title="a title"
+        path=Path(datafiles), geovisio=geovisio_with_token, title="a title"
     )
 
     assert len(uploadReport.uploaded_pictures) == 0
     assert len(uploadReport.errors) == 1
 
     status = requests.get(f"{uploadReport.location}/geovisio_status")
     assert (
@@ -189,29 +190,31 @@
     )
     assert "Failed to establish a new connection:" in msg
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
-def test_upload_on_invalid_url_path(geovisio, datafiles):
+def test_upload_on_invalid_url_path(geovisio_with_token, datafiles):
     with pytest.raises(exception.CliException) as e:
         sequence.upload(
             path=Path(datafiles),
-            geovisio=model.Geovisio(url=geovisio.url + "/some_additional_path"),
+            geovisio=model.Geovisio(
+                url=geovisio_with_token.url + "/some_additional_path"
+            ),
             title=None,
         )
     msg = str(e.value)
     assert msg.startswith(
         f"""The API URL is not valid.
 
 Note that your URL should be the API root (something like https://geovisio.fr, https://panoramax.ign.fr or any other geovisio instance).
 Please make sure you gave the correct URL and retry.
 
-[bold]Used URL:[/bold] {geovisio.url}/some_additional_path/api/collections
+[bold]Used URL:[/bold] {geovisio_with_token.url}/some_additional_path/api/collections
 [bold]Error:[/bold]"""
     )
 
 
 @pytest.mark.datafiles(
     os.path.join(FIXTURE_DIR, "e1.jpg"),
 )
```

### Comparing `geovisio_cli-0.1.0/tests/test_process.py` & `geovisio_cli-0.2.0/tests/test_process.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/tests/test_sequence.py` & `geovisio_cli-0.2.0/tests/test_sequence.py`

 * *Files identical despite different names*

### Comparing `geovisio_cli-0.1.0/PKG-INFO` & `geovisio_cli-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: geovisio_cli
-Version: 0.1.0
+Version: 0.2.0
 Summary: Geovio client cli tool
 Author-email: Antoine Desbordes <antoine.desbordes@gmail.com>
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: requests ~= 2.28.0
 Requires-Dist: typer ~= 0.7.0
 Requires-Dist: rich[all] ~= 13.3.0
 Requires-Dist: toml ~= 0.10.2
+Requires-Dist: qrcode ~= 7.4.2
 Requires-Dist: flit ~= 3.8.0 ; extra == "build"
 Requires-Dist: black ~= 22.8.0 ; extra == "dev"
 Requires-Dist: mypy ~= 1.0.0 ; extra == "dev"
 Requires-Dist: types-requests ~= 2.28.0 ; extra == "dev"
 Requires-Dist: pytest ~= 7.2.0 ; extra == "dev"
 Requires-Dist: testcontainers-compose ~= 0.0.1rc1 ; extra == "dev"
 Requires-Dist: pytest-datafiles ~= 2.0.1 ; extra == "dev"
@@ -142,21 +143,25 @@
 
 You can also add a `--wait` flag to wait for geovisio to process all the pictures.
 
 Note that you can launch again the same command to recover a partial sequence import, for example if only some pictures failed to upload.
 
 #### Authentication
 
-If the GeoVisio API requires a login for the upload, the user/password can either be set:
-* with command-line arguments (`--user` / `--password`)
-* with environment variables (`GEOVISIO_USER` / `GEOVISIO_PASSWORD`)
+If the GeoVisio API requires a login for the upload, the `upload` command will ask for a login on the instance by visiting a given url with a browser. 
 
-If no information is set but required by the GeoVisio instance, they will be asked interactively. This is the best way to enter the password so it will not be stored in the command-line history.
+You can also login before hand with the command:
 
-Note: the password is not stored, and sent directly to geovisio. If the future, this will be removed in favor of API keys when geovisio will support those.
+```bash
+geovisio login --api-url http://localhost:5000/
+```
+
+Both will store the credentials in a configuration file, located either in a [XDG](https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html) defined directory or in a user specific .config, in a subdirectory `geovisio/config.toml`.
+
+If you do not want to use this, you can also provide a geovisio token with the `--token` parameter.
 
 ### Collection status
 
 Prints the status of a collection.
 
 ```bash
 geovisio collection-status --id <some collection id> --api-url http://localhost:5000
```

