# Comparing `tmp/feed2fedi-2.0.0.tar.gz` & `tmp/feed2fedi-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "feed2fedi-2.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "feed2fedi-3.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `feed2fedi-2.0.0.tar` & `feed2fedi-3.0.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     4434 2024-01-17 04:49:58.350604 feed2fedi-2.0.0/README.rst
--rw-r--r--   0        0        0     3483 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/pyproject.toml
--rw-r--r--   0        0        0      295 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/__init__.py
--rw-r--r--   0        0        0     3702 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/app.py
--rw-r--r--   0        0        0     5434 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/collect.py
--rw-r--r--   0        0        0    13019 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/control.py
--rw-r--r--   0        0        0     8295 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/publish.py
--rw-r--r--   0        0        0     2625 2024-01-17 04:49:58.354604 feed2fedi-2.0.0/src/feed2fedi/utils.py
--rw-r--r--   0        0        0     5679 1970-01-01 00:00:00.000000 feed2fedi-2.0.0/PKG-INFO
+-rw-r--r--   0        0        0     4434 2024-01-17 05:15:22.877778 feed2fedi-3.0.0/README.rst
+-rw-r--r--   0        0        0     2578 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/pyproject.toml
+-rw-r--r--   0        0        0      462 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/__init__.py
+-rw-r--r--   0        0        0     3816 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/app.py
+-rw-r--r--   0        0        0     5501 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/collect.py
+-rw-r--r--   0        0        0    12998 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/control.py
+-rw-r--r--   0        0        0     9349 2024-04-07 23:31:13.160487 feed2fedi-3.0.0/src/feed2fedi/publish.py
+-rw-r--r--   0        0        0     2656 2024-04-07 23:31:13.163821 feed2fedi-3.0.0/src/feed2fedi/utils.py
+-rw-r--r--   0        0        0     5776 1970-01-01 00:00:00.000000 feed2fedi-3.0.0/PKG-INFO
```

### Comparing `feed2fedi-2.0.0/README.rst` & `feed2fedi-3.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `feed2fedi-2.0.0/pyproject.toml` & `feed2fedi-3.0.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -5,39 +5,42 @@
 [project]
 name = "feed2fedi"
 description = "Makes posts to Fediverse from one or more feeds"
 readme = "README.rst"
 authors = [
     {name = "marvin8", email = "marvin8@tuta.io"},
 ]
-requires-python = ">=3.8,<3.12"
+requires-python = ">=3.9,<3.13"
 license = {text = "AGPL-3.0-or-later"}
-dynamic = ["version"]
+version = "3.0.0"
 classifiers = [
-  "Development Status :: 3 - Alpha",
+  "Development Status :: 5 - Production/Stable",
   "Environment :: Console",
   "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
   "Programming Language :: Python",
-  "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
   "Programming Language :: Python :: 3.11",
+  "Programming Language :: Python :: 3.12",
 ]
 
 dependencies = [
-    "aiosqlite>=0.19.0",
-    "beautifulsoup4>=4.12.2",
+    "aiosqlite>=0.20.0",
+    "beautifulsoup4>=4.12.3",
     "feedparser>=6.0.11",
-    "markdownify>=0.11.6",
-    "minimal-activitypub>=0.5.11",
-    "msgspec>=0.18.5",
+    "h2>=4.1.0",
+    "httpx>=0.27.0",
+    "markdownify>=0.12.1",
+    "minimal-activitypub>=1.2.0",
+    "msgspec>=0.18.6",
     "pycryptodomex>=3.20.0",
     "python-magic>=0.4.27",
-    "typer>=0.9.0",
-    "yt-dlp>=2023.12.30",
+    "stamina>=24.2.0",
+    "typer>=0.12.1",
+    "yt-dlp>=2024.3.10",
 ]
 
 [project.scripts]
 feed2fedi = "feed2fedi.app:start_main"
 feed2fedi_import_cache = "feed2fedi.app:start_import"
 feed2fedi_convert_config = "feed2fedi.utils:start_conversion"
 
@@ -79,58 +82,11 @@
 strict_equality = true
 warn_redundant_casts = true
 warn_return_any = true
 warn_unreachable = true
 warn_unused_configs = true
 no_implicit_reexport = true
 
-[tool.ruff]
-select = ["ARG", "B", "C4", "C90", "D", "E", "ERA", "F", "I", "PL", "RUF", "S", "UP", "W"]
-ignore = ["D107", "D203", "D205", "D213", "PLR2004"]
-
-# Allow autofix for all enabled rules (when `--fix`) is provided.
-fixable = ["A", "B", "C", "D", "E", "F", "I", "UP"]
-unfixable = []
-
-# Exclude a variety of commonly ignored directories.
-exclude = [
-    ".bzr",
-    ".direnv",
-    ".eggs",
-    ".git",
-    ".hg",
-    ".mypy_cache",
-    ".nox",
-    ".pants.d",
-    ".ruff_cache",
-    ".svn",
-    ".tox",
-    ".venv",
-    "__pypackages__",
-    "_build",
-    "buck-out",
-    "build",
-    "dist",
-    "node_modules",
-    "venv",
-]
-
-# Same as Black.
-line-length = 120
-
-# Allow unused variables when underscore-prefixed.
-dummy-variable-rgx = "^(_+|(_+[a-zA-Z0-9_]*[a-zA-Z0-9]+?))$"
-
-# Assume Python 3.8.
-target-version = "py38"
-
-[tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
-max-complexity = 10
-
-[tool.ruff.isort]
-force-single-line = true
-
 [tool.scriv]
 categories = "Breaking, Added, Changed, Deprecated, Removed, Fixed, Security"
 format = "rst"
-version = "literal: src/feed2fedi/__init__.py: __version__"
+version = "literal: pyproject.toml: project.version"
```

