# Comparing `tmp/faust-streaming-0.9.4rc1.tar.gz` & `tmp/faust-streaming-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faust-streaming-0.9.4rc1.tar", last modified: Fri Nov  4 18:50:57 2022, max compression
+gzip compressed data, was "faust-streaming-0.9.5.tar", last modified: Mon Nov 21 21:46:48 2022, max compression
```

## Comparing `faust-streaming-0.9.4rc1.tar` & `faust-streaming-0.9.5.tar`

### file list

```diff
@@ -1,831 +1,831 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/
--rw-r--r--   0 runner    (1001) docker     (121)      967 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/.github/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)      537 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      491 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/workflows/dist.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/workflows/gh-pages.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (121)      489 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (121)    27389 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)    23042 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    17044 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/TODO.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/artwork/
--rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/artwork/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    18109 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/artwork/banner-alt1.png
--rw-r--r--   0 runner    (1001) docker     (121)    18238 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/artwork/banner-alt2.png
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/artwork/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     7635 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/artwork/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     8844 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/_ext/
--rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/_ext/faustdocs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6737 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/_ext/typehints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/_static/.keep
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/_templates/.keep
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)    22743 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/copyright.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/developerguide/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/developerguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/developerguide/overview.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/developerguide/partition_assignor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/faq.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/glossary.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/history/
--rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-0.9.rst
--rw-r--r--   0 runner    (1001) docker     (121)    22837 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.0.rst
--rw-r--r--   0 runner    (1001) docker     (121)    15975 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.1.rst
--rw-r--r--   0 runner    (1001) docker     (121)    13076 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.10.rst
--rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.2.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.3.rst
--rw-r--r--   0 runner    (1001) docker     (121)    11398 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.4.rst
--rw-r--r--   0 runner    (1001) docker     (121)    14788 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.5.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.6.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10030 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.7.rst
--rw-r--r--   0 runner    (1001) docker     (121)     8604 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.8.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/changelog-1.9.rst
--rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/history/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.602848 faust-streaming-0.9.4rc1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (121)    18109 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/images/banner-alt1.png
--rw-r--r--   0 runner    (1001) docker     (121)    18238 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/images/banner-alt2.png
--rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/images/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (121)     7635 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/images/logo.png
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.606848 faust-streaming-0.9.4rc1/docs/includes/
--rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/blurb.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/code-of-conduct.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/faq.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/installation.txt
--rw-r--r--   0 runner    (1001) docker     (121)     5140 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/intro.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/introduction.txt
--rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/kafka.txt
--rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/resources.txt
--rw-r--r--   0 runner    (1001) docker     (121)    60257 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/settingref.txt
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/includes/tags.txt
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10694 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/introduction.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.606848 faust-streaming-0.9.4rc1/docs/keepachangelog/
--rw-r--r--   0 runner    (1001) docker     (121)      350 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/keepachangelog/changelog.md
--rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/keepachangelog/commit.md
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/keepachangelog/section.md
--rw-r--r--   0 runner    (1001) docker     (121)      543 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/keepachangelog/version.md
--rw-r--r--   0 runner    (1001) docker     (121)     7204 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.606848 faust-streaming-0.9.4rc1/docs/playbooks/
--rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/cheatsheet.rst
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/leaderelection.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/pageviews.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/quickstart.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/vscelery.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/playbooks/vskafka.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.614848 faust-streaming-0.9.4rc1/docs/reference/
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.actor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.agent.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.manager.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.replies.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.agents.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.app.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.app.router.rst
--rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.app.rst
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.assignor.client_assignment.rst
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.assignor.cluster_assignment.rst
--rw-r--r--   0 runner    (1001) docker     (121)      324 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.assignor.copartitioned_assignor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.assignor.leader_assignor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.assignor.partition_assignor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.auth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.channels.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.agents.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.clean_versions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.completion.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.faust.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.livecheck.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.model.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.params.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.reset.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.send.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.cli.worker.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.contrib.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.contrib.sentry.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.events.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.fixups.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.fixups.django.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.fixups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.joins.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.app.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.case.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.locals.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.patches.aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.patches.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.runners.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.livecheck.signals.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.models.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.models.fields.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.models.record.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.models.tags.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.models.typing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.datadog.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.monitor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.prometheus.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.sensors.statsd.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.serializers.codecs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.serializers.registry.rst
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.serializers.schemas.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.stores.aerospike.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.stores.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.stores.memory.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.stores.rocksdb.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.stores.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.streams.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.globaltable.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.manager.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.objects.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.recovery.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.sets.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.table.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.tables.wrappers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.topics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.conductor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.consumer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.drivers.aiokafka.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.drivers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.producer.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.transport.utils.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.agents.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.app.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.assignor.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.auth.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.channels.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.codecs.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.core.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.enums.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.events.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.fixups.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.joins.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.models.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.router.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.sensors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.serializers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.settings.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.settings.params.rst
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.settings.sections.rst
--rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.settings.settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.stores.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.streams.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.topics.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.transports.rst
--rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.tuples.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.web.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.types.windows.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.codegen.rst
--rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.cron.rst
--rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.functional.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.iso8601.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.json.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.platforms.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.terminal.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.terminal.spinners.rst
--rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.terminal.tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.tracing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.urls.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.utils.venusian.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.apps.graph.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.apps.router.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.apps.stats.rst
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.blueprints.rst
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.backends.base.rst
--rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.backends.memory.rst
--rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.backends.redis.rst
--rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.backends.rst
--rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.cache.rst
--rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.drivers.aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.drivers.rst
--rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.web.views.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.windows.rst
--rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/faust.worker.rst
--rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/reference/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/spelling_wordlist.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/docs/templates/
--rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/templates/readme.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/docs/userguide/
--rw-r--r--   0 runner    (1001) docker     (121)    17611 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/agents.rst
--rw-r--r--   0 runner    (1001) docker     (121)    43716 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/application.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/channels.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16620 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/cli.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/debugging.rst
--rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/kafka.rst
--rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/livecheck.rst
--rw-r--r--   0 runner    (1001) docker     (121)    31769 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/models.rst
--rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/sensors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/settings.rst
--rw-r--r--   0 runner    (1001) docker     (121)    16290 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/streams.rst
--rw-r--r--   0 runner    (1001) docker     (121)    17049 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/tables.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/tasks.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6069 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/testing.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6275 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/docs/userguide/workers.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/advanced/
--rwxr-xr-x   0 runner    (1001) docker     (121)     3348 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/advanced/isolated_partitions_crashing.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1162 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/advanced/rpc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1015 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/advanced/service.py
--rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/bound_agent.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      650 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/concurrency.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/crontab/
--rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/crontab/tz_aware.py
--rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/crontab/tz_unaware.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/django/
--rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/django/accounts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/agents.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/django/accounts/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/accounts/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/django/faustapp/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/faustapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      602 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/faustapp/app.py
--rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/faustapp/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.618848 faust-streaming-0.9.4rc1/examples/django/faustapp/migrations/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/faustapp/migrations/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      797 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/django/proj/
--rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/proj/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      197 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/proj/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/proj/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/proj/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/proj/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/django/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/requirements/default.txt
--rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/django/setup.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/kubernetes/
--rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/
--rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      872 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)      451 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/consumer.yml
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/consumer/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/kubernetes/producer/
--rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/producer/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/producer/README.md
--rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/producer/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/producer/producer.yml
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/kubernetes/producer/requirements.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)      406 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/leader.py
--rw-r--r--   0 runner    (1001) docker     (121)     6757 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/livecheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/tableofset.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2438 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/tabletest.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2819 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/task_queue.py
--rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/windowed_aggregation.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/examples/windowing/
--rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/windowing/hopping.py
--rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/windowing/hopping_2.py
--rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/windowing/tumbling.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2860 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/withdrawals.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1812 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/examples/word_count.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.594848 faust-streaming-0.9.4rc1/extra/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/bandit/
--rw-r--r--   0 runner    (1001) docker     (121)    58920 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/bandit/baseline.json
--rw-r--r--   0 runner    (1001) docker     (121)     8335 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/bandit/config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/macOS/
--rw-r--r--   0 runner    (1001) docker     (121)      843 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/macOS/com.fauststream.worker.plist
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/release/
--rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/release/sphinx2rst_config.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/supervisord/
--rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/supervisord/faust.conf
--rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/supervisord/supervisord.conf
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/systemd/
--rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/systemd/faust.conf
--rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/systemd/faust.service
--rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/systemd/faust.tmpfiles
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/extra/tools/
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/benchmark.py
--rw-r--r--   0 runner    (1001) docker     (121)     7699 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/render_configuration_reference.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      628 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/verify_ascending.py
--rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/verify_doc_defaults.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1051 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/verify_tabletest.sh
--rw-r--r--   0 runner    (1001) docker     (121)      670 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/extra/tools/verify_tabletest_changelog.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/faust/
--rw-r--r--   0 runner    (1001) docker     (121)     8948 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.622848 faust-streaming-0.9.4rc1/faust/_cython/
--rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7315 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/_cython/streams.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/_cython/windows.pyx
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/agents/
--rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/actor.py
--rw-r--r--   0 runner    (1001) docker     (121)    41704 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/agents/replies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/app/
--rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/app/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/app/_attached.py
--rw-r--r--   0 runner    (1001) docker     (121)    74386 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/app/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/app/router.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/assignor/
--rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/client_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/cluster_assignment.py
--rw-r--r--   0 runner    (1001) docker     (121)    10589 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/copartitioned_assignor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/leader_assignor.py
--rw-r--r--   0 runner    (1001) docker     (121)    17020 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/assignor/partition_assignor.py
--rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)    23234 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/channels.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/cli/
--rw-r--r--   0 runner    (1001) docker     (121)      175 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/agents.py
--rw-r--r--   0 runner    (1001) docker     (121)    32845 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      762 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/clean_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/completion.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/faust.py
--rw-r--r--   0 runner    (1001) docker     (121)      580 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/livecheck.py
--rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/reset.py
--rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/send.py
--rw-r--r--   0 runner    (1001) docker     (121)      635 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     6377 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/cli/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/contrib/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/contrib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/contrib/sentry.py
--rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/events.py
--rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/fixups/
--rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/fixups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      722 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/fixups/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/fixups/django.py
--rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/joins.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/livecheck/
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13396 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/app.py
--rw-r--r--   0 runner    (1001) docker     (121)    17279 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/case.py
--rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      900 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/locals.py
--rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/models.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.626848 faust-streaming-0.9.4rc1/faust/livecheck/patches/
--rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/patches/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/patches/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     7694 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/runners.py
--rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/livecheck/signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/models/
--rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16568 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    18922 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/fields.py
--rw-r--r--   0 runner    (1001) docker     (121)    22164 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/record.py
--rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/tags.py
--rw-r--r--   0 runner    (1001) docker     (121)    21565 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/models/typing.py
--rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11467 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13006 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/datadog.py
--rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/distributed_tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)    24709 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    19443 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9253 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/sensors/statsd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10321 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/serializers/codecs.py
--rw-r--r--   0 runner    (1001) docker     (121)     6440 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/serializers/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/serializers/schemas.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/stores/
--rw-r--r--   0 runner    (1001) docker     (121)      455 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9733 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/stores/aerospike.py
--rw-r--r--   0 runner    (1001) docker     (121)     7431 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/stores/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/stores/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)    23240 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/stores/rocksdb.py
--rw-r--r--   0 runner    (1001) docker     (121)    50406 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/streams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/tables/
--rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    23772 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/globaltable.py
--rw-r--r--   0 runner    (1001) docker     (121)     7421 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    42437 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/recovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/table.py
--rw-r--r--   0 runner    (1001) docker     (121)    18920 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/tables/wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)    18134 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/topics.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/transport/
--rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/transport/_cython/
--rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/_cython/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/_cython/conductor.pyx
--rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    17480 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/conductor.py
--rw-r--r--   0 runner    (1001) docker     (121)    55642 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/consumer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.630848 faust-streaming-0.9.4rc1/faust/transport/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)      357 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    60775 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/drivers/aiokafka.py
--rw-r--r--   0 runner    (1001) docker     (121)     8383 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/transport/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/types/
--rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     8750 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/agents.py
--rw-r--r--   0 runner    (1001) docker     (121)    14784 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/assignor.py
--rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5794 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/channels.py
--rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/codecs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/core.py
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/events.py
--rw-r--r--   0 runner    (1001) docker     (121)      536 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/fixups.py
--rw-r--r--   0 runner    (1001) docker     (121)      542 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/joins.py
--rw-r--r--   0 runner    (1001) docker     (121)     7812 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/router.py
--rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/sensors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/serializers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/types/settings/
--rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/settings/base.py
--rw-r--r--   0 runner    (1001) docker     (121)    22607 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/settings/params.py
--rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/settings/sections.py
--rw-r--r--   0 runner    (1001) docker     (121)    81664 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/settings/settings.py
--rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/stores.py
--rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/streams.py
--rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/topics.py
--rw-r--r--   0 runner    (1001) docker     (121)    13238 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/transports.py
--rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/tuples.py
--rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/web.py
--rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/types/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/_iso8601_python.py
--rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/agent_stopper.py
--rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/cron.py
--rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/functional.py
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/iso8601.py
--rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/json.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/utils/kafka/
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/kafka/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/admin.py
--rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/platforms.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/utils/terminal/
--rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/terminal/spinners.py
--rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/terminal/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/tracing.py
--rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/utils/venusian.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/web/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.634848 faust-streaming-0.9.4rc1/faust/web/apps/
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/graph.py
--rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/production_index.py
--rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/router.py
--rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/stats.py
--rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/apps/tables.py
--rw-r--r--   0 runner    (1001) docker     (121)    11674 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/blueprints.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/faust/web/cache/
--rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/faust/web/cache/backends/
--rw-r--r--   0 runner    (1001) docker     (121)      533 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/backends/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/backends/base.py
--rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/backends/memory.py
--rw-r--r--   0 runner    (1001) docker     (121)     6128 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/backends/redis.py
--rw-r--r--   0 runner    (1001) docker     (121)     6303 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/cache.py
--rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/cache/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/faust/web/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/drivers/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/web/views.py
--rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/windows.py
--rw-r--r--   0 runner    (1001) docker     (121)    14142 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/faust/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/faust_streaming.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    23042 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    22066 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      844 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-04 18:50:57.000000 faust-streaming-0.9.4rc1/faust_streaming.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/requirements/
--rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/ci.txt
--rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/dist.txt
--rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/docs.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/aerospike.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/aiodns.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/aiomonitor.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/cchardet.txt
--rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/ciso8601.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/cython.txt
--rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/datadog.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/debug.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/eventlet.txt
--rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/fast.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/orjson.txt
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/prometheus.txt
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/redis.txt
--rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/rocksdb.txt
--rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/sentry.txt
--rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/setproctitle.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/statsd.txt
--rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/uvloop.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/extras/yaml.txt
--rw-r--r--   0 runner    (1001) docker     (121)      237 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/test.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/requirements/typecheck.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.638848 faust-streaming-0.9.4rc1/scripts/
--rwxr-xr-x   0 runner    (1001) docker     (121)      543 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/README.md
--rwxr-xr-x   0 runner    (1001) docker     (121)      187 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/build
--rwxr-xr-x   0 runner    (1001) docker     (121)      304 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/check
--rwxr-xr-x   0 runner    (1001) docker     (121)      242 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/clean
--rwxr-xr-x   0 runner    (1001) docker     (121)      199 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/coverage
--rwxr-xr-x   0 runner    (1001) docker     (121)      119 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/docs
--rwxr-xr-x   0 runner    (1001) docker     (121)      480 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/install
--rwxr-xr-x   0 runner    (1001) docker     (121)      270 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/lint
--rwxr-xr-x   0 runner    (1001) docker     (121)      389 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/scripts/tests
--rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     6907 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/bench/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/bench/base.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      244 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/bench/baseline.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      837 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/bench/forward.py
--rw-r--r--   0 runner    (1001) docker     (121)     8780 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/consistency/
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/consistency/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/consistency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8075 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/consistency/consistency_checker.py
--rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/consistency/test_consistency.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/agents/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/agents/helpers.py
--rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/agents/test_concurrency.py
--rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/agents/test_current_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/agents/test_isolated_partitions.py
--rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12309 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/models/test_typing.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/sensors/test_statsd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/serializers/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_aiokafka.py
--rw-r--r--   0 runner    (1001) docker     (121)    39511 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_channels.py
--rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_faust.py
--rw-r--r--   0 runner    (1001) docker     (121)    43494 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)    28914 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/test_streams.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/functional/web/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/web/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    14125 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/web/test_cache.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/web/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/functional/web/test_views.py
--rw-r--r--   0 runner    (1001) docker     (121)      842 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/integration/
--rwxr-xr-x   0 runner    (1001) docker     (121)      768 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/app.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/integration/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/cli/test_agents.py
--rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/cli/test_model.py
--rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/cli/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/integration/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.598848 faust-streaming-0.9.4rc1/tests/meticulous/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/meticulous/assignor/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/meticulous/assignor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5609 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/meticulous/assignor/test_copartitioned_assignor.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/old/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/old/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/old/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/old/test_simple.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/regression/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.642848 faust-streaming-0.9.4rc1/tests/regression/i323/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/faust.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/bar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/bar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/bar/baz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/bar/baz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/proj323/foo/bar/baz/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i323/test_autodiscover.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i324/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/faust.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/bar/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/bar/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/bar/baz/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/bar/baz/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/bar/baz/commands.py
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/proj324/foo/test_x.py
--rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/regression/i324/test_autodiscover.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/app.py
--rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/killer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/producer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/reports/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/app.py
--rw-r--r--   0 runner    (1001) docker     (121)     7344 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/checks.py
--rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/collector.py
--rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/models.py
--rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/states.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/reports/templates/
--rwxr-xr-x   0 runner    (1001) docker     (121)     9468 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/templates/dashboard.html
--rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/reports/web.py
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/tests/forwarder/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/forwarder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/forwarder/app.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/forwarder/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/tests/simple/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/simple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/simple/app.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/simple/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/stress/tests/tables/
--rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/tables/app.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/stress/tests/tables/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.646848 faust-streaming-0.9.4rc1/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/agents/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/agents/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/agents/test_actor.py
--rw-r--r--   0 runner    (1001) docker     (121)    33389 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/agents/test_agent.py
--rw-r--r--   0 runner    (1001) docker     (121)     4008 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/agents/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/agents/test_replies.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/app/
--rw-r--r--   0 runner    (1001) docker     (121)    42781 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/app/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/app/test_router.py
--rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/app/test_service.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/conftest.py
--rw-r--r--   0 runner    (1001) docker     (121)    23550 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/test_clean_versions.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/test_completion.py
--rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/test_env.py
--rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/cli/test_params.py
--rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/fixups/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/fixups/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/fixups/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/fixups/test_django.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/livecheck/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/livecheck/patches/
--rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/patches/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)    10489 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_app.py
--rw-r--r--   0 runner    (1001) docker     (121)    19775 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_case.py
--rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_locals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_models.py
--rw-r--r--   0 runner    (1001) docker     (121)     8700 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_runners.py
--rw-r--r--   0 runner    (1001) docker     (121)     9116 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/livecheck/test_signals.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/models/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5971 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/models/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (121)      726 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/models/test_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/sensors/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)    13614 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/test_datadog.py
--rw-r--r--   0 runner    (1001) docker     (121)    17056 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/test_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)    16309 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/test_prometheus.py
--rw-r--r--   0 runner    (1001) docker     (121)     9503 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/sensors/test_statsd.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/serializers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/serializers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/serializers/test_codecs.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/stores/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/stores/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8669 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/stores/test_aerospike.py
--rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/stores/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     4635 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/stores/test_memory.py
--rw-r--r--   0 runner    (1001) docker     (121)    25221 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/stores/test_rocksdb.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.650848 faust-streaming-0.9.4rc1/tests/unit/tables/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    22060 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (121)     4728 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (121)    13966 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_recovery.py
--rw-r--r--   0 runner    (1001) docker     (121)    14096 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_sets.py
--rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_table.py
--rw-r--r--   0 runner    (1001) docker     (121)    17193 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/tables/test_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (121)     5784 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_events.py
--rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_faust.py
--rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_joins.py
--rw-r--r--   0 runner    (1001) docker     (121)     7926 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_streams.py
--rw-r--r--   0 runner    (1001) docker     (121)    18043 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_topics.py
--rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/test_worker.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/transport/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/transport/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    69289 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/drivers/test_aiokafka.py
--rw-r--r--   0 runner    (1001) docker     (121)     8555 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/test_conductor.py
--rw-r--r--   0 runner    (1001) docker     (121)    46456 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (121)     8961 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/test_producer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/transport/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/utils/terminal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/terminal/test_spinners.py
--rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/terminal/test_tables.py
--rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_cron.py
--rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_iso8601.py
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_urls.py
--rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/utils/test_venusian.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/web/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/web/drivers/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/drivers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    11169 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/drivers/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/test_base.py
--rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/test_blueprints.py
--rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/web/test_views.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-04 18:50:57.654848 faust-streaming-0.9.4rc1/tests/unit/windows/
--rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/windows/test_hopping_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/windows/test_sliding_window.py
--rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tests/unit/windows/test_tumbling_window.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-04 18:50:26.000000 faust-streaming-0.9.4rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.181380 faust-streaming-0.9.5/.github/
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)      537 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      491 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (121)      295 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.181380 faust-streaming-0.9.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2448 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1890 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/workflows/dist.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1223 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/workflows/gh-pages.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1327 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (121)      489 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)      623 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     3484 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (121)    27389 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (121)     2490 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      385 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     6915 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/Makefile
+-rw-r--r--   0 runner    (1001) docker     (121)    23039 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    17044 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     4471 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/TODO.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.181380 faust-streaming-0.9.5/artwork/
+-rw-r--r--   0 runner    (1001) docker     (121)      242 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/artwork/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    18109 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/artwork/banner-alt1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18238 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/artwork/banner-alt2.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/artwork/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     7635 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/artwork/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (121)     8844 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/_ext/
+-rw-r--r--   0 runner    (1001) docker     (121)     4040 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/_ext/faustdocs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6737 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/_ext/typehints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/_static/.keep
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/_templates/.keep
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3696 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22743 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      927 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/copyright.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/developerguide/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/developerguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4357 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/developerguide/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5085 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/developerguide/partition_assignor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4053 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/glossary.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.185380 faust-streaming-0.9.5/docs/history/
+-rw-r--r--   0 runner    (1001) docker     (121)     1623 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-0.9.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    22837 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.0.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    15975 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.1.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    13076 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.10.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     9151 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.2.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2900 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.3.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    11398 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.4.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    14788 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.5.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2384 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.6.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10030 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.7.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     8604 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.8.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/changelog-1.9.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      434 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/history/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.189380 faust-streaming-0.9.5/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (121)    18109 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/images/banner-alt1.png
+-rw-r--r--   0 runner    (1001) docker     (121)    18238 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/images/banner-alt2.png
+-rw-r--r--   0 runner    (1001) docker     (121)     1150 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/images/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (121)     7635 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/images/logo.png
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.189380 faust-streaming-0.9.5/docs/includes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1302 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/blurb.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2050 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/code-of-conduct.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2172 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/faq.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2496 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/installation.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     5140 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/intro.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2454 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/introduction.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     4870 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/kafka.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      845 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/resources.txt
+-rw-r--r--   0 runner    (1001) docker     (121)    60257 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/settingref.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/includes/tags.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10694 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/introduction.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.189380 faust-streaming-0.9.5/docs/keepachangelog/
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/keepachangelog/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (121)      435 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/keepachangelog/commit.md
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/keepachangelog/section.md
+-rw-r--r--   0 runner    (1001) docker     (121)      543 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/keepachangelog/version.md
+-rw-r--r--   0 runner    (1001) docker     (121)     7204 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.189380 faust-streaming-0.9.5/docs/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (121)     2854 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/cheatsheet.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3331 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/leaderelection.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4378 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/pageviews.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3882 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/quickstart.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2165 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/vscelery.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5618 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/playbooks/vskafka.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.213380 faust-streaming-0.9.5/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.actor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.agent.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.manager.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.replies.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.agents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.app.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.app.router.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      240 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.assignor.client_assignment.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.assignor.cluster_assignment.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      324 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.assignor.copartitioned_assignor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.assignor.leader_assignor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      312 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.assignor.partition_assignor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      243 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.channels.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.agents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.clean_versions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.completion.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.faust.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.livecheck.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.model.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.params.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.reset.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.send.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.cli.worker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.contrib.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.contrib.sentry.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.events.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.fixups.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.fixups.django.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.fixups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      246 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.joins.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.case.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.locals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.patches.aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.patches.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.runners.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.livecheck.signals.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.models.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.models.fields.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.models.record.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.models.tags.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.models.typing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      228 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.datadog.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.monitor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.prometheus.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.sensors.statsd.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.serializers.codecs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.serializers.registry.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.serializers.schemas.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.stores.aerospike.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.stores.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.stores.memory.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.stores.rocksdb.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.stores.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.streams.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.globaltable.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.manager.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.objects.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.recovery.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.sets.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.table.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.tables.wrappers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.topics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.conductor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.consumer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      309 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.drivers.aiokafka.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.drivers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.producer.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.transport.utils.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.agents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.app.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.assignor.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.auth.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.channels.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.codecs.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.core.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.enums.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.events.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.fixups.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.joins.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.router.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.serializers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.settings.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.settings.params.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.settings.sections.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      301 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.settings.settings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.stores.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.streams.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.topics.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.transports.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      267 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.tuples.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.web.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.types.windows.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.codegen.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.cron.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.functional.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.iso8601.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.json.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.platforms.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.terminal.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.terminal.spinners.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      294 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.terminal.tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.tracing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      261 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.urls.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.utils.venusian.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.apps.graph.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.apps.router.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.apps.stats.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      255 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.blueprints.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      300 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.backends.base.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      306 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.backends.memory.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      303 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.backends.redis.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      285 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.backends.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      276 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.cache.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      288 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.drivers.aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.drivers.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      258 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.web.views.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      252 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.windows.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      249 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/faust.worker.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     4523 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/reference/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     5832 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/spelling_wordlist.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.213380 faust-streaming-0.9.5/docs/templates/
+-rw-r--r--   0 runner    (1001) docker     (121)     2108 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/templates/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.213380 faust-streaming-0.9.5/docs/userguide/
+-rw-r--r--   0 runner    (1001) docker     (121)    17611 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/agents.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    43716 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/application.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2791 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/channels.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16620 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/cli.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     3674 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/debugging.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      320 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/index.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      206 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/kafka.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     2303 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/livecheck.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    31769 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/models.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     7781 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/sensors.rst
+-rw-r--r--   0 runner    (1001) docker     (121)      694 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/settings.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    16290 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/streams.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    17049 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/tables.rst
+-rw-r--r--   0 runner    (1001) docker     (121)    10621 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/tasks.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6069 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/testing.rst
+-rw-r--r--   0 runner    (1001) docker     (121)     6275 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/docs/userguide/workers.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/advanced/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3348 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/advanced/isolated_partitions_crashing.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1162 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/advanced/rpc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1015 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/advanced/service.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/bound_agent.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      650 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/concurrency.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/crontab/
+-rw-r--r--   0 runner    (1001) docker     (121)      893 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/crontab/tz_aware.py
+-rw-r--r--   0 runner    (1001) docker     (121)      734 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/crontab/tz_unaware.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/django/
+-rw-r--r--   0 runner    (1001) docker     (121)     1003 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/django/accounts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      756 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/agents.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/django/accounts/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)     1193 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/accounts/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/django/faustapp/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/faustapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      602 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/faustapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/faustapp/apps.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.217380 faust-streaming-0.9.5/examples/django/faustapp/migrations/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/faustapp/migrations/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      797 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/manage.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/django/proj/
+-rw-r--r--   0 runner    (1001) docker     (121)     1053 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/proj/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      197 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/proj/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3401 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/proj/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)      761 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/proj/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      386 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/proj/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/django/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       49 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/requirements/default.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       32 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2721 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/django/setup.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      458 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (121)     1805 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/kubernetes/consumer/
+-rw-r--r--   0 runner    (1001) docker     (121)      204 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/consumer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      651 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/consumer/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)      872 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/consumer/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      451 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/consumer/consumer.yml
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/consumer/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/kubernetes/producer/
+-rw-r--r--   0 runner    (1001) docker     (121)      178 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/producer/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/producer/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)     1381 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/producer/producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)      387 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/producer/producer.yml
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/kubernetes/producer/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (121)      406 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/leader.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6757 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/livecheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1293 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/tableofset.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2438 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/tabletest.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2819 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/task_queue.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1659 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/windowed_aggregation.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/examples/windowing/
+-rw-r--r--   0 runner    (1001) docker     (121)     2338 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/windowing/hopping.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2820 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/windowing/hopping_2.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2141 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/windowing/tumbling.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2860 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/withdrawals.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1812 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/examples/word_count.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.173380 faust-streaming-0.9.5/extra/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/extra/bandit/
+-rw-r--r--   0 runner    (1001) docker     (121)    58920 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/bandit/baseline.json
+-rw-r--r--   0 runner    (1001) docker     (121)     8335 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/bandit/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/extra/macOS/
+-rw-r--r--   0 runner    (1001) docker     (121)      843 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/macOS/com.fauststream.worker.plist
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/extra/release/
+-rw-r--r--   0 runner    (1001) docker     (121)      372 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/release/sphinx2rst_config.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/extra/supervisord/
+-rw-r--r--   0 runner    (1001) docker     (121)      917 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/supervisord/faust.conf
+-rw-r--r--   0 runner    (1001) docker     (121)     1082 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/supervisord/supervisord.conf
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.221380 faust-streaming-0.9.5/extra/systemd/
+-rw-r--r--   0 runner    (1001) docker     (121)      436 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/systemd/faust.conf
+-rw-r--r--   0 runner    (1001) docker     (121)      336 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/systemd/faust.service
+-rw-r--r--   0 runner    (1001) docker     (121)       72 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/systemd/faust.tmpfiles
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.225380 faust-streaming-0.9.5/extra/tools/
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7699 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/render_configuration_reference.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      628 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/verify_ascending.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3720 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/verify_doc_defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1051 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/verify_tabletest.sh
+-rw-r--r--   0 runner    (1001) docker     (121)      670 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/extra/tools/verify_tabletest_changelog.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.225380 faust-streaming-0.9.5/faust/
+-rw-r--r--   0 runner    (1001) docker     (121)     8948 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.225380 faust-streaming-0.9.5/faust/_cython/
+-rw-r--r--   0 runner    (1001) docker     (121)       39 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7315 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/_cython/streams.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     3402 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/_cython/windows.pyx
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.225380 faust-streaming-0.9.5/faust/agents/
+-rw-r--r--   0 runner    (1001) docker     (121)      317 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2984 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/actor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    41704 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4447 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)      961 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6669 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/agents/replies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.229380 faust-streaming-0.9.5/faust/app/
+-rw-r--r--   0 runner    (1001) docker     (121)       90 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/app/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7446 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/app/_attached.py
+-rw-r--r--   0 runner    (1001) docker     (121)    74386 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/app/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4480 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/app/router.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.229380 faust-streaming-0.9.5/faust/assignor/
+-rw-r--r--   0 runner    (1001) docker     (121)      145 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/client_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/cluster_assignment.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10589 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/copartitioned_assignor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1466 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/leader_assignor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17020 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/assignor/partition_assignor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3002 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23234 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/channels.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.229380 faust-streaming-0.9.5/faust/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)      175 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1868 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/agents.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32845 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      762 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/clean_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/completion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/faust.py
+-rw-r--r--   0 runner    (1001) docker     (121)      580 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/livecheck.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2805 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1675 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2101 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/params.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1088 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/reset.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2931 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/send.py
+-rw-r--r--   0 runner    (1001) docker     (121)      635 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6377 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/cli/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.229380 faust-streaming-0.9.5/faust/contrib/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/contrib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4697 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/contrib/sentry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8140 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2609 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.233380 faust-streaming-0.9.5/faust/fixups/
+-rw-r--r--   0 runner    (1001) docker     (121)      751 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/fixups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      722 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/fixups/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2754 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/fixups/django.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1132 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/joins.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.233380 faust-streaming-0.9.5/faust/livecheck/
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13396 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17279 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/case.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1228 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      900 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/locals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4120 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/models.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.233380 faust-streaming-0.9.5/faust/livecheck/patches/
+-rw-r--r--   0 runner    (1001) docker     (121)      226 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2770 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/patches/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7694 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/runners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6124 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/livecheck/signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.233380 faust-streaming-0.9.5/faust/models/
+-rw-r--r--   0 runner    (1001) docker     (121)      290 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16568 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18922 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22164 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/record.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5187 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/tags.py
+-rw-r--r--   0 runner    (1001) docker     (121)    21565 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/models/typing.py
+-rw-r--r--   0 runner    (1001) docker     (121)       56 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.233380 faust-streaming-0.9.5/faust/sensors/
+-rw-r--r--   0 runner    (1001) docker     (121)      181 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11467 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13006 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/datadog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5959 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/distributed_tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24709 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19443 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9253 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/sensors/statsd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)      158 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10321 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/serializers/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6440 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/serializers/registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6662 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/serializers/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/stores/
+-rw-r--r--   0 runner    (1001) docker     (121)      455 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9733 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/stores/aerospike.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7431 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/stores/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3238 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/stores/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23240 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/stores/rocksdb.py
+-rw-r--r--   0 runner    (1001) docker     (121)    50406 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/streams.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/tables/
+-rw-r--r--   0 runner    (1001) docker     (121)      378 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23772 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      433 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/globaltable.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7421 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6062 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    42437 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/recovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10092 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3252 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18920 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/tables/wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18134 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/topics.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/transport/
+-rw-r--r--   0 runner    (1001) docker     (121)       88 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/transport/_cython/
+-rw-r--r--   0 runner    (1001) docker     (121)       45 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/_cython/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5132 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/_cython/conductor.pyx
+-rw-r--r--   0 runner    (1001) docker     (121)     2472 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17480 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/conductor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    55642 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/consumer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.237380 faust-streaming-0.9.5/faust/transport/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)      357 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    60775 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/drivers/aiokafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8383 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3920 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/transport/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.241380 faust-streaming-0.9.5/faust/types/
+-rw-r--r--   0 runner    (1001) docker     (121)     2035 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1385 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8750 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/agents.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14784 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/assignor.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1227 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5794 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/channels.py
+-rw-r--r--   0 runner    (1001) docker     (121)      788 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/codecs.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2197 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/core.py
+-rw-r--r--   0 runner    (1001) docker     (121)      127 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2135 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/events.py
+-rw-r--r--   0 runner    (1001) docker     (121)      536 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/fixups.py
+-rw-r--r--   0 runner    (1001) docker     (121)      542 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/joins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7812 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1273 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/router.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3783 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3473 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.241380 faust-streaming-0.9.5/faust/types/settings/
+-rw-r--r--   0 runner    (1001) docker     (121)      110 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6543 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/settings/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22607 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/settings/params.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3436 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/settings/sections.py
+-rw-r--r--   0 runner    (1001) docker     (121)    81664 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/settings/settings.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2638 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/stores.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12089 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3582 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/topics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13238 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/transports.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7069 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/tuples.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4274 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/web.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1023 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/types/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.245380 faust-streaming-0.9.5/faust/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)      184 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/_iso8601_python.py
+-rw-r--r--   0 runner    (1001) docker     (121)      415 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/agent_stopper.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7095 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)      621 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/cron.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1435 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/functional.py
+-rw-r--r--   0 runner    (1001) docker     (121)      264 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5456 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/json.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.245380 faust-streaming-0.9.5/faust/utils/kafka/
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/kafka/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.245380 faust-streaming-0.9.5/faust/utils/kafka/protocol/
+-rw-r--r--   0 runner    (1001) docker     (121)       34 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/kafka/protocol/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/kafka/protocol/admin.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1421 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/kafka/protocol/api.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/platforms.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.245380 faust-streaming-0.9.5/faust/utils/terminal/
+-rw-r--r--   0 runner    (1001) docker     (121)      291 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3339 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/terminal/spinners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2564 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/terminal/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4349 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/tracing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2484 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      710 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/utils/venusian.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.245380 faust-streaming-0.9.5/faust/web/
+-rw-r--r--   0 runner    (1001) docker     (121)      334 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/faust/web/apps/
+-rw-r--r--   0 runner    (1001) docker     (121)       25 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      906 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/graph.py
+-rw-r--r--   0 runner    (1001) docker     (121)      473 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/production_index.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2508 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/router.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1594 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/stats.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3128 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/apps/tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11674 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5701 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/blueprints.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/faust/web/cache/
+-rw-r--r--   0 runner    (1001) docker     (121)       61 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/faust/web/cache/backends/
+-rw-r--r--   0 runner    (1001) docker     (121)      533 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/backends/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3117 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/backends/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3016 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/backends/memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6128 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/backends/redis.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6303 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)      143 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/cache/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/faust/web/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)      379 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10314 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/drivers/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11493 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/web/views.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5025 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/windows.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14142 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/faust/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/faust_streaming.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    23039 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    22066 2022-11-21 21:46:48.000000 faust-streaming-0.9.5/faust_streaming.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       47 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)      851 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-21 21:46:47.000000 faust-streaming-0.9.5/faust_streaming.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.249380 faust-streaming-0.9.5/requirements/
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/ci.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/dist.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      107 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/docs.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.253380 faust-streaming-0.9.5/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/aerospike.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/aiodns.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/aiomonitor.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/cchardet.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        9 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/ciso8601.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/cython.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        8 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/datadog.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/debug.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/eventlet.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       94 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/fast.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/orjson.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       17 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/prometheus.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       19 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/redis.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       31 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/rocksdb.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       59 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/sentry.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       18 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/setproctitle.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/statsd.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       14 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/uvloop.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/extras/yaml.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      244 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      498 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/test.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/requirements/typecheck.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.253380 faust-streaming-0.9.5/scripts/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      543 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (121)      187 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/build
+-rwxr-xr-x   0 runner    (1001) docker     (121)      304 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/check
+-rwxr-xr-x   0 runner    (1001) docker     (121)      242 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/clean
+-rwxr-xr-x   0 runner    (1001) docker     (121)      199 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/coverage
+-rwxr-xr-x   0 runner    (1001) docker     (121)      119 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/docs
+-rwxr-xr-x   0 runner    (1001) docker     (121)      480 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/install
+-rwxr-xr-x   0 runner    (1001) docker     (121)      270 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/lint
+-rwxr-xr-x   0 runner    (1001) docker     (121)      389 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/scripts/tests
+-rw-r--r--   0 runner    (1001) docker     (121)      405 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     6907 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/bench/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3821 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/bench/base.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      244 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/bench/baseline.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      837 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/bench/forward.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8780 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/consistency/
+-rw-r--r--   0 runner    (1001) docker     (121)        7 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/consistency/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/consistency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8075 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/consistency/consistency_checker.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6216 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/consistency/test_consistency.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/functional/agents/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6665 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/agents/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1803 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/agents/test_concurrency.py
+-rw-r--r--   0 runner    (1001) docker     (121)      481 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/agents/test_current_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2839 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/agents/test_isolated_partitions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3246 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)      771 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/functional/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12309 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/models/test_typing.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.257380 faust-streaming-0.9.5/tests/functional/sensors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      907 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/sensors/test_statsd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/functional/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5991 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/serializers/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (121)      199 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_aiokafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)    39511 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7024 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_channels.py
+-rw-r--r--   0 runner    (1001) docker     (121)       53 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_faust.py
+-rw-r--r--   0 runner    (1001) docker     (121)    43494 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)    28914 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/test_streams.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/functional/web/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      563 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/web/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14125 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/web/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/web/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1694 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/functional/web/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (121)      842 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/integration/
+-rwxr-xr-x   0 runner    (1001) docker     (121)      768 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/app.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/integration/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      980 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/cli/test_agents.py
+-rw-r--r--   0 runner    (1001) docker     (121)      170 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      984 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/cli/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (121)      953 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/cli/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1598 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/integration/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.177380 faust-streaming-0.9.5/tests/meticulous/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/meticulous/assignor/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/meticulous/assignor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5609 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/meticulous/assignor/test_copartitioned_assignor.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/old/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/old/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      278 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/old/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/old/test_simple.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/regression/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/regression/i323/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/regression/i323/proj323/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/faust.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.261380 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/bar/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/bar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/bar/baz/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/bar/baz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/proj323/foo/bar/baz/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1050 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i323/test_autodiscover.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i324/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      214 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i324/proj324/
+-rw-r--r--   0 runner    (1001) docker     (121)       87 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)       69 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      154 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/faust.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/bar/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/bar/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/bar/baz/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/bar/baz/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      105 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/bar/baz/commands.py
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/proj324/foo/test_x.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1162 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/regression/i324/test_autodiscover.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/stress/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2200 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)      966 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/config.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2743 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/killer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1009 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1718 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/producer.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/stress/reports/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2055 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7344 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/checks.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2109 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/collector.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1940 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/logging.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1450 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/models.py
+-rw-r--r--   0 runner    (1001) docker     (121)      193 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/states.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.265380 faust-streaming-0.9.5/tests/stress/reports/templates/
+-rwxr-xr-x   0 runner    (1001) docker     (121)     9468 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/templates/dashboard.html
+-rw-r--r--   0 runner    (1001) docker     (121)      197 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/reports/web.py
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/stress/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/stress/tests/forwarder/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/forwarder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3663 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/forwarder/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/forwarder/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/stress/tests/simple/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/simple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      650 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/simple/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/simple/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/stress/tests/tables/
+-rw-r--r--   0 runner    (1001) docker     (121)       40 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5133 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/tables/app.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/stress/tests/tables/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/unit/agents/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/agents/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3234 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/agents/test_actor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    33389 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/agents/test_agent.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4008 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/agents/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7953 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/agents/test_replies.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.269380 faust-streaming-0.9.5/tests/unit/app/
+-rw-r--r--   0 runner    (1001) docker     (121)    42781 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/app/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5664 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/app/test_router.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4946 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/app/test_service.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (121)    23550 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1004 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/test_clean_versions.py
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/test_completion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      205 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/test_env.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1371 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/cli/test_params.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1012 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/fixups/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/fixups/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      388 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/fixups/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2940 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/fixups/test_django.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/livecheck/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1306 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/livecheck/patches/
+-rw-r--r--   0 runner    (1001) docker     (121)     1886 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/patches/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10489 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_app.py
+-rw-r--r--   0 runner    (1001) docker     (121)    19775 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_case.py
+-rw-r--r--   0 runner    (1001) docker     (121)      672 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_locals.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1602 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8700 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_runners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9116 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/livecheck/test_signals.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/models/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5971 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/models/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (121)      726 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/models/test_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/sensors/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8056 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13614 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/test_datadog.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17056 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/test_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16309 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/test_prometheus.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9503 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/sensors/test_statsd.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.273380 faust-streaming-0.9.5/tests/unit/serializers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/serializers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2114 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/serializers/test_codecs.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.277380 faust-streaming-0.9.5/tests/unit/stores/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/stores/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8669 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/stores/test_aerospike.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5415 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/stores/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4635 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/stores/test_memory.py
+-rw-r--r--   0 runner    (1001) docker     (121)    25221 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/stores/test_rocksdb.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.277380 faust-streaming-0.9.5/tests/unit/tables/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    22060 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5413 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4728 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (121)    13966 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_recovery.py
+-rw-r--r--   0 runner    (1001) docker     (121)    14096 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_sets.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4937 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17193 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/tables/test_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5016 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5784 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_events.py
+-rw-r--r--   0 runner    (1001) docker     (121)      134 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_faust.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1212 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_joins.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7926 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_streams.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18043 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_topics.py
+-rw-r--r--   0 runner    (1001) docker     (121)    10304 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/test_worker.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.277380 faust-streaming-0.9.5/tests/unit/transport/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.277380 faust-streaming-0.9.5/tests/unit/transport/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    69289 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/drivers/test_aiokafka.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8555 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/test_conductor.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46456 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8961 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/test_producer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1881 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/transport/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/tests/unit/utils/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/tests/unit/utils/terminal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3066 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/terminal/test_spinners.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3417 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/terminal/test_tables.py
+-rw-r--r--   0 runner    (1001) docker     (121)      838 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1030 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_cron.py
+-rw-r--r--   0 runner    (1001) docker     (121)      418 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (121)      754 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_iso8601.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2132 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_urls.py
+-rw-r--r--   0 runner    (1001) docker     (121)      164 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      506 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/utils/test_venusian.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/tests/unit/web/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/tests/unit/web/drivers/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/drivers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    11169 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/drivers/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3438 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1017 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/test_blueprints.py
+-rw-r--r--   0 runner    (1001) docker     (121)      318 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6963 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/web/test_views.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-21 21:46:48.281380 faust-streaming-0.9.5/tests/unit/windows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2286 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/windows/test_hopping_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2085 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/windows/test_sliding_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)      902 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tests/unit/windows/test_tumbling_window.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2022-11-21 21:46:38.000000 faust-streaming-0.9.5/tox.ini
```

### Comparing `faust-streaming-0.9.4rc1/.coveragerc` & `faust-streaming-0.9.5/.coveragerc`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/CODE_OF_CONDUCT.md` & `faust-streaming-0.9.5/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/ISSUE_TEMPLATE.md` & `faust-streaming-0.9.5/.github/ISSUE_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/workflows/codeql-analysis.yml` & `faust-streaming-0.9.5/.github/workflows/codeql-analysis.yml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/workflows/dist.yml` & `faust-streaming-0.9.5/.github/workflows/dist.yml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/workflows/gh-pages.yml` & `faust-streaming-0.9.5/.github/workflows/gh-pages.yml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.github/workflows/python-package.yml` & `faust-streaming-0.9.5/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/.pre-commit-config.yaml` & `faust-streaming-0.9.5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/AUTHORS.md` & `faust-streaming-0.9.5/AUTHORS.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/CHANGELOG.md` & `faust-streaming-0.9.5/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/CODE_OF_CONDUCT.md` & `faust-streaming-0.9.5/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/LICENSE` & `faust-streaming-0.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/Makefile` & `faust-streaming-0.9.5/Makefile`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/PKG-INFO` & `faust-streaming-0.9.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faust-streaming
-Version: 0.9.4rc1
+Version: 0.9.5
 Summary: Python Stream processing.
 Home-page: https://github.com/faust-streaming/faust
 Author: Robinhood Markets, Inc.
 Author-email: schrohm@gmail.com, vpatki@wayfair.com, williambbarnhart@gmail.com
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/faust-streaming/faust/issues
 Project-URL: Source, https://github.com/faust-streaming/faust
