# Comparing `tmp/hltv_async_api-0.4.1.tar.gz` & `tmp/hltv_async_api-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hltv_async_api-0.4.1.tar", last modified: Thu Apr  4 14:29:38 2024, max compression
+gzip compressed data, was "hltv_async_api-0.4.2.tar", last modified: Mon Apr  8 18:01:29 2024, max compression
```

## Comparing `hltv_async_api-0.4.1.tar` & `hltv_async_api-0.4.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 14:29:38.761338 hltv_async_api-0.4.1/
--rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.1/LICENSE
--rw-rw-rw-   0        0        0     5751 2024-04-04 14:29:38.759272 hltv_async_api-0.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5128 2024-04-04 03:09:51.000000 hltv_async_api-0.4.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-04 14:29:38.696456 hltv_async_api-0.4.1/hltv_async_api/
--rw-rw-rw-   0        0        0      124 2024-04-04 14:29:35.000000 hltv_async_api-0.4.1/hltv_async_api/__init__.py
--rw-rw-rw-   0        0        0    30473 2024-04-04 14:28:48.000000 hltv_async_api-0.4.1/hltv_async_api/aiohltv.py
-drwxrwxrwx   0        0        0        0 2024-04-04 14:29:38.757089 hltv_async_api-0.4.1/hltv_async_api.egg-info/
--rw-rw-rw-   0        0        0     5751 2024-04-04 14:29:38.000000 hltv_async_api-0.4.1/hltv_async_api.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2024-04-04 14:29:38.000000 hltv_async_api-0.4.1/hltv_async_api.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-04 14:29:38.000000 hltv_async_api-0.4.1/hltv_async_api.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       15 2024-04-04 14:29:38.000000 hltv_async_api-0.4.1/hltv_async_api.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      537 2024-04-04 14:29:35.000000 hltv_async_api-0.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-04 14:29:38.761397 hltv_async_api-0.4.1/setup.cfg
--rw-rw-rw-   0        0        0      922 2024-04-04 14:29:35.000000 hltv_async_api-0.4.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.783122 hltv_async_api-0.4.2/
+-rw-rw-rw-   0        0        0     1091 2024-04-02 00:22:12.000000 hltv_async_api-0.4.2/LICENSE
+-rw-rw-rw-   0        0        0     8671 2024-04-08 18:01:29.782120 hltv_async_api-0.4.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8048 2024-04-08 17:31:52.000000 hltv_async_api-0.4.2/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.723698 hltv_async_api-0.4.2/hltv_async_api/
+-rw-rw-rw-   0        0        0      124 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/hltv_async_api/__init__.py
+-rw-rw-rw-   0        0        0    33610 2024-04-08 17:31:52.000000 hltv_async_api-0.4.2/hltv_async_api/aiohltv.py
+drwxrwxrwx   0        0        0        0 2024-04-08 18:01:29.780125 hltv_async_api-0.4.2/hltv_async_api.egg-info/
+-rw-rw-rw-   0        0        0     8671 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       15 2024-04-08 18:01:29.000000 hltv_async_api-0.4.2/hltv_async_api.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      537 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 18:01:29.784122 hltv_async_api-0.4.2/setup.cfg
+-rw-rw-rw-   0        0        0      922 2024-04-08 18:01:25.000000 hltv_async_api-0.4.2/setup.py
```

### Comparing `hltv_async_api-0.4.1/LICENSE` & `hltv_async_api-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hltv_async_api-0.4.1/hltv_async_api/aiohltv.py` & `hltv_async_api-0.4.2/hltv_async_api/aiohltv.py`

 * *Files 10% similar despite different names*

```diff
@@ -159,39 +159,41 @@
                 result = await response.text()
                 if await self._cloudflare_check(result):
                     return False, await self._parse_error_handler(delay)
 
                 return True, result
         except (ClientProxyConnectionError, ClientResponseError, ClientOSError,
                 ServerDisconnectedError, TimeoutError, ClientHttpProxyError) as e:
+            self.logger.debug(e)
             delay = await self._parse_error_handler(delay)
             return False, delay
 
     async def _fetch(self, url, delay: int = 0):
         if not self.session:
             await self._create_session()
 
         status = False
         try_ = 1
         result = None
