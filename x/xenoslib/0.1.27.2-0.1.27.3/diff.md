# Comparing `tmp/xenoslib-0.1.27.2.tar.gz` & `tmp/xenoslib-0.1.27.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.27.2.tar", last modified: Wed May 24 00:15:12 2023, max compression
+gzip compressed data, was "xenoslib-0.1.27.3.tar", last modified: Wed May 24 00:24:07 2023, max compression
```

## Comparing `xenoslib-0.1.27.2.tar` & `xenoslib-0.1.27.3.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.257803 xenoslib-0.1.27.2/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:24:07.298535 xenoslib-0.1.27.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:24:07.298535 xenoslib-0.1.27.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:24:07.298535 xenoslib-0.1.27.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:24:07.294535 xenoslib-0.1.27.3/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 00:23:52.000000 xenoslib-0.1.27.3/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:24:07.298535 xenoslib-0.1.27.3/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:24:07.000000 xenoslib-0.1.27.3/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 00:24:07.000000 xenoslib-0.1.27.3/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:24:07.000000 xenoslib-0.1.27.3/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 00:24:07.000000 xenoslib-0.1.27.3/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 00:24:07.000000 xenoslib-0.1.27.3/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.27.2/LICENSE` & `xenoslib-0.1.27.3/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/README.md` & `xenoslib-0.1.27.3/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/setup.py` & `xenoslib-0.1.27.3/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/base.py` & `xenoslib-0.1.27.3/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/dev.py` & `xenoslib-0.1.27.3/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/extend.py` & `xenoslib-0.1.27.3/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/linux.py` & `xenoslib-0.1.27.3/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/mail.py` & `xenoslib-0.1.27.3/xenoslib/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,22 +40,26 @@
     Usage:
 
     from xenoslib.mail import MailFetcher
     for email_data in MailFetcher(imap_server, mail_addr, mail_pwd, interval=30, days=30):
         print(email_data["subject"])
     """
 
-    msg_ids = deque(maxlen=999)
-
-    def __new__(cls, imap_server, mail_addr, mail_pwd, interval=30, days=1):
+    def __new__(cls, imap_server, mail_addr, mail_pwd, interval=30, days=1, skip_current=False):
         self = super().__new__(cls)
         self.imap_server = imap_server
         self.mail_addr = mail_addr
         self.mail_pwd = mail_pwd
         self.days = days
+
+        self.msg_ids = deque(maxlen=999)
+        if skip_current:  # mark current mails
+            logger.debug("Skipping...")
+            mails = self.fetch_emails()
+            self.msg_ids.extend(mails.keys())
         return self.fetching(interval=interval)
 
     def fetching(self, interval=30):
         """Continuously fetch emails at the specified interval."""
         logger.debug("Start checking emails...")
         while True:
             try:
@@ -143,15 +147,17 @@
     try:
         import env  # noqa
     except ModuleNotFoundError:
         pass
     imap_server = os.environ["IMAP_SERVER"]
     mail_addr = os.environ["IMAP_ADDR"]
     mail_pwd = os.environ["IMAP_PASS"]
-    for email_data in MailFetcher(imap_server, mail_addr, mail_pwd, interval=1, days=30):
+    for email_data in MailFetcher(
+        imap_server, mail_addr, mail_pwd, interval=1, days=30, skip_current=True
+    ):
         print(email_data["subject"])
 
 
 def test():
     try:
         import env  # noqa
     except ModuleNotFoundError:
@@ -163,8 +169,9 @@
     message = '<span style="color:red">This is a test email.</span>'
     email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=465)
     # email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=587)
     email_sender.send(subject=subject, message=message, receiver=[os.environ["RECEIVER"]])
 
 
 if __name__ == "__main__":
-    test()
+    test_imap()
+    # test()
```

### Comparing `xenoslib-0.1.27.2/xenoslib/mock.py` & `xenoslib-0.1.27.3/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/onedrive.py` & `xenoslib-0.1.27.3/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/win_trayicon.py` & `xenoslib-0.1.27.3/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.2/xenoslib/windows.py` & `xenoslib-0.1.27.3/xenoslib/windows.py`

 * *Files identical despite different names*