```

### Comparing `faust-streaming-0.9.4rc1/README.md` & `faust-streaming-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/TODO.rst` & `faust-streaming-0.9.5/TODO.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/artwork/banner-alt1.png` & `faust-streaming-0.9.5/artwork/banner-alt1.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/artwork/banner-alt2.png` & `faust-streaming-0.9.5/artwork/banner-alt2.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/artwork/favicon.ico` & `faust-streaming-0.9.5/artwork/favicon.ico`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/artwork/logo.png` & `faust-streaming-0.9.5/artwork/logo.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/Makefile` & `faust-streaming-0.9.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/_ext/faustdocs.py` & `faust-streaming-0.9.5/docs/_ext/faustdocs.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/_ext/typehints.py` & `faust-streaming-0.9.5/docs/_ext/typehints.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/conf.py` & `faust-streaming-0.9.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/contributing.rst` & `faust-streaming-0.9.5/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/copyright.rst` & `faust-streaming-0.9.5/docs/copyright.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/developerguide/overview.rst` & `faust-streaming-0.9.5/docs/developerguide/overview.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/developerguide/partition_assignor.rst` & `faust-streaming-0.9.5/docs/developerguide/partition_assignor.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/glossary.rst` & `faust-streaming-0.9.5/docs/glossary.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-0.9.rst` & `faust-streaming-0.9.5/docs/history/changelog-0.9.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.0.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.0.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.1.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.1.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.10.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.10.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.2.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.2.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.3.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.3.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.4.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.4.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.5.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.5.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.6.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.6.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.7.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.7.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.8.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.8.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/history/changelog-1.9.rst` & `faust-streaming-0.9.5/docs/history/changelog-1.9.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/images/banner-alt1.png` & `faust-streaming-0.9.5/docs/images/banner-alt1.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/images/banner-alt2.png` & `faust-streaming-0.9.5/docs/images/banner-alt2.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/images/favicon.ico` & `faust-streaming-0.9.5/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/images/logo.png` & `faust-streaming-0.9.5/docs/images/logo.png`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/blurb.txt` & `faust-streaming-0.9.5/docs/includes/blurb.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/code-of-conduct.txt` & `faust-streaming-0.9.5/docs/includes/code-of-conduct.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/faq.txt` & `faust-streaming-0.9.5/docs/includes/faq.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/installation.txt` & `faust-streaming-0.9.5/docs/includes/installation.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/intro.txt` & `faust-streaming-0.9.5/docs/includes/intro.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/introduction.txt` & `faust-streaming-0.9.5/docs/includes/introduction.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/kafka.txt` & `faust-streaming-0.9.5/docs/includes/kafka.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/resources.txt` & `faust-streaming-0.9.5/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/includes/settingref.txt` & `faust-streaming-0.9.5/docs/includes/settingref.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/index.rst` & `faust-streaming-0.9.5/docs/index.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/introduction.rst` & `faust-streaming-0.9.5/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/keepachangelog/version.md` & `faust-streaming-0.9.5/docs/keepachangelog/version.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/make.bat` & `faust-streaming-0.9.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/cheatsheet.rst` & `faust-streaming-0.9.5/docs/playbooks/cheatsheet.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/leaderelection.rst` & `faust-streaming-0.9.5/docs/playbooks/leaderelection.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/pageviews.rst` & `faust-streaming-0.9.5/docs/playbooks/pageviews.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/quickstart.rst` & `faust-streaming-0.9.5/docs/playbooks/quickstart.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/vscelery.rst` & `faust-streaming-0.9.5/docs/playbooks/vscelery.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/playbooks/vskafka.rst` & `faust-streaming-0.9.5/docs/playbooks/vskafka.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/reference/index.rst` & `faust-streaming-0.9.5/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/spelling_wordlist.txt` & `faust-streaming-0.9.5/docs/spelling_wordlist.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/templates/readme.txt` & `faust-streaming-0.9.5/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/agents.rst` & `faust-streaming-0.9.5/docs/userguide/agents.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/application.rst` & `faust-streaming-0.9.5/docs/userguide/application.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/channels.rst` & `faust-streaming-0.9.5/docs/userguide/channels.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/cli.rst` & `faust-streaming-0.9.5/docs/userguide/cli.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/debugging.rst` & `faust-streaming-0.9.5/docs/userguide/debugging.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/livecheck.rst` & `faust-streaming-0.9.5/docs/userguide/livecheck.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/models.rst` & `faust-streaming-0.9.5/docs/userguide/models.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/sensors.rst` & `faust-streaming-0.9.5/docs/userguide/sensors.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/settings.rst` & `faust-streaming-0.9.5/docs/userguide/settings.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/streams.rst` & `faust-streaming-0.9.5/docs/userguide/streams.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/tables.rst` & `faust-streaming-0.9.5/docs/userguide/tables.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/tasks.rst` & `faust-streaming-0.9.5/docs/userguide/tasks.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/testing.rst` & `faust-streaming-0.9.5/docs/userguide/testing.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/docs/userguide/workers.rst` & `faust-streaming-0.9.5/docs/userguide/workers.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/advanced/isolated_partitions_crashing.py` & `faust-streaming-0.9.5/examples/advanced/isolated_partitions_crashing.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/advanced/rpc.py` & `faust-streaming-0.9.5/examples/advanced/rpc.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/advanced/service.py` & `faust-streaming-0.9.5/examples/advanced/service.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/bound_agent.py` & `faust-streaming-0.9.5/examples/bound_agent.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/concurrency.py` & `faust-streaming-0.9.5/examples/concurrency.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/crontab/tz_aware.py` & `faust-streaming-0.9.5/examples/crontab/tz_aware.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/crontab/tz_unaware.py` & `faust-streaming-0.9.5/examples/crontab/tz_unaware.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/README.rst` & `faust-streaming-0.9.5/examples/django/README.rst`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/accounts/agents.py` & `faust-streaming-0.9.5/examples/django/accounts/agents.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/accounts/migrations/0001_initial.py` & `faust-streaming-0.9.5/examples/django/accounts/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/faustapp/app.py` & `faust-streaming-0.9.5/examples/django/faustapp/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/manage.py` & `faust-streaming-0.9.5/examples/django/manage.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/proj/__init__.py` & `faust-streaming-0.9.5/examples/django/proj/__init__.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/proj/settings.py` & `faust-streaming-0.9.5/examples/django/proj/settings.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/proj/urls.py` & `faust-streaming-0.9.5/examples/django/proj/urls.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/django/setup.py` & `faust-streaming-0.9.5/examples/django/setup.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/kubernetes/README.md` & `faust-streaming-0.9.5/examples/kubernetes/README.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/kubernetes/consumer/README.md` & `faust-streaming-0.9.5/examples/kubernetes/consumer/README.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/kubernetes/consumer/consumer.py` & `faust-streaming-0.9.5/examples/kubernetes/consumer/consumer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/kubernetes/producer/README.md` & `faust-streaming-0.9.5/examples/kubernetes/producer/README.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/kubernetes/producer/producer.py` & `faust-streaming-0.9.5/examples/kubernetes/producer/producer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/livecheck.py` & `faust-streaming-0.9.5/examples/livecheck.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/tableofset.py` & `faust-streaming-0.9.5/examples/tableofset.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/tabletest.py` & `faust-streaming-0.9.5/examples/tabletest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/task_queue.py` & `faust-streaming-0.9.5/examples/task_queue.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/windowed_aggregation.py` & `faust-streaming-0.9.5/examples/windowed_aggregation.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/windowing/hopping.py` & `faust-streaming-0.9.5/examples/windowing/hopping.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/windowing/hopping_2.py` & `faust-streaming-0.9.5/examples/windowing/hopping_2.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/windowing/tumbling.py` & `faust-streaming-0.9.5/examples/windowing/tumbling.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/withdrawals.py` & `faust-streaming-0.9.5/examples/withdrawals.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/examples/word_count.py` & `faust-streaming-0.9.5/examples/word_count.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/bandit/baseline.json` & `faust-streaming-0.9.5/extra/bandit/baseline.json`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/bandit/config.yaml` & `faust-streaming-0.9.5/extra/bandit/config.yaml`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/macOS/com.fauststream.worker.plist` & `faust-streaming-0.9.5/extra/macOS/com.fauststream.worker.plist`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/supervisord/faust.conf` & `faust-streaming-0.9.5/extra/supervisord/faust.conf`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/supervisord/supervisord.conf` & `faust-streaming-0.9.5/extra/supervisord/supervisord.conf`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/benchmark.py` & `faust-streaming-0.9.5/extra/tools/benchmark.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/render_configuration_reference.py` & `faust-streaming-0.9.5/extra/tools/render_configuration_reference.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/verify_ascending.py` & `faust-streaming-0.9.5/extra/tools/verify_ascending.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/verify_doc_defaults.py` & `faust-streaming-0.9.5/extra/tools/verify_doc_defaults.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/verify_tabletest.sh` & `faust-streaming-0.9.5/extra/tools/verify_tabletest.sh`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/extra/tools/verify_tabletest_changelog.py` & `faust-streaming-0.9.5/extra/tools/verify_tabletest_changelog.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/__init__.py` & `faust-streaming-0.9.5/faust/__init__.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/_cython/streams.pyx` & `faust-streaming-0.9.5/faust/_cython/streams.pyx`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/_cython/windows.pyx` & `faust-streaming-0.9.5/faust/_cython/windows.pyx`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/agents/actor.py` & `faust-streaming-0.9.5/faust/agents/actor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/agents/agent.py` & `faust-streaming-0.9.5/faust/agents/agent.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/agents/manager.py` & `faust-streaming-0.9.5/faust/agents/manager.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/agents/models.py` & `faust-streaming-0.9.5/faust/agents/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/agents/replies.py` & `faust-streaming-0.9.5/faust/agents/replies.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/app/_attached.py` & `faust-streaming-0.9.5/faust/app/_attached.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/app/base.py` & `faust-streaming-0.9.5/faust/app/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/app/router.py` & `faust-streaming-0.9.5/faust/app/router.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/assignor/client_assignment.py` & `faust-streaming-0.9.5/faust/assignor/client_assignment.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/assignor/cluster_assignment.py` & `faust-streaming-0.9.5/faust/assignor/cluster_assignment.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/assignor/copartitioned_assignor.py` & `faust-streaming-0.9.5/faust/assignor/copartitioned_assignor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/assignor/leader_assignor.py` & `faust-streaming-0.9.5/faust/assignor/leader_assignor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/assignor/partition_assignor.py` & `faust-streaming-0.9.5/faust/assignor/partition_assignor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/auth.py` & `faust-streaming-0.9.5/faust/auth.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/channels.py` & `faust-streaming-0.9.5/faust/channels.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/agents.py` & `faust-streaming-0.9.5/faust/cli/agents.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/base.py` & `faust-streaming-0.9.5/faust/cli/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/clean_versions.py` & `faust-streaming-0.9.5/faust/cli/clean_versions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/completion.py` & `faust-streaming-0.9.5/faust/cli/completion.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/faust.py` & `faust-streaming-0.9.5/faust/cli/faust.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/livecheck.py` & `faust-streaming-0.9.5/faust/cli/livecheck.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/model.py` & `faust-streaming-0.9.5/faust/cli/model.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/models.py` & `faust-streaming-0.9.5/faust/cli/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/params.py` & `faust-streaming-0.9.5/faust/cli/params.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/reset.py` & `faust-streaming-0.9.5/faust/cli/reset.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/send.py` & `faust-streaming-0.9.5/faust/cli/send.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/tables.py` & `faust-streaming-0.9.5/faust/cli/tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/cli/worker.py` & `faust-streaming-0.9.5/faust/cli/worker.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/contrib/sentry.py` & `faust-streaming-0.9.5/faust/contrib/sentry.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/events.py` & `faust-streaming-0.9.5/faust/events.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/exceptions.py` & `faust-streaming-0.9.5/faust/exceptions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/fixups/__init__.py` & `faust-streaming-0.9.5/faust/fixups/__init__.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/fixups/base.py` & `faust-streaming-0.9.5/faust/fixups/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/fixups/django.py` & `faust-streaming-0.9.5/faust/fixups/django.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/joins.py` & `faust-streaming-0.9.5/faust/joins.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/app.py` & `faust-streaming-0.9.5/faust/livecheck/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/case.py` & `faust-streaming-0.9.5/faust/livecheck/case.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/exceptions.py` & `faust-streaming-0.9.5/faust/livecheck/exceptions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/locals.py` & `faust-streaming-0.9.5/faust/livecheck/locals.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/models.py` & `faust-streaming-0.9.5/faust/livecheck/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/patches/aiohttp.py` & `faust-streaming-0.9.5/faust/livecheck/patches/aiohttp.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/runners.py` & `faust-streaming-0.9.5/faust/livecheck/runners.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/livecheck/signals.py` & `faust-streaming-0.9.5/faust/livecheck/signals.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/models/base.py` & `faust-streaming-0.9.5/faust/models/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/models/fields.py` & `faust-streaming-0.9.5/faust/models/fields.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/models/record.py` & `faust-streaming-0.9.5/faust/models/record.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/models/tags.py` & `faust-streaming-0.9.5/faust/models/tags.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/models/typing.py` & `faust-streaming-0.9.5/faust/models/typing.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/base.py` & `faust-streaming-0.9.5/faust/sensors/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/datadog.py` & `faust-streaming-0.9.5/faust/sensors/datadog.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/distributed_tracing.py` & `faust-streaming-0.9.5/faust/sensors/distributed_tracing.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/monitor.py` & `faust-streaming-0.9.5/faust/sensors/monitor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/prometheus.py` & `faust-streaming-0.9.5/faust/sensors/prometheus.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/sensors/statsd.py` & `faust-streaming-0.9.5/faust/sensors/statsd.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/serializers/codecs.py` & `faust-streaming-0.9.5/faust/serializers/codecs.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/serializers/registry.py` & `faust-streaming-0.9.5/faust/serializers/registry.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/serializers/schemas.py` & `faust-streaming-0.9.5/faust/serializers/schemas.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/stores/aerospike.py` & `faust-streaming-0.9.5/faust/stores/aerospike.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/stores/base.py` & `faust-streaming-0.9.5/faust/stores/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/stores/memory.py` & `faust-streaming-0.9.5/faust/stores/memory.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/stores/rocksdb.py` & `faust-streaming-0.9.5/faust/stores/rocksdb.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/streams.py` & `faust-streaming-0.9.5/faust/streams.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/base.py` & `faust-streaming-0.9.5/faust/tables/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/manager.py` & `faust-streaming-0.9.5/faust/tables/manager.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/objects.py` & `faust-streaming-0.9.5/faust/tables/objects.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/recovery.py` & `faust-streaming-0.9.5/faust/tables/recovery.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/sets.py` & `faust-streaming-0.9.5/faust/tables/sets.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/table.py` & `faust-streaming-0.9.5/faust/tables/table.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/tables/wrappers.py` & `faust-streaming-0.9.5/faust/tables/wrappers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/topics.py` & `faust-streaming-0.9.5/faust/topics.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/_cython/conductor.pyx` & `faust-streaming-0.9.5/faust/transport/_cython/conductor.pyx`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/base.py` & `faust-streaming-0.9.5/faust/transport/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/conductor.py` & `faust-streaming-0.9.5/faust/transport/conductor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/consumer.py` & `faust-streaming-0.9.5/faust/transport/consumer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/drivers/aiokafka.py` & `faust-streaming-0.9.5/faust/transport/drivers/aiokafka.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/producer.py` & `faust-streaming-0.9.5/faust/transport/producer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/transport/utils.py` & `faust-streaming-0.9.5/faust/transport/utils.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/__init__.py` & `faust-streaming-0.9.5/faust/types/__init__.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/_env.py` & `faust-streaming-0.9.5/faust/types/_env.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/agents.py` & `faust-streaming-0.9.5/faust/types/agents.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/app.py` & `faust-streaming-0.9.5/faust/types/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/assignor.py` & `faust-streaming-0.9.5/faust/types/assignor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/auth.py` & `faust-streaming-0.9.5/faust/types/auth.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/channels.py` & `faust-streaming-0.9.5/faust/types/channels.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/codecs.py` & `faust-streaming-0.9.5/faust/types/codecs.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/core.py` & `faust-streaming-0.9.5/faust/types/core.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/events.py` & `faust-streaming-0.9.5/faust/types/events.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/fixups.py` & `faust-streaming-0.9.5/faust/types/fixups.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/joins.py` & `faust-streaming-0.9.5/faust/types/joins.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/models.py` & `faust-streaming-0.9.5/faust/types/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/router.py` & `faust-streaming-0.9.5/faust/types/router.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/sensors.py` & `faust-streaming-0.9.5/faust/types/sensors.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/serializers.py` & `faust-streaming-0.9.5/faust/types/serializers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/settings/base.py` & `faust-streaming-0.9.5/faust/types/settings/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/settings/params.py` & `faust-streaming-0.9.5/faust/types/settings/params.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/settings/sections.py` & `faust-streaming-0.9.5/faust/types/settings/sections.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/settings/settings.py` & `faust-streaming-0.9.5/faust/types/settings/settings.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/stores.py` & `faust-streaming-0.9.5/faust/types/stores.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/streams.py` & `faust-streaming-0.9.5/faust/types/streams.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/tables.py` & `faust-streaming-0.9.5/faust/types/tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/topics.py` & `faust-streaming-0.9.5/faust/types/topics.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/transports.py` & `faust-streaming-0.9.5/faust/types/transports.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/tuples.py` & `faust-streaming-0.9.5/faust/types/tuples.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/web.py` & `faust-streaming-0.9.5/faust/types/web.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/types/windows.py` & `faust-streaming-0.9.5/faust/types/windows.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/_iso8601_python.py` & `faust-streaming-0.9.5/faust/utils/_iso8601_python.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/codegen.py` & `faust-streaming-0.9.5/faust/utils/codegen.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/cron.py` & `faust-streaming-0.9.5/faust/utils/cron.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/functional.py` & `faust-streaming-0.9.5/faust/utils/functional.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/json.py` & `faust-streaming-0.9.5/faust/utils/json.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/admin.py` & `faust-streaming-0.9.5/faust/utils/kafka/protocol/admin.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/kafka/protocol/api.py` & `faust-streaming-0.9.5/faust/utils/kafka/protocol/api.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/platforms.py` & `faust-streaming-0.9.5/faust/utils/platforms.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/terminal/spinners.py` & `faust-streaming-0.9.5/faust/utils/terminal/spinners.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/terminal/tables.py` & `faust-streaming-0.9.5/faust/utils/terminal/tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/tracing.py` & `faust-streaming-0.9.5/faust/utils/tracing.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/urls.py` & `faust-streaming-0.9.5/faust/utils/urls.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/utils/venusian.py` & `faust-streaming-0.9.5/faust/utils/venusian.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/apps/graph.py` & `faust-streaming-0.9.5/faust/web/apps/graph.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/apps/router.py` & `faust-streaming-0.9.5/faust/web/apps/router.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/apps/stats.py` & `faust-streaming-0.9.5/faust/web/apps/stats.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/apps/tables.py` & `faust-streaming-0.9.5/faust/web/apps/tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/base.py` & `faust-streaming-0.9.5/faust/web/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/blueprints.py` & `faust-streaming-0.9.5/faust/web/blueprints.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/cache/backends/__init__.py` & `faust-streaming-0.9.5/faust/web/cache/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/cache/backends/base.py` & `faust-streaming-0.9.5/faust/web/cache/backends/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/cache/backends/memory.py` & `faust-streaming-0.9.5/faust/web/cache/backends/memory.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/cache/backends/redis.py` & `faust-streaming-0.9.5/faust/web/cache/backends/redis.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/cache/cache.py` & `faust-streaming-0.9.5/faust/web/cache/cache.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/drivers/aiohttp.py` & `faust-streaming-0.9.5/faust/web/drivers/aiohttp.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/exceptions.py` & `faust-streaming-0.9.5/faust/web/exceptions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/web/views.py` & `faust-streaming-0.9.5/faust/web/views.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/windows.py` & `faust-streaming-0.9.5/faust/windows.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust/worker.py` & `faust-streaming-0.9.5/faust/worker.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust_streaming.egg-info/PKG-INFO` & `faust-streaming-0.9.5/faust_streaming.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faust-streaming
-Version: 0.9.4rc1
+Version: 0.9.5
 Summary: Python Stream processing.
 Home-page: https://github.com/faust-streaming/faust
 Author: Robinhood Markets, Inc.
 Author-email: schrohm@gmail.com, vpatki@wayfair.com, williambbarnhart@gmail.com
 License: BSD 3-Clause
 Project-URL: Bug Reports, https://github.com/faust-streaming/faust/issues
 Project-URL: Source, https://github.com/faust-streaming/faust
