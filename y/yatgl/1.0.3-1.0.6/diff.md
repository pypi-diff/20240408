# Comparing `tmp/yatgl-1.0.3.tar.gz` & `tmp/yatgl-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yatgl-1.0.3.tar", last modified: Tue Mar 26 03:45:56 2024, max compression
+gzip compressed data, was "yatgl-1.0.6.tar", last modified: Sun Apr  7 22:37:44 2024, max compression
```

## Comparing `yatgl-1.0.3.tar` & `yatgl-1.0.6.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-03-26 03:45:56.284180 yatgl-1.0.3/
--rw-rw-rw-   0        0        0    35821 2024-03-24 09:04:50.000000 yatgl-1.0.3/LICENSE
--rw-rw-rw-   0        0        0      585 2024-03-26 03:45:56.283160 yatgl-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      241 2024-03-24 23:02:09.000000 yatgl-1.0.3/README.md
--rw-rw-rw-   0        0        0       42 2024-03-26 03:45:56.284180 yatgl-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1333 2024-03-26 03:42:10.000000 yatgl-1.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-26 03:45:56.270159 yatgl-1.0.3/yatgl/
--rw-rw-rw-   0        0        0      756 2024-03-26 03:32:21.000000 yatgl-1.0.3/yatgl/__init__.py
--rw-rw-rw-   0        0        0    12428 2024-03-26 03:45:19.000000 yatgl-1.0.3/yatgl/client.py
-drwxrwxrwx   0        0        0        0 2024-03-26 03:45:56.281777 yatgl-1.0.3/yatgl.egg-info/
--rw-rw-rw-   0        0        0      585 2024-03-26 03:45:56.000000 yatgl-1.0.3/yatgl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2024-03-26 03:45:56.000000 yatgl-1.0.3/yatgl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-26 03:45:56.000000 yatgl-1.0.3/yatgl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2024-03-24 08:52:15.000000 yatgl-1.0.3/yatgl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       38 2024-03-26 03:45:56.000000 yatgl-1.0.3/yatgl.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-03-26 03:45:56.000000 yatgl-1.0.3/yatgl.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-07 22:37:44.526601 yatgl-1.0.6/
+-rw-rw-rw-   0        0        0    35821 2024-03-24 09:04:50.000000 yatgl-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      585 2024-04-07 22:37:44.525373 yatgl-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      241 2024-03-24 23:02:09.000000 yatgl-1.0.6/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-07 22:37:44.526601 yatgl-1.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1333 2024-04-02 04:17:37.000000 yatgl-1.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:37:44.511374 yatgl-1.0.6/yatgl/
+-rw-rw-rw-   0        0        0      756 2024-03-26 03:32:21.000000 yatgl-1.0.6/yatgl/__init__.py
+-rw-rw-rw-   0        0        0    14014 2024-04-02 04:32:54.000000 yatgl-1.0.6/yatgl/client.py
+drwxrwxrwx   0        0        0        0 2024-04-07 22:37:44.525373 yatgl-1.0.6/yatgl.egg-info/
+-rw-rw-rw-   0        0        0      585 2024-04-07 22:37:44.000000 yatgl-1.0.6/yatgl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      232 2024-04-07 22:37:44.000000 yatgl-1.0.6/yatgl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-07 22:37:44.000000 yatgl-1.0.6/yatgl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2024-03-24 08:52:15.000000 yatgl-1.0.6/yatgl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       38 2024-04-07 22:37:44.000000 yatgl-1.0.6/yatgl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2024-04-07 22:37:44.000000 yatgl-1.0.6/yatgl.egg-info/top_level.txt
```

### Comparing `yatgl-1.0.3/LICENSE` & `yatgl-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `yatgl-1.0.3/PKG-INFO` & `yatgl-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatgl
-Version: 1.0.3
+Version: 1.0.6
 Summary: An asynchronous NationStates Telegram API library.
 Home-page: https://github.com/NotAName320/yatgl
 Author: Nota
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp[speedups]
```

