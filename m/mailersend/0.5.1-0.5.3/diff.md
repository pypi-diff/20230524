# Comparing `tmp/mailersend-0.5.1.tar.gz` & `tmp/mailersend-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mailersend-0.5.1.tar", max compression
+gzip compressed data, was "mailersend-0.5.3.tar", max compression
```

## Comparing `mailersend-0.5.1.tar` & `mailersend-0.5.3.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1066 2023-03-03 13:15:16.242614 mailersend-0.5.1/LICENSE
--rw-r--r--   0        0        0    47283 2023-03-03 13:15:16.242614 mailersend-0.5.1/README.md
--rw-r--r--   0        0        0      170 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/__init__.py
--rw-r--r--   0        0        0      871 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/activity/__init__.py
--rw-r--r--   0        0        0     2808 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/analytics/__init__.py
--rw-r--r--   0        0        0        0 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/base/__init__.py
--rw-r--r--   0        0        0     1096 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/base/base.py
--rw-r--r--   0        0        0     3269 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/domains/__init__.py
--rw-r--r--   0        0        0     2406 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/email_verification/__init__.py
--rw-r--r--   0        0        0     3683 2023-03-03 13:15:16.242614 mailersend-0.5.1/mailersend/emails/__init__.py
--rw-r--r--   0        0        0     3554 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/inbound_routing/__init__.py
--rw-r--r--   0        0        0      787 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/messages/__init__.py
--rw-r--r--   0        0        0     7289 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/recipients/__init__.py
--rw-r--r--   0        0        0     1185 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/scheduled_messages/__init__.py
--rw-r--r--   0        0        0     3674 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sender_identities/__init__.py
--rw-r--r--   0        0        0     1840 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_activity/__init__.py
--rw-r--r--   0        0        0     3375 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_inbounds/__init__.py
--rw-r--r--   0        0        0     1147 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_messages/__init__.py
--rw-r--r--   0        0        0     2372 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_phone_numbers/__init__.py
--rw-r--r--   0        0        0     1986 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_recipients/__init__.py
--rw-r--r--   0        0        0     1141 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_sending/__init__.py
--rw-r--r--   0        0        0     2945 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/sms_webhooks/__init__.py
--rw-r--r--   0        0        0     1078 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/templates/__init__.py
--rw-r--r--   0        0        0     1394 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/tokens/__init__.py
--rw-r--r--   0        0        0     1015 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/utils/__init__.py
--rw-r--r--   0        0        0     3205 2023-03-03 13:15:16.246614 mailersend-0.5.1/mailersend/webhooks/__init__.py
--rw-r--r--   0        0        0      464 2023-03-03 13:15:16.246614 mailersend-0.5.1/pyproject.toml
--rw-r--r--   0        0        0    47962 1970-01-01 00:00:00.000000 mailersend-0.5.1/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-05-24 15:00:40.053931 mailersend-0.5.3/LICENSE
+-rw-r--r--   0        0        0    48200 2023-05-24 15:00:40.053931 mailersend-0.5.3/README.md
+-rw-r--r--   0        0        0      170 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/__init__.py
+-rw-r--r--   0        0        0      871 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/activity/__init__.py
+-rw-r--r--   0        0        0     2808 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/analytics/__init__.py
+-rw-r--r--   0        0        0      525 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/api_quota/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/base/__init__.py
+-rw-r--r--   0        0        0     1096 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/base/base.py
+-rw-r--r--   0        0        0     3196 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/domains/__init__.py
+-rw-r--r--   0        0        0     2406 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/email_verification/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/emails/__init__.py
+-rw-r--r--   0        0        0     3554 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/inbound_routing/__init__.py
+-rw-r--r--   0        0        0      787 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/messages/__init__.py
+-rw-r--r--   0        0        0     7289 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/recipients/__init__.py
+-rw-r--r--   0        0        0     1185 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/scheduled_messages/__init__.py
+-rw-r--r--   0        0        0     3674 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/sender_identities/__init__.py
+-rw-r--r--   0        0        0     1840 2023-05-24 15:00:40.053931 mailersend-0.5.3/mailersend/sms_activity/__init__.py
+-rw-r--r--   0        0        0     3375 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_inbounds/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_messages/__init__.py
+-rw-r--r--   0        0        0     2372 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_phone_numbers/__init__.py
+-rw-r--r--   0        0        0     1986 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_recipients/__init__.py
+-rw-r--r--   0        0        0     1141 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_sending/__init__.py
+-rw-r--r--   0        0        0     2945 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/sms_webhooks/__init__.py
+-rw-r--r--   0        0        0     1078 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/templates/__init__.py
+-rw-r--r--   0        0        0     1394 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/tokens/__init__.py
+-rw-r--r--   0        0        0     1015 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/utils/__init__.py
+-rw-r--r--   0        0        0     3205 2023-05-24 15:00:40.057931 mailersend-0.5.3/mailersend/webhooks/__init__.py
+-rw-r--r--   0        0        0      464 2023-05-24 15:00:40.057931 mailersend-0.5.3/pyproject.toml
+-rw-r--r--   0        0        0    48879 1970-01-01 00:00:00.000000 mailersend-0.5.3/PKG-INFO
```

### Comparing `mailersend-0.5.1/LICENSE` & `mailersend-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/README.md` & `mailersend-0.5.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,16 @@
     - [Delete an SMS inbound route](#delete-an-sms-inbound-route)
   - [Sender Identities](#sender-identities)
     - [Get a list of sender identities](#get-a-list-of-sender-identities)
     - [Get a sender identity](#get-a-sender-identity)
     - [Create a sender identity](#create-a-sender-identity)
     - [Update a sender identity](#update-a-sender-identity)
     - [Delete a sender identity](#delete-a-sender-identity)
+  - [API Quota](#api-quota)
+    - [Get API Quota](#get-api-quota)
 - [Troubleshooting](#troubleshooting)
   - [Emails not being sent](#emails-not-being-sent)
 - [Testing](#testing)
 - [Available endpoints](#available-endpoints)
 - [Support and Feedback](#support-and-feedback)
 - [License](#license)
 
@@ -144,15 +146,15 @@
 
 - Python > 3.6.1
 - Python `pip`
 - An API Key from [mailersend.com](https://www.mailersend.com)
 
 ## Authentication
 
-We recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env` file, and use it to store the API key. 
+We recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env` file, and use it to store the API key.
 
 - Using environment variable
 ```python
 from mailersend import emails
 
 # assigning NewEmail() without params defaults to MAILERSEND_API_KEY env var
 mailer = emails.NewEmail()
@@ -707,15 +709,14 @@
 mailer = activity.NewActivity(os.getenv('MAILERSEND_API_KEY'))
 
 page = 1
 limit = 20
 date_from = 1623073576
 date_to = 1623074976
 events = [
-    "processed",
     "queued",
     "sent",
     "delivered",
     "soft-bounced",
     "hard-bounced",
     "junk",
     "opened",
@@ -738,15 +739,14 @@
 load_dotenv()
 
 mailer = analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY'))
 
 date_from = 1623073576
 date_to = 1623074976
 events = [
-    "processed",
     "sent",
 ]
 
 # optional arguments
 domain_id = "domain-id"
 group_by = "days"
 
@@ -868,15 +868,15 @@
     {
         "type": "webhook",
         "value": "https://www.mailersend.com/hook"
     }
 ]
 mailer.set_name("Example route", options)
 mailer.set_domain_enabled(True, options)
-mailer.set_inbound_domain("test.remotecompany.com", options)
+mailer.set_inbound_domain("test.mailersend.com", options)
 mailer.set_catch_filter(_catch_filter, options)
 
 print(mailer.add_inbound_route())
 ```
 
 ### Update an inbound route
 
@@ -910,15 +910,15 @@
     {
         "type": "webhook",
         "value": "https://www.mailersend.com/hook"
     }
 ]
 mailer.set_name("Example route", options)
 mailer.set_domain_enabled(True, options)
-mailer.set_inbound_domain("test.remotecompany.com", options)
+mailer.set_inbound_domain("test.mailersend.com", options)
 mailer.set_catch_filter(_catch_filter, options)
 
 print(mailer.update_inbound_route(route_id))
 ```
 
 ### Delete an inbound route
 
@@ -986,15 +986,21 @@
 from mailersend import domains
 from dotenv import load_dotenv
 
 load_dotenv()
 
 mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
 
-mailer.add_domain("name", "example.com")
+domain_data = {
+    "name": "mydomain.com",
+    "return_path_subdomain": "rpsubdomain",
+    "custom_tracking_subdomain": "ctsubdomain",
+    "inbound_routing_subdomain": "irsubdomain"
+}
+mailer.add_domain("name", domain_data)
 ```
 
 
 ### Delete a domain
 
 ```python
 from mailersend import domains
@@ -1028,15 +1034,28 @@
 from mailersend import domains
 from dotenv import load_dotenv
 
 load_dotenv()
 
 mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
 
-mailer.update_domain_setting("domain-id", "send_paused", True)
+domain_data = {
+    "send_paused": True,
+    "track_clicks": True,
+    "track_opens": True,
+    "track_unsubscribe": True,
+    "track_unsubscribe_html": "<p>Click to <a href='{$unsubscribe}'>unsubscribe</a></p>",
+    "track_unsubscribe_plain": "Click to unsubscribe: {$unsubscribe}",
+    "track_content": True,
+    "custom_tracking_enabled": True,
+    "custom_tracking_subdomain": "email",
+    "precedence_bulk": False
+}
+
+mailer.update_domain_setting("domain-id", domain_data)
 ```
 
 ### Get DNS Records
 
 ```python
 from mailersend import domains
 from dotenv import load_dotenv
@@ -2098,14 +2117,27 @@
 load_dotenv()
 
 mailer = sender_identities.NewSenderIdentity(os.getenv('MAILERSEND_API_KEY'))
 
 print(mailer.delete_identity(identity_id="123456"))
 ```
 
+## API Quota
+### Get API Quota
+```python
+from mailersend import api_quota
+from dotenv import load_dotenv
+
+load_dotenv()
+
+mailer = api_quota.NewApiQuota(os.getenv('MAILERSEND_API_KEY'))
+
+print(mailer.get_quota())
+```
+
 # Troubleshooting
 
 ## Emails not being sent
 
 Print the output of `mailer.send()` to view status code and errors.
 
 ```python
@@ -2140,14 +2172,15 @@
 | SMS Activity      | `{GET} sms-activity`                    | ✅         |
 | SMS Phone numbers | `{GET, PUT, DELETE} sms-numbers`        | ✅         |
 | SMS Recipients    | `{GET, PUT} sms-recipients`             | ✅         |
 | SMS Messages      | `{GET} sms-messages`                    | ✅         |
 | SMS Webhooks      | `{GET, POST, PUT, DELETE} sms-webhooks` | ✅         |
 | SMS Inbounds      | `{GET, POST, PUT, DELETE} sms-inbounds` | ✅         |
 | Sender Identities | `{GET, POST, PUT, DELETE} identities`   | ✅         |
+| API Quota         | `{GET} api-quota`                       | ✅         |
 
 *If, at the moment, some endpoint is not available, please use other available tools to access it. [Refer to official API docs for more info](https://developers.mailersend.com/).*
 
 
 <a name="support-and-feedback"></a>
 # Support and Feedback
```

#### html2text {}

```diff
@@ -76,18 +76,19 @@
 SMS inbound route](#get-a-single-sms-inbound-route) - [Create an SMS inbound
 route](#create-an-sms-inbound-route) - [Update an SMS inbound route](#update-
 an-sms-inbound-route) - [Delete an SMS inbound route](#delete-an-sms-inbound-
 route) - [Sender Identities](#sender-identities) - [Get a list of sender
 identities](#get-a-list-of-sender-identities) - [Get a sender identity](#get-a-
 sender-identity) - [Create a sender identity](#create-a-sender-identity) -
 [Update a sender identity](#update-a-sender-identity) - [Delete a sender
-identity](#delete-a-sender-identity) - [Troubleshooting](#troubleshooting) -
-[Emails not being sent](#emails-not-being-sent) - [Testing](#testing) -
-[Available endpoints](#available-endpoints) - [Support and Feedback](#support-
-and-feedback) - [License](#license)  # Installation ``` $ python -m pip install
+identity](#delete-a-sender-identity) - [API Quota](#api-quota) - [Get API
+Quota](#get-api-quota) - [Troubleshooting](#troubleshooting) - [Emails not
+being sent](#emails-not-being-sent) - [Testing](#testing) - [Available
+endpoints](#available-endpoints) - [Support and Feedback](#support-and-
+feedback) - [License](#license)  # Installation ``` $ python -m pip install
 mailersend ``` ## Requirements - Python > 3.6.1 - Python `pip` - An API Key
 from [mailersend.com](https://www.mailersend.com) ## Authentication We
 recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env`
 file, and use it to store the API key. - Using environment variable ```python
 from mailersend import emails # assigning NewEmail() without params defaults to
 MAILERSEND_API_KEY env var mailer = emails.NewEmail() # define an empty dict to
 populate with mail values mail_body = {} mail_from = { "name": "Your Name",
@@ -218,60 +219,60 @@
 (mailer.get_bulk_status_by_id("bulk-email-id")) ```  ## Activity ### Get a list
 of activities (simple) ```python from mailersend import activity from dotenv
 import load_dotenv load_dotenv() mailer = activity.NewActivity(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_domain_activity("domain-id") ``` ### Get a
 list of activities (full) ```python from mailersend import activity from dotenv
 import load_dotenv load_dotenv() mailer = activity.NewActivity(os.getenv
 ('MAILERSEND_API_KEY')) page = 1 limit = 20 date_from = 1623073576 date_to =
-1623074976 events = [ "processed", "queued", "sent", "delivered", "soft-
-bounced", "hard-bounced", "junk", "opened", "clicked", "unsubscribed",
-"spam_complaints", ] mailer.get_domain_activity("domain-id", page, limit,
-date_from, date_to, events) ``` ## Analytics ### Activity data by date
-```python from mailersend import analytics from dotenv import load_dotenv
-load_dotenv() mailer = analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY'))
-date_from = 1623073576 date_to = 1623074976 events = [ "processed", "sent", ] #
-optional arguments domain_id = "domain-id" group_by = "days"
-mailer.get_activity_by_date(date_from, date_to, events, domain_id, group_by)
-``` ### Opens by country ```python from mailersend import analytics from dotenv
-import load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
-('MAILERSEND_API_KEY')) date_from = 1623073576 date_to = 1623074976 # optional
-arguments domain_id = "domain-id" mailer.get_opens_by_country(date_from,
-date_to, domain_id) ``` ### Opens by user-agent name ```python from mailersend
+1623074976 events = [ "queued", "sent", "delivered", "soft-bounced", "hard-
+bounced", "junk", "opened", "clicked", "unsubscribed", "spam_complaints", ]
+mailer.get_domain_activity("domain-id", page, limit, date_from, date_to,
+events) ``` ## Analytics ### Activity data by date ```python from mailersend
+import analytics from dotenv import load_dotenv load_dotenv() mailer =
+analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from = 1623073576
+date_to = 1623074976 events = [ "sent", ] # optional arguments domain_id =
+"domain-id" group_by = "days" mailer.get_activity_by_date(date_from, date_to,
+events, domain_id, group_by) ``` ### Opens by country ```python from mailersend
 import analytics from dotenv import load_dotenv load_dotenv() mailer =
 analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from = 1623073576
 date_to = 1623074976 # optional arguments domain_id = "domain-id"
-mailer.get_opens_by_user_agent(date_from, date_to, domain_id) ``` ### Opens by
-reading environment ```python from mailersend import analytics from dotenv
-import load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
+mailer.get_opens_by_country(date_from, date_to, domain_id) ``` ### Opens by
+user-agent name ```python from mailersend import analytics from dotenv import
+load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
 ('MAILERSEND_API_KEY')) date_from = 1623073576 date_to = 1623074976 # optional
-arguments domain_id = "domain-id" mailer.get_opens_by_reading_environment
-(date_from, date_to, domain_id) ``` ## Inbound Routes ### Get a list of inbound
-routes ```python from mailersend import inbound_routing from dotenv import
-load_dotenv load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
-('MAILERSEND_API_KEY')) print(mailer.get_inbound_routes()) ``` ### Get a single
-inbound route ```python from mailersend import inbound_routing from dotenv
-import load_dotenv load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
-('MAILERSEND_API_KEY')) print(mailer.get_inbound_by_id("inbound-id")) ``` ###
-Add an inbound route ```python from mailersend import inbound_routing from
-dotenv import load_dotenv load_dotenv() mailer = inbound_routing.NewInbound
-(os.getenv('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
+arguments domain_id = "domain-id" mailer.get_opens_by_user_agent(date_from,
+date_to, domain_id) ``` ### Opens by reading environment ```python from
+mailersend import analytics from dotenv import load_dotenv load_dotenv() mailer
+= analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from =
+1623073576 date_to = 1623074976 # optional arguments domain_id = "domain-id"
+mailer.get_opens_by_reading_environment(date_from, date_to, domain_id) ``` ##
+Inbound Routes ### Get a list of inbound routes ```python from mailersend
+import inbound_routing from dotenv import load_dotenv load_dotenv() mailer =
+inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
+(mailer.get_inbound_routes()) ``` ### Get a single inbound route ```python from
+mailersend import inbound_routing from dotenv import load_dotenv load_dotenv()
+mailer = inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
+(mailer.get_inbound_by_id("inbound-id")) ``` ### Add an inbound route ```python
+from mailersend import inbound_routing from dotenv import load_dotenv
+load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
+('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
 "catch_recipient", "filters": [ { "comparer": "equal", "value": "test" } ] }
 _match_filter = { "type": "match_all" } _forwards = [ { "type": "webhook",
 "value": "https://www.mailersend.com/hook" } ] mailer.set_name("Example route",
 options) mailer.set_domain_enabled(True, options) mailer.set_inbound_domain
-("test.remotecompany.com", options) mailer.set_catch_filter(_catch_filter,
+("test.mailersend.com", options) mailer.set_catch_filter(_catch_filter,
 options) print(mailer.add_inbound_route()) ``` ### Update an inbound route
 ```python from mailersend import inbound_routing from dotenv import load_dotenv
 load_dotenv() route_id = "inbound-route-id" mailer = inbound_routing.NewInbound
 (os.getenv('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
 "catch_recipient", "filters": [ { "comparer": "equal", "value": "test" } ] }
 _match_filter = { "type": "match_all" } _forwards = [ { "type": "webhook",
 "value": "https://www.mailersend.com/hook" } ] mailer.set_name("Example route",
 options) mailer.set_domain_enabled(True, options) mailer.set_inbound_domain
-("test.remotecompany.com", options) mailer.set_catch_filter(_catch_filter,
+("test.mailersend.com", options) mailer.set_catch_filter(_catch_filter,
 options) print(mailer.update_inbound_route(route_id)) ``` ### Delete an inbound
 route ```python from mailersend import inbound_routing from dotenv import
 load_dotenv load_dotenv() route_id = "inbound-route-id" mailer =
 inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.delete_inbound_route(route_id)) ``` ## Domains ### Get a list of
 domains ```python from mailersend import domains from dotenv import load_dotenv
 load_dotenv() mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
@@ -283,36 +284,44 @@
 load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
 ('MAILERSEND_API_KEY')) helper = utils.NewHelper(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_domain_by_id(helper.get_id_by_name
 ("domains","domain-name")) ``` ### Add a domain You can find a full list of
 settings [here](https://developers.mailersend.com/api/v1/domains.html#request-
 parameters-3). ```python from mailersend import domains from dotenv import
 load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
-('MAILERSEND_API_KEY')) mailer.add_domain("name", "example.com") ``` ### Delete
-a domain ```python from mailersend import domains from dotenv import
-load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
-('MAILERSEND_API_KEY')) mailer.delete_domain("domain-id") ``` ### Get a list of
-recipients per domain ```python from mailersend import domains from dotenv
-import load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
+('MAILERSEND_API_KEY')) domain_data = { "name": "mydomain.com",
+"return_path_subdomain": "rpsubdomain", "custom_tracking_subdomain":
+"ctsubdomain", "inbound_routing_subdomain": "irsubdomain" } mailer.add_domain
+("name", domain_data) ``` ### Delete a domain ```python from mailersend import
+domains from dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain
+(os.getenv('MAILERSEND_API_KEY')) mailer.delete_domain("domain-id") ``` ### Get
+a list of recipients per domain ```python from mailersend import domains from
+dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_recipients_for_domain("domain-id") ``` ###
 Update domain settings You can find a full list of settings [here](https://
 developers.mailersend.com/api/v1/domains.html#request-body). ```python from
 mailersend import domains from dotenv import load_dotenv load_dotenv() mailer =
-domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.update_domain_setting
-("domain-id", "send_paused", True) ``` ### Get DNS Records ```python from
+domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) domain_data =
+{ "send_paused": True, "track_clicks": True, "track_opens": True,
+"track_unsubscribe": True, "track_unsubscribe_html": "
+Click to unsubscribe
+", "track_unsubscribe_plain": "Click to unsubscribe: {$unsubscribe}",
+"track_content": True, "custom_tracking_enabled": True,
+"custom_tracking_subdomain": "email", "precedence_bulk": False }
+mailer.update_domain_setting("domain-id", domain_data) ``` ### Get DNS Records
+```python from mailersend import domains from dotenv import load_dotenv
+load_dotenv() mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
+mailer.get_dns_records("domain-id") ``` ### Verify a domain ```python from
 mailersend import domains from dotenv import load_dotenv load_dotenv() mailer =
-domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.get_dns_records
-("domain-id") ``` ### Verify a domain ```python from mailersend import domains
-from dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain
-(os.getenv('MAILERSEND_API_KEY')) mailer.verify_domain("domain-id") ``` ##
-Messages ### Get a list of messages ```python from mailersend import messages
-from dotenv import load_dotenv load_dotenv() mailer = messages.NewMessage
-(os.getenv('MAILERSEND_API_KEY')) mailer.get_messages() ``` ### Get a single
-message ```python from mailersend import messages from dotenv import
-load_dotenv load_dotenv() mailer = messages.NewMessage(os.getenv
+domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.verify_domain
+("domain-id") ``` ## Messages ### Get a list of messages ```python from
+mailersend import messages from dotenv import load_dotenv load_dotenv() mailer
+= messages.NewMessage(os.getenv('MAILERSEND_API_KEY')) mailer.get_messages()
+``` ### Get a single message ```python from mailersend import messages from
+dotenv import load_dotenv load_dotenv() mailer = messages.NewMessage(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_message_by_id("message-id") ``` ## Scheduled
 messages ### Get a list of scheduled messages ```python from mailersend import
 scheduled_messages from dotenv import load_dotenv load_dotenv() mailer =
 scheduled_messages.NewMessageSchedule(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.get_scheduled_messages()) ``` ### Get a single scheduled message
 ```python from mailersend import scheduled_messages from dotenv import
 load_dotenv load_dotenv() mailer = scheduled_messages.NewMessageSchedule
@@ -567,32 +576,35 @@
 sender_identities.NewSenderIdentity(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.update_identity( identity_id="123456", domain_id="123456", name="Abe
 Doe", email="email@mydomain.com", reply_to_email="reply@mydomain.com",
 reply_to_name="Doe Abe", add_note=False )) ``` ### Delete a sender identity
 ```python from mailersend import sender_identities from dotenv import
 load_dotenv load_dotenv() mailer = sender_identities.NewSenderIdentity
 (os.getenv('MAILERSEND_API_KEY')) print(mailer.delete_identity
-(identity_id="123456")) ``` # Troubleshooting ## Emails not being sent Print
-the output of `mailer.send()` to view status code and errors. ```python from
-mailersend import emails mailer = emails.NewEmail() mail_body = {} print
-(mailer.send(mail_body)) ``` # Testing TBD  # Available endpoints | Feature
-group | Endpoint | Available | |-------------------|---------------------------
---------------|-----------| | Activity | `GET activity` | â | | Analytics |
-`GET analytics` | â | | Domains | `{GET, PUT, DELETE} domains` | â | |
-Emails | `POST send` | â | | Messages | `GET messages` | â | | Recipients |
-`{GET, DELETE} recipients` | â | | Templates | `{GET, DELETE} templates` |
-â | | Tokens | `{POST, PUT, DELETE} tokens` | â | | Webhooks | `{GET, POST,
-PUT, DELETE} webhooks` | â | | SMS Sending | `{POST} sms` | â | | SMS
-Activity | `{GET} sms-activity` | â | | SMS Phone numbers | `{GET, PUT,
-DELETE} sms-numbers` | â | | SMS Recipients | `{GET, PUT} sms-recipients` |
-â | | SMS Messages | `{GET} sms-messages` | â | | SMS Webhooks | `{GET,
-POST, PUT, DELETE} sms-webhooks` | â | | SMS Inbounds | `{GET, POST, PUT,
-DELETE} sms-inbounds` | â | | Sender Identities | `{GET, POST, PUT, DELETE}
-identities` | â | *If, at the moment, some endpoint is not available, please
-use other available tools to access it. [Refer to official API docs for more
-info](https://developers.mailersend.com/).*  # Support and Feedback In case you
-find any bugs, submit an issue directly here in GitHub. You are welcome to
-create SDK for any other programming language. If you have any troubles using
-our API or SDK free to contact our support by email [info@mailersend.com]
-(mailto:info@mailersend.com) The official documentation is at [https://
-developers.mailersend.com](https://developers.mailersend.com)  # License [The
-MIT License (MIT)](LICENSE)
+(identity_id="123456")) ``` ## API Quota ### Get API Quota ```python from
+mailersend import api_quota from dotenv import load_dotenv load_dotenv() mailer
+= api_quota.NewApiQuota(os.getenv('MAILERSEND_API_KEY')) print(mailer.get_quota
+()) ``` # Troubleshooting ## Emails not being sent Print the output of
+`mailer.send()` to view status code and errors. ```python from mailersend
+import emails mailer = emails.NewEmail() mail_body = {} print(mailer.send
+(mail_body)) ``` # Testing TBD  # Available endpoints | Feature group |
+Endpoint | Available | |-------------------|-----------------------------------
+------|-----------| | Activity | `GET activity` | â | | Analytics | `GET
+analytics` | â | | Domains | `{GET, PUT, DELETE} domains` | â | | Emails |
+`POST send` | â | | Messages | `GET messages` | â | | Recipients | `{GET,
+DELETE} recipients` | â | | Templates | `{GET, DELETE} templates` | â | |
+Tokens | `{POST, PUT, DELETE} tokens` | â | | Webhooks | `{GET, POST, PUT,
+DELETE} webhooks` | â | | SMS Sending | `{POST} sms` | â | | SMS Activity |
+`{GET} sms-activity` | â | | SMS Phone numbers | `{GET, PUT, DELETE} sms-
+numbers` | â | | SMS Recipients | `{GET, PUT} sms-recipients` | â | | SMS
+Messages | `{GET} sms-messages` | â | | SMS Webhooks | `{GET, POST, PUT,
+DELETE} sms-webhooks` | â | | SMS Inbounds | `{GET, POST, PUT, DELETE} sms-
+inbounds` | â | | Sender Identities | `{GET, POST, PUT, DELETE} identities` |
+â | | API Quota | `{GET} api-quota` | â | *If, at the moment, some endpoint
+is not available, please use other available tools to access it. [Refer to
+official API docs for more info](https://developers.mailersend.com/).*  #
+Support and Feedback In case you find any bugs, submit an issue directly here
+in GitHub. You are welcome to create SDK for any other programming language. If
+you have any troubles using our API or SDK free to contact our support by email
+[info@mailersend.com](mailto:info@mailersend.com) The official documentation is
+at [https://developers.mailersend.com](https://developers.mailersend.com)  #
+License [The MIT License (MIT)](LICENSE)
```

### Comparing `mailersend-0.5.1/mailersend/activity/__init__.py` & `mailersend-0.5.3/mailersend/activity/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/analytics/__init__.py` & `mailersend-0.5.3/mailersend/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/base/base.py` & `mailersend-0.5.3/mailersend/base/base.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/domains/__init__.py` & `mailersend-0.5.3/mailersend/domains/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -33,29 +33,27 @@
         Returns the JSON response of MailerSend API
         """
         request = requests.get(
             f"{self.api_base}/domains/{domain_id}", headers=self.headers_default
         )
         return request.text
 
-    def add_domain(self, key, value):
+    def add_domain(self, domain_data):
         """
         Add a domain
 
         @params:
-          key (str): A key option to add
-          value (str): The respective value of key to add
+          domain_data (dic): Contains key:value data needed for creating a new domain
 
         """
-        data = {f"{key}": value}
 
         request = requests.post(
             f"{self.api_base}/domains",
             headers=self.headers_default,
-            json=data,
+            json=domain_data,
         )
         return request.text
 
     def delete_domain(self, domain_id):
         """
         Delete a domain
 
@@ -80,30 +78,27 @@
         """
         request = requests.get(
             f"{self.api_base}/domains/{domain_id}/recipients",
             headers=self.headers_default,
         )
         return request.text
 
-    def update_domain_setting(self, domain_id, key, value):
+    def update_domain_setting(self, domain_id, domain_data):
         """
         Returns the JSON response of MailerSend API
 
         @params:
           domain_id (str): A domain ID
-          key (str): An key option to update
-          value (str): The respective value of key to update
+          domain_data (dict): A key:value list that contains parameters for updating domain name
 
         """
-        data = {f"{key}": value}
-
         request = requests.put(
             f"{self.api_base}/domains/{domain_id}/settings",
             headers=self.headers_default,
-            json=data,
+            json=domain_data,
         )
         return request.text
 
     def get_dns_records(self, domain_id):
         """
         Returns the JSON response of dns records
```

### Comparing `mailersend-0.5.1/mailersend/email_verification/__init__.py` & `mailersend-0.5.3/mailersend/email_verification/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/emails/__init__.py` & `mailersend-0.5.3/mailersend/emails/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/inbound_routing/__init__.py` & `mailersend-0.5.3/mailersend/inbound_routing/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/messages/__init__.py` & `mailersend-0.5.3/mailersend/messages/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/recipients/__init__.py` & `mailersend-0.5.3/mailersend/recipients/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/scheduled_messages/__init__.py` & `mailersend-0.5.3/mailersend/scheduled_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sender_identities/__init__.py` & `mailersend-0.5.3/mailersend/sender_identities/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_activity/__init__.py` & `mailersend-0.5.3/mailersend/sms_activity/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_inbounds/__init__.py` & `mailersend-0.5.3/mailersend/sms_inbounds/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_messages/__init__.py` & `mailersend-0.5.3/mailersend/sms_messages/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_phone_numbers/__init__.py` & `mailersend-0.5.3/mailersend/sms_phone_numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_recipients/__init__.py` & `mailersend-0.5.3/mailersend/sms_recipients/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_sending/__init__.py` & `mailersend-0.5.3/mailersend/sms_sending/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/sms_webhooks/__init__.py` & `mailersend-0.5.3/mailersend/sms_webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/templates/__init__.py` & `mailersend-0.5.3/mailersend/templates/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/tokens/__init__.py` & `mailersend-0.5.3/mailersend/tokens/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/utils/__init__.py` & `mailersend-0.5.3/mailersend/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/mailersend/webhooks/__init__.py` & `mailersend-0.5.3/mailersend/webhooks/__init__.py`

 * *Files identical despite different names*

### Comparing `mailersend-0.5.1/PKG-INFO` & `mailersend-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mailersend
-Version: 0.5.1
+Version: 0.5.3
 Summary: The official MailerSend Python SDK
 Keywords: mailersend,mail
 Author: Igor Hrček
 Author-email: igor@mailerlite.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
@@ -140,14 +140,16 @@
     - [Delete an SMS inbound route](#delete-an-sms-inbound-route)
   - [Sender Identities](#sender-identities)
     - [Get a list of sender identities](#get-a-list-of-sender-identities)
     - [Get a sender identity](#get-a-sender-identity)
     - [Create a sender identity](#create-a-sender-identity)
     - [Update a sender identity](#update-a-sender-identity)
     - [Delete a sender identity](#delete-a-sender-identity)
+  - [API Quota](#api-quota)
+    - [Get API Quota](#get-api-quota)
 - [Troubleshooting](#troubleshooting)
   - [Emails not being sent](#emails-not-being-sent)
 - [Testing](#testing)
 - [Available endpoints](#available-endpoints)
 - [Support and Feedback](#support-and-feedback)
 - [License](#license)
 
@@ -163,15 +165,15 @@
 
 - Python > 3.6.1
 - Python `pip`
 - An API Key from [mailersend.com](https://www.mailersend.com)
 
 ## Authentication
 
-We recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env` file, and use it to store the API key. 
+We recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env` file, and use it to store the API key.
 
 - Using environment variable
 ```python
 from mailersend import emails
 
 # assigning NewEmail() without params defaults to MAILERSEND_API_KEY env var
 mailer = emails.NewEmail()
@@ -726,15 +728,14 @@
 mailer = activity.NewActivity(os.getenv('MAILERSEND_API_KEY'))
 
 page = 1
 limit = 20
 date_from = 1623073576
 date_to = 1623074976
 events = [
-    "processed",
     "queued",
     "sent",
     "delivered",
     "soft-bounced",
     "hard-bounced",
     "junk",
     "opened",
@@ -757,15 +758,14 @@
 load_dotenv()
 
 mailer = analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY'))
 
 date_from = 1623073576
 date_to = 1623074976
 events = [
-    "processed",
     "sent",
 ]
 
 # optional arguments
 domain_id = "domain-id"
 group_by = "days"
 
@@ -887,15 +887,15 @@
     {
         "type": "webhook",
         "value": "https://www.mailersend.com/hook"
     }
 ]
 mailer.set_name("Example route", options)
 mailer.set_domain_enabled(True, options)
-mailer.set_inbound_domain("test.remotecompany.com", options)
+mailer.set_inbound_domain("test.mailersend.com", options)
 mailer.set_catch_filter(_catch_filter, options)
 
 print(mailer.add_inbound_route())
 ```
 
 ### Update an inbound route
 
@@ -929,15 +929,15 @@
     {
         "type": "webhook",
         "value": "https://www.mailersend.com/hook"
     }
 ]
 mailer.set_name("Example route", options)
 mailer.set_domain_enabled(True, options)
-mailer.set_inbound_domain("test.remotecompany.com", options)
+mailer.set_inbound_domain("test.mailersend.com", options)
 mailer.set_catch_filter(_catch_filter, options)
 
 print(mailer.update_inbound_route(route_id))
 ```
 
 ### Delete an inbound route
 
@@ -1005,15 +1005,21 @@
 from mailersend import domains
 from dotenv import load_dotenv
 
 load_dotenv()
 
 mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
 
-mailer.add_domain("name", "example.com")
+domain_data = {
+    "name": "mydomain.com",
+    "return_path_subdomain": "rpsubdomain",
+    "custom_tracking_subdomain": "ctsubdomain",
+    "inbound_routing_subdomain": "irsubdomain"
+}
+mailer.add_domain("name", domain_data)
 ```
 
 
 ### Delete a domain
 
 ```python
 from mailersend import domains
@@ -1047,15 +1053,28 @@
 from mailersend import domains
 from dotenv import load_dotenv
 
 load_dotenv()
 
 mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
 
-mailer.update_domain_setting("domain-id", "send_paused", True)
+domain_data = {
+    "send_paused": True,
+    "track_clicks": True,
+    "track_opens": True,
+    "track_unsubscribe": True,
+    "track_unsubscribe_html": "<p>Click to <a href='{$unsubscribe}'>unsubscribe</a></p>",
+    "track_unsubscribe_plain": "Click to unsubscribe: {$unsubscribe}",
+    "track_content": True,
+    "custom_tracking_enabled": True,
+    "custom_tracking_subdomain": "email",
+    "precedence_bulk": False
+}
+
+mailer.update_domain_setting("domain-id", domain_data)
 ```
 
 ### Get DNS Records
 
 ```python
 from mailersend import domains
 from dotenv import load_dotenv
@@ -2117,14 +2136,27 @@
 load_dotenv()
 
 mailer = sender_identities.NewSenderIdentity(os.getenv('MAILERSEND_API_KEY'))
 
 print(mailer.delete_identity(identity_id="123456"))
 ```
 
+## API Quota
+### Get API Quota
+```python
+from mailersend import api_quota
+from dotenv import load_dotenv
+
+load_dotenv()
+
+mailer = api_quota.NewApiQuota(os.getenv('MAILERSEND_API_KEY'))
+
+print(mailer.get_quota())
+```
+
 # Troubleshooting
 
 ## Emails not being sent
 
 Print the output of `mailer.send()` to view status code and errors.
 
 ```python
@@ -2159,14 +2191,15 @@
 | SMS Activity      | `{GET} sms-activity`                    | ✅         |
 | SMS Phone numbers | `{GET, PUT, DELETE} sms-numbers`        | ✅         |
 | SMS Recipients    | `{GET, PUT} sms-recipients`             | ✅         |
 | SMS Messages      | `{GET} sms-messages`                    | ✅         |
 | SMS Webhooks      | `{GET, POST, PUT, DELETE} sms-webhooks` | ✅         |
 | SMS Inbounds      | `{GET, POST, PUT, DELETE} sms-inbounds` | ✅         |
 | Sender Identities | `{GET, POST, PUT, DELETE} identities`   | ✅         |
+| API Quota         | `{GET} api-quota`                       | ✅         |
 
 *If, at the moment, some endpoint is not available, please use other available tools to access it. [Refer to official API docs for more info](https://developers.mailersend.com/).*
 
 
 <a name="support-and-feedback"></a>
 # Support and Feedback
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: mailersend Version: 0.5.1 Summary: The official
+Metadata-Version: 2.1 Name: mailersend Version: 0.5.3 Summary: The official
 MailerSend Python SDK Keywords: mailersend,mail Author: Igor HrÄek Author-
 email: igor@mailerlite.com Requires-Python: >=3.7,<4.0 Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Requires-Dist: pre-commit
 (>=2.12.1,<3.0.0) Requires-Dist: requests (>=2.25.0,<3.0.0) Requires-Dist:
@@ -85,18 +85,19 @@
 SMS inbound route](#get-a-single-sms-inbound-route) - [Create an SMS inbound
 route](#create-an-sms-inbound-route) - [Update an SMS inbound route](#update-
 an-sms-inbound-route) - [Delete an SMS inbound route](#delete-an-sms-inbound-
 route) - [Sender Identities](#sender-identities) - [Get a list of sender
 identities](#get-a-list-of-sender-identities) - [Get a sender identity](#get-a-
 sender-identity) - [Create a sender identity](#create-a-sender-identity) -
 [Update a sender identity](#update-a-sender-identity) - [Delete a sender
-identity](#delete-a-sender-identity) - [Troubleshooting](#troubleshooting) -
-[Emails not being sent](#emails-not-being-sent) - [Testing](#testing) -
-[Available endpoints](#available-endpoints) - [Support and Feedback](#support-
-and-feedback) - [License](#license)  # Installation ``` $ python -m pip install
+identity](#delete-a-sender-identity) - [API Quota](#api-quota) - [Get API
+Quota](#get-api-quota) - [Troubleshooting](#troubleshooting) - [Emails not
+being sent](#emails-not-being-sent) - [Testing](#testing) - [Available
+endpoints](#available-endpoints) - [Support and Feedback](#support-and-
+feedback) - [License](#license)  # Installation ``` $ python -m pip install
 mailersend ``` ## Requirements - Python > 3.6.1 - Python `pip` - An API Key
 from [mailersend.com](https://www.mailersend.com) ## Authentication We
 recommend you to define `MAILERSEND_API_KEY` environment variable in the `.env`
 file, and use it to store the API key. - Using environment variable ```python
 from mailersend import emails # assigning NewEmail() without params defaults to
 MAILERSEND_API_KEY env var mailer = emails.NewEmail() # define an empty dict to
 populate with mail values mail_body = {} mail_from = { "name": "Your Name",
@@ -227,60 +228,60 @@
 (mailer.get_bulk_status_by_id("bulk-email-id")) ```  ## Activity ### Get a list
 of activities (simple) ```python from mailersend import activity from dotenv
 import load_dotenv load_dotenv() mailer = activity.NewActivity(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_domain_activity("domain-id") ``` ### Get a
 list of activities (full) ```python from mailersend import activity from dotenv
 import load_dotenv load_dotenv() mailer = activity.NewActivity(os.getenv
 ('MAILERSEND_API_KEY')) page = 1 limit = 20 date_from = 1623073576 date_to =
-1623074976 events = [ "processed", "queued", "sent", "delivered", "soft-
-bounced", "hard-bounced", "junk", "opened", "clicked", "unsubscribed",
-"spam_complaints", ] mailer.get_domain_activity("domain-id", page, limit,
-date_from, date_to, events) ``` ## Analytics ### Activity data by date
-```python from mailersend import analytics from dotenv import load_dotenv
-load_dotenv() mailer = analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY'))
-date_from = 1623073576 date_to = 1623074976 events = [ "processed", "sent", ] #
-optional arguments domain_id = "domain-id" group_by = "days"
-mailer.get_activity_by_date(date_from, date_to, events, domain_id, group_by)
-``` ### Opens by country ```python from mailersend import analytics from dotenv
-import load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
-('MAILERSEND_API_KEY')) date_from = 1623073576 date_to = 1623074976 # optional
-arguments domain_id = "domain-id" mailer.get_opens_by_country(date_from,
-date_to, domain_id) ``` ### Opens by user-agent name ```python from mailersend
+1623074976 events = [ "queued", "sent", "delivered", "soft-bounced", "hard-
+bounced", "junk", "opened", "clicked", "unsubscribed", "spam_complaints", ]
+mailer.get_domain_activity("domain-id", page, limit, date_from, date_to,
+events) ``` ## Analytics ### Activity data by date ```python from mailersend
+import analytics from dotenv import load_dotenv load_dotenv() mailer =
+analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from = 1623073576
+date_to = 1623074976 events = [ "sent", ] # optional arguments domain_id =
+"domain-id" group_by = "days" mailer.get_activity_by_date(date_from, date_to,
+events, domain_id, group_by) ``` ### Opens by country ```python from mailersend
 import analytics from dotenv import load_dotenv load_dotenv() mailer =
 analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from = 1623073576
 date_to = 1623074976 # optional arguments domain_id = "domain-id"
-mailer.get_opens_by_user_agent(date_from, date_to, domain_id) ``` ### Opens by
-reading environment ```python from mailersend import analytics from dotenv
-import load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
+mailer.get_opens_by_country(date_from, date_to, domain_id) ``` ### Opens by
+user-agent name ```python from mailersend import analytics from dotenv import
+load_dotenv load_dotenv() mailer = analytics.NewAnalytics(os.getenv
 ('MAILERSEND_API_KEY')) date_from = 1623073576 date_to = 1623074976 # optional
-arguments domain_id = "domain-id" mailer.get_opens_by_reading_environment
-(date_from, date_to, domain_id) ``` ## Inbound Routes ### Get a list of inbound
-routes ```python from mailersend import inbound_routing from dotenv import
-load_dotenv load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
-('MAILERSEND_API_KEY')) print(mailer.get_inbound_routes()) ``` ### Get a single
-inbound route ```python from mailersend import inbound_routing from dotenv
-import load_dotenv load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
-('MAILERSEND_API_KEY')) print(mailer.get_inbound_by_id("inbound-id")) ``` ###
-Add an inbound route ```python from mailersend import inbound_routing from
-dotenv import load_dotenv load_dotenv() mailer = inbound_routing.NewInbound
-(os.getenv('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
+arguments domain_id = "domain-id" mailer.get_opens_by_user_agent(date_from,
+date_to, domain_id) ``` ### Opens by reading environment ```python from
+mailersend import analytics from dotenv import load_dotenv load_dotenv() mailer
+= analytics.NewAnalytics(os.getenv('MAILERSEND_API_KEY')) date_from =
+1623073576 date_to = 1623074976 # optional arguments domain_id = "domain-id"
+mailer.get_opens_by_reading_environment(date_from, date_to, domain_id) ``` ##
+Inbound Routes ### Get a list of inbound routes ```python from mailersend
+import inbound_routing from dotenv import load_dotenv load_dotenv() mailer =
+inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
+(mailer.get_inbound_routes()) ``` ### Get a single inbound route ```python from
+mailersend import inbound_routing from dotenv import load_dotenv load_dotenv()
+mailer = inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
+(mailer.get_inbound_by_id("inbound-id")) ``` ### Add an inbound route ```python
+from mailersend import inbound_routing from dotenv import load_dotenv
+load_dotenv() mailer = inbound_routing.NewInbound(os.getenv
+('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
 "catch_recipient", "filters": [ { "comparer": "equal", "value": "test" } ] }
 _match_filter = { "type": "match_all" } _forwards = [ { "type": "webhook",
 "value": "https://www.mailersend.com/hook" } ] mailer.set_name("Example route",
 options) mailer.set_domain_enabled(True, options) mailer.set_inbound_domain
-("test.remotecompany.com", options) mailer.set_catch_filter(_catch_filter,
+("test.mailersend.com", options) mailer.set_catch_filter(_catch_filter,
 options) print(mailer.add_inbound_route()) ``` ### Update an inbound route
 ```python from mailersend import inbound_routing from dotenv import load_dotenv
 load_dotenv() route_id = "inbound-route-id" mailer = inbound_routing.NewInbound
 (os.getenv('MAILERSEND_API_KEY')) options = {} _catch_filter = { "type":
 "catch_recipient", "filters": [ { "comparer": "equal", "value": "test" } ] }
 _match_filter = { "type": "match_all" } _forwards = [ { "type": "webhook",
 "value": "https://www.mailersend.com/hook" } ] mailer.set_name("Example route",
 options) mailer.set_domain_enabled(True, options) mailer.set_inbound_domain
-("test.remotecompany.com", options) mailer.set_catch_filter(_catch_filter,
+("test.mailersend.com", options) mailer.set_catch_filter(_catch_filter,
 options) print(mailer.update_inbound_route(route_id)) ``` ### Delete an inbound
 route ```python from mailersend import inbound_routing from dotenv import
 load_dotenv load_dotenv() route_id = "inbound-route-id" mailer =
 inbound_routing.NewInbound(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.delete_inbound_route(route_id)) ``` ## Domains ### Get a list of
 domains ```python from mailersend import domains from dotenv import load_dotenv
 load_dotenv() mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
@@ -292,36 +293,44 @@
 load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
 ('MAILERSEND_API_KEY')) helper = utils.NewHelper(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_domain_by_id(helper.get_id_by_name
 ("domains","domain-name")) ``` ### Add a domain You can find a full list of
 settings [here](https://developers.mailersend.com/api/v1/domains.html#request-
 parameters-3). ```python from mailersend import domains from dotenv import
 load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
-('MAILERSEND_API_KEY')) mailer.add_domain("name", "example.com") ``` ### Delete
-a domain ```python from mailersend import domains from dotenv import
-load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
-('MAILERSEND_API_KEY')) mailer.delete_domain("domain-id") ``` ### Get a list of
-recipients per domain ```python from mailersend import domains from dotenv
-import load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
+('MAILERSEND_API_KEY')) domain_data = { "name": "mydomain.com",
+"return_path_subdomain": "rpsubdomain", "custom_tracking_subdomain":
+"ctsubdomain", "inbound_routing_subdomain": "irsubdomain" } mailer.add_domain
+("name", domain_data) ``` ### Delete a domain ```python from mailersend import
+domains from dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain
+(os.getenv('MAILERSEND_API_KEY')) mailer.delete_domain("domain-id") ``` ### Get
+a list of recipients per domain ```python from mailersend import domains from
+dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_recipients_for_domain("domain-id") ``` ###
 Update domain settings You can find a full list of settings [here](https://
 developers.mailersend.com/api/v1/domains.html#request-body). ```python from
 mailersend import domains from dotenv import load_dotenv load_dotenv() mailer =
-domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.update_domain_setting
-("domain-id", "send_paused", True) ``` ### Get DNS Records ```python from
+domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) domain_data =
+{ "send_paused": True, "track_clicks": True, "track_opens": True,
+"track_unsubscribe": True, "track_unsubscribe_html": "
+Click to unsubscribe
+", "track_unsubscribe_plain": "Click to unsubscribe: {$unsubscribe}",
+"track_content": True, "custom_tracking_enabled": True,
+"custom_tracking_subdomain": "email", "precedence_bulk": False }
+mailer.update_domain_setting("domain-id", domain_data) ``` ### Get DNS Records
+```python from mailersend import domains from dotenv import load_dotenv
+load_dotenv() mailer = domains.NewDomain(os.getenv('MAILERSEND_API_KEY'))
+mailer.get_dns_records("domain-id") ``` ### Verify a domain ```python from
 mailersend import domains from dotenv import load_dotenv load_dotenv() mailer =
-domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.get_dns_records
-("domain-id") ``` ### Verify a domain ```python from mailersend import domains
-from dotenv import load_dotenv load_dotenv() mailer = domains.NewDomain
-(os.getenv('MAILERSEND_API_KEY')) mailer.verify_domain("domain-id") ``` ##
-Messages ### Get a list of messages ```python from mailersend import messages
-from dotenv import load_dotenv load_dotenv() mailer = messages.NewMessage
-(os.getenv('MAILERSEND_API_KEY')) mailer.get_messages() ``` ### Get a single
-message ```python from mailersend import messages from dotenv import
-load_dotenv load_dotenv() mailer = messages.NewMessage(os.getenv
+domains.NewDomain(os.getenv('MAILERSEND_API_KEY')) mailer.verify_domain
+("domain-id") ``` ## Messages ### Get a list of messages ```python from
+mailersend import messages from dotenv import load_dotenv load_dotenv() mailer
+= messages.NewMessage(os.getenv('MAILERSEND_API_KEY')) mailer.get_messages()
+``` ### Get a single message ```python from mailersend import messages from
+dotenv import load_dotenv load_dotenv() mailer = messages.NewMessage(os.getenv
 ('MAILERSEND_API_KEY')) mailer.get_message_by_id("message-id") ``` ## Scheduled
 messages ### Get a list of scheduled messages ```python from mailersend import
 scheduled_messages from dotenv import load_dotenv load_dotenv() mailer =
 scheduled_messages.NewMessageSchedule(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.get_scheduled_messages()) ``` ### Get a single scheduled message
 ```python from mailersend import scheduled_messages from dotenv import
 load_dotenv load_dotenv() mailer = scheduled_messages.NewMessageSchedule
@@ -576,32 +585,35 @@
 sender_identities.NewSenderIdentity(os.getenv('MAILERSEND_API_KEY')) print
 (mailer.update_identity( identity_id="123456", domain_id="123456", name="Abe
 Doe", email="email@mydomain.com", reply_to_email="reply@mydomain.com",
 reply_to_name="Doe Abe", add_note=False )) ``` ### Delete a sender identity
 ```python from mailersend import sender_identities from dotenv import
 load_dotenv load_dotenv() mailer = sender_identities.NewSenderIdentity
 (os.getenv('MAILERSEND_API_KEY')) print(mailer.delete_identity
-(identity_id="123456")) ``` # Troubleshooting ## Emails not being sent Print
-the output of `mailer.send()` to view status code and errors. ```python from
-mailersend import emails mailer = emails.NewEmail() mail_body = {} print
-(mailer.send(mail_body)) ``` # Testing TBD  # Available endpoints | Feature
-group | Endpoint | Available | |-------------------|---------------------------
---------------|-----------| | Activity | `GET activity` | â | | Analytics |
-`GET analytics` | â | | Domains | `{GET, PUT, DELETE} domains` | â | |
-Emails | `POST send` | â | | Messages | `GET messages` | â | | Recipients |
-`{GET, DELETE} recipients` | â | | Templates | `{GET, DELETE} templates` |
-â | | Tokens | `{POST, PUT, DELETE} tokens` | â | | Webhooks | `{GET, POST,
-PUT, DELETE} webhooks` | â | | SMS Sending | `{POST} sms` | â | | SMS
-Activity | `{GET} sms-activity` | â | | SMS Phone numbers | `{GET, PUT,
-DELETE} sms-numbers` | â | | SMS Recipients | `{GET, PUT} sms-recipients` |
-â | | SMS Messages | `{GET} sms-messages` | â | | SMS Webhooks | `{GET,
-POST, PUT, DELETE} sms-webhooks` | â | | SMS Inbounds | `{GET, POST, PUT,
-DELETE} sms-inbounds` | â | | Sender Identities | `{GET, POST, PUT, DELETE}
-identities` | â | *If, at the moment, some endpoint is not available, please
-use other available tools to access it. [Refer to official API docs for more
-info](https://developers.mailersend.com/).*  # Support and Feedback In case you
-find any bugs, submit an issue directly here in GitHub. You are welcome to
-create SDK for any other programming language. If you have any troubles using
-our API or SDK free to contact our support by email [info@mailersend.com]
-(mailto:info@mailersend.com) The official documentation is at [https://
-developers.mailersend.com](https://developers.mailersend.com)  # License [The
-MIT License (MIT)](LICENSE)
+(identity_id="123456")) ``` ## API Quota ### Get API Quota ```python from
+mailersend import api_quota from dotenv import load_dotenv load_dotenv() mailer
+= api_quota.NewApiQuota(os.getenv('MAILERSEND_API_KEY')) print(mailer.get_quota
+()) ``` # Troubleshooting ## Emails not being sent Print the output of
+`mailer.send()` to view status code and errors. ```python from mailersend
+import emails mailer = emails.NewEmail() mail_body = {} print(mailer.send
+(mail_body)) ``` # Testing TBD  # Available endpoints | Feature group |
+Endpoint | Available | |-------------------|-----------------------------------
+------|-----------| | Activity | `GET activity` | â | | Analytics | `GET
+analytics` | â | | Domains | `{GET, PUT, DELETE} domains` | â | | Emails |
+`POST send` | â | | Messages | `GET messages` | â | | Recipients | `{GET,
+DELETE} recipients` | â | | Templates | `{GET, DELETE} templates` | â | |
+Tokens | `{POST, PUT, DELETE} tokens` | â | | Webhooks | `{GET, POST, PUT,
+DELETE} webhooks` | â | | SMS Sending | `{POST} sms` | â | | SMS Activity |
+`{GET} sms-activity` | â | | SMS Phone numbers | `{GET, PUT, DELETE} sms-
+numbers` | â | | SMS Recipients | `{GET, PUT} sms-recipients` | â | | SMS
+Messages | `{GET} sms-messages` | â | | SMS Webhooks | `{GET, POST, PUT,
+DELETE} sms-webhooks` | â | | SMS Inbounds | `{GET, POST, PUT, DELETE} sms-
+inbounds` | â | | Sender Identities | `{GET, POST, PUT, DELETE} identities` |
+â | | API Quota | `{GET} api-quota` | â | *If, at the moment, some endpoint
+is not available, please use other available tools to access it. [Refer to
+official API docs for more info](https://developers.mailersend.com/).*  #
+Support and Feedback In case you find any bugs, submit an issue directly here
+in GitHub. You are welcome to create SDK for any other programming language. If
+you have any troubles using our API or SDK free to contact our support by email
+[info@mailersend.com](mailto:info@mailersend.com) The official documentation is
+at [https://developers.mailersend.com](https://developers.mailersend.com)  #
+License [The MIT License (MIT)](LICENSE)
```

