# Comparing `tmp/xenoslib-0.1.27.1.tar.gz` & `tmp/xenoslib-0.1.27.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.27.1.tar", last modified: Tue May 23 08:08:32 2023, max compression
+gzip compressed data, was "xenoslib-0.1.27.2.tar", last modified: Wed May 24 00:15:12 2023, max compression
```

## Comparing `xenoslib-0.1.27.1.tar` & `xenoslib-0.1.27.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.522583 xenoslib-0.1.27.1/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.257803 xenoslib-0.1.27.2/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5688 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-24 00:14:56.000000 xenoslib-0.1.27.2/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 00:15:12.261803 xenoslib-0.1.27.2/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-24 00:15:12.000000 xenoslib-0.1.27.2/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.27.1/LICENSE` & `xenoslib-0.1.27.2/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/README.md` & `xenoslib-0.1.27.2/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/setup.py` & `xenoslib-0.1.27.2/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/base.py` & `xenoslib-0.1.27.2/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/dev.py` & `xenoslib-0.1.27.2/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/extend.py` & `xenoslib-0.1.27.2/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/linux.py` & `xenoslib-0.1.27.2/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/mail.py` & `xenoslib-0.1.27.2/xenoslib/mail.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 # Send email
 sender = EmailSender(smtp_server, sender, password, smtp_port=25)
 sender.send(subject, message, receiver, cc, bcc, filename)
 
 """
 import os
 import datetime
-from time import sleep, time
+from time import sleep
 import logging
 from collections import deque
 import smtplib
 import email
 from email.mime.text import MIMEText
 from email.header import Header
 from email.mime.application import MIMEApplication
 from email.mime.multipart import MIMEMultipart
+from email.utils import make_msgid
 
 from imapclient import IMAPClient
 
 
 logger = logging.getLogger(__name__)
 
 
@@ -100,46 +101,48 @@
 
 class SMTPMail:
     def __init__(self, smtp_server="", sender="", password="", smtp_port=25):
         self.smtp_server = smtp_server
         self.smtp_port = int(smtp_port)
         self.sender = sender
         self.password = password
-        if self.smtp_port == 25:
-            self.SMTP = smtplib.SMTP
-        else:
+        if self.smtp_port == 465:
             self.SMTP = smtplib.SMTP_SSL
+        else:
+            self.SMTP = smtplib.SMTP
 
     def send(self, subject, message, receiver=[], cc=[], bcc=[], filename=None):
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
         msg["From"] = Header(self.sender, "utf-8")
         msg["To"] = ";".join(receiver)
         msg["Cc"] = ";".join(cc)
-        msg["Message-ID"] = f"<{time()}>"
+        msg["Message-ID"] = make_msgid()
         receiver.extend(cc)
         receiver.extend(bcc)
         msg.attach(MIMEText(message, "html", "utf-8"))
 
         if filename:
             attachment = MIMEApplication(open(filename, "rb").read())
             attachment.add_header("Content-Disposition", "attachment", filename=filename)
             msg.attach(attachment)
 
-        with smtplib.SMTP(self.smtp_server, self.smtp_port) as smtp:
+        with self.SMTP(self.smtp_server, self.smtp_port) as smtp:
+            print(smtp.has_extn("STARTTLS"))
             if smtp.has_extn("STARTTLS"):
                 smtp.starttls()
             try:
                 smtp.login(self.sender, self.password)
             except Exception as exc:
                 logger.warning(exc)
                 return False
             smtp.sendmail(self.sender, receiver, msg.as_string())
             return True
 
+
 def test_imap():
     try:
         import env  # noqa
     except ModuleNotFoundError:
         pass
     imap_server = os.environ["IMAP_SERVER"]
     mail_addr = os.environ["IMAP_ADDR"]
@@ -155,12 +158,13 @@
         pass
     mail_addr = os.environ["SMTP_ADDR"]
     mail_pwd = os.environ["SMTP_PASS"]
     smtp_server = os.environ["SMTP_SERVER"]
     subject = "Test Email2"
     message = '<span style="color:red">This is a test email.</span>'
     email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=465)
+    # email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=587)
     email_sender.send(subject=subject, message=message, receiver=[os.environ["RECEIVER"]])
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `xenoslib-0.1.27.1/xenoslib/mock.py` & `xenoslib-0.1.27.2/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/onedrive.py` & `xenoslib-0.1.27.2/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/win_trayicon.py` & `xenoslib-0.1.27.2/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.1/xenoslib/windows.py` & `xenoslib-0.1.27.2/xenoslib/windows.py`

 * *Files identical despite different names*

