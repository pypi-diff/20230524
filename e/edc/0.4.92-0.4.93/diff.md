# Comparing `tmp/edc-0.4.92.tar.gz` & `tmp/edc-0.4.93.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edc-0.4.92.tar", last modified: Fri May 12 17:56:07 2023, max compression
+gzip compressed data, was "edc-0.4.93.tar", last modified: Wed May 24 17:36:30 2023, max compression
```

## Comparing `edc-0.4.92.tar` & `edc-0.4.93.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.095125 edc-0.4.92/
--rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.92/.gitignore
--rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.92/.pre-commit-config.yaml
--rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.92/.yamllint
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.92/AUTHORS
--rw-r--r--   0 erikvw     (501) staff       (20)    39242 2023-05-12 17:55:59.000000 edc-0.4.92/CHANGES
--rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.92/LICENSE
--rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.92/MANIFEST.in
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 17:56:07.095229 edc-0.4.92/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.92/README.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.081873 edc-0.4.92/bin/
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.084725 edc-0.4.92/bin/nginx/
--rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc-sites.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc-uat.conf
--rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.92/bin/nginx/edc.conf
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.085376 edc-0.4.92/bin/scripts/
--rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.92/bin/scripts/dev_repos.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.92/bin/scripts/list_db_files.sh
--rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.92/bin/scripts/restore_db_file.sh
--rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.92/bin/scripts/update_edc.sh
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.086547 edc-0.4.92/bin/systemd/
--rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celery-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celery.service
--rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celerybeat-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/celerybeat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn-uat.service
--rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn-uat.socket
--rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn.service
--rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.92/bin/systemd/gunicorn.socket
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.090528 edc-0.4.92/docs/
--rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.92/docs/Makefile
--rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.92/docs/README.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.92/docs/backup.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.92/docs/celery.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.92/docs/conda.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.92/docs/conf.py
--rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.92/docs/configure_web_services.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.92/docs/deploy_new_droplet.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.92/docs/dump_users.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.92/docs/exporting_encrypted_data.rst
--rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.92/docs/forms_reference.md
--rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.92/docs/index.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.92/docs/landing_page.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.92/docs/make.bat
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.92/docs/multisite_deployment.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.92/docs/prepare_database.rst
--rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.92/docs/printing.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.92/docs/redis.rst
--rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.92/docs/update_deployment.rst
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.091517 edc-0.4.92/edc.egg-info/
--rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/PKG-INFO
--rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/SOURCES.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/dependency_links.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.92/edc.egg-info/not-zip-safe
--rw-r--r--   0 erikvw     (501) staff       (20)     1922 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/requires.txt
--rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-12 17:56:07.000000 edc-0.4.92/edc.egg-info/top_level.txt
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.091645 edc-0.4.92/image/
--rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.92/image/icon-pycharm.png
--rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.92/pyproject.toml
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.094533 edc-0.4.92/requirements.tests/
--rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.92/requirements.tests/coverage.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.92/requirements.tests/docs.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.92/requirements.tests/edc.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.92/requirements.tests/edc_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.92/requirements.tests/edc_offline.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.92/requirements.tests/lint.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.92/requirements.tests/mysql.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.92/requirements.tests/postgres.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.92/requirements.tests/test_utils.txt
--rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.92/requirements.tests/third_party_dev.txt
--rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.92/requirements.tests/tox.txt
--rw-r--r--   0 erikvw     (501) staff       (20)     2994 2023-05-12 17:56:07.095650 edc-0.4.92/setup.cfg
-drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-12 17:56:07.094892 edc-0.4.92/utils/
--rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.92/utils/__init__.py
--rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.92/utils/get_edc_requirements.py
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.651573 edc-0.4.93/
+-rw-r--r--   0 erikvw     (501) staff       (20)     1410 2022-05-03 03:22:05.000000 edc-0.4.93/.gitignore
+-rw-r--r--   0 erikvw     (501) staff       (20)     1076 2023-05-12 04:49:20.000000 edc-0.4.93/.pre-commit-config.yaml
+-rw-r--r--   0 erikvw     (501) staff       (20)      291 2022-08-08 18:50:02.000000 edc-0.4.93/.yamllint
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2022-05-03 03:22:05.000000 edc-0.4.93/AUTHORS
+-rw-r--r--   0 erikvw     (501) staff       (20)    39637 2023-05-24 17:36:22.000000 edc-0.4.93/CHANGES
+-rw-r--r--   0 erikvw     (501) staff       (20)    35147 2020-03-07 14:11:38.000000 edc-0.4.93/LICENSE
+-rw-r--r--   0 erikvw     (501) staff       (20)      151 2020-03-07 14:11:38.000000 edc-0.4.93/MANIFEST.in
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-24 17:36:30.651677 edc-0.4.93/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)    37432 2022-11-29 06:04:52.000000 edc-0.4.93/README.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.637368 edc-0.4.93/bin/
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.640439 edc-0.4.93/bin/nginx/
+-rw-r--r--   0 erikvw     (501) staff       (20)      350 2022-07-30 01:15:42.000000 edc-0.4.93/bin/nginx/edc-sites.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      706 2022-07-30 01:15:42.000000 edc-0.4.93/bin/nginx/edc-uat.conf
+-rw-r--r--   0 erikvw     (501) staff       (20)      656 2022-07-30 01:15:42.000000 edc-0.4.93/bin/nginx/edc.conf
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.641134 edc-0.4.93/bin/scripts/
+-rw-r--r--   0 erikvw     (501) staff       (20)     2753 2022-10-05 21:50:32.000000 edc-0.4.93/bin/scripts/dev_repos.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      276 2020-03-07 14:11:38.000000 edc-0.4.93/bin/scripts/list_db_files.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)      416 2020-03-07 14:11:38.000000 edc-0.4.93/bin/scripts/restore_db_file.sh
+-rw-r--r--   0 erikvw     (501) staff       (20)     2408 2022-07-30 01:15:42.000000 edc-0.4.93/bin/scripts/update_edc.sh
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.642486 edc-0.4.93/bin/systemd/
+-rw-r--r--   0 erikvw     (501) staff       (20)      835 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/celery-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      820 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/celery.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      501 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/celerybeat-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      487 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/celerybeat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      485 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/gunicorn-uat.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      121 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/gunicorn-uat.socket
+-rw-r--r--   0 erikvw     (501) staff       (20)      474 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/gunicorn.service
+-rw-r--r--   0 erikvw     (501) staff       (20)      111 2020-03-07 14:11:38.000000 edc-0.4.93/bin/systemd/gunicorn.socket
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.646448 edc-0.4.93/docs/
+-rw-r--r--   0 erikvw     (501) staff       (20)      634 2022-09-26 00:00:10.000000 edc-0.4.93/docs/Makefile
+-rw-r--r--   0 erikvw     (501) staff       (20)    12969 2023-01-25 02:44:13.000000 edc-0.4.93/docs/README.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     4441 2022-07-30 01:15:42.000000 edc-0.4.93/docs/backup.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     5437 2022-07-30 01:15:42.000000 edc-0.4.93/docs/celery.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      580 2022-07-20 12:27:13.000000 edc-0.4.93/docs/conda.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      975 2022-09-26 00:00:10.000000 edc-0.4.93/docs/conf.py
+-rw-r--r--   0 erikvw     (501) staff       (20)     4806 2022-07-30 01:15:42.000000 edc-0.4.93/docs/configure_web_services.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3646 2023-01-25 02:44:13.000000 edc-0.4.93/docs/deploy_new_droplet.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      163 2020-03-07 14:11:38.000000 edc-0.4.93/docs/dump_users.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      845 2020-03-07 14:11:38.000000 edc-0.4.93/docs/exporting_encrypted_data.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)   258708 2022-07-30 01:15:42.000000 edc-0.4.93/docs/forms_reference.md
+-rw-r--r--   0 erikvw     (501) staff       (20)      445 2022-09-26 00:00:10.000000 edc-0.4.93/docs/index.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      778 2020-03-07 14:11:38.000000 edc-0.4.93/docs/landing_page.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      765 2022-09-26 00:00:10.000000 edc-0.4.93/docs/make.bat
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2020-04-05 21:20:27.000000 edc-0.4.93/docs/multisite_deployment.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     3928 2023-01-25 02:44:13.000000 edc-0.4.93/docs/prepare_database.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)     1211 2022-07-30 01:15:42.000000 edc-0.4.93/docs/printing.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      187 2021-01-28 23:38:49.000000 edc-0.4.93/docs/redis.rst
+-rw-r--r--   0 erikvw     (501) staff       (20)      766 2020-03-07 14:11:38.000000 edc-0.4.93/docs/update_deployment.rst
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.647444 edc-0.4.93/edc.egg-info/
+-rw-r--r--   0 erikvw     (501) staff       (20)    38295 2023-05-24 17:36:30.000000 edc-0.4.93/edc.egg-info/PKG-INFO
+-rw-r--r--   0 erikvw     (501) staff       (20)     1508 2023-05-24 17:36:30.000000 edc-0.4.93/edc.egg-info/SOURCES.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2023-05-24 17:36:30.000000 edc-0.4.93/edc.egg-info/dependency_links.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        1 2022-05-04 16:05:20.000000 edc-0.4.93/edc.egg-info/not-zip-safe
+-rw-r--r--   0 erikvw     (501) staff       (20)     1923 2023-05-24 17:36:30.000000 edc-0.4.93/edc.egg-info/requires.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)        6 2023-05-24 17:36:30.000000 edc-0.4.93/edc.egg-info/top_level.txt
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.647573 edc-0.4.93/image/
+-rw-r--r--   0 erikvw     (501) staff       (20)   160721 2022-03-16 23:21:44.000000 edc-0.4.93/image/icon-pycharm.png
+-rw-r--r--   0 erikvw     (501) staff       (20)      162 2022-05-04 16:05:08.000000 edc-0.4.93/pyproject.toml
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.651033 edc-0.4.93/requirements.tests/
+-rw-r--r--   0 erikvw     (501) staff       (20)       21 2022-08-12 15:19:56.000000 edc-0.4.93/requirements.tests/coverage.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       14 2022-08-10 01:27:44.000000 edc-0.4.93/requirements.tests/docs.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     1053 2023-04-19 03:05:56.000000 edc-0.4.93/requirements.tests/edc.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     4100 2022-09-27 03:34:08.000000 edc-0.4.93/requirements.tests/edc_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       68 2021-04-15 14:46:29.000000 edc-0.4.93/requirements.tests/edc_offline.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       54 2022-08-12 15:19:56.000000 edc-0.4.93/requirements.tests/lint.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       11 2022-07-30 01:15:42.000000 edc-0.4.93/requirements.tests/mysql.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       22 2021-01-28 19:17:27.000000 edc-0.4.93/requirements.tests/postgres.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       86 2022-07-30 01:15:42.000000 edc-0.4.93/requirements.tests/test_utils.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)      238 2022-08-23 12:40:42.000000 edc-0.4.93/requirements.tests/third_party_dev.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)       50 2022-05-03 03:22:05.000000 edc-0.4.93/requirements.tests/tox.txt
+-rw-r--r--   0 erikvw     (501) staff       (20)     2995 2023-05-24 17:36:30.652071 edc-0.4.93/setup.cfg
+drwxr-xr-x   0 erikvw     (501) staff       (20)        0 2023-05-24 17:36:30.651355 edc-0.4.93/utils/
+-rw-r--r--   0 erikvw     (501) staff       (20)        0 2021-02-09 03:49:51.000000 edc-0.4.93/utils/__init__.py
+-rw-r--r--   0 erikvw     (501) staff       (20)      721 2022-05-03 03:22:05.000000 edc-0.4.93/utils/get_edc_requirements.py
```

### Comparing `edc-0.4.92/.gitignore` & `edc-0.4.93/.gitignore`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/.pre-commit-config.yaml` & `edc-0.4.93/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/CHANGES` & `edc-0.4.93/CHANGES`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 Changes
 -------
 
