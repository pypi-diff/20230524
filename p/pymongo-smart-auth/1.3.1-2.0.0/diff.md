# Comparing `tmp/pymongo_smart_auth-1.3.1.tar.gz` & `tmp/pymongo_smart_auth-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymongo_smart_auth-1.3.1.tar", last modified: Tue Aug 23 14:55:52 2022, max compression
+gzip compressed data, was "pymongo_smart_auth-2.0.0.tar", last modified: Wed May 24 09:39:56 2023, max compression
```

## Comparing `pymongo_smart_auth-1.3.1.tar` & `pymongo_smart_auth-2.0.0.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2022-08-23 14:55:52.900778 pymongo_smart_auth-1.3.1/
--rw-------   0 peetersp   (501) staff       (20)     1077 2018-10-11 21:28:49.000000 pymongo_smart_auth-1.3.1/LICENSE
--rw-r--r--   0 peetersp   (501) staff       (20)      362 2022-08-23 14:55:52.900946 pymongo_smart_auth-1.3.1/PKG-INFO
--rw-------   0 peetersp   (501) staff       (20)     3836 2022-08-23 14:40:43.000000 pymongo_smart_auth-1.3.1/README.md
-drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2022-08-23 14:55:52.894199 pymongo_smart_auth-1.3.1/pymongo_smart_auth/
--rw-------   0 peetersp   (501) staff       (20)    11191 2022-08-23 14:54:41.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth/AuthMongoClient.py
--rw-------   0 peetersp   (501) staff       (20)      138 2022-08-23 14:46:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth/__init__.py
-drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2022-08-23 14:55:52.900022 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/
--rw-------   0 peetersp   (501) staff       (20)      362 2022-08-23 14:55:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/PKG-INFO
--rw-------   0 peetersp   (501) staff       (20)      351 2022-08-23 14:55:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/SOURCES.txt
--rw-------   0 peetersp   (501) staff       (20)        1 2022-08-23 14:55:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/dependency_links.txt
--rw-------   0 peetersp   (501) staff       (20)        8 2022-08-23 14:55:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/requires.txt
--rw-------   0 peetersp   (501) staff       (20)       19 2022-08-23 14:55:52.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/top_level.txt
--rw-------   0 peetersp   (501) staff       (20)        1 2018-10-11 21:28:49.000000 pymongo_smart_auth-1.3.1/pymongo_smart_auth.egg-info/zip-safe
--rw-------   0 peetersp   (501) staff       (20)       67 2022-08-23 14:55:52.901535 pymongo_smart_auth-1.3.1/setup.cfg
--rw-------   0 peetersp   (501) staff       (20)      535 2022-08-23 14:55:04.000000 pymongo_smart_auth-1.3.1/setup.py
+drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2023-05-24 09:39:56.811185 pymongo_smart_auth-2.0.0/
+-rw-------   0 peetersp   (501) staff       (20)     1077 2018-10-11 21:28:49.000000 pymongo_smart_auth-2.0.0/LICENSE
+-rw-r--r--   0 peetersp   (501) staff       (20)      385 2023-05-24 09:39:56.811389 pymongo_smart_auth-2.0.0/PKG-INFO
+-rw-r--r--   0 peetersp   (501) staff       (20)     4202 2023-05-24 09:37:57.000000 pymongo_smart_auth-2.0.0/README.md
+drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2023-05-24 09:39:56.781811 pymongo_smart_auth-2.0.0/pymongo_smart_auth/
+-rw-r--r--   0 peetersp   (501) staff       (20)    11416 2023-05-24 09:37:57.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth/AuthMongoClient.py
+-rw-------   0 peetersp   (501) staff       (20)      138 2022-08-23 14:46:52.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth/__init__.py
+drwxr-xr-x   0 peetersp   (501) staff       (20)        0 2023-05-24 09:39:56.810093 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/
+-rw-------   0 peetersp   (501) staff       (20)      385 2023-05-24 09:39:56.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/PKG-INFO
+-rw-------   0 peetersp   (501) staff       (20)      366 2023-05-24 09:39:56.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/SOURCES.txt
+-rw-------   0 peetersp   (501) staff       (20)        1 2023-05-24 09:39:56.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/dependency_links.txt
+-rw-------   0 peetersp   (501) staff       (20)       13 2023-05-24 09:39:56.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/requires.txt
+-rw-------   0 peetersp   (501) staff       (20)       19 2023-05-24 09:39:56.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/top_level.txt
+-rw-------   0 peetersp   (501) staff       (20)        1 2018-10-11 21:28:49.000000 pymongo_smart_auth-2.0.0/pymongo_smart_auth.egg-info/zip-safe
+-rw-r--r--   0 peetersp   (501) staff       (20)       83 2023-05-24 09:37:57.000000 pymongo_smart_auth-2.0.0/pyproject.toml
+-rw-r--r--   0 peetersp   (501) staff       (20)      171 2023-05-24 09:39:56.811915 pymongo_smart_auth-2.0.0/setup.cfg
+-rw-r--r--   0 peetersp   (501) staff       (20)      571 2023-05-24 09:37:57.000000 pymongo_smart_auth-2.0.0/setup.py
```

### Comparing `pymongo_smart_auth-1.3.1/LICENSE` & `pymongo_smart_auth-2.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymongo_smart_auth-1.3.1/README.md` & `pymongo_smart_auth-2.0.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -22,58 +22,70 @@
 
 ## Usage
 
 The `MongoClient` class from the `PyMongo-Smart-Auth` package is a drop-in replacement for PyMongo's `MongoClient` that simplifies authentication management.
 
 The constructor works in the same way as the `MongoClient` constructor with four additional parameters, all optional:
 
