# Comparing `tmp/mwxlib-0.83.6-py3-none-any.whl.zip` & `tmp/mwxlib-0.83.8-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,24 +1,24 @@
-Zip file size: 161726 bytes, number of entries: 22
+Zip file size: 162191 bytes, number of entries: 22
 -rw-rw-rw-  2.0 fat     2520 b- defN 23-May-02 16:40 mwx/__init__.py
 -rw-rw-rw-  2.0 fat    43445 b- defN 23-May-02 17:15 mwx/controls.py
--rw-rw-rw-  2.0 fat    73366 b- defN 23-May-22 02:21 mwx/framework.py
--rw-rw-rw-  2.0 fat    69534 b- defN 23-May-17 15:10 mwx/graphman.py
+-rw-rw-rw-  2.0 fat    73366 b- defN 23-May-23 16:14 mwx/framework.py
+-rw-rw-rw-  2.0 fat    69534 b- defN 23-May-23 16:21 mwx/graphman.py
 -rw-rw-rw-  2.0 fat    46248 b- defN 23-Feb-21 08:49 mwx/images.py
 -rw-rw-rw-  2.0 fat    36017 b- defN 23-May-17 04:56 mwx/matplot2.py
 -rw-rw-rw-  2.0 fat    68253 b- defN 23-May-17 11:19 mwx/matplot2g.py
 -rw-rw-rw-  2.0 fat    27606 b- defN 23-Apr-27 09:45 mwx/matplot2lg.py
 -rw-rw-rw-  2.0 fat     6878 b- defN 23-Feb-21 08:50 mwx/mgplt.py
--rw-rw-rw-  2.0 fat   137383 b- defN 23-May-23 08:19 mwx/nutshell.py
+-rw-rw-rw-  2.0 fat   138533 b- defN 23-May-23 16:14 mwx/nutshell.py
 -rw-rw-rw-  2.0 fat    37504 b- defN 23-May-23 07:00 mwx/utilus.py
 -rw-rw-rw-  2.0 fat    11343 b- defN 23-May-16 07:42 mwx/wxmon.py
 -rw-rw-rw-  2.0 fat    19367 b- defN 23-May-16 07:42 mwx/wxpdb.py
 -rw-rw-rw-  2.0 fat     5254 b- defN 23-May-16 07:42 mwx/wxwil.py
 -rw-rw-rw-  2.0 fat     7424 b- defN 23-May-16 07:42 mwx/wxwit.py
 -rw-rw-rw-  2.0 fat        0 b- defN 23-Jan-23 14:06 mwx/py/__init__.py
 -rw-rw-rw-  2.0 fat    16794 b- defN 23-Apr-27 09:45 mwx/py/filling.py
--rw-rw-rw-  2.0 fat     1091 b- defN 23-May-23 08:20 mwxlib-0.83.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     1893 b- defN 23-May-23 08:20 mwxlib-0.83.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 08:20 mwxlib-0.83.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        4 b- defN 23-May-23 08:20 mwxlib-0.83.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat     1609 b- defN 23-May-23 08:20 mwxlib-0.83.6.dist-info/RECORD
-22 files, 613625 bytes uncompressed, 159224 bytes compressed:  74.1%
+-rw-rw-rw-  2.0 fat     1091 b- defN 23-May-23 16:21 mwxlib-0.83.8.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat     1893 b- defN 23-May-23 16:21 mwxlib-0.83.8.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-23 16:21 mwxlib-0.83.8.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat        4 b- defN 23-May-23 16:21 mwxlib-0.83.8.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat     1609 b- defN 23-May-23 16:21 mwxlib-0.83.8.dist-info/RECORD
+22 files, 614775 bytes uncompressed, 159689 bytes compressed:  74.0%
```

## zipnote {}

```diff
@@ -45,23 +45,23 @@
 
 Filename: mwx/py/__init__.py
 Comment: 
 
 Filename: mwx/py/filling.py
 Comment: 
 
