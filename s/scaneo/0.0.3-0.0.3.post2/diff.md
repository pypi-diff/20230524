# Comparing `tmp/scaneo-0.0.3.tar.gz` & `tmp/scaneo-0.0.3.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scaneo-0.0.3.tar", max compression
+gzip compressed data, was "scaneo-0.0.3.post2.tar", max compression
```

## Comparing `scaneo-0.0.3.tar` & `scaneo-0.0.3.post2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     6199 2023-05-24 09:26:01.616553 scaneo-0.0.3/README.md
--rw-r--r--   0        0        0      344 2023-05-24 10:39:54.251378 scaneo-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-24 09:29:06.132298 scaneo-0.0.3/scaneo/__init__.py
--rw-r--r--   0        0        0      437 2023-05-24 10:35:00.270028 scaneo-0.0.3/scaneo/api.py
--rw-r--r--   0        0        0      232 2023-05-24 09:59:09.946610 scaneo-0.0.3/scaneo/main.py
--rw-r--r--   0        0        0     7056 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/chunks/index.6dba6488.js
--rw-r--r--   0        0        0     2836 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/chunks/singletons.1df1af67.js
--rw-r--r--   0        0        0      238 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/chunks/stores.a2dd7dd6.js
--rw-r--r--   0        0        0     5722 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/entry/app.77ddf75f.js
--rw-r--r--   0        0        0    23876 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/entry/start.8814d3e0.js
--rw-r--r--   0        0        0      719 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/nodes/0.663a3db5.js
--rw-r--r--   0        0        0      800 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/nodes/1.86013cb7.js
--rw-r--r--   0        0        0     1328 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/nodes/2.35154476.js
--rw-r--r--   0        0        0      372 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/immutable/nodes/3.cb33ee2b.js
--rw-r--r--   0        0        0       27 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/_app/version.json
--rw-r--r--   0        0        0     1571 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/favicon.png
--rw-r--r--   0        0        0     1574 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/index.html
--rw-r--r--   0        0        0     1363 2023-05-24 10:34:07.157773 scaneo-0.0.3/ui/build/kk.html
--rw-r--r--   0        0        0     6884 1970-01-01 00:00:00.000000 scaneo-0.0.3/setup.py
--rw-r--r--   0        0        0     6579 1970-01-01 00:00:00.000000 scaneo-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     6199 2023-05-24 09:26:01.616553 scaneo-0.0.3.post2/README.md
+-rw-r--r--   0        0        0      346 2023-05-24 10:42:16.364002 scaneo-0.0.3.post2/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-24 09:29:06.132298 scaneo-0.0.3.post2/scaneo/__init__.py
+-rw-r--r--   0        0        0      530 2023-05-24 10:42:10.143975 scaneo-0.0.3.post2/scaneo/api.py
+-rw-r--r--   0        0        0      232 2023-05-24 09:59:09.946610 scaneo-0.0.3.post2/scaneo/main.py
+-rw-r--r--   0        0        0     7056 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/chunks/index.6dba6488.js
+-rw-r--r--   0        0        0     2836 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/chunks/singletons.1df1af67.js
+-rw-r--r--   0        0        0      238 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/chunks/stores.a2dd7dd6.js
+-rw-r--r--   0        0        0     5722 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/entry/app.77ddf75f.js
+-rw-r--r--   0        0        0    23876 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/entry/start.8814d3e0.js
+-rw-r--r--   0        0        0      719 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/0.663a3db5.js
+-rw-r--r--   0        0        0      800 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/1.86013cb7.js
+-rw-r--r--   0        0        0     1328 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/2.35154476.js
+-rw-r--r--   0        0        0      372 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/3.cb33ee2b.js
+-rw-r--r--   0        0        0       27 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/_app/version.json
+-rw-r--r--   0        0        0     1571 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/favicon.png
+-rw-r--r--   0        0        0     1574 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/index.html
+-rw-r--r--   0        0        0     1363 2023-05-24 10:34:07.157773 scaneo-0.0.3.post2/ui/build/kk.html
+-rw-r--r--   0        0        0     6890 1970-01-01 00:00:00.000000 scaneo-0.0.3.post2/setup.py
+-rw-r--r--   0        0        0     6585 1970-01-01 00:00:00.000000 scaneo-0.0.3.post2/PKG-INFO
```

### Comparing `scaneo-0.0.3/README.md` & `scaneo-0.0.3.post2/README.md`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/chunks/index.6dba6488.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/chunks/index.6dba6488.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/chunks/singletons.1df1af67.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/chunks/singletons.1df1af67.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/entry/app.77ddf75f.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/entry/app.77ddf75f.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/entry/start.8814d3e0.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/entry/start.8814d3e0.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/nodes/0.663a3db5.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/0.663a3db5.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/nodes/1.86013cb7.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/1.86013cb7.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/_app/immutable/nodes/2.35154476.js` & `scaneo-0.0.3.post2/ui/build/_app/immutable/nodes/2.35154476.js`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/favicon.png` & `scaneo-0.0.3.post2/ui/build/favicon.png`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/index.html` & `scaneo-0.0.3.post2/ui/build/index.html`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/ui/build/kk.html` & `scaneo-0.0.3.post2/ui/build/kk.html`

 * *Files identical despite different names*

### Comparing `scaneo-0.0.3/setup.py` & `scaneo-0.0.3.post2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 {'': ['*']}
 
 entry_points = \
 {'console_scripts': ['scaneo = scaneo.api:app']}
 
 setup_kwargs = {
     'name': 'scaneo',
-    'version': '0.0.3',
+    'version': '0.0.3.post2',
     'description': '',
     'long_description': "# scan-new\n\n\n\n## Getting started\n\nTo make it easy for you to get started with GitLab, here's a list of recommended next steps.\n\nAlready a pro? Just edit this README.md and make it your own. Want to make it easy? [Use the template at the bottom](#editing-this-readme)!\n\n## Add your files\n\n- [ ] [Create](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#create-a-file) or [upload](https://docs.gitlab.com/ee/user/project/repository/web_editor.html#upload-a-file) files\n- [ ] [Add files using the command line](https://docs.gitlab.com/ee/gitlab-basics/add-file.html#add-a-file-using-the-command-line) or push an existing Git repository with the following command:\n\n```\ncd existing_repo\ngit remote add origin https://gitlab.com/earthpulse/scan-new.git\ngit branch -M main\ngit push -uf origin main\n```\n\n## Integrate with your tools\n\n- [ ] [Set up project integrations](https://gitlab.com/earthpulse/scan-new/-/settings/integrations)\n\n## Collaborate with your team\n\n- [ ] [Invite team members and collaborators](https://docs.gitlab.com/ee/user/project/members/)\n- [ ] [Create a new merge request](https://docs.gitlab.com/ee/user/project/merge_requests/creating_merge_requests.html)\n- [ ] [Automatically close issues from merge requests](https://docs.gitlab.com/ee/user/project/issues/managing_issues.html#closing-issues-automatically)\n- [ ] [Enable merge request approvals](https://docs.gitlab.com/ee/user/project/merge_requests/approvals/)\n- [ ] [Automatically merge when pipeline succeeds](https://docs.gitlab.com/ee/user/project/merge_requests/merge_when_pipeline_succeeds.html)\n\n## Test and Deploy\n\nUse the built-in continuous integration in GitLab.\n\n- [ ] [Get started with GitLab CI/CD](https://docs.gitlab.com/ee/ci/quick_start/index.html)\n- [ ] [Analyze your code for known vulnerabilities with Static Application Security Testing(SAST)](https://docs.gitlab.com/ee/user/application_security/sast/)\n- [ ] [Deploy to Kubernetes, Amazon EC2, or Amazon ECS using Auto Deploy](https://docs.gitlab.com/ee/topics/autodevops/requirements.html)\n- [ ] [Use pull-based deployments for improved Kubernetes management](https://docs.gitlab.com/ee/user/clusters/agent/)\n- [ ] [Set up protected environments](https://docs.gitlab.com/ee/ci/environments/protected_environments.html)\n\n***\n\n# Editing this README\n\nWhen you're ready to make this README your own, just edit this file and use the handy template below (or feel free to structure it however you want - this is just a starting point!). Thank you to [makeareadme.com](https://www.makeareadme.com/) for this template.\n\n## Suggestions for a good README\nEvery project is different, so consider which of these sections apply to yours. The sections used in the template are suggestions for most open source projects. Also keep in mind that while a README can be too long and detailed, too long is better than too short. If you think your README is too long, consider utilizing another form of documentation rather than cutting out information.\n\n## Name\nChoose a self-explaining name for your project.\n\n## Description\nLet people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.\n\n## Badges\nOn some READMEs, you may see small images that convey metadata, such as whether or not all the tests are passing for the project. You can use Shields to add some to your README. Many services also have instructions for adding a badge.\n\n## Visuals\nDepending on what you are making, it can be a good idea to include screenshots or even a video (you'll frequently see GIFs rather than actual videos). Tools like ttygif can help, but check out Asciinema for a more sophisticated method.\n\n## Installation\nWithin a particular ecosystem, there may be a common way of installing things, such as using Yarn, NuGet, or Homebrew. However, consider the possibility that whoever is reading your README is a novice and would like more guidance. Listing specific steps helps remove ambiguity and gets people to using your project as quickly as possible. If it only runs in a specific context like a particular programming language version or operating system or has dependencies that have to be installed manually, also add a Requirements subsection.\n\n## Usage\nUse examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.\n\n## Support\nTell people where they can go to for help. It can be any combination of an issue tracker, a chat room, an email address, etc.\n\n## Roadmap\nIf you have ideas for releases in the future, it is a good idea to list them in the README.\n\n## Contributing\nState if you are open to contributions and what your requirements are for accepting them.\n\nFor people who want to make changes to your project, it's helpful to have some documentation on how to get started. Perhaps there is a script that they should run or some environment variables that they need to set. Make these steps explicit. These instructions could also be useful to your future self.\n\nYou can also document commands to lint the code or run tests. These steps help to ensure high code quality and reduce the likelihood that the changes inadvertently break something. Having instructions for running tests is especially helpful if it requires external setup, such as starting a Selenium server for testing in a browser.\n\n## Authors and acknowledgment\nShow your appreciation to those who have contributed to the project.\n\n## License\nFor open source projects, say how it is licensed.\n\n## Project status\nIf you have run out of energy or time for your project, put a note at the top of the README saying that development has slowed down or stopped completely. Someone may choose to fork your project or volunteer to step in as a maintainer or owner, allowing your project to keep going. You can also make an explicit request for maintainers.\n",
     'author': 'Juan Sensio',
     'author_email': 'it@earthpulse.es',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `scaneo-0.0.3/PKG-INFO` & `scaneo-0.0.3.post2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scaneo
-Version: 0.0.3
+Version: 0.0.3.post2
 Summary: 
 Author: Juan Sensio
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

