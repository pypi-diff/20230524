# Comparing `tmp/molecule_multipass-0.4.9.tar.gz` & `tmp/molecule_multipass-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "molecule_multipass-0.4.9.tar", last modified: Sat May 20 20:03:39 2023, max compression
+gzip compressed data, was "molecule_multipass-0.5.0.tar", last modified: Wed May 24 12:50:55 2023, max compression
```

## Comparing `molecule_multipass-0.4.9.tar` & `molecule_multipass-0.5.0.tar`

### file list

```diff
@@ -1,32 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.452741 molecule_multipass-0.4.9/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.452741 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
--rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/driver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass/playbooks/
--rw-r--r--   0 runner    (1001) docker     (123)     3235 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/playbooks/create.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1586 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/playbooks/destroy.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass/playbooks/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/molecule_multipass/playbooks/templates/cloud-init.yml.j2
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/molecule_multipass.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      297 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-20 20:03:39.000000 molecule_multipass-0.4.9/molecule_multipass.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-20 20:03:30.000000 molecule_multipass-0.4.9/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 20:03:39.456741 molecule_multipass-0.4.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.605668 molecule_multipass-0.5.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.609668 molecule_multipass-0.5.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.github/workflows/ansible-lint.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.github/workflows/pycodestyle.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.609668 molecule_multipass-0.5.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.609668 molecule_multipass-0.5.0/molecule_multipass/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.609668 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/converge.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2036 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/driver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/molecule_multipass/playbooks/
+-rw-r--r--   0 runner    (1001) docker     (123)     4350 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/playbooks/create.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/playbooks/destroy.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/molecule_multipass/playbooks/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/molecule_multipass/playbooks/templates/cloud-init.yml.j2
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/molecule_multipass.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1458 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-24 12:50:55.000000 molecule_multipass-0.5.0/molecule_multipass.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-24 12:50:44.000000 molecule_multipass-0.5.0/requirements.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-24 12:50:55.613669 molecule_multipass-0.5.0/setup.cfg
```

### Comparing `molecule_multipass-0.4.9/.github/workflows/python-publish.yml` & `molecule_multipass-0.5.0/.github/workflows/python-publish.yml`

 * *Files 2% similar despite different names*

```diff
@@ -9,31 +9,35 @@
 
 jobs:
   deploy:
     runs-on: ubuntu-latest
 
     steps:
     - uses: actions/checkout@v3
+
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.x'
+
     - name: Install dependencies
       run: >-
         python -m
         pip install
         build
         --user
+
     - name: Build a binary wheel and a source tarball
       run: >-
         python -m
         build
         --sdist
         --wheel
         --outdir dist/
         .
+
     - name: Publish package
       if: startsWith(github.ref, 'refs/tags')
       uses: pypa/gh-action-pypi-publish@release/v1
       with:
         user: __token__
         password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `molecule_multipass-0.4.9/.gitignore` & `molecule_multipass-0.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.9/LICENSE` & `molecule_multipass-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.9/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml` & `molecule_multipass-0.5.0/molecule_multipass/cookiecutter/{{cookiecutter.molecule_directory}}/{{cookiecutter.scenario_name}}/prepare.yml`

 * *Files identical despite different names*

### Comparing `molecule_multipass-0.4.9/molecule_multipass/driver.py` & `molecule_multipass-0.5.0/molecule_multipass/driver.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,10 +66,9 @@
             return {}
         except IOError:
             return {}
 
     def _get_instance_config(self, instance_name):
         instance_config_dict = util.safe_load_file(self._config.driver.instance_config)
         return next(
-            item for item in instance_config_dict if item["instance"] == instance_name
+            item for item in instance_config_dict if item["name"] == instance_name
         )
-
```

### Comparing `molecule_multipass-0.4.9/molecule_multipass/playbooks/destroy.yml` & `molecule_multipass-0.5.0/molecule_multipass/playbooks/destroy.yml`

 * *Files 8% similar despite different names*

```diff
@@ -4,54 +4,56 @@
   gather_facts: false
   no_log: "{{ molecule_no_log }}"
 
   vars:
     multipass_executable: "multipass"
 
   tasks:
-    - name: Get multipass executable path
+    - name: Get multipass executable path  # noqa: command-instead-of-shell
       ansible.builtin.shell: "command -v {{ multipass_executable }}"
       register: multipass_path
       changed_when: false
 
     - name: Set multipass executable path
       ansible.builtin.set_fact:
         multipass_cmd: "{{ multipass_path.stdout }}"
 
-    - block:
+    - name: Prepare VMs config
+      block:
         - name: Prepare VMs config
-          set_fact:
+          ansible.builtin.set_fact:
             instance_conf: "{{ lookup('file', molecule_instance_config) | from_yaml }}"
       rescue:
         - name: Prepare VMs config when file missing
-          set_fact:
+          ansible.builtin.set_fact:
             instance_conf: {}
 
-    - name: Destroy VMs
+    - name: Destroy VMs  # noqa: no-changed-when
       ansible.builtin.command: >
         {{ multipass_cmd }} delete --purge {{ item.instance }}
       loop: "{{ instance_conf }}"
       loop_control:
-        label: "{{ item.instance }}"
+        label: "{{ item.name }}"
       async: 7200
       poll: 0
       register: multipass_destroy
 
     - name: Wait for VMs to be destroyed
       ansible.builtin.async_status:
         jid: "{{ item.ansible_job_id }}"
       loop: "{{ multipass_destroy.results }}"
       loop_control:
-        label: "{{ item.item.instance }}"
+        label: "{{ item.item.name }}"
       register: multipass_destroy_status
       until: multipass_destroy_status.finished
       retries: 30
       delay: 5
 
     - name: Prepare VMs config list
-      set_fact:
+      ansible.builtin.set_fact:
         instance_conf: {}
 
     - name: Dump VMs config
-      copy:
+      ansible.builtin.copy:
         content: "{{ instance_conf | to_json | from_json | to_yaml }}"
         dest: "{{ molecule_instance_config }}"
+        mode: "0644"
```

### Comparing `molecule_multipass-0.4.9/molecule_multipass.egg-info/SOURCES.txt` & `molecule_multipass-0.5.0/molecule_multipass.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 .gitignore
 LICENSE
+Makefile
 README.md
 pyproject.toml
+requirements.yml
+setup.cfg
+.github/workflows/ansible-lint.yml
+.github/workflows/pycodestyle.yml
 .github/workflows/python-publish.yml
 .github/workflows/release.yml
+.vscode/settings.json
 molecule_multipass/__init__.py
 molecule_multipass/driver.py
 molecule_multipass.egg-info/PKG-INFO
 molecule_multipass.egg-info/SOURCES.txt
 molecule_multipass.egg-info/dependency_links.txt
 molecule_multipass.egg-info/entry_points.txt
 molecule_multipass.egg-info/requires.txt
```

### Comparing `molecule_multipass-0.4.9/pyproject.toml` & `molecule_multipass-0.5.0/pyproject.toml`

 * *Files identical despite different names*