-Filename: mwxlib-0.83.6.dist-info/LICENSE
+Filename: mwxlib-0.83.8.dist-info/LICENSE
 Comment: 
 
-Filename: mwxlib-0.83.6.dist-info/METADATA
+Filename: mwxlib-0.83.8.dist-info/METADATA
 Comment: 
 
-Filename: mwxlib-0.83.6.dist-info/WHEEL
+Filename: mwxlib-0.83.8.dist-info/WHEEL
 Comment: 
 
-Filename: mwxlib-0.83.6.dist-info/top_level.txt
+Filename: mwxlib-0.83.8.dist-info/top_level.txt
 Comment: 
 
-Filename: mwxlib-0.83.6.dist-info/RECORD
+Filename: mwxlib-0.83.8.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## mwx/framework.py

```diff
@@ -1,14 +1,14 @@
 #! python3
 # -*- coding: utf-8 -*-
 """mwxlib framework
 
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 """
-__version__ = "0.83.6"
+__version__ = "0.83.8"
 __author__ = "Kazuya O'moto <komoto@jeol.co.jp>"
 
 from functools import wraps, partial
 from importlib import reload
 import traceback
 import builtins
 import datetime
@@ -1179,15 +1179,15 @@
                     style=wx.FD_OPEN|wx.FD_FILE_MUST_EXIST|wx.FD_CHANGE_DIR) as dlg:
                 if dlg.ShowModal() != wx.ID_OK:
                     return
                 rc = dlg.Path
         
         if flush:
             for book in self.get_all_pages(type(self.Log)):
-                book.remove_all_buffers()
+                book.delete_all_buffers()
         
         self.SESSION_FILE = os.path.abspath(rc)
         try:
             scratch = self.Scratch.default_buffer
             if not scratch or scratch.mtdelta is not None:
                 scratch = self.Scratch.new_buffer()
             scratch.LoadFile(self.SCRATCH_FILE)
```

## mwx/nutshell.py