-        while not status and (try_ != self.max_retries):
+        while (not status) and (try_ != self.max_retries):
             self.logger.debug(f'Trying connect to {url}, try {try_}/{self.max_retries}')
 
             # if status = True, result = page,
             # if status = False result = delay (default=0)
             status, result = await self._parse(url, delay)
 
             if not status and result:
                 delay = result
             try_ += 1
 
         # After Parse
         if not self.TRUE_SESSION:
             # Automaticaly close session after parse
             await self.close_session()
+            self.session = None
 
         if status:
             loop = get_running_loop()
             parsed = await loop.run_in_executor(None, partial(self._f, result))
             return parsed
         else:
             self.logger.error('Connection failed')
@@ -208,31 +210,46 @@
             'May': '5', 'Jun': '6', 'Jul': '7', 'Aug': '8',
             'Sep': '9', 'Oct': '10', 'Nov': '11', 'Dec': '12'
         }
         month = month_abbreviations[parts[0]]
         day = parts[1][:-2]
         return day + '-' + month
 
-    # TODO rewrite
-    async def get_live_matches(self):
+    async def get(self, type: str, id: int | str | None = None,
+                  title: str | None = None,
+                  team1: str | None = None,
+                  team2: str | None = None):
+        if type == 'event':
+            if id:
+                return await self.get_event_info(id, title)
+            else:
+                return await self.get_events()
+        elif type == 'match':
+            if id:
+                return await self.get_match_info(str(id), team1, team2, title)
+            else:
+                return await self.get_upcoming_matches()
+        elif type == 'news':
+            return await self.get_last_news()
+        elif type == 'team':
+            if id:
+                return await self.get_team_info(id, title)
+            else:
+                return await self.get_top_teams()
+
+    async def get_live_matches(self, max_ = 10):
         """returns a list of all LIVE matches on HLTV along with the maps being played and the star ratings"""
         r = await self._fetch("https://www.hltv.org/matches")
         if not r:
             return
 
         live_matches = r.find("div", {'class', "liveMatchesContainer"})
-        if live_matches is None:
-            return []
-        else:
-            teams = [line.getText() for line in live_matches.find_all("div", {'class', "matchTeamName text-ellipsis"})]
-            matches = [(team1, team2) for team1, team2 in tuple(zip(teams, teams[1:]))[::2]]
-            liveMatchContainer = live_matches.find_all("div", {'class', "liveMatch-container"})
-            maps = [str(line.get('data-maps')).split(',') for line in liveMatchContainer]
-            stars = [line.get('stars') for line in liveMatchContainer]
-            return [{'teams': teams, 'maps': maps, 'stars': stars} for teams, maps, stars in zip(matches, maps, stars)]
+
+        #cant find a way, mby use socketio by hltv-score-bot ?? | other url ?
+
 
     async def get_upcoming_matches(self, days: int = 7, min_rating: int = 1):
         """returns a list of all upcoming matches on HLTV"""
         r = await self._fetch("https://www.hltv.org/matches")
         if not r:return
 
         matches = []
@@ -284,21 +301,21 @@
                     'date': date_,
                     'matches': matches_today
                 })
         except AttributeError:
             return None
         return matches
 
-
     async def get_match_info(self, match_id: str, team1: str, team2: str, event_title: str, stats: bool = True):
         r = await self._fetch(f"https://www.hltv.org/matches/{match_id}/"
                              f"{team1.replace(' ', '-')}-vs-"
                              f"{team2.replace(' ', '-')}-"
                              f"{event_title.replace(' ', '-')}")
-
+        if not r:
+            return
 
         status = r.find('div', {'class': 'countdown'}).text
 
         score1, score2 = 0, 0
 
         if status == 'Match over':
             scores = r.find_all('div', class_='team')
@@ -334,15 +351,31 @@
                         'id': player_id,
                         'name': nickname,
                         'kd': kd,
                         'adr': adr,
                         'rating': rating
                     })
 