+0.4.93
+------
+- update precommit config, setup python_requires = >=3.10,
+  gh-actions for 3.10, 3.11, dj4.1, dj4.2 (all edc modules)
+- use factory for model_mixin, RESULT_QUANTIFIER_NA, optional
+  field name for fasting, get fieldset from func (edc-glucose)
+- minor refactoring to increase use of constants (edc-adverse-event)
+- fix form validator (edc_dx)
+- add mixins for new HE crf (edc-he)
+
 0.4.92
 ------
 - override methods for url and message in validator (edc-screening)
 
 0.4.91
 ------
 - add attr for custom identity fields in search (edc-listboard)
```

### Comparing `edc-0.4.92/LICENSE` & `edc-0.4.93/LICENSE`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/PKG-INFO` & `edc-0.4.93/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.92
+Version: 0.4.93
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.92/README.rst` & `edc-0.4.93/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/nginx/edc-uat.conf` & `edc-0.4.93/bin/nginx/edc-uat.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/nginx/edc.conf` & `edc-0.4.93/bin/nginx/edc.conf`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/scripts/dev_repos.sh` & `edc-0.4.93/bin/scripts/dev_repos.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/scripts/update_edc.sh` & `edc-0.4.93/bin/scripts/update_edc.sh`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/systemd/celery-uat.service` & `edc-0.4.93/bin/systemd/celery-uat.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/bin/systemd/celery.service` & `edc-0.4.93/bin/systemd/celery.service`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/Makefile` & `edc-0.4.93/docs/Makefile`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/README.rst` & `edc-0.4.93/docs/README.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/backup.rst` & `edc-0.4.93/docs/backup.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/celery.rst` & `edc-0.4.93/docs/celery.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/conda.rst` & `edc-0.4.93/docs/conda.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/conf.py` & `edc-0.4.93/docs/conf.py`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/configure_web_services.rst` & `edc-0.4.93/docs/configure_web_services.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/deploy_new_droplet.rst` & `edc-0.4.93/docs/deploy_new_droplet.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/exporting_encrypted_data.rst` & `edc-0.4.93/docs/exporting_encrypted_data.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/forms_reference.md` & `edc-0.4.93/docs/forms_reference.md`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/landing_page.rst` & `edc-0.4.93/docs/landing_page.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/make.bat` & `edc-0.4.93/docs/make.bat`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/prepare_database.rst` & `edc-0.4.93/docs/prepare_database.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/printing.rst` & `edc-0.4.93/docs/printing.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/docs/update_deployment.rst` & `edc-0.4.93/docs/update_deployment.rst`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/edc.egg-info/PKG-INFO` & `edc-0.4.93/edc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edc
-Version: 0.4.92
+Version: 0.4.93
 Summary: EDC core modules for clinicedc/edc projects.
 Home-page: https://github.com/clinicedc/edc
 Author: Erik van Widenfelt
 Author-email: ew2789@gmail.com
 License: GPL license, see LICENSE
 Keywords: django edc clinical trials research
 Classifier: Environment :: Web Environment
```

