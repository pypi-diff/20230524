# Comparing `tmp/flux-local-1.1.3.tar.gz` & `tmp/flux-local-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flux-local-1.1.3.tar", last modified: Sat Mar 25 20:13:27 2023, max compression
+gzip compressed data, was "flux-local-1.2.0.tar", last modified: Wed May 24 02:37:09 2023, max compression
```

## Comparing `flux-local-1.1.3.tar` & `flux-local-1.2.0.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:13:27.760666 flux-local-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-03-25 20:13:12.000000 flux-local-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-03-25 20:13:27.760666 flux-local-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-03-25 20:13:12.000000 flux-local-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:13:27.760666 flux-local-1.1.3/flux_local/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/command.py
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5808 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)    14657 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/manifest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:13:27.760666 flux-local-1.1.3/flux_local/tool/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/build.py
--rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/diff.py
--rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/flux_local.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/format.py
--rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/selector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-03-25 20:13:12.000000 flux-local-1.1.3/flux_local/tool/visitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:13:27.760666 flux-local-1.1.3/flux_local.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-03-25 20:13:27.000000 flux-local-1.1.3/flux_local.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-03-25 20:13:27.760666 flux-local-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-03-25 20:13:12.000000 flux-local-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-25 20:13:27.760666 flux-local-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-03-25 20:13:12.000000 flux-local-1.1.3/tests/test_command.py
--rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-03-25 20:13:12.000000 flux-local-1.1.3/tests/test_git_repo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-03-25 20:13:12.000000 flux-local-1.1.3/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-03-25 20:13:12.000000 flux-local-1.1.3/tests/test_kustomize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-25 20:13:12.000000 flux-local-1.1.3/tests/test_manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.747829 flux-local-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-24 02:36:58.000000 flux-local-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-24 02:37:09.747829 flux-local-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9356 2023-05-24 02:36:58.000000 flux-local-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3108 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20614 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6548 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9404 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/manifest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local/tool/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14698 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/diff.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2719 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/flux_local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7143 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4514 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/selector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13798 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10083 2023-05-24 02:36:58.000000 flux-local-1.2.0/flux_local/tool/visitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/flux_local.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9853 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-24 02:37:09.000000 flux-local-1.2.0/flux_local.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-24 02:37:09.747829 flux-local-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-24 02:36:58.000000 flux-local-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 02:37:09.743829 flux-local-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13334 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_git_repo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5393 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_kustomize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-24 02:36:58.000000 flux-local-1.2.0/tests/test_manifest.py
```

### Comparing `flux-local-1.1.3/LICENSE` & `flux-local-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/PKG-INFO` & `flux-local-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.1.3
+Version: 1.2.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.1.3/README.md` & `flux-local-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/command.py` & `flux-local-1.2.0/flux_local/command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/exceptions.py` & `flux-local-1.2.0/flux_local/exceptions.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/git_repo.py` & `flux-local-1.2.0/flux_local/git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/helm.py` & `flux-local-1.2.0/flux_local/helm.py`

 * *Files 6% similar despite different names*

```diff
@@ -40,27 +40,34 @@
 from typing import Any
 
 import aiofiles
 import yaml
 
 from . import command
 from .kustomize import Kustomize
-from .manifest import HelmRelease, HelmRepository, CRD_KIND, SECRET_KIND
+from .manifest import HelmRelease, HelmRepository, CRD_KIND, SECRET_KIND, REPO_TYPE_OCI
 from .exceptions import HelmException
 
 __all__ = [
     "Helm",
 ]
 
 _LOGGER = logging.getLogger(__name__)
 
 
 HELM_BIN = "helm"
 
 
+def _chart_name(repo: HelmRepository, release: HelmRelease) -> str:
+    """Return the helm chart name used for the helm template command."""
+    if repo.repo_type == REPO_TYPE_OCI:
+        return f"{repo.url}/{release.chart.name}"
+    return release.chart.chart_name
+
+
 class RepositoryConfig:
     """Generates a helm repository configuration from flux HelmRepository objects."""
 
     def __init__(self, repos: list[HelmRepository]) -> None:
         """Initialize RepositoryConfig."""
         self._repos = repos
 