-* `user`: the user to authenticate with
+* `username`: the username to authenticate with
 * `password`: the password to authenticate with
 * `credentials_file`: a file where credentials can be found
 * `authenticate`: a boolean indicating whether the client should authenticate (defaults to `True`)
 
-When using a credentials file, it should either have a single line with a fully authenticated URI or have the authentication database on the first line, the user on the second and the password on the third. Empty lines are ignored. Example:
+### Credentials file
 
-    admin
-    administrator
-    P4ssw0rd
+When using a credentials file, it should either have:
+
+* a single line with a fully authenticated URI
+* the authentication database on the first line, the user on the second and the password on the third. Empty lines are ignored. Example file:
+
+        admin
+        administrator
+        P4ssw0rd
+
+### Credential lookup order
 
 Upon initialisation with the default `authenticate=True`, the client looks for credentials in the following order:
 
-1. The `user` and `password` parameters
+1. The `username` and `password` parameters
 2. The passed `credentials_file`
 3. The `MONGO_CREDENTIAL_FILE` environment variable formatted with the kwargs of the constructor, if applicable
 4. The `MONGO_AUTHENTICATED_URI` environment variable
 5. The `MONGO_AUTHENTICATION_DATABASE`, `MONGO_USERNAME` and `MONGO_PASSWORD` environment variables
 6. The `.mongo_credentials` file in the user's home
 7. The `mongo_credentials` file in the `/etc` folder
 
-Usage examples:
+### Usage examples
 
 ```python
 from pymongo_smart_auth import MongoClient
 
 # Explicit user and password
-mongo1 = MongoClient(user='user', password='p4ssw0rd')
+mongo1 = MongoClient(username='user', password='p4ssw0rd')
 database1 = mongo1['database1'] # Automatically authenticated
 
 # Explicit user and password with separate authentication database
-mongo2 = MongoClient(user='user', password='p4ssw0rd', authentication_database='mongo_users')
+mongo2 = MongoClient(username='user', password='p4ssw0rd', authentication_database='mongo_users')
 database2 = mongo2['database2'] # Automatically authenticated
 
 # Will read /some/path/mongo_credentials
 mongo3 = MongoClient(credentials_file='/some/path/mongo_credentials')
 database3 = mongo3['database3'] # Automatically authenticated
 
-# Will read the environment variables if they exist, otherwise ~/.mongo_credentials if it exists, otherwise /etc/mongo_credentials
+# Will read the file in the MONGO_CREDENTIAL_FILE environment variable if set,
+# then the file in MONGO_CREDENTIAL_FILE environment variable if set,
+# then the MONGO_AUTHENTICATION_DATABASE, MONGO_USERNAME and MONGO_PASSWORD environment variables if set,
+# then ~/.mongo_credentials if it exists,
+# otherwise /etc/mongo_credentials
 mongo4 = MongoClient()
 database4 = mongo4['database4'] # Automatically authenticated
 
 # Will authenticate with a file defined in the environment with a keyword argument
-# Assuming MONGO_CREDENTIAL_FILE=/etc/credentials_{group}
+# Assuming MONGO_CREDENTIAL_FILE=/etc/credentials_{group},
+# this will authenticate with the credentials in /etc/credentials_my_group
 mongo5 = MongoClient(group='my_group')
 database5 = mongo6['my_group_database'] # Automatically authenticated
 
 # Will not authenticate
 mongo6 = MongoClient(authenticate=False)
 database6 = mongo5['database5'] # Not authenticated
 ```
