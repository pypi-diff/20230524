# Comparing `tmp/xenoslib-0.1.27.0.tar.gz` & `tmp/xenoslib-0.1.27.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xenoslib-0.1.27.0.tar", last modified: Tue May 23 06:16:12 2023, max compression
+gzip compressed data, was "xenoslib-0.1.27.1.tar", last modified: Tue May 23 08:08:32 2023, max compression
```

## Comparing `xenoslib-0.1.27.0.tar` & `xenoslib-0.1.27.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:16:12.378028 xenoslib-0.1.27.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 06:16:12.378028 xenoslib-0.1.27.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 06:16:12.378028 xenoslib-0.1.27.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:16:12.378028 xenoslib-0.1.27.0/xenoslib/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/about.py
--rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/dev.py
--rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/extend.py
--rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/linux.py
--rw-r--r--   0 runner    (1001) docker     (123)     4849 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/mail.py
--rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/onedrive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/win_trayicon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-23 06:16:00.000000 xenoslib-0.1.27.0/xenoslib/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 06:16:12.378028 xenoslib-0.1.27.0/xenoslib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 06:16:12.000000 xenoslib-0.1.27.0/xenoslib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 06:16:12.000000 xenoslib-0.1.27.0/xenoslib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 06:16:12.000000 xenoslib-0.1.27.0/xenoslib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 06:16:12.000000 xenoslib-0.1.27.0/xenoslib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 06:16:12.000000 xenoslib-0.1.27.0/xenoslib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3231 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1049 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.522583 xenoslib-0.1.27.1/xenoslib/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/about.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11564 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1236 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/dev.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4942 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/extend.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1318 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/linux.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5521 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/mail.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3572 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7783 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/onedrive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12161 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/win_trayicon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2587 2023-05-23 08:08:18.000000 xenoslib-0.1.27.1/xenoslib/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-23 08:08:32.526583 xenoslib-0.1.27.1/xenoslib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      336 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-23 08:08:32.000000 xenoslib-0.1.27.1/xenoslib.egg-info/top_level.txt
```

### Comparing `xenoslib-0.1.27.0/LICENSE` & `xenoslib-0.1.27.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/README.md` & `xenoslib-0.1.27.1/README.md`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/setup.py` & `xenoslib-0.1.27.1/setup.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/base.py` & `xenoslib-0.1.27.1/xenoslib/base.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/dev.py` & `xenoslib-0.1.27.1/xenoslib/dev.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/extend.py` & `xenoslib-0.1.27.1/xenoslib/extend.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/linux.py` & `xenoslib-0.1.27.1/xenoslib/linux.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/mail.py` & `xenoslib-0.1.27.1/xenoslib/mail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,27 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
+"""
+Description: Utility functions for fetching and sending emails.
+
+Usage:
+from xenoslib.mail import EmailFetcher, EmailSender
+
+# Fetch emails
+for email_data in EmailFetcher(imap_server, mail_addr, mail_pwd, interval=30, days=30):
+    print(email_data["subject"])
+
+# Send email
+sender = EmailSender(smtp_server, sender, password, smtp_port=25)
+sender.send(subject, message, receiver, cc, bcc, filename)
+
+"""
 import os
 import datetime
-from time import sleep
+from time import sleep, time
 import logging
 from collections import deque
 import smtplib
 import email
 from email.mime.text import MIMEText
 from email.header import Header
 from email.mime.application import MIMEApplication
@@ -80,69 +95,72 @@
             client.select_folder("INBOX", readonly=True)
             messages = client.search(["SINCE", date_str])
             emails = client.fetch(messages, ["INTERNALDATE", "BODY.PEEK[]"])
             return emails
 
 
 class SMTPMail:
-    def __init__(self, smtp_server="", sender="", pasword="", smtp_port=25):
+    def __init__(self, smtp_server="", sender="", password="", smtp_port=25):
         self.smtp_server = smtp_server
         self.smtp_port = int(smtp_port)
         self.sender = sender
-        self.pasword = pasword
+        self.password = password
         if self.smtp_port == 25:
             self.SMTP = smtplib.SMTP
         else:
             self.SMTP = smtplib.SMTP_SSL
 
     def send(self, subject, message, receiver=[], cc=[], bcc=[], filename=None):
         msg = MIMEMultipart()
         msg["Subject"] = Header(subject, "utf-8")
         msg["From"] = Header(self.sender, "utf-8")
         msg["To"] = ";".join(receiver)
         msg["Cc"] = ";".join(cc)
+        msg["Message-ID"] = f"<{time()}>"
         receiver.extend(cc)
         receiver.extend(bcc)
         msg.attach(MIMEText(message, "html", "utf-8"))
 
         if filename:
             attachment = MIMEApplication(open(filename, "rb").read())
             attachment.add_header("Content-Disposition", "attachment", filename=filename)
             msg.attach(attachment)
 
-        smtp = self.SMTP(self.smtp_server, self.smtp_port)
-        try:
-            smtp.login(self.sender, self.pasword)
-        except Exception as exc:
-            print(exc)
-            return False
-        smtp.sendmail(self.sender, receiver, msg.as_string())
-        smtp.quit()
-        return True
-
+        with smtplib.SMTP(self.smtp_server, self.smtp_port) as smtp:
+            if smtp.has_extn("STARTTLS"):
+                smtp.starttls()
+            try:
+                smtp.login(self.sender, self.password)
+            except Exception as exc:
+                logger.warning(exc)
+                return False
+            smtp.sendmail(self.sender, receiver, msg.as_string())
+            return True
 
 def test_imap():
     try:
         import env  # noqa
     except ModuleNotFoundError:
         pass
-    imap_server = os.environ["imap_server"]
-    mail_addr = os.environ["imap_addr"]
-    mail_pwd = os.environ["imap_pass"]
+    imap_server = os.environ["IMAP_SERVER"]
+    mail_addr = os.environ["IMAP_ADDR"]
+    mail_pwd = os.environ["IMAP_PASS"]
     for email_data in MailFetcher(imap_server, mail_addr, mail_pwd, interval=1, days=30):
         print(email_data["subject"])
 
 
 def test():
     try:
         import env  # noqa
     except ModuleNotFoundError:
         pass
     mail_addr = os.environ["SMTP_ADDR"]
     mail_pwd = os.environ["SMTP_PASS"]
     smtp_server = os.environ["SMTP_SERVER"]
-    mail = SMTPMail(smtp_server, sender=mail_addr, pasword=mail_pwd, smtp_port=465)
-    mail.send(subject="test", message="test mail", receiver=[os.environ["RECEIVER"]])
+    subject = "Test Email2"
+    message = '<span style="color:red">This is a test email.</span>'
+    email_sender = SMTPMail(smtp_server, sender=mail_addr, password=mail_pwd, smtp_port=465)
+    email_sender.send(subject=subject, message=message, receiver=[os.environ["RECEIVER"]])
 
 
 if __name__ == "__main__":
     test()
```

### Comparing `xenoslib-0.1.27.0/xenoslib/mock.py` & `xenoslib-0.1.27.1/xenoslib/mock.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/onedrive.py` & `xenoslib-0.1.27.1/xenoslib/onedrive.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/win_trayicon.py` & `xenoslib-0.1.27.1/xenoslib/win_trayicon.py`

 * *Files identical despite different names*

### Comparing `xenoslib-0.1.27.0/xenoslib/windows.py` & `xenoslib-0.1.27.1/xenoslib/windows.py`

 * *Files identical despite different names*