-        return match_id, score1, score2, status, maps, stats
+        if status == "LIVE":
+            for map in maps:
+                if map["r_team1"] == '13':
+                    if len(map) != 1:
+                        score1 += 1
+                    else:
+                        score1 = 13
+                        score2 = int(map["r_team2"])
+
+                elif map["r_team1"] == '13':
+                    if len(map) != 1:
+                        score2 += 1
+                    else:
+                        score2 = 13
+                        score1 = int(map["r_team1"])
+
+        return match_id, score1, score2, status, maps, stats_
 
 
     async def get_big_results(self, offset=0) -> list[dict[str, Any]] | None:
         """returns a list of big event matches results"""
         r = await self._fetch("https://www.hltv.org/results?offset=" + str(offset))
         if not r:
             return
@@ -397,89 +430,129 @@
                 })
             match_results.append({
                 'date': date,
                 'matches': match_date,
             })
         return match_results
 
-    async def get_event_matches(self, event_id: str | int):
+    async def get_event_matches(self, event_id: str | int, days: int = 1):
         r = await self._fetch("https://www.hltv.org/events/" + str(event_id) + "/matches")
         if not r:
             return
 
         live_matches: List | Any
         matches = []
         try:
-            live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div", {'class', 'liveMatch'})
+            live_matches = r.find("div", {'class', 'liveMatchesSection'}).find_all("div", {'class', 'liveMatch-container'})
         except AttributeError:
             live_matches = []
         live_mat = []
         for live in live_matches:
             id_ = live.find('a', {'class': 'match a-reset'})['href'].split('/')[2]
             teams = live.find_all("div", class_="matchTeamName text-ellipsis")
             team1 = teams[0].text.strip()
             team2 = teams[1].text.strip()
+            t1_id = live['team1']
+            t2_id = live['team2']
+
 
             # TODO FIX SCORES
-            try:
+            """try:
                 scores = live.find("td", class_="matchTeamScore").text.strip().split('-')
                 score_team1 = scores[0].strip()
                 score_team2 = scores[1].strip()
             except AttributeError:
                 score_team1 = 0
-                score_team2 = 0
+                score_team2 = 0"""
 
             live_mat.append({
                 'id': id_,
                 'team1': team1,
                 'team2': team2,
+                't1_id': t1_id,
+                't2_id': t2_id
             })
 
         matches.append({
             'date': 'LIVE',
             'matches': live_mat,
         })
-
         for date_sect in r.find_all('div', {'class': 'upcomingMatchesSection'}):
+            upc_matches = []
             date_ = date_sect.find('span', {'class': 'matchDayHeadline'}).text.split(' ')[-1]
-            for match in date_sect.find_all('div', {'class': 'match a-reset'}):
-                teams = match.find_all("div", class_="matchTeamName text-ellipsis")
-                if teams or len(teams) > 1:
-                    id_ = match['href'].split('/')[2]
-                    team1 = teams[0].text.strip()
-                    team2 = teams[1].text.strip()
-
-                    time_ = match.find('div', {'class', 'matchTime'}).text
+            for match in date_sect.find_all('div', {'class': 'upcomingMatch'}):
+                teams_ = match.find_all("div", class_="matchTeamName text-ellipsis")
+                id_ = match.find('a')['href'].split('/')[2]
+                t1_id = 0
+                t2_id = 0
+                time_ = match.find('div', {'class', 'matchTime'}).text
+                team1_ = 'TBD'
+                team2_ = 'TBD'
+                try:
+                    team1_ = teams_[0].text.strip()
+                    team2_ = teams_[1].text.strip()
+                    t1_id = match['team1']
+                    t2_id = match['team2']
+                except IndexError:
+                    pass
 
