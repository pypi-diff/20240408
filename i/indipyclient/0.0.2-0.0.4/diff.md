# Comparing `tmp/indipyclient-0.0.2.tar.gz` & `tmp/indipyclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "indipyclient-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "indipyclient-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `indipyclient-0.0.2.tar` & `indipyclient-0.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.2/LICENSE
--rw-r--r--   0        0        0     2686 2024-04-03 21:19:09.000000 indipyclient-0.0.2/README.md
--rw-r--r--   0        0        0      291 2024-03-31 16:30:35.000000 indipyclient-0.0.2/indipyclient/__init__.py
--rw-r--r--   0        0        0     2998 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/__main__.py
--rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.2/indipyclient/console/__init__.py
--rw-r--r--   0        0        0    19759 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/consoleclient.py
--rw-r--r--   0        0        0    48568 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/widgets.py
--rw-r--r--   0        0        0   142902 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/console/windows.py
--rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.2/indipyclient/error.py
--rw-r--r--   0        0        0    24609 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/events.py
--rw-r--r--   0        0        0    34076 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/ipyclient.py
--rw-r--r--   0        0        0    13587 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/propertymembers.py
--rw-r--r--   0        0        0    25114 2024-04-03 21:17:26.000000 indipyclient-0.0.2/indipyclient/propertyvectors.py
--rw-r--r--   0        0        0      935 2024-03-31 16:29:51.000000 indipyclient-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 indipyclient-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1078 2024-03-29 22:07:10.000000 indipyclient-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2686 2024-04-03 21:19:09.000000 indipyclient-0.0.4/README.md
+-rw-r--r--   0        0        0      291 2024-04-08 21:07:14.000000 indipyclient-0.0.4/indipyclient/__init__.py
+-rw-r--r--   0        0        0     3089 2024-04-03 21:43:04.000000 indipyclient-0.0.4/indipyclient/__main__.py
+-rw-r--r--   0        0        0        0 2023-08-14 16:40:46.000000 indipyclient-0.0.4/indipyclient/console/__init__.py
+-rw-r--r--   0        0        0    19759 2024-04-04 21:35:51.000000 indipyclient-0.0.4/indipyclient/console/consoleclient.py
+-rw-r--r--   0        0        0    48364 2024-04-05 12:12:41.000000 indipyclient-0.0.4/indipyclient/console/widgets.py
+-rw-r--r--   0        0        0   143996 2024-04-08 20:45:37.000000 indipyclient-0.0.4/indipyclient/console/windows.py
+-rw-r--r--   0        0        0      192 2023-09-20 21:15:05.000000 indipyclient-0.0.4/indipyclient/error.py
+-rw-r--r--   0        0        0    24609 2024-04-03 21:17:26.000000 indipyclient-0.0.4/indipyclient/events.py
+-rw-r--r--   0        0        0    34586 2024-04-04 22:04:06.000000 indipyclient-0.0.4/indipyclient/ipyclient.py
+-rw-r--r--   0        0        0    15364 2024-04-07 22:08:45.000000 indipyclient-0.0.4/indipyclient/propertymembers.py
+-rw-r--r--   0        0        0    25114 2024-04-03 21:17:26.000000 indipyclient-0.0.4/indipyclient/propertyvectors.py
+-rw-r--r--   0        0        0      935 2024-04-08 21:06:58.000000 indipyclient-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3457 1970-01-01 00:00:00.000000 indipyclient-0.0.4/PKG-INFO
```

### Comparing `indipyclient-0.0.2/LICENSE` & `indipyclient-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.2/README.md` & `indipyclient-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.2/indipyclient/__main__.py` & `indipyclient-0.0.4/indipyclient/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,14 +22,15 @@
         await asyncio.sleep(0)
 
 
 def main():
     """The main routine."""
 
     parser = argparse.ArgumentParser(usage="indipyclient [options]",
+                                     formatter_class=argparse.RawDescriptionHelpFormatter,
                                      description="Terminal client to communicate to an INDI service.",
                                      epilog="""The BLOB's folder can also be set from within the session.
 Setting loglevel and logfile should only be used for brief
 diagnostic purposes, the logfile could grow very big.
 loglevel:1 Information and error messages only,
 loglevel:2 log vector tags without members or contents,
 loglevel:3 log vectors and members - but not BLOB contents,
```

### Comparing `indipyclient-0.0.2/indipyclient/console/consoleclient.py` & `indipyclient-0.0.4/indipyclient/console/consoleclient.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.2/indipyclient/console/widgets.py` & `indipyclient-0.0.4/indipyclient/console/widgets.py`

 * *Files 2% similar despite different names*

```diff
@@ -155,39 +155,35 @@
         self.window = window
         self.row = row
         self.col = col
         self._focus = False
         self._show = True
         if txtlen:
             # txtlen includes the two [ ] brackets
-            if len(text) > txtlen-2:
-                self._text = shorten(text, width=txtlen-2, placeholder="...")
-            elif len(text) == txtlen-2:
-                self._text = text
-            else:
-                self._text = text.ljust(txtlen-2)
             self.txtlen = txtlen
+            # call text property setter
+            self.text = text
         else:
             # no txtlen given
             self._text = text
             self.txtlen = len(self._text) + 2
 
 
     @property
     def text(self):
-        return self._text.strip()
+        return self._text
 
     @text.setter
     def text(self, text):
         if len(text) > self.txtlen-2:
             self._text = shorten(text, width=self.txtlen-2, placeholder="...")
         elif len(text) == self.txtlen-2:
             self._text = text
         else:
-            self._text = text.ljust(self.txtlen-2)
+            self._text = text.ljust(self.txtlen-2)  # pads space to right of the text
 
 
     def __contains__(self, mouse):
         "Returns True if the mouse y, x are within this field"
         if not self._show:
             return False
         originrow, origincol = self.window.getbegyx()
@@ -250,22 +246,21 @@
     def __init__(self, stdscr, row, startcol, endcol, text):
         "Class to input text"
         self.stdscr = stdscr
         self.row = row
         self.startcol = startcol
         self.endcol = endcol
         self.length = endcol - startcol + 1
-        self.text = text.strip()
-        if len(self.text) > self.length:
-            self.text = self.text[:self.length]
+        if len(text) > self.length:
+            self.text = text[:self.length]
+        else:
+            # pad text with right hand spaces
+            self.text = text.ljust(self.length)
         # put curser at end of text
-        self.stringpos = len(self.text)
-
-        # pad text with right hand spaces
-        self.text = self.text.ljust(self.length)
+        self.stringpos = len(self.text.rstrip())
         self.movecurs()
 
     def insertch(self, ch):
         "Insert a character at stringpos"
         if self.stringpos >= self.length:
             # stringpos must be less than the length
             return
@@ -358,14 +353,16 @@
         # linecount is the number of lines this widget takes up,
         # including an end empty line
         self.linecount = 4
         self.name_btn = Button(window, self.name, 0, 1, namelen+2)
         self._focus = False
         # if close string is set, it becomes the return value from input routines
         self._close = ""
+        # self._newvalue is the value edited
+        self._newvalue = ""
 
     def close(self, value):
         self._close = value
 
     def value(self):
         return self.vector[self.name]
 
@@ -394,14 +391,17 @@
         if not startline is None:
             self.startline = startline
         displaylabel = shorten(self.vector.memberlabel(self.name), width=self.maxcols-5, placeholder="...")
         self.window.addstr( self.startline, 1, displaylabel, curses.A_BOLD )
         self.name_btn.row = self.startline+1
         self.name_btn.draw()
 
+    def newvalue(self):
+        return self._newvalue
+
 
     def setkey(self, key):
         return key
 
     async def keyinput(self):
         """Waits for a key press,
            if self.control.stop is True, returns 'Stop',
@@ -522,14 +522,16 @@
                 return "focused"
         if key in self.on:
             if self.on.focus:
                 self.on.bold = True
                 self.off.bold = False
                 self.on.draw()
                 self.off.draw()
+                if self.vector.rule != 'AnyOfMany':  ### 'OneOfMany','AtMostOne' both require this to be the only on button
+                    return "set_on"
                 return "focused"
             else:
                 self._focus = True
                 self.on.focus = True
                 self.on.draw()
                 self.off.focus = False
                 self.off.draw()
@@ -577,14 +579,16 @@
         elif self.on.focus:
             if key == 10:                  # 10 return
                 # set on key as bold, off key as standard
                 self.on.bold = True
                 self.off.bold = False
                 self.on.draw()
                 self.off.draw()
+                if self.vector.rule != 'AnyOfMany':  ### 'OneOfMany','AtMostOne' both require this to be the only on button
+                    return "set_on"
             elif key in (338, 339, 258, 259):   # 338 page down, 258 down arrow, 339 page up, 259 up arrow
                 # go to next or previous member widget
                 self.on.focus = False
                 self.on.draw()
                 return key
             elif key in (353, 260): # 353 shift tab, 260 left arrow
                 # back to name_btn
@@ -704,58 +708,54 @@
     def __init__(self, stdscr, control, window, tstatewin, vector, name, namelen=0):
         super().__init__(stdscr, control, window, tstatewin, vector, name, namelen)
         if self.vector.perm == "ro":
             self.linecount = 3
         else:
             self.linecount = 4
         # the newvalue to be edited and sent
-        self._newvalue = self.vector.getformattedvalue(self.name)
+        self._newvalue = self.member.getformattedvalue()
 
                                     # window         text        row col, length of field
         self.edit_txt = Text(self.window, self._newvalue, self.startline+2, self.maxcols-21, txtlen=16)
 
     @property
     def focus(self):
         return self._focus
 
     @focus.setter
     def focus(self, value):
+        "Sets focus to be either False, or if True, set the name_btn focus as True"
         self._focus = value
         self.name_btn.focus = value
         # and regardless of value, set self.edit_txt to False, but check number ok
         if self.edit_txt.focus:
             self.checknumber()
             self.edit_txt.text = self._newvalue
             self.edit_txt.focus = False
 
 
-    def newvalue(self):
-        value = self._newvalue.strip()
-        if len(value) > 16:
-            value = value[:16]
-        return value
-
-
     def reset(self):
         "Reset the widget removing any value updates, called by cancel"
         if self.vector.perm == "ro":
             return
         self._newvalue = self.member.getformattedvalue()
         # draw the value to be edited
-        self.edit_txt.text = self.newvalue()
+        self.edit_txt.text = self._newvalue
         self.edit_txt.draw()
 
 
     def draw(self, startline=None):
         super().draw(startline)
 
         # draw the number value
         text = self.member.getformattedvalue().strip()
         if len(text) > 16:
             text = text[:16]
+        else:
+            text = text.ljust(16)
         # draw the value
         self.window.addstr(self.startline+1, self.maxcols-20, text, curses.A_BOLD)
 
         if self.vector.perm == "ro":
             return
         self.edit_txt.row = self.startline+2
         self.edit_txt.draw()
@@ -843,18 +843,17 @@
                 if key == 353:
                     self.window.noutrefresh()
                     curses.doupdate()
                     return
                 self.window.noutrefresh()
                 curses.doupdate()
                 return 9 # tab key for next item
-            value = editstring.getnumber(key)
-            self._newvalue = value.strip()
+            self._newvalue = editstring.getnumber(key)
             # set new value back into self.edit_txt
-            self.edit_txt.text = value
+            self.edit_txt.text = self._newvalue
             self.edit_txt.draw()
             self.window.noutrefresh()
             editstring.movecurs()
             curses.doupdate()
         curses.curs_set(0)
 
     def checknumber(self):
@@ -927,37 +926,34 @@
     def focus(self, value):
         if self._focus == value:
             return
         self._focus = value
         self.name_btn.focus = value
         self.edit_txt.focus = False
 
-    def newvalue(self):
-        value = self._newvalue.strip()
-        if len(value) > 30:
-            value = value[:30]
-        return value
 
     def reset(self):
         "Reset the widget removing any value updates, called by cancel"
         if self.vector.perm == "ro":
             return
         self._newvalue = self.member.membervalue
         # draw the value to be edited
-        self.edit_txt.text = self.newvalue()
+        self.edit_txt.text = self._newvalue
         self.edit_txt.draw()
 
 
     def draw(self, startline=None):
         super().draw(startline)
 
         # draw the text
-        text = self.member.membervalue.strip()
+        text = self.member.membervalue
         if len(text) > 30:
             text = text[:30]
+        else:
+            text = text.ljust(30)
         # draw the value
         self.window.addstr(self.startline+1, self.maxcols-34, text, curses.A_BOLD)
 
         if self.vector.perm == "ro":
             return
         self.edit_txt.row = self.startline+2
         self.edit_txt.draw()
@@ -1041,18 +1037,17 @@
                 if key == 353:
                     self.window.noutrefresh()
                     curses.doupdate()
                     return
                 self.window.noutrefresh()
                 curses.doupdate()
                 return 9 # tab key for next item
-            value = editstring.gettext(key)
-            self._newvalue = value.strip()
+            self._newvalue = editstring.gettext(key)
             # set new value back into self.edit_txt
-            self.edit_txt.text = value
+            self.edit_txt.text = self._newvalue
             self.edit_txt.draw()
             self.window.noutrefresh()
             editstring.movecurs()
             curses.doupdate()
         curses.curs_set(0)
 
 
@@ -1083,16 +1078,14 @@
 
     def __init__(self, stdscr, control, window, tstatewin, vector, name, namelen=0):
         super().__init__(stdscr, control, window, tstatewin, vector, name, namelen)
         if self.vector.perm == "ro":
             self.linecount = 3
         else:
             self.linecount = 4
-        # the filename to be edited and sent
-        self._newvalue = ""
         # length of editable field, start with nominal 40
                                # window         text        row                col           length of field
         self.edit_txt = Text(self.window, self._newvalue, self.startline+2, self.maxcols-55, txtlen=40)
         self.send_btn = Button(window, "Send", 0, self.maxcols-9, 6)
 
 
     @property
@@ -1113,29 +1106,21 @@
         "Returns filename of last file received and saved"
         nametuple = (self.vector.devicename, self.vector.name, self.name)
         if nametuple in self.control.BLOBfiles:
             return self.control.BLOBfiles[nametuple].name
         else:
             return ""
 
-    def newvalue(self):
-        if not self._newvalue:
-            return ""
-        value = self._newvalue.strip()
-        if len(value) > 40:
-            value = value[:40]
-        return value
-
     def reset(self):
         "Reset the widget removing any value updates, called by cancel"
         if self.vector.perm == "ro":
             return
         self._newvalue = self.member.membervalue
         # draw the value to be edited
-        self.edit_txt.text = self.newvalue()
+        self.edit_txt.text = self._newvalue
         self.edit_txt.draw()
 
 
     def draw(self, startline=None):
         super().draw(startline)
 
         # draw the received file
@@ -1335,16 +1320,15 @@
                 self.edit_txt.draw()
                 self.window.noutrefresh()
                 curses.doupdate()
                 # goes back to the VectorScreen inputs method
                 # which gets a key, and as this widget is still in focus
                 # calls this widgets setkey method
                 return
-            value = editstring.gettext(key)
-            self._newvalue = value.strip()
+            self._newvalue = editstring.gettext(key)
             # set new value back into self.edit_txt
-            self.edit_txt.text = value
+            self.edit_txt.text = self._newvalue
             self.edit_txt.draw()
             self.window.noutrefresh()
             editstring.movecurs()
             curses.doupdate()
         curses.curs_set(0)
```

### Comparing `indipyclient-0.0.2/indipyclient/console/windows.py` & `indipyclient-0.0.4/indipyclient/console/windows.py`

 * *Files 2% similar despite different names*

```diff
@@ -2192,14 +2192,15 @@
 
 
     def draw(self, devicename, groupname, change=False):
 
         # change is a flag to indicate the window needs to be redrawn
 
         if (groupname != self.groupname) or (devicename != self.devicename):
+            self.topindex = 0
             change = True
 
         self.devicename = devicename
         self.device = self.client[devicename]
         self.groupname = groupname
 
         vectornames = [vector.name for vector in self.device.values() if vector.group == self.groupname and vector.enable]
@@ -3296,14 +3297,27 @@
         for index, widget in enumerate(self.displayed):
             result = widget.handlemouse(key)
             # result is "focused' or 'edit' if mouse landed on a field
             if result:
                 windex = index
                 break
 
+
+        if result == "set_on":  ###
+            # special case of a switch widget being turned on
+            # set all other widgets Off
+            for widget in self.memberwidgets:
+                if not widget.focus:
+                    widget.on.bold = False
+                    widget.off.bold = True
+                    widget.on.draw()
+                    widget.off.draw()
+            self.memwin.noutrefresh()
+            return "focused"
+
         if result:
             # remove focus from any other button
             for index, widget in enumerate(self.displayed):
                 if index == windex:
                     continue
                 if widget.focus:
                     widget.focus = False
@@ -3339,14 +3353,26 @@
                     result = widget.setkey(key)
                     if result == "edit":
                         # this sets an input awaitable
                         self._inputfield = widget.inputfield
                         return result
                     else:
                         self._inputfield = None
+                    if result == "set_on":  ###
+                        # special case of a switch widget being turned on
+                        # set all other widgets Off
+                        for widget in self.memberwidgets:
+                            if not widget.focus:
+                                widget.on.bold = False
+                                widget.off.bold = True
+                                widget.on.draw()
+                                widget.off.draw()
+                        self.memwin.noutrefresh()
+                        curses.doupdate()
+                        return
                     if result:
                         # if the widget returns a key. then continue with
                         # checking it
                         key = result
                         break
                     # the widget has handled the key, and returns None
                     # to indicate no further checks required.
```

### Comparing `indipyclient-0.0.2/indipyclient/events.py` & `indipyclient-0.0.4/indipyclient/events.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.2/indipyclient/ipyclient.py` & `indipyclient-0.0.4/indipyclient/ipyclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,20 +85,19 @@
 
 
 class IPyClient(collections.UserDict):
 
     """This class can be used to create your own scripts or client, and provides
        a connection to an INDI service, with parsing of the XML protocol.
        You should create your own class, inheriting from this, and overriding the
-       rxevent method.  Use asyncio.run() to run the asyncrun() method and a call
-       will be made to the given indihost and indiport.
+       rxevent method.
        The argument clientdata provides any named arguments you may wish to pass
        into the object when instantiating it.
-       The IPyClient object is also a mapping of devicename to device object, populated
-       as devices and their vectors are learned from the INDI protocol."""
+       The IPyClient object is also a mapping of devicename to device object, which
+       is populated as devices and their vectors are learned from the INDI protocol."""
 
 
     def __init__(self, indihost="localhost", indiport=7624, **clientdata):
         "An instance of this is a mapping of devicename to device object"
 
         self.indihost = indihost
         self.indiport = indiport
@@ -167,29 +166,31 @@
     def logfp(self):
         "Can be read, but only set via setlogging method"
         return self._logfp
 
     def setlogging(self, level, logfile):
         """Sets the logging level and logfile, returns the level, which will be None on failure.
            As default, the level is None, indicating no logging. Apart from None, level should
-           be an integer, one of 1, 2, 3 or 4"""
+           be an integer, one of 1, 2, 3 or 4
+           Be warned, there is no logfile ration, files can become large.
+           Note: it may be useful in another terminal to try tail -f logfile"""
         try:
             if self._logfp:
                 self._logfp.close()
                 self._logfp = None
 
             if level in (1, 2, 3, 4):
                 self._level = level
             else:
                 self._level = None
                 self._logfile = None
                 return None
 
             logfile = pathlib.Path(logfile).expanduser().resolve()
-            self._logfp = open(logfile, "wb")
+            self._logfp = open(logfile, "wb", buffering=0)
             if not self._logfp.writable():
                 self._logfp.close()
                 self._level = None
                 self._logfp = None
                 self._logfile = None
                 return None
         except:
@@ -211,31 +212,41 @@
             self._logfile = None
         self._stop = True
 
     async def report(self, message):
         """This injects a message into the received data, which will be
            picked up by the rxevent method. It is a way to set a message
            on to your client display, in the same way messages come from
-           the INDI service. If logging is enabled the message will be
-           written to the logfile"""
+           the INDI service. If logging is enabled the message will also
+           be written to the logfile"""
         try:
             timestamp = datetime.now(tz=timezone.utc)
             timestamp = timestamp.replace(tzinfo=None)
             if self._level:
-                reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}" 
+                reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}"
                 self._logfp.write(reportmessage.encode())
             root = ET.fromstring(f"<message timestamp=\"{timestamp.isoformat(sep='T')}\" message=\"{message}\" />")
             event = events.Message(root, None, self)
             await self.rxevent(event)
         except Exception as e:
             if self._level:
                 bytex = "".join(traceback.format_exception(e)).encode()
                 self._logfp.write(bytex)
 
 
+    def log(self, message):
+        """If logging is enabled, this writes the message, with a timestamp
+           to the logfile"""
+        if self._level:
+            timestamp = datetime.now(tz=timezone.utc)
+            timestamp = timestamp.replace(tzinfo=None)
+            reportmessage  = f"\n{timestamp.isoformat(sep='T')} {message}"
+            self._logfp.write(reportmessage.encode())
+
+
     def enabledlen(self):
         "Returns the number of enabled devices"
         return sum(map(lambda x:1 if x.enable else 0, self.data.values()))
 
 
     def __setitem__(self, device):
         "Devices are added by being learnt from the driver, they cannot be manually added"
@@ -261,14 +272,16 @@
                                          self._run_rx(reader),
                                          self._check_alive(writer)
                                          )
                 except ConnectionRefusedError:
                     await self.report(f"Error: Connection refused on {self.indihost}:{self.indiport}")
                 except ConnectionResetError:
                     await self.report("Error: Connection Lost")
+                except Exception:
+                    await self.report("Error: Connection failed")
                 self._clear_connection()
                 if self._stop:
                     break
                 else:
                     await self.report(f"Connection failed, re-trying...")
 
                 # wait five seconds before re-trying, but keep checking
@@ -649,18 +662,17 @@
             elif propertyvector.vectortype == "BLOBVector":
                 propertyvector.send_newBLOBVector(timestamp, members)
         except KeyboardInterrupt:
             self.shutdown()
 
     def set_vector_timeouts(self, timeout_enable=None, timeout_min=None, timeout_max=None):
         """Whenever you send updated values, a timer is started and if a timeout occurs
-           before the server responds with a new vector setting, a VectorTimeOut event
-           will be created, which you could choose to ignore, or take action such as
-           setting a vector Alert flag.
-           The protocol allows the server to set a timeout for each vector, this method
+           before the server responds, a VectorTimeOut event will be created, which you
+           could choose to ignore, or take action such as setting an Alert flag.
+           The protocol allows the server to suggest a timeout for each vector. This method
            allows you to set minimum and maximum timeouts, which should be given as integer
            values. If any parameter is not provided (left at None) then that value will not be
            changed. If timeout_enable is set to False, no VectorTimeOut events will occur.
            As default, timeouts are enabled, minimum is set to 2 seconds, maximum 10 seconds."""
         if not timeout_enable is None:
             self.vector_timeout_enable = timeout_enable
         if not timeout_min is None:
@@ -713,15 +725,14 @@
             if self._level:
                 bytex = "".join(traceback.format_exception(e)).encode()
                 self._logfp.write(bytex)
         finally:
             self.shutdown()
 
 
-
     def send_getProperties(self, devicename=None, vectorname=None):
         """Sends a getProperties request. On startup the IPyClient object
            will automatically send getProperties, so typically you will
            not have to use this method."""
         if self.connected:
             xmldata = ET.Element('getProperties')
             xmldata.set("version", "1.7")
@@ -752,15 +763,15 @@
         """Override this.
            On receiving data, this is called, and should handle any necessary actions.
            event is an object with attributes according to the data received."""
         pass
 
 
     async def asyncrun(self):
-        """Runs this object to start communications."""
+        "Await this method to run the client."
         self._stop = False
         await asyncio.gather(self._comms(), self._rxhandler(), self._timeout_monitor(), return_exceptions=True)
         self.stopped = True
 
 
 class Device(collections.UserDict):
```

### Comparing `indipyclient-0.0.2/indipyclient/propertymembers.py` & `indipyclient-0.0.4/indipyclient/propertymembers.py`

 * *Files 10% similar despite different names*

```diff
@@ -121,21 +121,21 @@
     def __init__(self, name, label=None, format='', min='0', max='0', step='0', membervalue='0'):
         super().__init__(name, label, membervalue)
         self.format = format
         self.min = min
         self.max = max
         self.step = step
 
-
     def getfloatvalue(self):
         """The INDI spec allows a number of different number formats, this method returns
            this members value as a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
         return self.getfloat(self._membervalue)
 
+
     def getfloat(self, value):
         """The INDI spec allows a number of different number formats, given a number,
            this returns a float.
            If an error occurs while parsing the number, a TypeError exception is raised."""
         try:
             if isinstance(value, float):
                 return value
@@ -146,109 +146,142 @@
             # negative is True, if the value is negative
             value = value.strip()
             negative = value.startswith("-")
             if negative:
                 value = value.lstrip("-")
             # Is the number provided in sexagesimal form?
             if value == "":
-                parts = [0, 0, 0]
+                parts = ["0", "0", "0"]
             elif " " in value:
                 parts = value.split(" ")
             elif ":" in value:
                 parts = value.split(":")
             elif ";" in value:
                 parts = value.split(";")
             else:
                 # not sexagesimal
                 parts = [value, "0", "0"]
+            if len(parts) > 3:
+                raise TypeError
             # Any missing parts should have zero
+            if len(parts) == 1:
+                parts.append("0")
+                parts.append("0")
             if len(parts) == 2:
-                # assume seconds are missing, set to zero
                 parts.append("0")
             assert len(parts) == 3
-            number_strings = list(x if x else "0" for x in parts)
-            # convert strings to integers or floats
-            number_list = []
-            for part in number_strings:
-                try:
-                    num = int(part)
-                except ValueError:
-                    num = float(part)
-                number_list.append(num)
-            floatvalue = number_list[0] + (number_list[1]/60) + (number_list[2]/360)
+            # a part could be empty string, ie if 2:5: is given
+            numbers = list(float(x) if x else 0.0 for x in parts)
+            floatvalue = numbers[0] + (numbers[1]/60) + (numbers[2]/3600)
             if negative:
                 floatvalue = -1 * floatvalue
         except:
             raise TypeError("Error: Unable to parse number value")
         return floatvalue
 
 
     def getformattedvalue(self):
-        """This method returns this members value as a float."""
+        """This method returns this members value as a string float."""
         return self.getformattedstring(self._membervalue)
 
 
     def getformattedstring(self, value):
         """Given a number this returns a formatted string"""
-        value = self.getfloat(value)
-        if (not self.format.startswith("%")) or (not self.format.endswith("m")):
-            return self.format % value
-        # sexagesimal format
-        if value<0:
-            negative = True
-            value = abs(value)
-        else:
-            negative = False
-        # number list will be degrees, minutes, seconds
-        number_list = [0,0,0]
-        if isinstance(value, int):
-            number_list[0] = value
-        else:
-            # get integer part and fraction part
-            fractdegrees, degrees = math.modf(value)
-            number_list[0] = int(degrees)
-            mins = 60*fractdegrees
-            fractmins, mins = math.modf(mins)
-            number_list[1] = int(mins)
-            number_list[2] = 60*fractmins
-
-        # so number list is a valid degrees, minutes, seconds
-        # degrees
-        if negative:
-            number = f"-{number_list[0]}:"
-        else:
-            number = f"{number_list[0]}:"
-        # format string is of the form  %<w>.<f>m
-        w,f = self.format.split(".")
-        w = w.lstrip("%")
-        f = f.rstrip("m")
-        if (f == "3") or (f == "5"):
-            # no seconds, so create minutes value
-            minutes = float(number_list[1]) + number_list[2]/60.0
-            if f == "5":
-                number += f"{minutes:04.1f}"
-            else:
-                number += f"{minutes:02.0f}"
-        else:
-            number += f"{number_list[1]:02d}:"
-            seconds = float(number_list[2])
-            if f == "6":
-                number += f"{seconds:02.0f}"
-            elif f == "8":
-                number += f"{seconds:04.1f}"
+        try:
+            value = self.getfloat(value)
+            if (not self.format.startswith("%")) or (not self.format.endswith("m")):
+                return self.format % value
+            # sexagesimal
+            # format string is of the form  %<w>.<f>m
+            w,f = self.format.split(".")
+            w = w.lstrip("%")
+            f = f.rstrip("m")
+
+            if value<0:
+                negative = True
             else:
-                number += f"{seconds:05.2f}"
+                negative = False
+            absvalue = abs(value)
+
+            # get integer part and fraction part
+            degrees = math.floor(absvalue)
+            minutes = (absvalue - degrees) * 60.0
 
-        # w is the overall length of the string, prepend with spaces to make the length up to w
-        w = int(w)
-        l = len(number)
-        if w>l:
-            number = " "*(w-l) + number
-        return number
+            if f == "3":   # three fractional values including the colon ":mm"
+                # create nearest integer minutes
+                minutes = round(minutes)
+                if minutes == 60:
+                    minutes = 0
+                    degrees = degrees + 1
+                valstring = f"{'-' if negative else ''}{degrees}:{minutes:02d}"
+                # w is the overall length of the string, prepend with spaces to make the length up to w
+                if w:
+                    return valstring.rjust(int(w), ' ')
+                # it is possible w is an empty string
+                return valstring
+
+            if f == "5":  # five fractional values including the colon and decimal point ":mm.m"
+                minutes = round(minutes,1)
+                if minutes == 60.0:
+                    minutes = 0.0
+                    degrees = degrees + 1
+                valstring = f"{'-' if negative else ''}{degrees}:{minutes:04.1f}"
+                if w:
+                    return valstring.rjust(int(w), ' ')
+                return valstring
+
+            integerminutes = math.floor(minutes)
+            seconds = (minutes - integerminutes) * 60.0
+
+            if f == "6":    # six fractional values including two colons ":mm:ss"
+                seconds = round(seconds)
+                if seconds == 60:
+                    seconds = 0
+                    integerminutes = integerminutes + 1
+                    if integerminutes == 60:
+                        integerminutes = 0
+                        degrees = degrees + 1
+                valstring = f"{'-' if negative else ''}{degrees}:{integerminutes:02d}:{seconds:02d}"
+                if w:
+                    return valstring.rjust(int(w), ' ')
+                return valstring
+
+
+            if f == "8":    # eight fractional values including two colons and decimal point ":mm:ss.s"
+                seconds = round(seconds,1)
+                if seconds == 60.0:
+                    seconds = 0.0
+                    integerminutes = integerminutes + 1
+                    if integerminutes == 60:
+                        integerminutes = 0
+                        degrees = degrees + 1
+                valstring = f"{'-' if negative else ''}{degrees}:{integerminutes:02d}:{seconds:04.1f}"
+                if w:
+                    return valstring.rjust(int(w), ' ')
+                return valstring
+
+            fn = int(f)
+            if fn>8 and fn<15:    # make maximum of 14
+                seconds = round(seconds,1)
+                if seconds == 60.0:
+                    seconds = 0.0
+                    integerminutes = integerminutes + 1
+                    if integerminutes == 60:
+                        integerminutes = 0
+                        degrees = degrees + 1
+                valstring = f"{'-' if negative else ''}{degrees}:{integerminutes:02d}:{seconds:0{fn-4}.{fn-7}f}"
+                if w:
+                    return valstring.rjust(int(w), ' ')
+                return valstring
+
+        except:
+            raise TypeError("Error: Unable to parse number value")
 
+        # no other options accepted
+        raise TypeError("Error: Unable to process number format")
 
 
 class NumberMember(ParentNumberMember):
     """Contains a number, the attributes inform the client how the number should be
        displayed.
 
        format is a C printf style format, for example %7.2f means the client should
```

### Comparing `indipyclient-0.0.2/indipyclient/propertyvectors.py` & `indipyclient-0.0.4/indipyclient/propertyvectors.py`

 * *Files identical despite different names*

### Comparing `indipyclient-0.0.2/pyproject.toml` & `indipyclient-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "indipyclient"
 authors = [{name = "Bernard Czenkusz", email = "bernie@skipole.co.uk"}]
 license = {file = "LICENSE"}
 classifiers = ["License :: OSI Approved :: MIT License", "Operating System :: POSIX :: Linux","Topic :: Scientific/Engineering :: Astronomy", "Topic :: Scientific/Engineering :: Interface Engine/Protocol Translator"]
-version = "0.0.2"
+version = "0.0.4"
 description="Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol."
 readme = "README.md"
 requires-python = ">=3.10"
 keywords=['indi', 'client', 'astronomy', 'instrument']
 
 [project.urls]
 Documentation = "https://indipyclient.readthedocs.io"
```

### Comparing `indipyclient-0.0.2/PKG-INFO` & `indipyclient-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: indipyclient
-Version: 0.0.2
+Version: 0.0.4
 Summary: Pure python package, providing a terminal client and a set of classes which can be used to create scripts or clients to control remote instruments using the INDI protocol.
 Keywords: indi,client,astronomy,instrument
 Author-email: Bernard Czenkusz <bernie@skipole.co.uk>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

