# Comparing `tmp/python_substack-0.1.7.tar.gz` & `tmp/python_substack-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_substack-0.1.7.tar", max compression
+gzip compressed data, was "python_substack-0.1.8.tar", max compression
```

## Comparing `python_substack-0.1.7.tar` & `python_substack-0.1.8.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1063 2023-05-11 16:10:44.701266 python_substack-0.1.7/LICENSE
--rw-r--r--   0        0        0      724 2023-05-11 16:10:44.701266 python_substack-0.1.7/README.md
--rw-r--r--   0        0        0      619 2023-05-11 16:10:44.701266 python_substack-0.1.7/pyproject.toml
--rw-r--r--   0        0        0      388 2023-05-11 16:10:44.701266 python_substack-0.1.7/substack/__init__.py
--rw-r--r--   0        0        0     8472 2023-05-11 16:10:44.701266 python_substack-0.1.7/substack/api.py
--rw-r--r--   0        0        0      841 2023-05-11 16:10:44.701266 python_substack-0.1.7/substack/exceptions.py
--rw-r--r--   0        0        0     5669 2023-05-11 16:10:44.701266 python_substack-0.1.7/substack/post.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 python_substack-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-05-24 14:01:21.167468 python_substack-0.1.8/LICENSE
+-rw-r--r--   0        0        0      745 2023-05-24 14:01:21.167468 python_substack-0.1.8/README.md
+-rw-r--r--   0        0        0      619 2023-05-24 14:01:21.171468 python_substack-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      388 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/__init__.py
+-rw-r--r--   0        0        0     8472 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/api.py
+-rw-r--r--   0        0        0      841 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/exceptions.py
+-rw-r--r--   0        0        0     7104 2023-05-24 14:01:21.171468 python_substack-0.1.8/substack/post.py
+-rw-r--r--   0        0        0     1610 1970-01-01 00:00:00.000000 python_substack-0.1.8/PKG-INFO
```

### Comparing `python_substack-0.1.7/LICENSE` & `python_substack-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `python_substack-0.1.7/README.md` & `python_substack-0.1.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -17,12 +17,14 @@
 Set the following environment variables by creating a **.env** file:
 
     PUBLICATION_URL=https://ma2za.substack.com
     EMAIL=
     PASSWORD=
     USER_ID=
 
-The only way I found to discover the USER_ID is to inspect
-the payload to a **/drafts** request. Under the fields **draftBylines**
-or **postBylines** there is a subfield **user_id** or **id**
+To discover the USER_ID go to your public profile page,
+in the URL bar of the browser you find the substack address 
+followed by your USER_ID and your username:
+https://substack.com/profile/[USER_ID]-[username]
 
-The .env file will be ignored by git but always be careful.
+
+The .env file will be ignored by git but always be careful.
```

### Comparing `python_substack-0.1.7/pyproject.toml` & `python_substack-0.1.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-substack"
-version = "0.1.7"
+version = "0.1.8"
 description = "A Python wrapper around the Substack API."
 authors = ["Paolo Mazza <mazzapaolo2019@gmail.com>"]
 license = "MIT"
 packages = [
     { include = "substack" }
 ]
```

### Comparing `python_substack-0.1.7/substack/api.py` & `python_substack-0.1.8/substack/api.py`

 * *Files identical despite different names*

### Comparing `python_substack-0.1.7/substack/exceptions.py` & `python_substack-0.1.8/substack/exceptions.py`

 * *Files identical despite different names*

### Comparing `python_substack-0.1.7/substack/post.py` & `python_substack-0.1.8/substack/post.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,22 +1,42 @@
 import json
 from typing import Dict
 
 
 class Post:
 
-    def __init__(self, title, subtitle, user_id):
+    def __init__(self, title: str, subtitle: str, user_id,
+                 audience: str = None,
+                 write_comment_permissions: str = None):
+        """
+
+        Args:
+            title:
+            subtitle:
+            user_id:
+            audience: possible values: everyone, only_paid, founding, only_free
+            write_comment_permissions: none, only_paid, everyone (this field is a mess)
+        """
         self.draft_title = title
         self.draft_subtitle = subtitle
         self.draft_body = {"type": "doc", "content": []}
         self.draft_bylines = [{"id": int(user_id), "is_guest": False}]
+        self.audience = audience if audience is not None else "everyone"
+
+        # TODO better understand the possible values and combinations with audience
+        if write_comment_permissions is not None:
+            self.write_comment_permissions = write_comment_permissions
+        else:
+            self.write_comment_permissions = self.audience
 
     def add(self, item: Dict):
         """
 
+        Add item to draft body.
+
         Args:
             item:
 
         Returns:
 
         """
 
@@ -36,30 +56,61 @@
         marks = item.get("marks")
         if marks is not None:
             self.marks(marks)
 
         return self
 
     def paragraph(self, content=None):