-                    matches.append({
+                upc_matches.append({
                         'id': id_,
-                        'team1': team1,
-                        'team2': team2,
-                        'date': date_ + " " + time_
+                        'time': time_,
+                        'team1': team1_,
+                        'team2': team2_,
+                        't1_id': t1_id,
+                        't2_id': t2_id
                     })
-                else:
-                    break
+
+            matches.append({'date': date_, 'matches': upc_matches})
 
         return matches
+    async def get_featured_events(self, max_: int = 1):
+        r = await self._fetch('https://www.hltv.org/events')
+
+        events = []
+        try:
+            for i, event in enumerate(r.find('div', {'class': 'tab-content', 'id': 'FEATURED'}).find_all('a', {'class': 'a-reset ongoing-event'}), start=1):
+                if i > max_:
+                    break
+                event_name = event.find('div', {'class': 'text-ellipsis'}).text.strip()
+                event_start_date = self._normalize_date(
+                    event.find('span', {'data-time-format': 'MMM do'}).text.strip().split())
+
+                event_end_date = self._normalize_date(
+                    event.find_all('span', {'data-time-format': 'MMM do'})[1].text.strip().split())
+                event_id = event['href'].split('/')[-2]
+
+                events.append({
+                    'id': event_id,
+                    'name': event_name,
+                    'start_date': event_start_date,
+                    'end_date': event_end_date,
+                })
+        except AttributeError:
+            pass
 
-    async def get_events(self, outgoing=True, future=True, max_events=10):
+        return events
+    async def get_events(self, featured=True, outgoing=True, future=True, max_events=10):
         """Returns events
         :params:
         outgoing - include live tournaments
         future - include future tournamets
         max_events - use only if future=True
         :return:
         [('id', 'title', 'startdate', 'enddate')]
         """
 
         r = await self._fetch('https://www.hltv.org/events')
         if not r:
             return
 
         events = []
+
         if outgoing:
             for event in r.find('div', {'class': 'tab-content', 'id': 'TODAY'}).find_all('a', {
                                 'class': 'a-reset ongoing-event'}):
                 event_name = event.find('div', {'class': 'text-ellipsis'}).text.strip()
                 event_start_date = self._normalize_date(
                     event.find('span', {'data-time-format': 'MMM do'}).text.strip().split())
 
@@ -513,14 +586,16 @@
                         'start_date': event_start_date,
                         'end_date': event_end_date
                     })
 
         return events
 
     async def get_event_info(self, event_id: str | int, event_title: str):
+        #TODO ADD PLACEC FOR PAST EVENTS? OR WINNER?
+
         r = await self._fetch(f"https://www.hltv.org/events/{str(event_id)}/{event_title.replace(' ', '-')}")
         if not r:
             return
 
         event_date_div = r.find('td', {'class', 'eventdate'}).find_all('span')
 
         event_start = self._normalize_date(event_date_div[0].text.split())
@@ -752,12 +827,20 @@
             if only_today:
                 break
 
         return news
 
 
 async def test():
-    hltv = Hltv(debug=True)
-    print(await hltv.get_match_info('2370727', 'faze', 'natus-vincere', 'pgl-cs2-major-copenhagen-2024'))
+    hltv = Hltv(debug=True, timeout=1, max_delay=5, true_session=True, use_proxy=True, proxy_list=['', ''])
+    print(await hltv.get_event_matches(7757))
+    print(await hltv.get_events())
+    print(await hltv.get_event_info(7437, 'betboom-dacha-belgrade-2024-europe-closed-qualifier'))
+    print(await hltv.get_event_results(7437))
+    print(await hltv.get_upcoming_matches(1, 3))
+    print(await hltv.get_match_info('2370913', 'FURIA', 'MOUZ', 'betboom-dacha-belgrade-2024-europe-closed-qualifier'))
+    print(await hltv.get_last_news())
+    print(await hltv.get_top_teams())
+    print(await hltv.get_best_players())
 
 if __name__ == "__main__":
     asyncio.run(test())
```

### Comparing `hltv_async_api-0.4.1/pyproject.toml` & `hltv_async_api-0.4.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "hltv_async_api"
-version = "0.4.1"
+version = "0.4.2"
 authors = [
   { name="Akim Slys", email="akimslys2003@gmail.com" },
 ]
 description = "Hltv-aio An unofficial asynchronous HLTV API Wrapper for Python"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `hltv_async_api-0.4.1/setup.py` & `hltv_async_api-0.4.2/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hltv_async_api',
-    version='0.4.1',
+    version='0.4.2',
     author='akimerslys',
     author_email='akimslys2003@gmail.com',
     description='Hltv-aio: An unofficial asynchronous HLTV API Wrapper for Python',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/akimerslys/aiohltv',
     packages=find_packages(),
```