@@ -109,15 +116,18 @@
 
     async def update(self) -> None:
         """Return command line arguments to update the local repo.
 
         Typically the repository must be updated before doing any chart templating.
         """
         _LOGGER.debug("Updating %d repositories", len(self._repos))
-        content = yaml.dump(RepositoryConfig(self._repos).config, sort_keys=False)
+        repos = [repo for repo in self._repos if repo.repo_type != REPO_TYPE_OCI]
+        if not repos:
+            return
+        content = yaml.dump(RepositoryConfig(repos).config, sort_keys=False)
         async with aiofiles.open(str(self._repo_config_file), mode="w") as config_file:
             await config_file.write(content)
         await command.run(
             command.Command(
                 [HELM_BIN, "repo", "update"] + self._flags, exc=HelmException
             )
         )
@@ -134,19 +144,28 @@
     ) -> Kustomize:
         """Return command line arguments to template the specified chart.
 
         The default values will come from the `HelmRelease`, though you can
         also specify values directory if not present in cluster manifest
         e.g. it came from a truncated yaml.
         """
+        repo = next(
+            iter([repo for repo in self._repos if repo.repo_name == release.repo_name]),
+            None,
+        )
+        if not repo:
+            raise HelmException(
+                f"Unable to find HelmRepository for {release.chart.chart_name} for "
+                f"HelmRelease {release.name}"
+            )
         args: list[str] = [
             HELM_BIN,
             "template",
             release.name,
-            release.chart.chart_name,
+            _chart_name(repo, release),
             "--namespace",
             release.namespace,
         ]
         if skip_crds:
             args.append("--skip-crds")
         if skip_tests:
             args.append("--skip-tests")
```

### Comparing `flux-local-1.1.3/flux_local/kustomize.py` & `flux-local-1.2.0/flux_local/kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/manifest.py` & `flux-local-1.2.0/flux_local/manifest.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,14 +32,17 @@
 KUSTOMIZE_DOMAIN = "kustomize.config.k8s.io"
 HELM_REPO_DOMAIN = "source.toolkit.fluxcd.io"
 HELM_RELEASE_DOMAIN = "helm.toolkit.fluxcd.io"
 CLUSTER_POLICY_DOMAIN = "kyverno.io"
 CRD_KIND = "CustomResourceDefinition"
 SECRET_KIND = "Secret"
 
+REPO_TYPE_DEFAULT = "default"
+REPO_TYPE_OCI = "oci"
+
 
 def _check_version(doc: dict[str, Any], version: str) -> None:
     """Assert that the resource has the specified version."""
     if not (api_version := doc.get("apiVersion")):
         raise InputException(f"Invalid object missing apiVersion: {doc}")
     if not api_version.startswith(version):
         raise InputException(f"Invalid object expected '{version}': {doc}")
@@ -155,14 +158,19 @@
         )
 
     @property
     def release_name(self) -> str:
         """Identifier for the HelmRelease."""
         return f"{self.namespace}-{self.name}"
 
+    @property
+    def repo_name(self) -> str:
+        """Identifier for the HelmRepository identified in the HelmChart."""
+        return f"{self.chart.repo_namespace}-{self.chart.repo_name}"
+
     _COMPACT_EXCLUDE_FIELDS = {
         "values": True,
         "chart": HelmChart._COMPACT_EXCLUDE_FIELDS,
     }
 
 
 class HelmRepository(BaseManifest):
@@ -173,29 +181,37 @@
 
     namespace: str
     """The namespace of owning the HelmRepository."""
 
     url: str
     """The URL to the repository of helm charts."""
 
+    repo_type: str | None = None
+    """The type of the HelmRepository."""
+
     @classmethod
     def parse_doc(cls, doc: dict[str, Any]) -> "HelmRepository":
         """Parse a HelmRepository from a kubernetes resource."""
         _check_version(doc, HELM_REPO_DOMAIN)
         if not (metadata := doc.get("metadata")):
             raise InputException(f"Invalid {cls} missing metadata: {doc}")
         if not (name := metadata.get("name")):
             raise InputException(f"Invalid {cls} missing metadata.name: {doc}")
         if not (namespace := metadata.get("namespace")):
             raise InputException(f"Invalid {cls} missing metadata.namespace: {doc}")
         if not (spec := doc.get("spec")):
             raise InputException(f"Invalid {cls} missing spec: {doc}")
         if not (url := spec.get("url")):
             raise InputException(f"Invalid {cls} missing spec.url: {doc}")