+        """
+
+        Args:
+            content:
+
+        Returns:
+
+        """
         item = {"type": "paragraph"}
         if content is not None:
             item["content"] = content
         return self.add(item)
 
-    def heading(self, content=None, level=1):
+    def heading(self, content=None, level: int = 1):
+        """
+
+        Args:
+            content:
+            level:
+
+        Returns:
+
+        """
+
         item = {"type": "heading"}
         if content is not None:
             item["content"] = content
         item["level"] = level
         return self.add(item)
 
     def horizontal_rule(self):
+        """
+
+        Returns:
+
+        """
         return self.add({"type": "horizontal_rule"})
 
     def attrs(self, level):
+        """
+
+        Args:
+            level:
+
+        Returns:
+
+        """
         content_attrs = self.draft_body["content"][-1].get("attrs", {})
         content_attrs.update({"level": level})
         self.draft_body["content"][-1]["attrs"] = content_attrs
         return self
 
     def captioned_image(self,
                         src: str,
@@ -112,15 +163,15 @@
             "belowTheFold": belowTheFold,
             "internalRedirect": internalRedirect
 
         }}]
         self.draft_body["content"][-1]["content"] = content
         return self
 
-    def text(self, value):
+    def text(self, value: str):
         """
 
         Add text to the last paragraph.
 
         Args:
             value: Text to add to paragraph.
 
@@ -129,56 +180,93 @@
         """
         content = self.draft_body["content"][-1].get("content", [])
         content += [{"type": "text", "text": value}]
         self.draft_body["content"][-1]["content"] = content
         return self
 
     def add_complex_text(self, text):
+        """
+
+        Args:
+            text:
+        """
         if isinstance(text, str):
             self.text(text)
         else:
             for chunk in text:
                 if chunk:
                     self.text(chunk.get("content")).marks(chunk.get("marks"))
 
     def marks(self, marks):
+        """
+
+        Args:
+            marks:
+
+        Returns:
+
+        """
         content = self.draft_body["content"][-1].get("content", [])[-1]
         content_marks = content.get("marks", [])
         for mark in marks:
             new_mark = {"type": mark.get("type")}
             if mark.get("type") == "link":
                 href = mark.get("href")
                 new_mark.update({"attrs": {
                     "href": href
                 }})
             content_marks.append(new_mark)
         content["marks"] = content_marks
         return self
 
     def remove_last_paragraph(self):
+        """
+
+        """
         del self.draft_body.get("content")[-1]
 
     def get_draft(self):
+        """
+
+        Returns:
+
+        """
         out = vars(self)
         out["draft_body"] = json.dumps(out["draft_body"])
         return out
 
-    def subscribe_with_caption(self, value):
+    def subscribe_with_caption(self, value: str):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        """
         content = self.draft_body["content"][-1].get("content", [])
         content += [{"type": "subscribeWidget",
                      "attrs": {"url": "%%checkout_url%%", "text": "Subscribe"},
                      "content": [
                          {
                              "type": "ctaCaption",
                              "content": [{"type": "text",
                                           "text": f"""Thanks for reading {value}! 
                                           Subscribe for free to receive new posts and support my work."""}]
                          }
                      ]}]
         self.draft_body["content"][-1]["content"] = content
         return self
 
-    def youtube(self, value):
+    def youtube(self, value: str):
+        """
+
+        Args:
+            value:
+
+        Returns:
+
+        """
         content_attrs = self.draft_body["content"][-1].get("attrs", {})
         content_attrs.update({"videoId": value})
         self.draft_body["content"][-1]["attrs"] = content_attrs
         return self
```

### Comparing `python_substack-0.1.7/PKG-INFO` & `python_substack-0.1.8/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-substack
-Version: 0.1.7
+Version: 0.1.8
 Summary: A Python wrapper around the Substack API.
 Home-page: https://github.com/ma2za/python-substack
 License: MIT
 Keywords: substack
 Author: Paolo Mazza
 Author-email: mazzapaolo2019@gmail.com
 Requires-Python: >=3.7,<4.0
@@ -40,12 +40,15 @@
 Set the following environment variables by creating a **.env** file:
 
     PUBLICATION_URL=https://ma2za.substack.com
     EMAIL=
     PASSWORD=
     USER_ID=
 
-The only way I found to discover the USER_ID is to inspect
-the payload to a **/drafts** request. Under the fields **draftBylines**
-or **postBylines** there is a subfield **user_id** or **id**
+To discover the USER_ID go to your public profile page,
+in the URL bar of the browser you find the substack address 
+followed by your USER_ID and your username:
+https://substack.com/profile/[USER_ID]-[username]
+
 
 The .env file will be ignored by git but always be careful.
+
```