```

### Comparing `pymongo_smart_auth-1.3.1/pymongo_smart_auth/AuthMongoClient.py` & `pymongo_smart_auth-2.0.0/pymongo_smart_auth/AuthMongoClient.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,154 +1,156 @@
 import inspect
 import logging
 import os
 import stat
 import sys
-
 from string import Formatter
 
-from pymongo import MongoClient
-from pymongo.errors import ConfigurationError
+import pymongo
+
+PYMONGO_MAJOR_VERSION = int(pymongo.__version__.split('.')[0])
 
 logging.basicConfig()
 logger = logging.getLogger('pymongo_smart_auth')
 
 
-class AuthMongoClient(MongoClient):
-    USER_CREDENTIALS = '%s/.mongo_credentials' % os.path.expanduser('~')
+class AuthMongoClient(pymongo.MongoClient):
+    USER_CREDENTIALS = '{}/.mongo_credentials'.format(os.path.expanduser('~'))
     SERVER_CREDENTIALS = '/etc/mongo_credentials'
     __missing_credentials_warning_shown = False
-    __PYMONGO_ARGS = set(inspect.getfullargspec(MongoClient).args)
+    __PYMONGO_ARGS = set(inspect.getfullargspec(pymongo.MongoClient).args)
 
     # On Unix systems, check the permissions of the credential file
     if sys.platform in ('linux', 'linux2', 'darwin') and os.path.exists(USER_CREDENTIALS):
         # Get the file stats
         cred_file_stats = os.stat(USER_CREDENTIALS)
 
         # Issue a warning if the file is group readable
         if bool(cred_file_stats.st_mode & stat.S_IRGRP):
             logger.warning("{0} is readable by the group. It should only be readable by the user. Fix by running:\nchmod 600 \"{0}\"".format(USER_CREDENTIALS))
 
         # Issue a warning if the file is readable by others
         if bool(cred_file_stats.st_mode & stat.S_IROTH):
             logger.warning("{0} is readable by others. It should only be readable by the user. Fix by running:\nchmod 600 \"{0}\"".format(USER_CREDENTIALS))
 
