# Comparing `tmp/gamdl-1.9.9.4.tar.gz` & `tmp/gamdl-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gamdl-1.9.9.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "gamdl-2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `gamdl-1.9.9.4.tar` & `gamdl-2.0.tar`

### file list

```diff
@@ -1,11 +1,20 @@
--rw-r--r--   0        0        0     1137 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/.github/workflows/main.yml
--rw-r--r--   0        0        0       79 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/.gitignore
--rw-r--r--   0        0        0    10188 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/README.md
--rw-r--r--   0        0        0       24 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/gamdl/__init__.py
--rw-r--r--   0        0        0       30 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/gamdl/__main__.py
--rw-r--r--   0        0        0    21548 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/gamdl/cli.py
--rw-r--r--   0        0        0     4701 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/gamdl/constants.py
--rw-r--r--   0        0        0    27636 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/gamdl/downloader.py
--rw-r--r--   0        0        0      525 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/pyproject.toml
--rw-r--r--   0        0        0       36 2023-11-09 18:27:25.434380 gamdl-1.9.9.4/requirements.txt
--rw-r--r--   0        0        0    10617 1970-01-01 00:00:00.000000 gamdl-1.9.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1137 2024-04-08 18:49:22.867913 gamdl-2.0/.github/workflows/main.yml
+-rw-r--r--   0        0        0       79 2024-04-08 18:49:22.867913 gamdl-2.0/.gitignore
+-rw-r--r--   0        0        0    11148 2024-04-08 18:49:22.867913 gamdl-2.0/README.md
+-rw-r--r--   0        0        0       20 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/__init__.py
+-rw-r--r--   0        0        0       30 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/__main__.py
+-rw-r--r--   0        0        0     7930 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/apple_music_api.py
+-rw-r--r--   0        0        0    26206 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/cli.py
+-rw-r--r--   0        0        0     5522 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/constants.py
+-rw-r--r--   0        0        0    12570 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader.py
+-rw-r--r--   0        0        0     9847 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_music_video.py
+-rw-r--r--   0        0        0     2121 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_post.py
+-rw-r--r--   0        0        0    13316 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_song.py
+-rw-r--r--   0        0        0     3691 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/downloader_song_legacy.py
+-rw-r--r--   0        0        0      801 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/enums.py
+-rw-r--r--   0        0        0     4015 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/hardcoded_wvd.py
+-rw-r--r--   0        0        0     2418 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/itunes_api.py
+-rw-r--r--   0        0        0      347 2024-04-08 18:49:22.867913 gamdl-2.0/gamdl/models.py
+-rw-r--r--   0        0        0      560 2024-04-08 18:49:22.867913 gamdl-2.0/pyproject.toml
+-rw-r--r--   0        0        0       54 2024-04-08 18:49:22.867913 gamdl-2.0/requirements.txt
+-rw-r--r--   0        0        0    11621 1970-01-01 00:00:00.000000 gamdl-2.0/PKG-INFO
```

### Comparing `gamdl-1.9.9.4/.github/workflows/main.yml` & `gamdl-2.0/.github/workflows/main.yml`

 * *Files identical despite different names*

### Comparing `gamdl-1.9.9.4/README.md` & `gamdl-2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,86 +1,106 @@
-# gamdl - Glomatico's Apple Music Downloader
-A Python script to download Apple Music songs/music videos/albums/playlists. This is a rework of https://github.com/loveyoursupport/AppleMusic-Downloader/tree/661a274d62586b521feec5a7de6bee0e230fdb7d.
+Metadata-Version: 2.1
+Name: gamdl
+Version: 2.0
+Summary: Download Apple Music songs/music videos/albums/playlists
+Author: glomatico
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+Requires-Dist: ciso8601
+Requires-Dist: click
+Requires-Dist: m3u8
+Requires-Dist: tabulate
+Requires-Dist: pywidevine
+Requires-Dist: pyyaml
+Requires-Dist: yt-dlp
+Project-URL: homepage, https://github.com/glomatico/gamdl
+Project-URL: repository, https://github.com/glomatico/gamdl
+
+# Glomatico's Apple Music Downloader
+A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
 
 ## Features