```

### Comparing `faust-streaming-0.9.4rc1/faust_streaming.egg-info/SOURCES.txt` & `faust-streaming-0.9.5/faust_streaming.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/faust_streaming.egg-info/requires.txt` & `faust-streaming-0.9.5/faust_streaming.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 aiohttp<4.0,>=3.5.2
 aiohttp_cors<2.0,>=0.7
-aiokafka<0.8.0,>=0.7.1
+aiokafka<0.9.0,>=0.7.1
 click<8.2,>=6.7
 croniter>=0.3.16
 intervaltree
-mode-streaming>=0.2.0
+mode-streaming<0.3.0,>=0.2.0
 mypy_extensions
 opentracing<=2.4.0,>=1.3.0
 six
 terminaltables<4.0,>=3.1
 venusian==3.0.0
 yarl<2.0,>=1.0
```

### Comparing `faust-streaming-0.9.4rc1/scripts/README.md` & `faust-streaming-0.9.5/scripts/README.md`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/setup.py` & `faust-streaming-0.9.5/setup.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/bench/base.py` & `faust-streaming-0.9.5/tests/bench/base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/bench/forward.py` & `faust-streaming-0.9.5/tests/bench/forward.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/conftest.py` & `faust-streaming-0.9.5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/consistency/consistency_checker.py` & `faust-streaming-0.9.5/tests/consistency/consistency_checker.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/consistency/test_consistency.py` & `faust-streaming-0.9.5/tests/consistency/test_consistency.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/agents/helpers.py` & `faust-streaming-0.9.5/tests/functional/agents/helpers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/agents/test_concurrency.py` & `faust-streaming-0.9.5/tests/functional/agents/test_concurrency.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/agents/test_isolated_partitions.py` & `faust-streaming-0.9.5/tests/functional/agents/test_isolated_partitions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/conftest.py` & `faust-streaming-0.9.5/tests/functional/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/helpers.py` & `faust-streaming-0.9.5/tests/functional/helpers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/models/test_typing.py` & `faust-streaming-0.9.5/tests/functional/models/test_typing.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/sensors/test_statsd.py` & `faust-streaming-0.9.5/tests/functional/sensors/test_statsd.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/serializers/test_registry.py` & `faust-streaming-0.9.5/tests/functional/serializers/test_registry.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/test_app.py` & `faust-streaming-0.9.5/tests/functional/test_app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/test_channels.py` & `faust-streaming-0.9.5/tests/functional/test_channels.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/test_models.py` & `faust-streaming-0.9.5/tests/functional/test_models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/test_streams.py` & `faust-streaming-0.9.5/tests/functional/test_streams.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/web/conftest.py` & `faust-streaming-0.9.5/tests/functional/web/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/web/test_cache.py` & `faust-streaming-0.9.5/tests/functional/web/test_cache.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/web/test_tables.py` & `faust-streaming-0.9.5/tests/functional/web/test_tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/functional/web/test_views.py` & `faust-streaming-0.9.5/tests/functional/web/test_views.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/helpers.py` & `faust-streaming-0.9.5/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/integration/app.py` & `faust-streaming-0.9.5/tests/integration/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/integration/cli/test_agents.py` & `faust-streaming-0.9.5/tests/integration/cli/test_agents.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/integration/cli/test_model.py` & `faust-streaming-0.9.5/tests/integration/cli/test_model.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/integration/cli/test_models.py` & `faust-streaming-0.9.5/tests/integration/cli/test_models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/integration/conftest.py` & `faust-streaming-0.9.5/tests/integration/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/meticulous/assignor/test_copartitioned_assignor.py` & `faust-streaming-0.9.5/tests/meticulous/assignor/test_copartitioned_assignor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/old/test_simple.py` & `faust-streaming-0.9.5/tests/old/test_simple.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/regression/i323/test_autodiscover.py` & `faust-streaming-0.9.5/tests/regression/i323/test_autodiscover.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/regression/i324/test_autodiscover.py` & `faust-streaming-0.9.5/tests/regression/i324/test_autodiscover.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/app.py` & `faust-streaming-0.9.5/tests/stress/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/config.py` & `faust-streaming-0.9.5/tests/stress/config.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/killer.py` & `faust-streaming-0.9.5/tests/stress/killer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/models.py` & `faust-streaming-0.9.5/tests/stress/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/producer.py` & `faust-streaming-0.9.5/tests/stress/producer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/app.py` & `faust-streaming-0.9.5/tests/stress/reports/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/checks.py` & `faust-streaming-0.9.5/tests/stress/reports/checks.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/collector.py` & `faust-streaming-0.9.5/tests/stress/reports/collector.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/logging.py` & `faust-streaming-0.9.5/tests/stress/reports/logging.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/models.py` & `faust-streaming-0.9.5/tests/stress/reports/models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/reports/templates/dashboard.html` & `faust-streaming-0.9.5/tests/stress/reports/templates/dashboard.html`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/tests/forwarder/app.py` & `faust-streaming-0.9.5/tests/stress/tests/forwarder/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/tests/simple/app.py` & `faust-streaming-0.9.5/tests/stress/tests/simple/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/stress/tests/tables/app.py` & `faust-streaming-0.9.5/tests/stress/tests/tables/app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/agents/test_actor.py` & `faust-streaming-0.9.5/tests/unit/agents/test_actor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/agents/test_agent.py` & `faust-streaming-0.9.5/tests/unit/agents/test_agent.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/agents/test_manager.py` & `faust-streaming-0.9.5/tests/unit/agents/test_manager.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/agents/test_replies.py` & `faust-streaming-0.9.5/tests/unit/agents/test_replies.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/app/test_base.py` & `faust-streaming-0.9.5/tests/unit/app/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/app/test_router.py` & `faust-streaming-0.9.5/tests/unit/app/test_router.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/app/test_service.py` & `faust-streaming-0.9.5/tests/unit/app/test_service.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/cli/test_base.py` & `faust-streaming-0.9.5/tests/unit/cli/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/cli/test_clean_versions.py` & `faust-streaming-0.9.5/tests/unit/cli/test_clean_versions.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/cli/test_completion.py` & `faust-streaming-0.9.5/tests/unit/cli/test_completion.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/cli/test_params.py` & `faust-streaming-0.9.5/tests/unit/cli/test_params.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/conftest.py` & `faust-streaming-0.9.5/tests/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/fixups/test_django.py` & `faust-streaming-0.9.5/tests/unit/fixups/test_django.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/conftest.py` & `faust-streaming-0.9.5/tests/unit/livecheck/conftest.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/patches/test_aiohttp.py` & `faust-streaming-0.9.5/tests/unit/livecheck/patches/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_app.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_app.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_case.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_case.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_locals.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_locals.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_models.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_models.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_runners.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_runners.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/livecheck/test_signals.py` & `faust-streaming-0.9.5/tests/unit/livecheck/test_signals.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/models/test_fields.py` & `faust-streaming-0.9.5/tests/unit/models/test_fields.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/models/test_tags.py` & `faust-streaming-0.9.5/tests/unit/models/test_tags.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/sensors/test_base.py` & `faust-streaming-0.9.5/tests/unit/sensors/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/sensors/test_datadog.py` & `faust-streaming-0.9.5/tests/unit/sensors/test_datadog.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/sensors/test_monitor.py` & `faust-streaming-0.9.5/tests/unit/sensors/test_monitor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/sensors/test_prometheus.py` & `faust-streaming-0.9.5/tests/unit/sensors/test_prometheus.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/sensors/test_statsd.py` & `faust-streaming-0.9.5/tests/unit/sensors/test_statsd.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/serializers/test_codecs.py` & `faust-streaming-0.9.5/tests/unit/serializers/test_codecs.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/stores/test_aerospike.py` & `faust-streaming-0.9.5/tests/unit/stores/test_aerospike.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/stores/test_base.py` & `faust-streaming-0.9.5/tests/unit/stores/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/stores/test_memory.py` & `faust-streaming-0.9.5/tests/unit/stores/test_memory.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/stores/test_rocksdb.py` & `faust-streaming-0.9.5/tests/unit/stores/test_rocksdb.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_base.py` & `faust-streaming-0.9.5/tests/unit/tables/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_manager.py` & `faust-streaming-0.9.5/tests/unit/tables/test_manager.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_objects.py` & `faust-streaming-0.9.5/tests/unit/tables/test_objects.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_recovery.py` & `faust-streaming-0.9.5/tests/unit/tables/test_recovery.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_sets.py` & `faust-streaming-0.9.5/tests/unit/tables/test_sets.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_table.py` & `faust-streaming-0.9.5/tests/unit/tables/test_table.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/tables/test_wrappers.py` & `faust-streaming-0.9.5/tests/unit/tables/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_auth.py` & `faust-streaming-0.9.5/tests/unit/test_auth.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_events.py` & `faust-streaming-0.9.5/tests/unit/test_events.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_joins.py` & `faust-streaming-0.9.5/tests/unit/test_joins.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_streams.py` & `faust-streaming-0.9.5/tests/unit/test_streams.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_topics.py` & `faust-streaming-0.9.5/tests/unit/test_topics.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/test_worker.py` & `faust-streaming-0.9.5/tests/unit/test_worker.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/transport/drivers/test_aiokafka.py` & `faust-streaming-0.9.5/tests/unit/transport/drivers/test_aiokafka.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/transport/test_conductor.py` & `faust-streaming-0.9.5/tests/unit/transport/test_conductor.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/transport/test_consumer.py` & `faust-streaming-0.9.5/tests/unit/transport/test_consumer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/transport/test_producer.py` & `faust-streaming-0.9.5/tests/unit/transport/test_producer.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/transport/test_utils.py` & `faust-streaming-0.9.5/tests/unit/transport/test_utils.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/terminal/test_spinners.py` & `faust-streaming-0.9.5/tests/unit/utils/terminal/test_spinners.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/terminal/test_tables.py` & `faust-streaming-0.9.5/tests/unit/utils/terminal/test_tables.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/test_codegen.py` & `faust-streaming-0.9.5/tests/unit/utils/test_codegen.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/test_cron.py` & `faust-streaming-0.9.5/tests/unit/utils/test_cron.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/test_iso8601.py` & `faust-streaming-0.9.5/tests/unit/utils/test_iso8601.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/test_json.py` & `faust-streaming-0.9.5/tests/unit/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/utils/test_urls.py` & `faust-streaming-0.9.5/tests/unit/utils/test_urls.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/web/drivers/test_aiohttp.py` & `faust-streaming-0.9.5/tests/unit/web/drivers/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/web/test_base.py` & `faust-streaming-0.9.5/tests/unit/web/test_base.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/web/test_blueprints.py` & `faust-streaming-0.9.5/tests/unit/web/test_blueprints.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/web/test_views.py` & `faust-streaming-0.9.5/tests/unit/web/test_views.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/windows/test_hopping_window.py` & `faust-streaming-0.9.5/tests/unit/windows/test_hopping_window.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/windows/test_sliding_window.py` & `faust-streaming-0.9.5/tests/unit/windows/test_sliding_window.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tests/unit/windows/test_tumbling_window.py` & `faust-streaming-0.9.5/tests/unit/windows/test_tumbling_window.py`

 * *Files identical despite different names*

### Comparing `faust-streaming-0.9.4rc1/tox.ini` & `faust-streaming-0.9.5/tox.ini`

 * *Files identical despite different names*