### Comparing `feed2fedi-2.0.0/src/feed2fedi/app.py` & `feed2fedi-3.0.0/src/feed2fedi/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 """Main processing and main entry point methods for Feed2Fedi."""
+
 import asyncio
 import sys
 import traceback
 from pathlib import Path
 
 import typer
 from minimal_activitypub.client_2_server import ActivityPubError
 from typing_extensions import Annotated
 
-from . import DISPLAY_NAME
-from . import __version__
-from .collect import FeedReader
-from .control import Configuration
-from .control import PostRecorder
-from .publish import Fediverse
+from feed2fedi import DISPLAY_NAME
+from feed2fedi import __version__
+from feed2fedi.collect import FeedReader
+from feed2fedi.control import Configuration
+from feed2fedi.control import PostRecorder
+from feed2fedi.publish import Fediverse
 
 
 async def main(config_file: Path):
     """Read configuration and feeds, then make posts while avoiding duplicates.
 
     :param config_file: Path and file name of file to use for reading and storing configuration from
     """
@@ -64,15 +65,18 @@
     await post_recorder.import_urls(url_file=Path(url_file))
 
     await post_recorder.close_db()
 
 
 def start_main() -> None:
     """Start processing, i.e. main entry point."""
-    typer.run(start_main_shim)
+    try:
+        typer.run(start_main_shim)
+    except asyncio.CancelledError:
+        pass
 
 
 def start_main_shim(
     config_file: Annotated[
         Path,
         typer.Option(
             "--config-file",
```

### Comparing `feed2fedi-2.0.0/src/feed2fedi/collect.py` & `feed2fedi-3.0.0/src/feed2fedi/collect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 """Classes and methods to collect information needed by Feed2Fedi to make posts on Fediverse instance."""
-import asyncio
+
 import os
 import re
 from pathlib import Path
 from typing import Any
 from typing import List
 from typing import Optional
 from urllib.parse import urlsplit
 
-import aiohttp
 import feedparser
 from bs4 import BeautifulSoup
+from httpx import AsyncClient
+from httpx import HTTPError
+from httpx import StreamError
 from markdownify import markdownify
 
 
 class FeedReader:
     """Instance hold feed items for RSS/Atom feed passed during instantiation."""
 
     def __init__(self, feed: str) -> None:
@@ -80,42 +82,41 @@
 
         return images
 
 
 async def get_file(
     img_url: str,
     file: Any,
+    supported_mime_types: list[str],
 ) -> Optional[str]:
     """Save a file located at img_url to a file located at filepath.
 
     :param img_url: url of imgur image to download
     :param file: File to write image to
+    :param supported_mime_types: List of strings representing mime types supported by the instance server
 
     :returns:
         mime_type (string): mimetype as returned from URL
     """
     mime_type = await determine_mime_type(img_url=img_url)
 
-    chunk_size = 64 * 1024
     try:
-        if not mime_type:
+        if not mime_type or (mime_type not in supported_mime_types):
             return None
 
-        async with aiohttp.ClientSession(raise_for_status=True) as client:
-            response = await client.get(url=img_url)
-            async for data_chunk in response.content.iter_chunked(chunk_size):
-                file.write(data_chunk)
-            await asyncio.sleep(0)  # allow client session to close before continuing
+        async with AsyncClient(http2=True) as client:
+            async with client.stream(method="GET", url=img_url) as response:
+                response.raise_for_status()
+                async for data_chunk in response.aiter_bytes():
+                    file.write(data_chunk)
 
         return mime_type
 
-    except aiohttp.ClientError as save_image_error:
-        print(
-            "collect.py - get_file(...) -> None - download failed with: %s" % save_image_error,
-        )
+    except (HTTPError, StreamError) as save_image_error:
+        print(f"collect.py - get_file(...) -> None - download failed with: {save_image_error}")
 
     return None
 
 
 async def determine_mime_type(img_url: str) -> Optional[str]:
     """Determine suitable filename for an image based on URL.
 
@@ -139,24 +140,22 @@
         "video/mp4",
     )
 
     file_name = Path(os.path.basename(urlsplit(img_url).path))
 
     # Determine mime type of linked media
     try:
-        async with aiohttp.ClientSession(
-            raise_for_status=True,
-            read_timeout=30,
-        ) as client:
+        async with AsyncClient(http2=True) as client:
             response = await client.head(url=img_url)
+            response.raise_for_status()
             headers = response.headers
             content_type = headers.get("content-type", None)
 
-    except (aiohttp.ClientError, asyncio.exceptions.TimeoutError) as error:
-        print("Error while opening URL: %s " % error)
+    except HTTPError as error:
+        print(f"Error while opening URL: {error}")
         return None
 
     if content_type in image_formats:
         return str(content_type)
 
     if content_type == "application/octet-stream" and file_name.suffix == ".webp":
         return "image/webp"
```

### Comparing `feed2fedi-2.0.0/src/feed2fedi/control.py` & `feed2fedi-3.0.0/src/feed2fedi/control.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,45 @@
 """Classes and methods to control how Feed2Fedi works."""
+
 import re
 import sys
+from datetime import datetime
+from datetime import timedelta
 from enum import Enum
 from pathlib import Path
 from typing import Any
 from typing import Final
 from typing import List
 from typing import Optional
 from typing import Type
 from typing import TypeVar
 from typing import Union
 
-import aiohttp
 import aiosqlite
-import arrow
 import msgspec
+from httpx import AsyncClient
+from minimal_activitypub import Visibility
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ActivityPubError
 
-from . import DISPLAY_NAME
-from . import FILE_ENCODING
-from . import POST_RECORDER_SQLITE_DB
-from . import WEBSITE
+from feed2fedi import DISPLAY_NAME
+from feed2fedi import FILE_ENCODING
+from feed2fedi import POST_RECORDER_SQLITE_DB
+from feed2fedi import UTC
+from feed2fedi import WEBSITE
 
 CACHE_DB_PATH_DEFAULT: Final[str] = "./cache.sqlite"
 CACHE_MAX_AGE_DEFAULT_30_DAYS: Final[int] = 30
 BOT_POST_TEMPLATE_DEFAULT: Final[str] = r"{title}\n\n{link}"
 BOT_POST_IMAGE_SELECTOR_DEFAULT: Final[str] = "img[src]"
 
 ConfigClass = TypeVar("ConfigClass", bound="Configuration")
 PR = TypeVar("PR", bound="PostRecorder")
 
 
-class PostVisibility(str, Enum):
-    """Visibility values supported by Mastodon for a post."""
-
-    PUBLIC = "public"
-    UNLISTED = "unlisted"
-    PRIVATE = "private"
-    DIRECT = "direct"
-
-
 class Checks(str, Enum):
     """Supported filters checks."""
 
     REGEX = "regex"
     ANY = "any"
     NONE = "none"
 
@@ -83,26 +78,27 @@
 class FeedInfo(msgspec.Struct):
     """Dataclass to hold info needed for each feed."""
 
     url: str
     prefix: Optional[str] = None
     max_attachments: Union[int, str] = "max"
     filters: List[ItemsFilter] = []
+    post_videos: bool = True
 
 
 class Configuration(msgspec.Struct):
     """Dataclass to hold configuration settings for Feed2Fedi."""
 
     feeds: List[FeedInfo]
     fedi_instance: str
     fedi_access_token: str
     cache_max_age: int
     cache_db_path: str
     bot_post_media: bool
-    bot_post_visibility: PostVisibility
+    bot_post_visibility: Visibility
     bot_post_template: str
     bot_post_image_selector: str = BOT_POST_IMAGE_SELECTOR_DEFAULT
 
     @classmethod
     async def load_config(cls: Type[ConfigClass], config_file_path: Path) -> ConfigClass:
         """Load configuration values from file and create Configuration instance.
 
@@ -128,15 +124,15 @@
             feeds=[new_feed],
             fedi_instance=instance,
             fedi_access_token=access_token,
             cache_max_age=CACHE_MAX_AGE_DEFAULT_30_DAYS,
             cache_db_path=CACHE_DB_PATH_DEFAULT,
             bot_post_media=True,
             bot_post_image_selector=BOT_POST_IMAGE_SELECTOR_DEFAULT,
-            bot_post_visibility=PostVisibility.PUBLIC,
+            bot_post_visibility=Visibility.PUBLIC,
             bot_post_template=BOT_POST_TEMPLATE_DEFAULT,
         )
         json_config = msgspec.json.encode(new_config)
         with config_file_path.open(mode="wb") as config_file:
             config_file.write(msgspec.json.format(json_config, indent=4))
 
     @staticmethod
@@ -154,19 +150,18 @@
         """Get access token from fediverse instance.
 
         :param instance: URL to fediverse instance
         :returns:
             Access token
         """
         try:
-            async with aiohttp.ClientSession() as session:
-                # Create app
+            async with AsyncClient(http2=True) as client:
                 client_id, client_secret = await ActivityPub.create_app(
                     instance_url=instance,
-                    session=session,
+                    client=client,
                     user_agent=DISPLAY_NAME,
                     client_website=WEBSITE,
                 )
 
                 # Get Authorization Code / URL
                 authorization_request_url = await ActivityPub.generate_authorization_url(
                     instance_url=instance,
@@ -174,15 +169,15 @@
                     user_agent=DISPLAY_NAME,
                 )
                 print(f"Please go to the following URL and follow the instructions:\n" f"{authorization_request_url}")
                 authorization_code = input("[...] Please enter the authorization code: ")
 
                 # Validate authorization code and get access token
                 access_token = await ActivityPub.validate_authorization_code(
-                    session=session,
+                    client=client,
                     instance_url=instance,
                     authorization_code=authorization_code,
                     client_id=client_id,
                     client_secret=client_secret,
                 )
 
         except ActivityPubError as error:
@@ -255,15 +250,15 @@
 
         :param shared_url:
                 URL of feed item
         """
         if self.history_db is None:
             raise AssertionError("Have you called db_init() first?")
 
-        timestamp = arrow.utcnow().timestamp()
+        timestamp = datetime.now(tz=UTC).timestamp()
         await self.history_db.execute(
             "INSERT INTO share (url, shared_ts) VALUES (?, ?)",
             (
                 shared_url,
                 timestamp,
             ),
         )
@@ -318,15 +313,15 @@
         """Prune entries from db that are older than max_age_in_days.
 
         :param max_age_in_days: Maximum age of records to keep in DB
         """
         if self.history_db is None:
             raise AssertionError("Have you called db_init() first?")
 
-        max_age_ts = arrow.utcnow().shift(days=-max_age_in_days).timestamp()
+        max_age_ts = (datetime.now(tz=UTC) - timedelta(days=max_age_in_days)).timestamp()
         await self.history_db.execute(
             "DELETE FROM share WHERE shared_ts<:max_age_ts",
             {"max_age_ts": max_age_ts},
         )
         await self.history_db.commit()
 
     async def close_db(self: PR) -> None:
```

### Comparing `feed2fedi-2.0.0/src/feed2fedi/publish.py` & `feed2fedi-3.0.0/src/feed2fedi/publish.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,36 @@
 """Classes and methods needed to publish posts on a Fediverse instance."""
+
 import asyncio
 import re
 import tempfile
 import traceback
+from datetime import datetime
 from pathlib import Path
 from typing import List
 
-import aiohttp
-import arrow
 import magic
 import yt_dlp
 from feedparser import FeedParserDict
+from httpx import AsyncClient
 from minimal_activitypub.client_2_server import ActivityPub
 from minimal_activitypub.client_2_server import ClientError
+from minimal_activitypub.client_2_server import NetworkError
 from minimal_activitypub.client_2_server import RatelimitError
+from stamina import retry
+from stamina import retry_context
 
-from .collect import FeedReader
-from .collect import get_file
-from .control import Actions
-from .control import Configuration
-from .control import FeedInfo
-from .control import IgnoringLogger
-from .control import PostRecorder
+from feed2fedi import UTC
+from feed2fedi.collect import FeedReader
+from feed2fedi.collect import get_file
+from feed2fedi.control import Actions
+from feed2fedi.control import Configuration
+from feed2fedi.control import FeedInfo
+from feed2fedi.control import IgnoringLogger
+from feed2fedi.control import PostRecorder
 
 
 class Fediverse:
     """Helper class to publish posts on a fediverse instance from rss feed items."""
 
     def __init__(self, config: Configuration, post_recorder: PostRecorder) -> None:
         self.config = config
@@ -37,22 +42,24 @@
         feed: FeedInfo,
     ) -> None:
         """Publish posts to fediverse instance from content in the items list.
 
         :param items: Rss feed items to post
         :param feed: Section of config for current feed
         """
-        async with aiohttp.ClientSession() as session:
+        async with AsyncClient(http2=True) as client:
             fediverse = ActivityPub(
                 instance=self.config.fedi_instance,
-                session=session,
+                client=client,
                 access_token=self.config.fedi_access_token,
             )
-            await fediverse.determine_instance_type()
-            await fediverse.verify_credentials()
+            for attempt in retry_context(on=NetworkError, attempts=3):
+                with attempt:
+                    await fediverse.determine_instance_type()
+                    await fediverse.verify_credentials()
 
             if isinstance(feed.max_attachments, int):
                 max_media = min(fediverse.max_attachments, feed.max_attachments)
             else:
                 max_media = fediverse.max_attachments
 
             for item in items:
@@ -85,49 +92,57 @@
                     status += f"{feed.prefix} - "
                 status += self.config.bot_post_template.format(**item.params).replace("\\n", "\n")
                 media_ids: List[str] = []
 
                 try:
                     # Post media if configured to and media_thumbnail is present with an url
                     if self.config.bot_post_media and max_media:
-                        media_ids = await Fediverse._post_video(fediverse=fediverse, item=item)
+                        if feed.post_videos:
+                            media_ids = await Fediverse._post_video(fediverse=fediverse, item=item)
 
                         if len(media_ids) == 0:
                             media_ids = await Fediverse._post_images(
                                 fediverse=fediverse,
                                 item=item,
                                 max_images=max_media,
                                 image_selector=self.config.bot_post_image_selector,
+                                supported_mime_types=fediverse.supported_mime_types,
                             )
 
-                    posted_status = await fediverse.post_status(
-                        status=status,
-                        visibility=self.config.bot_post_visibility.value,
-                        media_ids=media_ids,
-                        sensitive=sensitive,
-                        spoiler_text=spoiler_text,
-                    )
+                    for attempt in retry_context(on=NetworkError, attempts=3):
+                        with attempt:
+                            posted_status = await fediverse.post_status(
+                                status=status,
+                                visibility=self.config.bot_post_visibility.value,
+                                media_ids=media_ids,
+                                sensitive=sensitive,
+                                spoiler_text=spoiler_text,
+                            )
 
                     print(f"Posted {posted_status['content']} to Fediverse at\n{posted_status['url']}")
 
                     await self.post_recorder.log_post(shared_url=item.link)
 
                 except RatelimitError:
                     reset = fediverse.ratelimit_reset
-                    seconds = reset.timestamp() - arrow.now().timestamp()
-                    print(f'!!! Server "cool down" - waiting for {seconds} seconds (until {reset})')
+                    seconds = reset.timestamp() - datetime.now(tz=UTC).timestamp()
+                    print(
+                        f'!!! Server "cool down" - waiting until {reset:%Y-%m-%d %H:%M:%S %z} '
+                        f"({round(number=seconds)} seconds)"
+                    )
                     await asyncio.sleep(delay=seconds)
 
                 except ClientError as error:
                     print(f"!!! Encountered error: {error}")
                     traceback.print_tb(error.__traceback__)
                     print("\nLog article to avoid repeat of error")
                     await self.post_recorder.log_post(shared_url=item.link)
 
     @staticmethod
+    @retry(on=NetworkError, attempts=3)
     async def _post_video(
         fediverse: ActivityPub,
         item: FeedParserDict,
     ) -> List[str]:
         """Post media to fediverse instance and return media ID.
 
         :param fediverse: ActivityPub api instance
@@ -169,37 +184,41 @@
                     raise ClientError from error
                 finally:
                     Path(filename).unlink()
 
         return media_ids
 
     @staticmethod
+    @retry(on=NetworkError, attempts=3)
     async def _post_images(
         fediverse: ActivityPub,
         item: FeedParserDict,
         image_selector: str,
+        supported_mime_types: list[str],
         max_images: int = 1,
     ) -> List[str]:
         """Post media to fediverse instance and return media ID.
 
         :param fediverse: ActivityPub api instance
         :param item: Feed item to load media from
         :param max_images: number of images to post. Defaults to 1
+        :param supported_mime_types:  List of strings representing mime types supported by the instance server
+
         :returns:
             List containing no, one  or multiple strings of the media id after upload
         """
         media_ids: List[str] = []
         media_urls = FeedReader.determine_image_url(item, image_selector)
 
         for url in media_urls:
             if len(media_ids) == max_images:
                 break
 
             with tempfile.TemporaryFile() as temp_image_file:
-                mime_type = await get_file(img_url=url, file=temp_image_file)
+                mime_type = await get_file(img_url=url, file=temp_image_file, supported_mime_types=supported_mime_types)
                 if mime_type:
                     temp_image_file.seek(0)
                     media = await fediverse.post_media(
                         file=temp_image_file,
                         mime_type=mime_type,
                     )
                     media_ids.append(media["id"])
```

### Comparing `feed2fedi-2.0.0/src/feed2fedi/utils.py` & `feed2fedi-3.0.0/src/feed2fedi/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 """Module containing utilities and helper methods."""
+
 import configparser
 from itertools import zip_longest
 from pathlib import Path
 from typing import List
 
 import msgspec
 import typer
+from minimal_activitypub import Visibility
 from typing_extensions import Annotated
 
-from .control import BOT_POST_IMAGE_SELECTOR_DEFAULT
-from .control import Configuration
-from .control import FeedInfo
-from .control import PostVisibility
+from feed2fedi.control import BOT_POST_IMAGE_SELECTOR_DEFAULT
+from feed2fedi.control import Configuration
+from feed2fedi.control import FeedInfo
 
 
 def convert_config_json(  # nocl
     config_file: Annotated[
         Path,
         typer.Option(
             "--config-file",
@@ -50,15 +51,15 @@
     old_prefixes = [prefix for _key, prefix in config_ini.items(section="Prefixes")]
 
     new_feeds: List[FeedInfo] = []
     for feed, prefix in zip_longest(old_feeds, old_prefixes, fillvalue=""):
         new_feeds.append(FeedInfo(url=feed, prefix=prefix, max_attachments=1))
 
     new_config = Configuration(
-        bot_post_visibility=PostVisibility(config_ini.get(section="Bot", option="post_visibility")),
+        bot_post_visibility=Visibility(config_ini.get(section="Bot", option="post_visibility")),
         bot_post_media=bool(config_ini.get(section="Bot", option="post_media")),
         bot_post_image_selector=BOT_POST_IMAGE_SELECTOR_DEFAULT,
         bot_post_template="{title}\n\n{link}",
         cache_max_age=int(config_ini.get(section="Cache", option="max-age")),
         cache_db_path=config_ini.get(section="Cache", option="db-path"),
         fedi_instance=config_ini.get(section="Fediverse", option="instance"),
         fedi_access_token=config_ini.get(section="Fediverse", option="access-token"),
```

### Comparing `feed2fedi-2.0.0/PKG-INFO` & `feed2fedi-3.0.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,35 @@
 Metadata-Version: 2.1
 Name: feed2fedi
-Version: 2.0.0
+Version: 3.0.0
 Summary: Makes posts to Fediverse from one or more feeds
 Author-email: marvin8 <marvin8@tuta.io>
-Requires-Python: >=3.8,<3.12
+Requires-Python: >=3.9,<3.13
 Description-Content-Type: text/x-rst
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiosqlite>=0.19.0
-Requires-Dist: beautifulsoup4>=4.12.2
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: aiosqlite>=0.20.0
+Requires-Dist: beautifulsoup4>=4.12.3
 Requires-Dist: feedparser>=6.0.11
-Requires-Dist: markdownify>=0.11.6
-Requires-Dist: minimal-activitypub>=0.5.11
-Requires-Dist: msgspec>=0.18.5
+Requires-Dist: h2>=4.1.0
+Requires-Dist: httpx>=0.27.0
+Requires-Dist: markdownify>=0.12.1
+Requires-Dist: minimal-activitypub>=1.2.0
+Requires-Dist: msgspec>=0.18.6
 Requires-Dist: pycryptodomex>=3.20.0
 Requires-Dist: python-magic>=0.4.27
-Requires-Dist: typer>=0.9.0
-Requires-Dist: yt-dlp>=2023.12.30
+Requires-Dist: stamina>=24.2.0
+Requires-Dist: typer>=0.12.1
+Requires-Dist: yt-dlp>=2024.3.10
 Project-URL: Changelog, https://codeberg.org/MarvinsMastodonTools/feed2fedi/src/branch/main/CHANGELOG.rst
 Project-URL: Issues, https://codeberg.org/MarvinsMastodonTools/feed2fedi/issues
 Project-URL: Source, https://codeberg.org/MarvinsMastodonTools/feed2fedi
 
 Feed2Fedi
 =========
```