-* Download songs in 256kbps AAC or in 64kbps HE-AAC
+* Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
-* Download synced lyrics
+* Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
-  
+
+## Prerequisites
+* Python 3.8 or higher
+* The cookies file of your Apple Music account (requires an active subscription)
+    * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
+        * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
+        * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
+* FFmpeg on your system PATH
+    * Older versions of FFmpeg may not work.
+    * Up to date binaries can be obtained from the links below:
+        * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
+        * Linux: https://johnvansickle.com/ffmpeg/
+* (Optional) mp4decrypt on your system PATH
+    * Required to download music videos and songs in non-legacy formats.
+    * Binaries can be obtained from here: https://www.bento4.com/downloads/.
+ 
 ## Installation
-1. Install Python 3.7 or higher
-2. Add [FFmpeg](https://ffmpeg.org/download.html) and [mp4decrypt](https://www.bento4.com/downloads/) to PATH
-    * mp4decrypt is only needed if you want to download music videos
-3. Place your cookies in the same folder that you will run gamdl as `cookies.txt`
-    * You can export your cookies by using this Google Chrome extension on Apple Music website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
-4. Place your .wvd file in the same folder that you will run gamdl as `device.wvd`
-    * To get a .wvd file, you can use [dumper](https://github.com/wvdumper/dumper) to dump a L3 CDM from an Android device. Once you have the L3 CDM, use pywidevine to create the .wvd file from it.
-        1. Install pywidevine with pip
-            ```bash
-            pip install pywidevine pyyaml
-            ```
-        2. Create the .wvd file
-            ```bash
-            pywidevine create-device -t ANDROID -l 3 -k private_key.pem -c client_id.bin -o .
-            ```
-5. Install gamdl using pip
+1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
+2. Place your cookies in the same directory you will run the script from and name it as `cookies.txt`
 
-## Examples
+## Usage
 * Download a song
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
     ```
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                            | Default value                      |
-| --------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------- |
-| `-f`, `--final-path` / `final_path`                             | Path where the downloaded files will be saved.                         | `./Apple Music`                    |
-| `-t`, `--temp-path` / `temp_path`                               | Path where the temporary files will be saved.                          | `./temp`                           |
-| `-c`, `--cookies-location` / `cookies_location`                 | Location of the cookies file.                                          | `./cookies.txt`                    |
-| `-w`, `--wvd-location` / `wvd_location`                         | Location of the .wvd file.                                             | `./device.wvd`                     |
-| `--ffmpeg-location` / `ffmpeg_location`                         | Location of the FFmpeg binary.                                         | `ffmpeg`                           |
-| `--mp4box-location` / `mp4box_location`                         | Location of the MP4Box binary.                                         | `MP4Box`                           |
-| `--mp4decrypt-location` / `mp4decrypt_location`                 | Location of the mp4decrypt binary.                                     | `mp4decrypt`                       |
-| `--nm3u8dlre-location` / `nm3u8dlre_location`                   | Location of the N_m3u8DL-RE binary.                                    | `N_m3u8DL-RE`                      |
-| `--config-location` / -                                         | Location of the config file.                                           | `<home_folder>/.gamdl/config.json` |
-| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                      | `{album_artist}/{album}`           |
-| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.          | `Compilations/{album}`             |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template of the track files for single-disc albums as a format string. | `{track:02d} {title}`              |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the track files for multi-disc albums as a format string.  | `{disc}-{track:02d} {title}`       |
-| `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                | `{artist}/Unknown Album`           |
-| `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                  | `{title}`                          |
-| `--cover-size` / `cover_size`                                   | Size of the cover.                                                     | `1200`                             |
-| `--cover-format` / `cover_format`                               | Format of the cover.                                                   | `jpg`                              |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                            | `ffmpeg`                           |
-| `--download-mode` / `download_mode`                             | Download mode.                                                         | `ytdlp`                            |
-| `-e`, `--exclude-tags` / `exclude_tags`                         | List of tags to exclude from file tagging separated by commas.         | `null`                             |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                               | `40`                               |
-| `-l`, `--log-level` / `log_level`                               | Log level.                                                             | `INFO`                             |
-| `--prefer-hevc` / `prefer_hevc`                                 | Prefer HEVC over AVC when downloading music videos.                    | `false`                            |
-| `--ask-video-format` / `ask_video_format`                       | Ask for the video format when downloading music videos.                | `false`                            |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.               | `false`                            |
-| `-l`, `--lrc-only` / `lrc_only`                                 | Download only the synced lyrics.                                       | `false`                            |
-| `-n`, `--no-lrc` / `no_lrc`                                     | Don't download the synced lyrics.                                      | `false`                            |
-| `-s`, `--save-cover` / `save_cover`                             | Save cover as a separate file.                                         | `false`                            |
-| `--songs-heaac` / `songs_heaac`                                 | Download songs in HE-AAC 64kbps.                                       | `false`                            |
-| `-o`, `--overwrite` / `overwrite`                               | Overwrite existing files.                                              | `false`                            |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                      | `false`                            |
-| `-u`, `--url-txt` / -                                           | Read URLs as location of text files containing URLs.                   | `false`                            |
-| `-n`, `--no-config-file` / -                                    | Don't use the config file.                                             | `false`                            |
+| Command line argument / Config file key                         | Description                                                        | Default value                                |
+| --------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.           | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                     | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                          | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.             | `false`                                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                   | `false`                                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                  | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                               | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                         | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                  | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                         | `./cookies.txt`                              |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                          | `./Apple Music`                              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                       | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                 | `null`                                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                        | `N_m3u8dl-RE`                                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                         | `mp4decrypt`                                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                             | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                             | `MP4Box`                                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                     | `ytdlp`                                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                        | `ffmpeg`                                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                      | `jpg`                                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.              | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.   | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album. | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.  | `{disc}-{track:02d} {title}`                 |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.      | `{artist}/Unknown Album`                     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.        | `{title}`                                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                 | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                   | `null`                                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                        | `1200`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                           | `40`                                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                        | `aac-legacy`                                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                              | `lrc`                                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                 | `h264-best`                                  |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                | `best`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                          | `false`                                      |
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
 * `album_sort`
@@ -106,40 +126,70 @@
 * `storefront`
 * `title`
 * `title_id`
 * `title_sort`
 * `track`
 * `track_total`
 * `xid`
-  
-### Remux mode
+
+### Remux modes
 The following remux modes are available:
 * `ffmpeg`
-    * Can decrypt and remux songs but can't decrypt music videos by itself
-    * Decryption may not work on older versions of FFmpeg
+    * Can be used without mp4decrypt only for songs and when using legacy song codecs
 * `mp4box`
     * Requires mp4decrypt
     * Doesn't convert closed captions in music videos that have them
     * Can be obtained from here: https://gpac.wp.imt.fr/downloads
 
-### Download mode
+### Download modes
 The following download modes are available:
 * `ytdlp`
 * `nm3u8dlre`
     * Faster than `ytdlp`
     * Requires FFmpeg
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
 
-## Music videos quality
-Music videos will be downloaded in the highest quality available by default. The available qualities are:
-* AVC 1080p 10mbps, AAC 256kbps
-* AVC 1080p 6.5mbps, AAC 256kbps
-* AVC 720p 4mbps, AAC 256kbps
-* AVC 576p 2mbps, AAC 256kbps
-* AVC 480p 1.5mbps, AAC 256kbps
-* AVC 360p 1mbps, AAC 256kbps
-
-By enabling the `prefer_hevc` option, music videos will be downloaded in the highest HEVC quality available. The available qualities are:
-* HEVC 4K 20mbps, AAC 256kbps
-* HEVC 4K 12mbps, AAC 256kbps
 
-Enable `ask_video_format` to select a custom audio/video format.
+### Song codecs
+The following codecs are available:
+* `aac-legacy`
+* `aac-he-legacy`
+* `aac`
+* `aac-he`
+* `aac-binaural`
+* `aac-downmix`
+* `aac-he-binaural`
+* `aac-he-downmix`
+* `alac`
+* `atmos`
+
+**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be decrypted  when using non-legacy codecs.**
+
+### Music videos codecs
+The following codecs are available:
+* `h264-best` (with AAC 256kbps, up to 1080p)
+* `h265-best` (With AAC 256kpbs, up to 2160p)
+* `ask`
+    * When using this option, the script will ask you which audio and video codec to use.
+  
+### Post videos/extra videos qualities
+The following qualities are available:
+* `best` (with AAC 256kbps, up to 1080p)
+* `ask`
+    * When using this option, the script will ask you which video quality to use.
+
+Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
+
+### Synced lyrics formats
+The following synced lyrics formats are available:
+* `lrc`
+* `srt`
+* `ttml`
+    * Native format for Apple Music synced lyrics.
+    * Highly unsupported by media players.
+  
+### Cover formats
+The following cover formats are available:
+* `jpg`
+* `png`
+
+
```

### Comparing `gamdl-1.9.9.4/pyproject.toml` & `gamdl-2.0/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [project]
 name = "gamdl"
 description = "Download Apple Music songs/music videos/albums/playlists"
-requires-python = ">=3.7"
-authors = [{name = "glomatico"}]
+requires-python = ">=3.8"
+authors = [{ name = "glomatico" }]
 dependencies = [
+    "ciso8601",
     "click",
     "m3u8",
+    "tabulate",
     "pywidevine",
     "pyyaml",
-    "yt-dlp"
+    "yt-dlp",
 ]
 readme = "README.md"
 dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/glomatico/gamdl"
 repository = "https://github.com/glomatico/gamdl"
```

### Comparing `gamdl-1.9.9.4/PKG-INFO` & `gamdl-2.0/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,101 +1,89 @@
-Metadata-Version: 2.1
-Name: gamdl
-Version: 1.9.9.4
-Summary: Download Apple Music songs/music videos/albums/playlists
-Author: glomatico
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-Requires-Dist: click
-Requires-Dist: m3u8
-Requires-Dist: pywidevine
-Requires-Dist: pyyaml
-Requires-Dist: yt-dlp
-Project-URL: homepage, https://github.com/glomatico/gamdl
-Project-URL: repository, https://github.com/glomatico/gamdl
-
-# gamdl - Glomatico's Apple Music Downloader
-A Python script to download Apple Music songs/music videos/albums/playlists. This is a rework of https://github.com/loveyoursupport/AppleMusic-Downloader/tree/661a274d62586b521feec5a7de6bee0e230fdb7d.
+# Glomatico's Apple Music Downloader
+A Python script to download Apple Music songs/music videos/albums/playlists/post videos.
 
 ## Features
-* Download songs in 256kbps AAC or in 64kbps HE-AAC
+* Download songs in AAC/Spatial AAC/Dolby Atmos/ALAC*
 * Download music videos up to 4K
-* Download synced lyrics
+* Download synced lyrics in LRC, SRT or TTML
 * Choose between FFmpeg and MP4Box for remuxing
 * Choose between yt-dlp and N_m3u8DL-RE for downloading
 * Highly customizable
-  
+
+## Prerequisites
+* Python 3.8 or higher
+* The cookies file of your Apple Music account (requires an active subscription)
+    * You can get your cookies by using one of the following extensions on your browser of choice at the Apple Music website with your account signed in:
+        * Firefox: https://addons.mozilla.org/addon/export-cookies-txt
+        * Chromium based browsers: https://chrome.google.com/webstore/detail/gdocmgbfkjnnpapoeobnolbbkoibbcif
+* FFmpeg on your system PATH
+    * Older versions of FFmpeg may not work.
+    * Up to date binaries can be obtained from the links below:
+        * Windows: https://github.com/AnimMouse/ffmpeg-stable-autobuild/releases
+        * Linux: https://johnvansickle.com/ffmpeg/
+* (Optional) mp4decrypt on your system PATH
+    * Required to download music videos and songs in non-legacy formats.
+    * Binaries can be obtained from here: https://www.bento4.com/downloads/.
+ 
 ## Installation
-1. Install Python 3.7 or higher
-2. Add [FFmpeg](https://ffmpeg.org/download.html) and [mp4decrypt](https://www.bento4.com/downloads/) to PATH
-    * mp4decrypt is only needed if you want to download music videos
-3. Place your cookies in the same folder that you will run gamdl as `cookies.txt`
-    * You can export your cookies by using this Google Chrome extension on Apple Music website: https://chrome.google.com/webstore/detail/open-cookiestxt/gdocmgbfkjnnpapoeobnolbbkoibbcif. Make sure to be logged in.
-4. Place your .wvd file in the same folder that you will run gamdl as `device.wvd`
-    * To get a .wvd file, you can use [dumper](https://github.com/wvdumper/dumper) to dump a L3 CDM from an Android device. Once you have the L3 CDM, use pywidevine to create the .wvd file from it.
-        1. Install pywidevine with pip
-            ```bash
-            pip install pywidevine pyyaml
-            ```
-        2. Create the .wvd file
-            ```bash
-            pywidevine create-device -t ANDROID -l 3 -k private_key.pem -c client_id.bin -o .
-            ```
-5. Install gamdl using pip
+1. Install the package `gamdl` using pip
     ```bash
     pip install gamdl
     ```
+2. Place your cookies in the same directory you will run the script from and name it as `cookies.txt`
 
-## Examples
+## Usage
 * Download a song
     ```bash
     gamdl "https://music.apple.com/us/album/never-gonna-give-you-up-2022-remaster/1626265761?i=1626265765"
     ```
 * Download an album
     ```bash
     gamdl "https://music.apple.com/us/album/whenever-you-need-somebody-2022-remaster/1626265761"
     ```
 
 ## Configuration
 You can configure gamdl by using the command line arguments or the config file. The config file is created automatically when you run gamdl for the first time at `~/.gamdl/config.json` on Linux and `%USERPROFILE%\.gamdl\config.json` on Windows. Config file values can be overridden using command line arguments.
-| Command line argument / Config file key                         | Description                                                            | Default value                      |
-| --------------------------------------------------------------- | ---------------------------------------------------------------------- | ---------------------------------- |
-| `-f`, `--final-path` / `final_path`                             | Path where the downloaded files will be saved.                         | `./Apple Music`                    |
-| `-t`, `--temp-path` / `temp_path`                               | Path where the temporary files will be saved.                          | `./temp`                           |
-| `-c`, `--cookies-location` / `cookies_location`                 | Location of the cookies file.                                          | `./cookies.txt`                    |
-| `-w`, `--wvd-location` / `wvd_location`                         | Location of the .wvd file.                                             | `./device.wvd`                     |
-| `--ffmpeg-location` / `ffmpeg_location`                         | Location of the FFmpeg binary.                                         | `ffmpeg`                           |
-| `--mp4box-location` / `mp4box_location`                         | Location of the MP4Box binary.                                         | `MP4Box`                           |
-| `--mp4decrypt-location` / `mp4decrypt_location`                 | Location of the mp4decrypt binary.                                     | `mp4decrypt`                       |
-| `--nm3u8dlre-location` / `nm3u8dlre_location`                   | Location of the N_m3u8DL-RE binary.                                    | `N_m3u8DL-RE`                      |
-| `--config-location` / -                                         | Location of the config file.                                           | `<home_folder>/.gamdl/config.json` |
-| `--template-folder-album` / `template_folder_album`             | Template of the album folders as a format string.                      | `{album_artist}/{album}`           |
-| `--template-folder-compilation` / `template_folder_compilation` | Template of the compilation album folders as a format string.          | `Compilations/{album}`             |
-| `--template-file-single-disc` / `template_file_single_disc`     | Template of the track files for single-disc albums as a format string. | `{track:02d} {title}`              |
-| `--template-file-multi-disc` / `template_file_multi_disc`       | Template of the track files for multi-disc albums as a format string.  | `{disc}-{track:02d} {title}`       |
-| `--template-folder-music-video` / `template_folder_music_video` | Template of the music video folders as a format string.                | `{artist}/Unknown Album`           |
-| `--template-file-music-video` / `template_file_music_video`     | Template of the music video files as a format string.                  | `{title}`                          |
-| `--cover-size` / `cover_size`                                   | Size of the cover.                                                     | `1200`                             |
-| `--cover-format` / `cover_format`                               | Format of the cover.                                                   | `jpg`                              |
-| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                            | `ffmpeg`                           |
-| `--download-mode` / `download_mode`                             | Download mode.                                                         | `ytdlp`                            |
-| `-e`, `--exclude-tags` / `exclude_tags`                         | List of tags to exclude from file tagging separated by commas.         | `null`                             |
-| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                               | `40`                               |
-| `-l`, `--log-level` / `log_level`                               | Log level.                                                             | `INFO`                             |
-| `--prefer-hevc` / `prefer_hevc`                                 | Prefer HEVC over AVC when downloading music videos.                    | `false`                            |
-| `--ask-video-format` / `ask_video_format`                       | Ask for the video format when downloading music videos.                | `false`                            |
-| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.               | `false`                            |
-| `-l`, `--lrc-only` / `lrc_only`                                 | Download only the synced lyrics.                                       | `false`                            |
-| `-n`, `--no-lrc` / `no_lrc`                                     | Don't download the synced lyrics.                                      | `false`                            |
-| `-s`, `--save-cover` / `save_cover`                             | Save cover as a separate file.                                         | `false`                            |
-| `--songs-heaac` / `songs_heaac`                                 | Download songs in HE-AAC 64kbps.                                       | `false`                            |
-| `-o`, `--overwrite` / `overwrite`                               | Overwrite existing files.                                              | `false`                            |
-| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                      | `false`                            |
-| `-u`, `--url-txt` / -                                           | Read URLs as location of text files containing URLs.                   | `false`                            |
-| `-n`, `--no-config-file` / -                                    | Don't use the config file.                                             | `false`                            |
+| Command line argument / Config file key                         | Description                                                        | Default value                                |
+| --------------------------------------------------------------- | ------------------------------------------------------------------ | -------------------------------------------- |
+| `--disable-music-video-skip` / `disable_music_video_skip`       | Don't skip downloading music videos in albums/playlists.           | `false`                                      |
+| `--save-cover`, `-s` / `save_cover`                             | Save cover as a separate file.                                     | `false`                                      |
+| `--overwrite` / `overwrite`                                     | Overwrite existing files.                                          | `false`                                      |
+| `--read-urls-as-txt`, `-r` / -                                  | Interpret URLs as paths to text files containing URLs.             | `false`                                      |
+| `--synced-lyrics-only` / `synced_lyrics_only`                   | Download only the synced lyrics.                                   | `false`                                      |
+| `--no-synced-lyrics` / `no_synced_lyrics`                       | Don't download the synced lyrics.                                  | `false`                                      |
+| `--config-path` / -                                             | Path to config file.                                               | `<home>/.spotify-web-downloader/config.json` |
+| `--log-level` / `log_level`                                     | Log level.                                                         | `INFO`                                       |
+| `--print-exceptions` / `print_exceptions`                       | Print exceptions.                                                  | `false`                                      |
+| `--cookies-path`, `-c` / `cookies_path`                         | Path to .txt cookies file.                                         | `./cookies.txt`                              |
+| `--output-path`, `-o` / `output_path`                           | Path to output directory.                                          | `./Apple Music`                              |
+| `--temp-path` / `temp_path`                                     | Path to temporary directory.                                       | `./temp`                                     |
+| `--wvd-path` / `wvd_path`                                       | Path to .wvd file.                                                 | `null`                                       |
+| `--nm3u8dlre-path` / `nm3u8dlre_path`                           | Path to N_m3u8DL-RE binary.                                        | `N_m3u8dl-RE`                                |
+| `--mp4decrypt-path` / `mp4decrypt_path`                         | Path to mp4decrypt binary.                                         | `mp4decrypt`                                 |
+| `--ffmpeg-path` / `ffmpeg_path`                                 | Path to FFmpeg binary.                                             | `ffmpeg`                                     |
+| `--mp4box-path` / `mp4box_path`                                 | Path to MP4Box binary.                                             | `MP4Box`                                     |
+| `--download-mode` / `download_mode`                             | Download mode.                                                     | `ytdlp`                                      |
+| `--remux-mode` / `remux_mode`                                   | Remux mode.                                                        | `ffmpeg`                                     |
+| `--cover-format` / `cover_format`                               | Cover format.                                                      | `jpg`                                        |
+| `--template-folder-album` / `template_folder_album`             | Template folder for tracks that are part of an album.              | `{album_artist}/{album}`                     |
+| `--template-folder-compilation` / `template_folder_compilation` | Template folder for tracks that are part of a compilation album.   | `Compilations/{album}`                       |
+| `--template-file-single-disc` / `template_file_single_disc`     | Template file for the tracks that are part of a single-disc album. | `{track:02d} {title}`                        |
+| `--template-file-multi-disc` / `template_file_multi_disc`       | Template file for the tracks that are part of a multi-disc album.  | `{disc}-{track:02d} {title}`                 |
+| `--template-folder-no-album` / `template_folder_no_album`       | Template folder for the tracks that are not part of an album.      | `{artist}/Unknown Album`                     |
+| `--template-file-no-album` / `template_file_no_album`           | Template file for the tracks that are not part of an album.        | `{title}`                                    |
+| `--template-date` / `template_date`                             | Date tag template.                                                 | `%Y-%m-%dT%H:%M:%SZ`                         |
+| `--exclude-tags` / `exclude_tags`                               | Comma-separated tags to exclude.                                   | `null`                                       |
+| `--cover-size` / `cover_size`                                   | Cover size.                                                        | `1200`                                       |
+| `--truncate` / `truncate`                                       | Maximum length of the file/folder names.                           | `40`                                         |
+| `--codec-song` / `codec_song`                                   | Song codec.                                                        | `aac-legacy`                                 |
+| `--synced-lyrics-format` / `synced_lyrics_format`               | Synced lyrics format.                                              | `lrc`                                        |
+| `--codec-music-video` / `codec_music_video`                     | Music video codec.                                                 | `h264-best`                                  |
+| `--quality-post` / `quality_post`                               | Post video quality.                                                | `best`                                       |
+| `--no-config-file`, `-n` / -                                    | Do not use a config file.                                          | `false`                                      |
 
 ### Tags variables
 The following variables can be used in the template folders/files and/or in the `exclude_tags` list:
 * `album`
 * `album_artist`
 * `album_id`
 * `album_sort`
@@ -121,41 +109,69 @@
 * `storefront`
 * `title`
 * `title_id`
 * `title_sort`
 * `track`
 * `track_total`
 * `xid`
-  
-### Remux mode
+
+### Remux modes
 The following remux modes are available:
 * `ffmpeg`
-    * Can decrypt and remux songs but can't decrypt music videos by itself
-    * Decryption may not work on older versions of FFmpeg
+    * Can be used without mp4decrypt only for songs and when using legacy song codecs
 * `mp4box`
     * Requires mp4decrypt
     * Doesn't convert closed captions in music videos that have them
     * Can be obtained from here: https://gpac.wp.imt.fr/downloads
 
-### Download mode
+### Download modes
 The following download modes are available:
 * `ytdlp`
 * `nm3u8dlre`
     * Faster than `ytdlp`
     * Requires FFmpeg
     * Can be obtained from here: https://github.com/nilaoda/N_m3u8DL-RE/releases
 
-## Music videos quality
-Music videos will be downloaded in the highest quality available by default. The available qualities are:
-* AVC 1080p 10mbps, AAC 256kbps
-* AVC 1080p 6.5mbps, AAC 256kbps
-* AVC 720p 4mbps, AAC 256kbps
-* AVC 576p 2mbps, AAC 256kbps
-* AVC 480p 1.5mbps, AAC 256kbps
-* AVC 360p 1mbps, AAC 256kbps
-
-By enabling the `prefer_hevc` option, music videos will be downloaded in the highest HEVC quality available. The available qualities are:
-* HEVC 4K 20mbps, AAC 256kbps
-* HEVC 4K 12mbps, AAC 256kbps
 
-Enable `ask_video_format` to select a custom audio/video format.
+### Song codecs
+The following codecs are available:
+* `aac-legacy`
+* `aac-he-legacy`
+* `aac`
+* `aac-he`
+* `aac-binaural`
+* `aac-downmix`
+* `aac-he-binaural`
+* `aac-he-downmix`
+* `alac`
+* `atmos`
+
+**Support for non-legacy codecs are not guaranteed, as most of the songs cannot be decrypted  when using non-legacy codecs.**
+
+### Music videos codecs
+The following codecs are available:
+* `h264-best` (with AAC 256kbps, up to 1080p)
+* `h265-best` (With AAC 256kpbs, up to 2160p)
+* `ask`
+    * When using this option, the script will ask you which audio and video codec to use.
+  
+### Post videos/extra videos qualities
+The following qualities are available:
+* `best` (with AAC 256kbps, up to 1080p)
+* `ask`
+    * When using this option, the script will ask you which video quality to use.
+
+Post videos doesn't require remuxing and are limited to `ytdlp` download mode.
+
+### Synced lyrics formats
+The following synced lyrics formats are available:
+* `lrc`
+* `srt`
+* `ttml`
+    * Native format for Apple Music synced lyrics.
+    * Highly unsupported by media players.
+  
+### Cover formats
+The following cover formats are available:
+* `jpg`
+* `png`
```