### Comparing `yatgl-1.0.3/setup.py` & `yatgl-1.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from setuptools import setup
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(name='yatgl',
-      version='1.0.3',
+      version='1.0.6',
       description='An asynchronous NationStates Telegram API library.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/NotAName320/yatgl',
       author='Nota',
       license='GPLv3',
       packages=['yatgl'],
```

### Comparing `yatgl-1.0.3/yatgl/__init__.py` & `yatgl-1.0.6/yatgl/__init__.py`

 * *Files identical despite different names*

### Comparing `yatgl-1.0.3/yatgl/client.py` & `yatgl-1.0.6/yatgl/client.py`

 * *Files 14% similar despite different names*

```diff
@@ -15,23 +15,25 @@
 You should have received a copy of the GNU General Public License
 along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import asyncio
 from collections import deque
 from collections.abc import Iterable
+from contextlib import asynccontextmanager
+from dataclasses import dataclass
 from enum import Enum
 from logging import getLogger
 from typing import NamedTuple
 
 import aiohttp
 from bs4 import BeautifulSoup
 
 API_URL = 'https://www.nationstates.net/cgi-bin/api.cgi'
-VERSION = '1.0.3'
+VERSION = '1.0.6'
 
 
 logger = getLogger(__name__)
 
 
 class Template(NamedTuple):
     secret_key: str
@@ -39,27 +41,34 @@
 
 
 class TelegramRequest(NamedTuple):
     template: Template
     recipient: str
 
 
-class UserAgent(NamedTuple):
+@dataclass
+class UserAgent:
     nation_name: str
     script_name: str
     script_version: str
 
+    def __str__(self):
+        return (f'yatgl v{VERSION} Developed by nation=Notanam, used by nation={self.nation_name} in '
+                f'script={self.script_name} v{self.script_version}')
+
 
 class NationGroup(Enum):
     NEW_WA_MEMBERS = 0
     ALL_WA_MEMBERS = 1
     NEW_FOUNDS = 2
     ALL_WA_DELEGATES = 3
     NEW_REGION_MEMBERS = 4
     ALL_REGION_MEMBERS = 5
+    DELEGATES_APPROVING = 7
+    DELEGATES_NOT_APPROVING = 9
 
 
 class _ClientMeta(type):
     """
     Singleton metaclass for Client, making sure that two action queues never exist at once
 
     Not meant to be externally instantiated.
@@ -106,18 +115,15 @@
         this for recruitment telegrams.
         """
         if 'client_key' in kwargs:
             self.client_key = kwargs.pop('client_key')
         if 'user_agent' in kwargs:
             self.user_agent = kwargs.pop('user_agent')
             if self._session:
-                self._session.headers['User-Agent'] = (f'yatgl v{VERSION} Developed by nation=Notanam, used by '
-                                                       f'nation={self.user_agent.nation_name} in '
-                                                       f'script={self.user_agent.script_name} '
-                                                       f'v{self.user_agent.script_version}')
+                self._session.headers['User-Agent'] = str(self.user_agent)
         if 'delay' in kwargs:
             delay = kwargs.pop('delay')
             if delay < 30:
                 raise ValueError('Delay can\'t be less than 30.')
             self.delay = delay
 
     def queue_tg(self, template: Template, recipient: str):
@@ -136,20 +142,18 @@
         Ensure that a client key has been provided.
         """
         if not self.client_key:
             raise AttributeError('No client key provided.')
         if not self.user_agent:
             raise AttributeError('Please set a User Agent.')
         if not self._tg_task:
-            self._tg_task = asyncio.create_task(self._process_stack())
+            self._tg_task = asyncio.create_task(self._process_queue())
             if not self._session or self._session.closed:
                 headers = {
-                    'User-Agent': f'yatgl v{VERSION} Developed by nation=Notanam, '
-                                  f'used by nation={self.user_agent.nation_name} in '
-                                  f'script={self.user_agent.script_name} v{self.user_agent.script_version}'
+                    'User-Agent': str(self.user_agent)
                 }
                 self._session = aiohttp.ClientSession(headers=headers)
             await self._tg_task
 
     async def stop(self):
         """
         Stops sending telegrams and/or queueing if the client has started, otherwise does nothing.
@@ -157,39 +161,38 @@
         if self._tg_task:
             self._tg_task.cancel()
             for task in self._queueing_tasks:
                 task.cancel()
             await self._session.close()
             self._tg_task, self._queueing_tasks = None, []
 
-    async def mass_telegram(self, template: Template, group: NationGroup, region: Iterable[str] = None):
+    async def mass_telegram(self, template: Template, group: NationGroup, *, regions: str | Iterable[str] = None,
+                            proposal: str = None):
         """
         Starts the telegram queue while autoqueueing a certain group of nations using the API.
 
         Ensure that a client key has been provided.
-
-        Note that when getting these nations, the client ignores ratelimits, which should be fine for most cases as
-        the requests are sparse enough that they're well under, but might break e.g. if targeting nations joining one of
-        50 regions, in which it may be time to reevaluate your region's foreign policy.
         :param template: The template to send to the nations.
         :param group: The group of nations to target specified by the enum :class:`NationGroup`.
-        :param region: A list of regions.
+        :param regions: A list of regions.
+        :param proposal: A proposal ID.
         """
         if not self._session or self._session.closed:
             headers = {
-                'User-Agent': f'yatgl v{VERSION} Developed by nation=Notanam, '
-                              f'used by nation={self.user_agent.nation_name} in script={self.user_agent.script_name} '
-                              f'v{self.user_agent.script_version}'
+                'User-Agent': str(self.user_agent)
             }
             self._session = aiohttp.ClientSession(headers=headers)
-        task = asyncio.create_task(self._mass_queue(template, group, region))
+        task = asyncio.create_task(self._mass_queue(template, group, regions, proposal))
         self._queueing_tasks.append(task)
         await asyncio.gather(self.start(), task)
 
-    async def _mass_queue(self, template: Template, group: NationGroup, regions: str | Iterable[str] | None):
+    async def _mass_queue(self, template: Template, group: NationGroup, regions: str | Iterable[str] | None,
+                          proposal: str | None):
+        if group in {NationGroup.DELEGATES_APPROVING, NationGroup.DELEGATES_NOT_APPROVING} and not proposal:
+            raise AttributeError('Proposal ID not provided to client.')
         if group in {NationGroup.ALL_REGION_MEMBERS, NationGroup.NEW_REGION_MEMBERS} and not regions:
             raise AttributeError('Region(s) not provided to client.')
         elif isinstance(regions, str):
             regions = [regions]
 
         # why did i code it like this?
         if group.value % 2 == 1:
@@ -203,14 +206,24 @@
                 case NationGroup.ALL_WA_MEMBERS:
                     for nation in await self._get_wa_members():
                         self.queue_tg(template, nation)
 
                 case NationGroup.ALL_WA_DELEGATES:
                     for nation in await self._get_wa_delegates():
                         self.queue_tg(template, nation)
+
+                case NationGroup.DELEGATES_APPROVING:
+                    for nation in await self._get_proposal_delegates_approving(proposal):
+                        self.queue_tg(template, nation)
+
+                case NationGroup.DELEGATES_NOT_APPROVING:
+                    all_delegates_approving = set(await self._get_proposal_delegates_approving(proposal))
+                    for nation in await self._get_wa_delegates():
+                        if nation not in all_delegates_approving:
+                            self.queue_tg(template, nation)
         else:
             # generate a list of nations to not send messages to
             existing = set()
             if group is NationGroup.NEW_REGION_MEMBERS:
                 for region in regions:
                     existing.update(await self._get_region_members(region))
             elif group is NationGroup.NEW_WA_MEMBERS:
@@ -241,48 +254,80 @@
 
     async def _get_region_members(self, region: str) -> list[str]:
         data = {
             'q': 'nations',
             'region': region
         }
 
-        async with self._session.post(API_URL, data=data) as resp:
+        async with self._api_request_wait(API_URL, data=data) as resp:
             parsed = BeautifulSoup(await resp.text(), 'xml')
             return parsed.REGION.NATIONS.string.split(':')
 
     async def _get_wa_members(self) -> list[str]:
         data = {
             'q': 'members',
             'wa': '1'
         }
 
-        async with self._session.post(API_URL, data=data) as resp:
+        async with self._api_request_wait(API_URL, data=data) as resp:
             parsed = BeautifulSoup(await resp.text(), 'xml')
             return parsed.WA.MEMBERS.string.split(',')
 
     async def _get_wa_delegates(self) -> list[str]:
         data = {
             'q': 'delegates',
             'wa': '1'
         }
 
-        async with self._session.post(API_URL, data=data) as resp:
+        async with self._api_request_wait(API_URL, data=data) as resp:
             parsed = BeautifulSoup(await resp.text(), 'xml')
             return parsed.WA.DELEGATES.string.split(',')
 
     async def _get_new_founds(self) -> list[str]:
         data = {
             'q': 'newnations'
         }
 
-        async with self._session.post(API_URL, data=data) as resp:
+        async with self._api_request_wait(API_URL, data=data) as resp:
             parsed = BeautifulSoup(await resp.text(), 'xml')
             return parsed.WORLD.NEWNATIONS.string.split(',')
 
-    async def _process_stack(self):
+    async def _get_proposal_delegates_approving(self, proposal: str, council='1') -> list[str]:
+        data = {
+            'q': 'proposals',
+            'wa': council
+        }
+
+        async with self._api_request_wait(API_URL, data=data) as resp:
+            parsed = BeautifulSoup(await resp.text(), 'xml')
+            proposal_xml = parsed.find(id=proposal)
+            if proposal_xml:
+                return proposal_xml.APPROVALS.string.split(':')
+
+        if council == '1':
+            return await self._get_proposal_delegates_approving(proposal, '2')
+        else:
+            return []
+
+    @asynccontextmanager
+    async def _api_request_wait(self, url: str, data: dict):
+        while True:
+            async with self._session.post(url, data=data) as resp:
+                if resp.status == 429:
+                    retry_after = int(resp.headers['Retry-After'])
+                    logger.warning(f'Hit normal API rate limit! Retrying in {retry_after}...')
+                    await asyncio.sleep(retry_after)
+                else:
+                    if remaining := int(resp.headers['RateLimit-Remaining']) <= 7:
+                        logger.info('Getting close to rate limit, slowing down requests a bit...')
+                        await asyncio.sleep(int(resp.headers['RateLimit-Reset']) / remaining)
+                    yield resp
+                    break
+
+    async def _process_queue(self):
         while True:
             if self.queue:
                 await self._send_tg(self.queue.pop())
                 await asyncio.sleep(self.delay)
             # so it doesn't block our async queue
             await asyncio.sleep(0)
```

### Comparing `yatgl-1.0.3/yatgl.egg-info/PKG-INFO` & `yatgl-1.0.6/yatgl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yatgl
-Version: 1.0.3
+Version: 1.0.6
 Summary: An asynchronous NationStates Telegram API library.
 Home-page: https://github.com/NotAName320/yatgl
 Author: Nota
 License: GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: aiohttp[speedups]
```