### Comparing `edc-0.4.92/edc.egg-info/SOURCES.txt` & `edc-0.4.93/edc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/edc.egg-info/requires.txt` & `edc-0.4.93/edc.egg-info/requires.txt`

 * *Files 17% similar despite different names*

```diff
@@ -19,77 +19,77 @@
 django-extensions
 django-logentry-admin
 django-multisite-edc==2.0.0
 django-revision==0.3.6
 django-simple-history>=3.1.1
 django-storages
 djangorestframework
-edc-action-item==0.3.51
-edc-adherence==0.1.20
-edc-adverse-event==0.3.47
-edc-appointment==0.3.70
-edc-auth==0.3.59
-edc-consent==0.3.44
-edc-constants==0.3.46
-edc-crf==0.3.41
-edc-dashboard==0.3.44
-edc-data-manager==0.3.52
-edc-device==0.3.10
-edc-document-status==0.1.3
-edc-dx==0.1.16
-edc-dx-review==0.1.37
-edc-egfr==0.1.10
-edc-export==0.3.25
-edc-facility==0.3.14
-edc-fieldsets==0.3.12
-edc-form-describer==0.3.12
-edc-form-label==0.3.8
-edc-form-validators==0.3.32
-edc-glucose==0.1.27
-edc-he==0.1.5
-edc-identifier==0.3.22
-edc-lab==0.3.42
-edc-lab-dashboard==0.3.10
-edc-lab-panel==0.1.14
-edc-lab-results==0.1.37
-edc-label==0.3.11
-edc-list-data==0.3.17
-edc-listboard==0.1.8
-edc-locator==0.3.22
-edc-ltfu==0.3.22
-edc-metadata==0.3.50
-edc-mnsi==0.1.15
-edc-model==0.3.29
-edc-model-admin==0.3.43
-edc-model-fields==0.3.6
-edc-model-form==0.1.10
-edc-model-wrapper==0.3.9
-edc-navbar==0.3.15
-edc-notification==0.3.16
-edc-offstudy==0.3.30
-edc-pdf-reports==0.3.11
-edc-pdutils==0.3.21
-edc-pharmacy==0.1.37
-edc-pharmacy-dashboard==0.1.2
+edc-action-item==0.3.52
+edc-adherence==0.1.21
+edc-adverse-event==0.3.51
+edc-appointment==0.3.71
+edc-auth==0.3.60
+edc-consent==0.3.45
+edc-constants==0.3.48
+edc-crf==0.3.42
+edc-dashboard==0.3.45
+edc-data-manager==0.3.53
+edc-device==0.3.11
+edc-document-status==0.1.4
+edc-dx==0.1.19
+edc-dx-review==0.1.38
+edc-egfr==0.1.11
+edc-export==0.3.26
+edc-facility==0.3.15
+edc-fieldsets==0.3.13
+edc-form-describer==0.3.13
+edc-form-label==0.3.9
+edc-form-validators==0.3.33
+edc-glucose==0.1.28
+edc-he==0.1.6
+edc-identifier==0.3.23
+edc-lab==0.3.43
+edc-lab-dashboard==0.3.11
+edc-lab-panel==0.1.15
+edc-lab-results==0.1.38
+edc-label==0.3.12
+edc-list-data==0.3.18
+edc-listboard==0.1.9
+edc-locator==0.3.23
+edc-ltfu==0.3.23
+edc-metadata==0.3.51
+edc-mnsi==0.1.16
+edc-model==0.3.30
+edc-model-admin==0.3.44
+edc-model-fields==0.3.7
+edc-model-form==0.1.11
+edc-model-wrapper==0.3.10
+edc-navbar==0.3.16
+edc-notification==0.3.17
+edc-offstudy==0.3.31
+edc-pdf-reports==0.3.13
+edc-pdutils==0.3.22
+edc-pharmacy==0.1.38
+edc-pharmacy-dashboard==0.1.3
 edc-prn==0.3.13
-edc-protocol==0.3.8
-edc-protocol-incident==0.1.24
-edc-qol==0.1.11
-edc-randomization==0.3.45
-edc-reference==0.3.14
-edc-refusal==0.1.10
-edc-registration==0.3.26
-edc-reportable==0.3.30
-edc-review-dashboard==0.3.18
-edc-rx==0.1.5
-edc-screening==0.3.32
-edc-search==0.3.6
-edc-sites==0.3.19
-edc-subject-dashboard==0.3.34
-edc-subject-model-wrappers==0.3.13
-edc-timepoint==0.3.10
-edc-transfer==0.3.13
-edc-unblinding==0.1.13
-edc-utils==0.3.19
-edc-visit-schedule==0.3.59
-edc-visit-tracking==0.3.50
-edc-vitals==0.1.10
+edc-protocol==0.3.9
+edc-protocol-incident==0.1.25
+edc-qol==0.1.13
+edc-randomization==0.3.46
+edc-reference==0.3.15
+edc-refusal==0.1.11
+edc-registration==0.3.28
+edc-reportable==0.3.31
+edc-review-dashboard==0.3.19
+edc-rx==0.1.6
+edc-screening==0.3.33
+edc-search==0.3.7
+edc-sites==0.3.20
+edc-subject-dashboard==0.3.36
+edc-subject-model-wrappers==0.3.15
+edc-timepoint==0.3.11
+edc-transfer==0.3.14
+edc-unblinding==0.1.14
+edc-utils==0.3.20
+edc-visit-schedule==0.3.61
+edc-visit-tracking==0.3.51
+edc-vitals==0.1.11
```

