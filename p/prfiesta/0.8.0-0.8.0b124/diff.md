# Comparing `tmp/prfiesta-0.8.0.tar.gz` & `tmp/prfiesta-0.8.0b124.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prfiesta-0.8.0.tar", max compression
+gzip compressed data, was "prfiesta-0.8.0b124.tar", max compression
```

## Comparing `prfiesta-0.8.0.tar` & `prfiesta-0.8.0b124.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1078 2023-05-22 18:59:38.045992 prfiesta-0.8.0/LICENSE
--rw-r--r--   0        0        0     6272 2023-05-22 18:59:38.045992 prfiesta-0.8.0/README.md
--rw-r--r--   0        0        0      487 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/__init__.py
--rw-r--r--   0        0        0     2763 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/__main__.py
--rw-r--r--   0        0        0        0 2023-05-22 18:59:38.053992 prfiesta-0.8.0/prfiesta/analysis/__init__.py
--rw-r--r--   0        0        0     4729 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/analysis/plot.py
--rw-r--r--   0        0        0     1007 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/analysis/view.py
--rw-r--r--   0        0        0        0 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/collectors/__init__.py
--rw-r--r--   0        0        0     4981 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/collectors/github.py
--rw-r--r--   0        0        0      571 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/environment.py
--rw-r--r--   0        0        0      975 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/output.py
--rw-r--r--   0        0        0      275 2023-05-22 18:59:38.057992 prfiesta-0.8.0/prfiesta/spinner.py
--rw-r--r--   0        0        0     3183 2023-05-22 18:59:50.026659 prfiesta-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     7617 1970-01-01 00:00:00.000000 prfiesta-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-24 05:22:40.958774 prfiesta-0.8.0b124/LICENSE
+-rw-r--r--   0        0        0     6603 2023-05-24 05:22:40.958774 prfiesta-0.8.0b124/README.md
+-rw-r--r--   0        0        0      487 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/__init__.py
+-rw-r--r--   0        0        0     2763 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/__init__.py
+-rw-r--r--   0        0        0     4729 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/plot.py
+-rw-r--r--   0        0        0     1007 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/analysis/view.py
+-rw-r--r--   0        0        0        0 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/collectors/__init__.py
+-rw-r--r--   0        0        0     4981 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/collectors/github.py
+-rw-r--r--   0        0        0      571 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/environment.py
+-rw-r--r--   0        0        0      975 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/output.py
+-rw-r--r--   0        0        0      275 2023-05-24 05:22:40.966774 prfiesta-0.8.0b124/prfiesta/spinner.py
+-rw-r--r--   0        0        0     3187 2023-05-24 05:22:48.510861 prfiesta-0.8.0b124/pyproject.toml
+-rw-r--r--   0        0        0     7952 1970-01-01 00:00:00.000000 prfiesta-0.8.0b124/PKG-INFO
```

### Comparing `prfiesta-0.8.0/LICENSE` & `prfiesta-0.8.0b124/LICENSE`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/README.md` & `prfiesta-0.8.0b124/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -71,31 +71,37 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
-### Time Filter
+### Date Filter
 
-When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` time dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](./docs/analysis.md).
 
 ## Using GitHub Enterprise
 
 If you trying to fetch data from a [GitHub Enterprise](https://docs.github.com/en/enterprise-cloud@latest/rest/enterprise-admin?apiVersion=2022-11-28) server, then much of the same functionality should work the same. You just need to make sure that:
 
 - `GH_HOST` is set to your enterprise instance's API URL. Reach out to your internal GitHub team if you are not sure what this should be.
 - `GITHUB_ENTERPRISE_TOKEN` a [personal access token](https://docs.github.com/en/enterprise-cloud@latest/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) generated on your GitHub Enterprise instance.
 
+## GitHub Rate Limiting
+
+Depending on your input parameters, you may end up in a situation where you are being [Rate Limited](https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=2022-11-28#rate-limiting) by the GitHub API.
+
+See this [Notebook](./notebooks/misc/rate_limit.ipynb) on a way to handle this.
+
 ## Environment Variables
 
 | Variable                  | Description                                                                                                                                  | Default                  |
 | ---------------           | ---------------                                                                                                                              | ------                   |
 | `GITHUB_TOKEN`            | The Github [`Token`](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to use |                          |
 | `GITHUB_ENTERPRISE_TOKEN` | Takes precedence over `GITHUB_TOKEN` when set                                                                                                |                          |
 | `GH_HOST`                 | The Github Host to communicate with (Override this with your company's GitHub Enterprise server if needed)                                   | `https://api.github.com` |
```

### Comparing `prfiesta-0.8.0/prfiesta/__main__.py` & `prfiesta-0.8.0b124/prfiesta/__main__.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/prfiesta/analysis/plot.py` & `prfiesta-0.8.0b124/prfiesta/analysis/plot.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/prfiesta/analysis/view.py` & `prfiesta-0.8.0b124/prfiesta/analysis/view.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/prfiesta/collectors/github.py` & `prfiesta-0.8.0b124/prfiesta/collectors/github.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/prfiesta/environment.py` & `prfiesta-0.8.0b124/prfiesta/environment.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/prfiesta/output.py` & `prfiesta-0.8.0b124/prfiesta/output.py`

 * *Files identical despite different names*

### Comparing `prfiesta-0.8.0/pyproject.toml` & `prfiesta-0.8.0b124/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "prfiesta"
-version = "0.8.0"
+version = "0.8.0b124"
 description = "Analyze Individual Contributor Pull Requests"
 authors = ["kiran94"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/kiran94/prfiesta"
 repository = "https://github.com/kiran94/prfiesta"
 documentation = "https://github.com/kiran94/prfiesta/blob/main/README.md"
```

### Comparing `prfiesta-0.8.0/PKG-INFO` & `prfiesta-0.8.0b124/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prfiesta
-Version: 0.8.0
+Version: 0.8.0b124
 Summary: Analyze Individual Contributor Pull Requests
 Home-page: https://github.com/kiran94/prfiesta
 License: MIT
 Keywords: pull-request,pull-request-review,performance-review
 Author: kiran94
 Requires-Python: >=3.8,<4.0
 Classifier: Intended Audience :: Developers
@@ -104,31 +104,37 @@
 You can control the output type using the `--output_type` option. Supported options:
 
 - `csv` (default)
 - `parquet`
 
 You can also customize the output file name using the `--output` option.
 
-### Time Filter
+### Date Filter
 
-When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` time dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
+When using the `--after` and `--before` date filters, by default `prfiesta` will use the `created` date dimension with these filters on the Git provider (e.g GitHub). This may not fit your use case and you may want to filter on when a pull request was updated instead. To do this you can use the `--use_updated` flag.
 
 See more information [here](https://docs.github.com/en/search-github/searching-on-github/searching-issues-and-pull-requests#search-by-when-an-issue-or-pull-request-was-created-or-last-updated).
 
 ## Analysis
 
 `prfiesta` ships with built in plots to help analyze your pull request data. These serve as a starting point in your analysis. See more information on the build in plots and views [here](./docs/analysis.md).
 
 ## Using GitHub Enterprise
 
 If you trying to fetch data from a [GitHub Enterprise](https://docs.github.com/en/enterprise-cloud@latest/rest/enterprise-admin?apiVersion=2022-11-28) server, then much of the same functionality should work the same. You just need to make sure that:
 
 - `GH_HOST` is set to your enterprise instance's API URL. Reach out to your internal GitHub team if you are not sure what this should be.
 - `GITHUB_ENTERPRISE_TOKEN` a [personal access token](https://docs.github.com/en/enterprise-cloud@latest/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) generated on your GitHub Enterprise instance.
 
+## GitHub Rate Limiting
+
+Depending on your input parameters, you may end up in a situation where you are being [Rate Limited](https://docs.github.com/en/rest/overview/resources-in-the-rest-api?apiVersion=2022-11-28#rate-limiting) by the GitHub API.
+
+See this [Notebook](./notebooks/misc/rate_limit.ipynb) on a way to handle this.
+
 ## Environment Variables
 
 | Variable                  | Description                                                                                                                                  | Default                  |
 | ---------------           | ---------------                                                                                                                              | ------                   |
 | `GITHUB_TOKEN`            | The Github [`Token`](https://docs.github.com/en/authentication/keeping-your-account-and-data-secure/creating-a-personal-access-token) to use |                          |
 | `GITHUB_ENTERPRISE_TOKEN` | Takes precedence over `GITHUB_TOKEN` when set                                                                                                |                          |
 | `GH_HOST`                 | The Github Host to communicate with (Override this with your company's GitHub Enterprise server if needed)                                   | `https://api.github.com` |
```