-    def __init__(
+    def __init__(  # noqa: C901
             self,
             host=None,
             port=None,
             document_class=dict,
             tz_aware=False,
             connect=True,
-            user=None,
-            password=None,
-            authentication_database=None,
             credentials_file=None,
             authenticate=True,
             **kwargs):
         """MongoDB connection with built-in authentication."""
 
         # If authentication is off for this connection, just initialise
         if not authenticate:
-            super(AuthMongoClient, self).__init__(host, port, document_class, tz_aware, connect, **kwargs)
+            super().__init__(host, port, document_class, tz_aware, connect, **kwargs)
 
             return
 
+        username = kwargs.get('username')
+        password = kwargs.get('password')
+        authSource = kwargs.get('authSource')
+        authenticated_mongodb_uri = None
+
         # If no user was passed, try to get the credentials elsewhere
-        if user is None:
+        if username is None:
             # If no credential file was passed
             if credentials_file is None:
                 # Check if a specific credential file was requested
                 logger.debug('Checking environment for credential file path...')
 
                 credentials_file = os.environ.get('MONGO_CREDENTIAL_FILE') or None
 
                 if credentials_file is not None:
-                    logger.debug('Got MONGO_CREDENTIAL_FILE = {}'.format(credentials_file))
+                    logger.debug(f'Got MONGO_CREDENTIAL_FILE = {credentials_file}')
 
                     # Check if the path is a format string
                     field_references = {field for _, field, _, _ in Formatter().parse(credentials_file) if field}
 
                     # If the string contains field references
                     if len(field_references) > 0:
-                        logger.debug('Fields in file path = {}'.format(field_references))
+                        logger.debug(f'Fields in file path = {field_references}')
 
                         # Create a set with the known arguments from PyMongo and our library
                         # and check that the fields do not clash with those
                         constructor_args = AuthMongoClient.__PYMONGO_ARGS.union(set(inspect.getargspec(AuthMongoClient).args))
                         name_clashes = field_references.intersection(constructor_args)
 
-                        logger.debug('Constructor args = {}'.format(constructor_args))
+                        logger.debug(f'Constructor args = {constructor_args}')
 
                         # If there are name clashes, raise a ConfigurationError
                         if len(name_clashes) > 0:
-                            raise ConfigurationError('The following variables in your MONGO_CREDENTIAL_FILE environment variable clash with the variables of either the AuthMongoClient or MongoClient constructor: {}.'.format(', '.join(name_clashes)))
+                            raise pymongo.errors.ConfigurationError('The following variables in your MONGO_CREDENTIAL_FILE environment variable clash with the variables of either the AuthMongoClient or MongoClient constructor: {}.'.format(', '.join(name_clashes)))
 
                         # Check that the kwargs contain the necessary fields
                         missing_kwargs = field_references - set(kwargs)
 
                         # If fields are missing, raise a ConfigurationError
                         if len(missing_kwargs) > 0:
-                            raise ConfigurationError('The following variables were found in your MONGO_CREDENTIAL_FILE environment variable but were not in the kwargs for the AuthMongoClient constructor: {}.'.format(', '.join(missing_kwargs)))
+                            raise pymongo.errors.ConfigurationError('The following variables were found in your MONGO_CREDENTIAL_FILE environment variable but were not in the kwargs for the AuthMongoClient constructor: {}.'.format(', '.join(missing_kwargs)))
 
                         # Pop the format string arguments from the kwargs
                         format_string_arguments = {}
 
                         for field in field_references:
                             format_string_arguments[field] = kwargs.pop(field)
 
                         # Build the final path to the credential file
-                        logger.info("Formatting credential file '{}' found in environment with arguments: {}.".format(credentials_file, format_string_arguments))
+                        logger.info(f'Formatting credential file {credentials_file!r} found in environment with arguments: {format_string_arguments}.')
                         credentials_file = credentials_file.format(**format_string_arguments)
                     else:
-                        logger.info("Using credential file found in environment: '{}'.".format(credentials_file))
+                        logger.info(f'Using credential file found in environment: {credentials_file!r}.')
                 else:
                     logger.debug('Got no credential file from the environment (MONGO_CREDENTIAL_FILE).')
 
             if credentials_file is None:
                 # Attempt to get the configuration from the environment
                 logger.debug('Checking environment for authenticated URI...')
 
                 authenticated_mongodb_uri = os.environ.get('MONGO_AUTHENTICATED_URI') or None
 
                 # If the environment does not contain a URI, check it for credentials
                 if authenticated_mongodb_uri is None:
                     logger.debug('Got no URI from the environment (MONGO_AUTHENTICATED_URI); checking environment for credentials...')
 
-                    authentication_database = os.environ.get('MONGO_AUTHENTICATION_DATABASE') or None
-                    user = os.environ.get('MONGO_USERNAME') or None
+                    authSource = os.environ.get('MONGO_AUTHENTICATION_DATABASE') or None
+                    username = os.environ.get('MONGO_USERNAME') or None
                     password = os.environ.get('MONGO_PASSWORD') or None
 
-                    logger.debug('Got MONGO_AUTHENTICATION_DATABASE = {}'.format(authentication_database))
-                    logger.debug('Got MONGO_USERNAME = {}'.format(user))
-                    logger.debug('MONGO_PASSWORD present and non-empty: {}'.format(password is not None))
+                    logger.debug(f'Got MONGO_AUTHENTICATION_DATABASE = {authSource}')
+                    logger.debug(f'Got MONGO_USERNAME = {username}')
+                    logger.debug(f'MONGO_PASSWORD present and non-empty: {password is not None}')
 
-                    values_to_check = {authentication_database, user, password}
+                    values_to_check = {authSource, username, password}
 
                     # If there are undefined environment variables
                     if None in values_to_check:
                         # If they aren't all undefined, raise a ConfigurationError
                         if len(values_to_check) > 1:
-                            raise ConfigurationError("MONGO_AUTHENTICATED_URI environment variable not set and missing other environment variables.")
+                            raise pymongo.errors.ConfigurationError('MONGO_AUTHENTICATED_URI environment variable not set and missing other environment variables.')
 
                         logger.debug('Got no credentials from environment; falling back to static credential files.')
 
                         # Fall back to the first existing credential file
                         # between the one in the user's home and the one in /etc
                         if os.path.exists(self.USER_CREDENTIALS):
                             credentials_file = self.USER_CREDENTIALS
                         elif os.path.exists(self.SERVER_CREDENTIALS):
                             credentials_file = self.SERVER_CREDENTIALS
                         elif not self.__missing_credentials_warning_shown:
-                            logger.warning("Mongo client is authenticated but no credential file was found at either '%s' or '%s' and environment variables were not defined." % (self.USER_CREDENTIALS, self.SERVER_CREDENTIALS))
+                            logger.warning(f"Mongo client is authenticated but no credential file was found at either '{self.USER_CREDENTIALS}' or '{self.SERVER_CREDENTIALS}' and environment variables were not defined.")
 
                             self.__missing_credentials_warning_shown = True
 
                         if credentials_file is not None:
-                            logger.info("Using static credential file: '{}'.".format(credentials_file))
+                            logger.info(f'Using static credential file: {credentials_file!r}.')
                     else:
                         logger.info('Using credentials found in environment.')
                 else:
                     logger.info('Using URI found in environment.')
 
             # If there is a credential file to check
             if credentials_file is not None:
@@ -157,57 +159,62 @@
                     with open(credentials_file) as credentials_file_obj:
                         # Read the file
                         lines = [line.strip() for line in credentials_file_obj.readlines() if line.strip() != '']
                         num_lines = len(lines)
 
                         # Verify the file has the expected number of lines
                         if num_lines not in {1, 3}:
-                            raise ConfigurationError("Credential file '%s' is badly formatted (should contain 1 or 3 non-blank lines)." % credentials_file)
+                            raise pymongo.errors.ConfigurationError(f"Credential file '{credentials_file}' is badly formatted (should contain 1 or 3 non-blank lines).")
 
                         if num_lines == 3:
                             # Get the authentication database, user and password from the contents
-                            authentication_database = lines[0] or None
-                            user = lines[1] or None
+                            authSource = lines[0] or None
+                            username = lines[1] or None
                             password = lines[2] or None
                             authenticated_mongodb_uri = None
                         else:
                             # Get the URI from the contents
                             authenticated_mongodb_uri = lines[0]
-                            authentication_database = None
-                            user = None
+                            authSource = None
+                            username = None
                             password = None
-                except IOError:
-                    raise ConfigurationError("Could not open credential file: '%s'." % credentials_file)
-        elif password is None or authentication_database is None:
-            raise ConfigurationError("You need to define a password and authentication database when setting a user.")
+                except OSError:
+                    raise pymongo.errors.ConfigurationError(f'Could not open credential file: {credentials_file!r}.')
+        elif password is None or authSource is None:
+            raise pymongo.errors.ConfigurationError('You need to define a password and authSource when setting a user.')
 
         can_manually_authenticate = False
 
         if authenticated_mongodb_uri is None:
-            authentication_parameters = {authentication_database, user, password}
+            authentication_parameters = {authSource, username, password}
 
             # If any of the authentication parameters is None
             if None in authentication_parameters:
                 # Raise a ConfigurationError if at least one of them was set
                 if len(authentication_parameters) > 1:
-                    raise ConfigurationError("Credentials are missing at least one parameter (authentication database, username or password).")
+                    raise pymongo.errors.ConfigurationError('Credentials are missing at least one parameter (authentication database, username or password).')
             else:
                 can_manually_authenticate = True
         else:
             if not authenticated_mongodb_uri.startswith('mongodb://'):
-                raise ConfigurationError('Mongo URI should start with mongodb://')
+                raise pymongo.errors.ConfigurationError('Mongo URI should start with mongodb://')
 
             logger.info('Authenticating with Mongo URI.')
 
             if host is not None:
-                raise ValueError("Ambiguous connection: a host was passed to the constructor, but a URI was extracted from environment variables or a credential file.")
+                raise ValueError('Ambiguous connection: a host was passed to the constructor, but a URI was extracted from environment variables or a credential file.')
 
             host = authenticated_mongodb_uri
             port = None
 
-        super(AuthMongoClient, self).__init__(host, port, document_class, tz_aware, connect, **kwargs)
+        if PYMONGO_MAJOR_VERSION >= 4:
+            kwargs['authSource'] = authSource
+            kwargs['username'] = username
+            kwargs['password'] = password
+
+        super().__init__(host, port, document_class, tz_aware, connect, **kwargs)
 
         # Authenticate the connection manually if possible
-        if can_manually_authenticate:
+        if PYMONGO_MAJOR_VERSION < 4 and can_manually_authenticate:
             logger.info('Authenticating with extracted credentials.')
 
-            self[authentication_database].authenticate(user, password)
+            self[authSource].authenticate(username, password)
```

### Comparing `pymongo_smart_auth-1.3.1/setup.py` & `pymongo_smart_auth-2.0.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from setuptools import setup
 
 setup(name='pymongo_smart_auth',
-      version='1.3.1',
+      version='2.0.0',
       description='This package extends PyMongo to provide built-in smart authentication.',
       url='https://github.com/PLPeeters/PyMongo-Smart-Auth',
       author='Pierre-Louis Peeters',
       author_email='PLPeeters@users.noreply.github.com',
       license='MIT',
       packages=['pymongo_smart_auth'],
+      python_requires='>=3.6',
       install_requires=[
-          'pymongo'
+          'pymongo<5,>3'
       ],
       keywords=['mongo', 'pymongo', 'authentication', 'seamless'],
       zip_safe=True)
```