### Comparing `edc-0.4.92/image/icon-pycharm.png` & `edc-0.4.93/image/icon-pycharm.png`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/requirements.tests/edc.txt` & `edc-0.4.93/requirements.tests/edc.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/requirements.tests/edc_dev.txt` & `edc-0.4.93/requirements.tests/edc_dev.txt`

 * *Files identical despite different names*

### Comparing `edc-0.4.92/setup.cfg` & `edc-0.4.93/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -48,84 +48,84 @@
 	django-extensions
 	django-logentry-admin
 	django-multisite-edc==2.0.0
 	django-revision==0.3.6
 	django-simple-history>=3.1.1
 	django-storages
 	djangorestframework
-	edc-action-item==0.3.51
-	edc-adherence==0.1.20
-	edc-adverse-event==0.3.47
-	edc-appointment==0.3.70
-	edc-auth==0.3.59
-	edc-consent==0.3.44
-	edc-constants==0.3.46
-	edc-crf==0.3.41
-	edc-dashboard==0.3.44
-	edc-data-manager==0.3.52
-	edc-device==0.3.10
-	edc-document-status==0.1.3
-	edc-dx==0.1.16
-	edc-dx-review==0.1.37
-	edc-egfr==0.1.10
-	edc-export==0.3.25
-	edc-facility==0.3.14
-	edc-fieldsets==0.3.12
-	edc-form-describer==0.3.12
-	edc-form-label==0.3.8
-	edc-form-validators==0.3.32
-	edc-glucose==0.1.27
-	edc-he==0.1.5
-	edc-identifier==0.3.22
-	edc-lab==0.3.42
-	edc-lab-dashboard==0.3.10
-	edc-lab-panel==0.1.14
-	edc-lab-results==0.1.37
-	edc-label==0.3.11
-	edc-list-data==0.3.17
-	edc-listboard==0.1.8
-	edc-locator==0.3.22
-	edc-ltfu==0.3.22
-	edc-metadata==0.3.50
-	edc-mnsi==0.1.15
-	edc-model==0.3.29
-	edc-model-admin==0.3.43
-	edc-model-fields==0.3.6
-	edc-model-form==0.1.10
-	edc-model-wrapper==0.3.9
-	edc-navbar==0.3.15
-	edc-notification==0.3.16
-	edc-offstudy==0.3.30
-	edc-pdf-reports==0.3.11
-	edc-pdutils==0.3.21
-	edc-pharmacy==0.1.37
-	edc-pharmacy-dashboard==0.1.2
+	edc-action-item==0.3.52
+	edc-adherence==0.1.21
+	edc-adverse-event==0.3.51
+	edc-appointment==0.3.71
+	edc-auth==0.3.60
+	edc-consent==0.3.45
+	edc-constants==0.3.48
+	edc-crf==0.3.42
+	edc-dashboard==0.3.45
+	edc-data-manager==0.3.53
+	edc-device==0.3.11
+	edc-document-status==0.1.4
+	edc-dx==0.1.19
+	edc-dx-review==0.1.38
+	edc-egfr==0.1.11
+	edc-export==0.3.26
+	edc-facility==0.3.15
+	edc-fieldsets==0.3.13
+	edc-form-describer==0.3.13
+	edc-form-label==0.3.9
+	edc-form-validators==0.3.33
+	edc-glucose==0.1.28
+	edc-he==0.1.6
+	edc-identifier==0.3.23
+	edc-lab==0.3.43
+	edc-lab-dashboard==0.3.11
+	edc-lab-panel==0.1.15
+	edc-lab-results==0.1.38
+	edc-label==0.3.12
+	edc-list-data==0.3.18
+	edc-listboard==0.1.9
+	edc-locator==0.3.23
+	edc-ltfu==0.3.23
+	edc-metadata==0.3.51
+	edc-mnsi==0.1.16
+	edc-model==0.3.30
+	edc-model-admin==0.3.44
+	edc-model-fields==0.3.7
+	edc-model-form==0.1.11
+	edc-model-wrapper==0.3.10
+	edc-navbar==0.3.16
+	edc-notification==0.3.17
+	edc-offstudy==0.3.31
+	edc-pdf-reports==0.3.13
+	edc-pdutils==0.3.22
+	edc-pharmacy==0.1.38
+	edc-pharmacy-dashboard==0.1.3
 	edc-prn==0.3.13