-        return cls(name=name, namespace=namespace, url=url)
+        return cls(
+            name=name,
+            namespace=namespace,
+            url=url,
+            repo_type=spec.get("type", REPO_TYPE_DEFAULT),
+        )
 
     @property
     def repo_name(self) -> str:
         """Identifier for the HelmRepository."""
         return f"{self.namespace}-{self.name}"
```

### Comparing `flux-local-1.1.3/flux_local/tool/build.py` & `flux-local-1.2.0/flux_local/tool/build.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/diff.py` & `flux-local-1.2.0/flux_local/tool/diff.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/flux_local.py` & `flux-local-1.2.0/flux_local/tool/flux_local.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/format.py` & `flux-local-1.2.0/flux_local/tool/format.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/get.py` & `flux-local-1.2.0/flux_local/tool/get.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/selector.py` & `flux-local-1.2.0/flux_local/tool/selector.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/test.py` & `flux-local-1.2.0/flux_local/tool/test.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local/tool/visitor.py` & `flux-local-1.2.0/flux_local/tool/visitor.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/flux_local.egg-info/PKG-INFO` & `flux-local-1.2.0/flux_local.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flux-local
-Version: 1.1.3
+Version: 1.2.0
 Summary: flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 Home-page: https://github.com/allenporter/flux-local
 Author: Allen Porter
 Author-email: allen.porter@gmail.com
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Description-Content-Type: text/markdown
```

### Comparing `flux-local-1.1.3/flux_local.egg-info/SOURCES.txt` & `flux-local-1.2.0/flux_local.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/setup.cfg` & `flux-local-1.2.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flux-local
-version = 1.1.3
+version = 1.2.0
 description = flux-local is a python library and set of tools for managing a flux gitops repository, with validation steps to help improve quality of commits, PRs, and general local testing.
 long_description = file: README.md
 long_description_content_type = text/markdown
 prodid = github.com/allenporter/flux-local
 url = https://github.com/allenporter/flux-local
 author = Allen Porter
 author_email = allen.porter@gmail.com
```

### Comparing `flux-local-1.1.3/tests/test_command.py` & `flux-local-1.2.0/tests/test_command.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/tests/test_git_repo.py` & `flux-local-1.2.0/tests/test_git_repo.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/tests/test_helm.py` & `flux-local-1.2.0/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/tests/test_kustomize.py` & `flux-local-1.2.0/tests/test_kustomize.py`

 * *Files identical despite different names*

### Comparing `flux-local-1.1.3/tests/test_manifest.py` & `flux-local-1.2.0/tests/test_manifest.py`

 * *Files 10% similar despite different names*

```diff
@@ -56,22 +56,31 @@
         },
     }
 
 
 def test_parse_helm_repository() -> None:
     """Test parsing a helm repository doc."""
 
-    docs = yaml.load_all(
-        (TESTDATA_DIR / "configs/helm-repositories.yaml").read_text(),
-        Loader=yaml.CLoader,
+    docs = list(
+        yaml.load_all(
+            (TESTDATA_DIR / "configs/helm-repositories.yaml").read_text(),
+            Loader=yaml.CLoader,
+        )
     )
-    repo = HelmRepository.parse_doc(next(iter(docs)))
+    assert len(docs) == 2
+    repo = HelmRepository.parse_doc(docs[0])
     assert repo.name == "bitnami"
     assert repo.namespace == "flux-system"
     assert repo.url == "https://charts.bitnami.com/bitnami"
+    assert repo.repo_type == "default"
+    repo = HelmRepository.parse_doc(docs[1])
+    assert repo.name == "podinfo"
+    assert repo.namespace == "flux-system"
+    assert repo.url == "oci://ghcr.io/stefanprodan/charts"
+    assert repo.repo_type == "oci"
 
 
 async def test_write_manifest_file() -> None:
     """Test reading an invalid manifest file."""
     await write_manifest(Path("/dev/null"), Manifest(clusters=[]))
```