```diff
@@ -30,14 +30,27 @@
 
 from .utilus import funcall as _F
 from .utilus import split_words, split_paren
 from .utilus import find_modules, deprecated
 from .framework import CtrlInterface, AuiNotebook, Menu
 
 
+## URL pattern (flag = re.M | re.A)
+url_re = r"https?://[\w/:%#\$&\?()~.=+-]+"
+
+## Python syntax pattern
+py_indent_re  = r"if|else|elif|for|while|with|def|class|try|except|finally"
+py_outdent_re = r"else:|elif\s+.*:|except(\s+.*)?:|finally:"
+py_closing_re = r"break|pass|return|raise|continue"
+
+## Python interp traceback pattern
+py_error_re = r"^\s+File \"(.*?)\", line ([0-9]+)"
+py_frame_re = r"^\s+file \'(.*?)\', line ([0-9]+)"
+
+
 def skip(v):
     v.Skip()
 
 
 def editable(f):
     @wraps(f)
     def _f(self, *args, **kwargs):
@@ -274,14 +287,19 @@
         self.IndicatorSetOutlineAlpha(1, 120)
         self.IndicatorSetForeground(0, "red")
         self.IndicatorSetForeground(1, "yellow")
         
         ## Custom indicator [2] for match_paren
         self.IndicatorSetStyle(2, stc.STC_INDIC_DOTS)
         self.IndicatorSetForeground(2, "light gray")
+        try:
+            self.IndicatorSetHoverStyle(2, stc.STC_INDIC_PLAIN)
+            self.IndicatorSetHoverForeground(2, "light gray")
+        except AttributeError:
+            pass
         
         ## Custom annotation
         self.AnnotationSetVisible(stc.STC_ANNOTATION_BOXED)
         
         ## Custom style of control-char, wrap-mode
         ## self.UseTabs = False
         ## self.ViewEOL = False
@@ -581,18 +599,14 @@
                 self.WordRightEnd()
                 q = self.cpos
             return self.GetTextRange(p, q)
     
     ## --------------------------------
     ## Python syntax and indentation
     ## --------------------------------
-    py_indent_re  = r"if|else|elif|for|while|with|def|class|try|except|finally"
-    py_outdent_re = r"else:|elif\s+.*:|except(\s+.*)?:|finally:"
-    py_closing_re = r"break|pass|return|raise|continue"
-    
     def on_indent_line(self, evt):
         if self.SelectedText:
             evt.Skip()
         else:
             self.py_indent_line()
     
     def on_outdent_line(self, evt):
@@ -625,15 +639,15 @@
     
     def py_current_indent(self):
         """Calculate indent spaces from previous line."""
         text = self.GetLine(self.cline - 1)
         indent = self.py_calc_indentation(text) # check previous line
         text = self.GetLine(self.cline)
         lstr, _indent = self.py_strip_indents(text) # check current line
-        if re.match(self.py_outdent_re, lstr):
+        if re.match(py_outdent_re, lstr):
             indent -= 4
         return indent
     
     def py_electric_indent(self):
         """Calculate indent spaces for the following line."""
         text, lp = self.CurLine
         return self.py_calc_indentation(text[:lp])
@@ -642,17 +656,17 @@
     def py_calc_indentation(self, text):
         """Returns indent spaces for the command text."""
         text = self.py_strip_comments(text)
         lstr, indent = self.py_strip_indents(text)
         text = text.rstrip()
         if text.endswith('\\'):
             return indent + 2
-        if text.endswith(':') and re.match(self.py_indent_re, lstr):
+        if text.endswith(':') and re.match(py_indent_re, lstr):
             return indent + 4
-        if re.match(self.py_closing_re, lstr):
+        if re.match(py_closing_re, lstr):
             return indent - 4
         return indent
     
     @classmethod
     def py_strip_indents(self, text):
         """Returns left-stripped text and the number of indent spaces."""
         text = self.py_strip_prompts(text) # cf. shell.lstripPrompt(text)
@@ -848,19 +862,14 @@
                 self.SetCaretStyle(stc.STC_CARETSTYLE_BLOCK)
         
         ## Custom indicator for search-word
         item = _map(spec.pop(stc.STC_P_WORD3, ''))
         if item:
             self.IndicatorSetForeground(0, item.get('fore') or "red")
             self.IndicatorSetForeground(1, item.get('back') or "yellow")
-            try:
-                self.IndicatorSetHoverStyle(1, stc.STC_INDIC_ROUNDBOX)
-                self.IndicatorSetHoverForeground(1, "blue")
-            except AttributeError:
-                pass
         
         ## Apply the rest of the style
         for key, value in spec.items():
             self.StyleSetSpec(key, value)
     
     def match_paren(self):
         ## self.SetIndicatorCurrent(2)
@@ -1015,36 +1024,40 @@
             else:
                 st = 'paren' # closed
         else:
             while self.get_style(p-1) == st and p > 0:
                 p -= 1
         return p, q, st
     
-    def grep_forward(self, pattern):
+    def grep_forward(self, pattern, flags=re.M):
         text = self.GetTextRange(self.eol, self.TextLength)
-        errs = re.finditer(pattern, text, re.M)
+        errs = re.finditer(pattern, text, flags)
         for err in errs:
             p, q = err.span()
             self.goto_char(q + self.eol)
             self.goto_char(self.bol)
             self.mark = self.cpos
             self.EnsureVisible(self.cline)
             yield err
     
-    def grep_barckward(self, pattern):
+    def grep_barckward(self, pattern, flags=re.M):
         text = self.GetTextRange(0, self.cpos)
-        errs = re.finditer(pattern, text, re.M)
+        errs = re.finditer(pattern, text, flags)
         for err in reversed(list(errs)):
             p, q = err.span()
             self.goto_char(p)
             self.goto_char(self.bol)
             self.mark = self.cpos
             self.EnsureVisible(self.cline)
             yield err
     
+    def grep(self, pattern, flags=re.M):
+        text = self.GetTextRange(0, self.TextLength)
+        yield from re.finditer(pattern, text, flags)
+    
     def search_text(self, text):
         """Yields raw-positions where `text` is found."""
         word = text.encode()
         raw = self.TextRaw
         pos = -1
         while 1:
             pos = raw.find(word, pos+1)
@@ -1437,15 +1450,15 @@
             = 0  : a file
             > 0  : a file edited externally
             < 0  : a url file
         """
         f = self.filename
         if f and os.path.isfile(f):
             return os.path.getmtime(f) - self.__mtime
-        elif f and re.match(r"https?://[\w/:%#\$&\?()~.=+-]+", f):
+        elif f and re.match(url_re, f):
             return -1
     
     @property
     def caption(self):
         prefix = ''
         dt = self.mtdelta
         if dt is not None:
@@ -1489,14 +1502,16 @@
         
         self.parent = parent
         self.filename = filename
         self.code = None
         
         self.Bind(stc.EVT_STC_UPDATEUI, self.OnUpdate) # skip to brace matching
         
+        self.Bind(stc.EVT_STC_INDICATOR_CLICK, self.OnIndicatorClick)
+        
         self.Bind(stc.EVT_STC_SAVEPOINTLEFT, self.OnSavePointLeft)
         self.Bind(stc.EVT_STC_SAVEPOINTREACHED, self.OnSavePointReached)
         
         def activate(v):
             self.handler('buffer_activated', self)
             v.Skip()
         self.Bind(wx.EVT_SET_FOCUS, activate)
@@ -1508,20 +1523,20 @@
         
         def dispatch(v):
             """Fork mouse events to the parent."""
             self.parent.handler(self.handler.current_event, v)
         
         self.handler.update({ # DNA<Buffer>
             None : {
-                  'stc_updated' : [ None, ],
-                 'buffer_saved' : [ None, self.on_activated, dispatch ],
-                'buffer_loaded' : [ None, self.on_activated, dispatch ],
+                 'buffer_saved' : [ None, dispatch ],
+                'buffer_loaded' : [ None, dispatch ],
+              'buffer_modified' : [ None, self.on_modified, dispatch ],
              'buffer_activated' : [ None, self.on_activated, dispatch ],
            'buffer_inactivated' : [ None, self.on_inactivated, dispatch ],
-           'py_region_executed' : [ None, self.on_activated ],
+       'buffer_region_executed' : [ None, ],
             },
             -1 : { # original action of the EditWindow
                     '* pressed' : (0, skip, self.on_exit_escmap),
                  '*alt pressed' : (-1, ),
                 '*ctrl pressed' : (-1, ),
                '*shift pressed' : (-1, ),
              '*[LR]win pressed' : (-1, ),
@@ -1544,17 +1559,38 @@
     def trace_position(self):
         text, lp = self.CurLine
         self.message("{:>6d}:{} ({})".format(self.cline, lp, self.cpos), pane=-1)
     
     def OnUpdate(self, evt): #<wx._stc.StyledTextEvent>
         if evt.Updated & (stc.STC_UPDATE_SELECTION | stc.STC_UPDATE_CONTENT):
             self.trace_position()
-            self.handler('stc_updated', evt)
+            if evt.Updated & stc.STC_UPDATE_CONTENT:
+                self.handler('buffer_modified', self)
         evt.Skip()
     
+    def OnIndicatorClick(self, evt):
+        if self.SelectedText:
+            evt.Skip()
+            return
+        pos = evt.Position
+        if self.IndicatorValueAt(2, pos):
+            p = self.IndicatorStart(2, pos)
+            q = self.IndicatorEnd(2, pos)
+            text = self.GetTextRange(p, q).strip()
+            ## Note: Do postcall a confirmation dialog.
+            wx.CallAfter(self.parent.load_url, text)
+    
+    def on_modified(self, buf):
+        """Called when the buffer is modified."""
+        self.SetIndicatorCurrent(2)
+        self.IndicatorClearRange(0, self.TextLength)
+        for m in self.grep(url_re):
+            p, q = m.span()
+            self.IndicatorFillRange(p, q-p)
+    
     def OnSavePointLeft(self, evt):
         if self.mtdelta is not None:
             self.parent.handler('buffer_caption_reset', self)
         evt.Skip()
     
     def OnSavePointReached(self, evt):
         if self.mtdelta is not None:
@@ -1666,15 +1702,15 @@
         try:
             code = compile(self.Text, filename, "exec")
             exec(code, globals, locals)
             dispatcher.send(signal='Interpreter.push',
                             sender=self, command=None, more=False)
         except Exception as e:
             msg = traceback.format_exc()
-            err = re.findall(r"^\s+File \"(.*?)\", line ([0-9]+)", msg, re.M)
+            err = re.findall(py_error_re, msg, re.M)
             lines = [int(l) for f,l in err if f == filename]
             if lines:
                 lx = lines[-1] - 1
                 self.red_arrow = lx
                 self.goto_line(lx)
                 self.EnsureVisible(lx) # expand if folded
                 self.EnsureCaretVisible()
@@ -1682,15 +1718,15 @@
                 self.AnnotationSetText(lx, msg)
             self.message("- {!r}".format(e))
             ## print(msg, file=sys.__stderr__)
         else:
             self.code = code
             del self.pointer # Reset pointer (debugger hook point).
             del self.red_arrow
-            self.handler('py_region_executed', self)
+            self.handler('buffer_region_executed', self)
             self.message("Evaluated {!r} successfully".format(filename))
             self.AnnotationClearAll()
     
     def py_get_region(self, line):
         """Line numbers of code head and tail containing the line.
         
         Requires a code object.
@@ -1739,15 +1775,15 @@
         
         self.Bind(aui.EVT_AUINOTEBOOK_PAGE_CLOSE, self.OnPageClose)
         self.Bind(aui.EVT_AUINOTEBOOK_PAGE_CLOSED, self.OnPageClosed)
         
         def destroy(v):
             obj = v.EventObject
             if isinstance(obj, Buffer):
-                self.handler('buffer_removed', obj)
+                self.handler('buffer_deleted', obj)
             v.Skip()
         self.Bind(wx.EVT_WINDOW_DESTROY, destroy)
         
         def dispatch(v):
             """Fork mouse events to the parent."""
             self.parent.handler(self.handler.current_event, v)
         
@@ -1755,29 +1791,28 @@
         self.make_keymap('C-c')
         
         self.handler.update({ # DNA<EditorBook>
             None : {
                    'buffer_new' : [ None, dispatch, ],
                  'buffer_saved' : [ None, dispatch, self.set_caption ],
                 'buffer_loaded' : [ None, dispatch, self.set_caption ],
-               'buffer_removed' : [ None, dispatch, ],
+               'buffer_deleted' : [ None, dispatch, ],
+              'buffer_modified' : [ None, dispatch, ],
              'buffer_activated' : [ None, dispatch, self.on_activated ],
            'buffer_inactivated' : [ None, dispatch, self.on_inactivated ],
          'buffer_caption_reset' : [ None, dispatch, self.set_caption ],
         'buffer_filename_reset' : [ None, dispatch, ],
              '*button* pressed' : [ None, dispatch, skip ],
             '*button* released' : [ None, dispatch, skip ],
             },
             0 : { # Normal mode
                     '* pressed' : (0, skip),
                    '* released' : (0, skip),
                  'M-up pressed' : (0, _F(self.previous_buffer)),
                'M-down pressed' : (0, _F(self.next_buffer)),
-               'M-left pressed' : (0, dispatch),
-              'M-right pressed' : (0, dispatch),
             },
         })
     
     def OnPageClose(self, evt): #<wx._aui.AuiNotebookEvent>
         nb = evt.EventObject
         buf = nb.all_buffers[evt.Selection]
         if buf.need_buffer_save:
@@ -1897,25 +1932,25 @@
             self.default_buffer = buf
         else:
             buf.ClearAll()
             ## buf.EmptyUndoBuffer()
         buf.SetFocus()
         return buf
     
-    def remove_buffer(self, buf=None):
+    def delete_buffer(self, buf=None):
         """Pop the current buffer from the buffer list."""
         if not buf:
             buf = self.buffer
         j = self.GetPageIndex(buf)
         if j != -1:
             self.DeletePage(j)  # the focus is moved
             if not self.buffer: # no buffers
                 self.new_buffer()
     
-    def remove_all_buffers(self):
+    def delete_all_buffers(self):
         """Initialize list of buffers."""
         self.DeleteAllPages()
         self.new_buffer()
     
     def next_buffer(self):
         self.Selection += 1
     
@@ -1985,15 +2020,15 @@
             org = self.buffer
             if buf._load_file(buf.filename, lineno):
                 self.swap_page(buf)
                 return True
             return False
         except Exception as e:
             self.post_message("Failed to load {!r}: {}".format(buf.name, e))
-            self.remove_buffer(buf)
+            self.delete_buffer(buf)
             if org:
                 self.swap_page(org)
             return False
         finally:
             self.Thaw()
     
     def save_file(self, filename, buf=None):
@@ -2083,28 +2118,28 @@
                     "You are closing unsaved content.\n\n"
                     "The changes will be discarded.\n"
                     "Continue closing?",
                     "Close {!r}".format(buf.name),
                     style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
                 self.post_message("The close has been canceled.")
                 return None
-        wx.CallAfter(self.remove_buffer, buf)
+        wx.CallAfter(self.delete_buffer, buf)
     
     def kill_all_buffers(self):
         for buf in self.all_buffers:
             if buf.need_buffer_save:
                 if wx.MessageBox( # Confirm close.
                         "You are closing unsaved content.\n\n"
                         "The changes will be discarded.\n"
                         "Continue closing?",
                         "Close {!r}".format(buf.name),
                         style=wx.YES_NO|wx.ICON_INFORMATION) != wx.YES:
                     self.post_message("The close has been canceled.")
                     return None
-        wx.CallAfter(self.remove_all_buffers)
+        wx.CallAfter(self.delete_all_buffers)
 
 
 class Interpreter(interpreter.Interpreter):
     """Interpreter based on code.InteractiveInterpreter.
     """
     def __init__(self, *args, **kwargs):
         parent = kwargs.pop('interpShell')
@@ -2392,17 +2427,17 @@
         
         def dispatch(v):
             """Fork mouse events to the parent."""
             self.parent.handler(self.handler.current_event, v)
         
         self.handler.update({ # DNA<Nautilus>
             None : {
-                  'stc_updated' : [ None, ],
                  'interp_error' : [ None, self.on_interp_error ],
                 'shell_deleted' : [ None, dispatch, self.on_deleted ],
+               'shell_modified' : [ None, dispatch, ],
               'shell_activated' : [ None, dispatch, self.on_activated ],
             'shell_inactivated' : [ None, dispatch, self.on_inactivated ],
              '*button* pressed' : [ None, dispatch, skip ],
             '*button* released' : [ None, dispatch, skip ],
             },
             -1 : { # original action of the wx.py.shell
                     '* pressed' : (0, skip, self.on_exit_escmap),
@@ -2624,15 +2659,16 @@
                 text = self.expr_at_caret
                 if text and text != self.__text:
                     name, argspec, tip = self.interp.getCallTip(text)
                     if tip:
                         tip = tip.splitlines()[0]
                     self.message(tip) # clear if no tip
                     self.__text = text
-            self.handler('stc_updated', evt)
+            if evt.Updated & stc.STC_UPDATE_CONTENT:
+                self.handler('shell_modified', self)
         evt.Skip()
     
     def OnCallTipClick(self, evt):
         self.parent.handler('add_help', self.__calltip)
         if self.CallTipActive():
             self.CallTipCancel()
         evt.Skip()
@@ -2904,15 +2940,15 @@
         """Called when [Enter] text (after push).
         Set markers at the last command line.
         
         Note:
             Argument `text` is raw output:str with no magic cast.
         """
         ln = self.cmdline_region[0]
-        err = re.findall(r"^\s+File \"(.*?)\", line ([0-9]+)", text, re.M)
+        err = re.findall(py_error_re, text, re.M)
         self.add_marker(ln, 1 if not err else 2) # 1:white-arrow 2:red-arrow
         return (not err)
     
     def on_interp_error(self, e):
         self.pointer = self.cmdline_region[0] + e.lineno - 1
     
     ## --------------------------------
@@ -3145,27 +3181,27 @@
             lines += atom
             if atom[0] not in '\r\n':
                 continue
             line = self.lstripPrompt(lines)
             lstr = line.lstrip()
             if (lstr and lstr == line # no indent
                 and not lstr.startswith('#') # no comment
-                and not re.match(self.py_outdent_re, lstr)): # no outdent pattern
+                and not re.match(py_outdent_re, lstr)): # no outdent pattern
                 if cmd:
                     commands.append(cmd) # Add stacked commands to the list
                 cmd = line
             else:
                 cmd += lines # multi-line command
             lines = ''
         commands.append(cmd + lines)
         
         if len(commands) > 1:
             suffix = sys.ps2
             for j, cmd in enumerate(commands):
-                if re.match(self.py_indent_re, cmd):
+                if re.match(py_indent_re, cmd):
                     ## multi-line code-block ends with [\r\n... ]
                     if not cmd.endswith(os.linesep):
                         cmd = cmd.rstrip('\r\n') + os.linesep
                     if not cmd.endswith(suffix):
                         cmd = cmd + suffix
                 else:
                     ## single line of code ends without [\r\n... ]
@@ -3187,15 +3223,15 @@
         command = self.regulate_cmd(text)
         commands = []
         cmd = ''
         for line in command.splitlines():
             lstr = line.lstrip()
             if (lstr and lstr == line # no indent
                 and not lstr.startswith('#') # no comment
-                and not re.match(self.py_outdent_re, lstr)): # no outdent pattern
+                and not re.match(py_outdent_re, lstr)): # no outdent pattern
                 if cmd:
                     commands.append(cmd) # Add the previous command to the list
                 cmd = line
             else:
                 cmd += '\n' + line # Multiline command; Add to the command
         commands.append(cmd)
         
@@ -3293,15 +3329,15 @@
             try:
                 cmd = self.magic_interpret(tokens)
                 cmd = self.regulate_cmd(cmd)
                 code = compile(cmd, filename, "exec")
                 self.exec(code)
             except Exception as e:
                 msg = traceback.format_exc()
-                err = re.findall(r"^\s+File \"(.*?)\", line ([0-9]+)", msg, re.M)
+                err = re.findall(py_error_re, msg, re.M)
                 lines = [int(l) for f,l in err if f == filename]
                 if lines:
                     region = self.get_region(self.cline)
                     self.pointer = region[0] + lines[-1] - 1
                 self.message("- {!r}".format(e))
                 ## print(msg, file=sys.__stderr__)
             else:
```

## Comparing `mwxlib-0.83.6.dist-info/LICENSE` & `mwxlib-0.83.8.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `mwxlib-0.83.6.dist-info/METADATA` & `mwxlib-0.83.8.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mwxlib
-Version: 0.83.6
+Version: 0.83.8
 Summary: A wrapper of matplotlib and wxPython (phoenix)
 Home-page: https://github.com/komoto48g/mwxlib
 Author: Kazuya O'moto <komoto@jeol.co.jp>
 Author-email: komoto@jeol.co.jp
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