-	edc-protocol==0.3.8
-	edc-protocol-incident==0.1.24
-	edc-qol==0.1.11
-	edc-randomization==0.3.45
-	edc-reference==0.3.14
-	edc-refusal==0.1.10
-	edc-registration==0.3.26
-	edc-reportable==0.3.30
-	edc-review-dashboard==0.3.18
-	edc-rx==0.1.5
-	edc-screening==0.3.32
-	edc-search==0.3.6
-	edc-sites==0.3.19
-	edc-subject-dashboard==0.3.34
-	edc-subject-model-wrappers==0.3.13
-	edc-timepoint==0.3.10
-	edc-transfer==0.3.13
-	edc-unblinding==0.1.13
-	edc-utils==0.3.19
-	edc-visit-schedule==0.3.59
-	edc-visit-tracking==0.3.50
-	edc-vitals==0.1.10
+	edc-protocol==0.3.9
+	edc-protocol-incident==0.1.25
+	edc-qol==0.1.13
+	edc-randomization==0.3.46
+	edc-reference==0.3.15
+	edc-refusal==0.1.11
+	edc-registration==0.3.28
+	edc-reportable==0.3.31
+	edc-review-dashboard==0.3.19
+	edc-rx==0.1.6
+	edc-screening==0.3.33
+	edc-search==0.3.7
+	edc-sites==0.3.20
+	edc-subject-dashboard==0.3.36
+	edc-subject-model-wrappers==0.3.15
+	edc-timepoint==0.3.11
+	edc-transfer==0.3.14
+	edc-unblinding==0.1.14
+	edc-utils==0.3.20
+	edc-visit-schedule==0.3.61
+	edc-visit-tracking==0.3.51
+	edc-vitals==0.1.11
 
 [options.packages.find]
 exclude = 
 	examples*
 	tools*
 	docs*
 	bin*
```

### Comparing `edc-0.4.92/utils/get_edc_requirements.py` & `edc-0.4.93/utils/get_edc_requirements.py`

 * *Files identical despite different names*

