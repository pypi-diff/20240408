# Comparing `tmp/RealTimeTTS-0.3.43.tar.gz` & `tmp/RealTimeTTS-0.3.44.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RealTimeTTS-0.3.43.tar", last modified: Thu Mar 21 19:29:46 2024, max compression
+gzip compressed data, was "RealTimeTTS-0.3.44.tar", last modified: Mon Apr  8 00:16:32 2024, max compression
```

## Comparing `RealTimeTTS-0.3.43.tar` & `RealTimeTTS-0.3.44.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2024-03-21 19:29:46.798023 RealTimeTTS-0.3.43/
--rw-rw-rw-   0        0        0    18536 2024-03-21 19:29:46.797021 RealTimeTTS-0.3.43/PKG-INFO
--rw-rw-rw-   0        0        0    17417 2024-03-21 19:28:35.000000 RealTimeTTS-0.3.43/README.md
-drwxrwxrwx   0        0        0        0 2024-03-21 19:29:46.796021 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/
--rw-rw-rw-   0        0        0    18536 2024-03-21 19:29:46.000000 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      768 2024-03-21 19:29:46.000000 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-21 19:29:46.000000 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      182 2024-03-21 19:29:46.000000 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-03-21 19:29:46.000000 RealTimeTTS-0.3.43/RealTimeTTS.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-03-21 19:29:46.777569 RealTimeTTS-0.3.43/RealtimeTTS/
--rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.43/RealtimeTTS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-21 19:29:46.792583 RealTimeTTS-0.3.43/RealtimeTTS/engines/
--rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/__init__.py
--rw-rw-rw-   0        0        0     9413 2024-03-15 16:54:18.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/azure_engine.py
--rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/base_engine.py
--rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/chinese.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/coqui_default_voice.json
--rw-rw-rw-   0        0        0    35572 2024-03-21 19:27:30.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/coqui_engine.py
--rw-rw-rw-   0        0        0    10331 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/elevenlabs_engine.py
--rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/female.json
--rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/male.json
--rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/openai_engine.py
--rw-rw-rw-   0        0        0     4834 2023-12-07 10:47:05.000000 RealTimeTTS-0.3.43/RealtimeTTS/engines/system_engine.py
--rw-rw-rw-   0        0        0     9725 2024-01-11 13:19:24.000000 RealTimeTTS-0.3.43/RealtimeTTS/stream_player.py
--rw-rw-rw-   0        0        0    27325 2024-03-21 19:08:11.000000 RealTimeTTS-0.3.43/RealtimeTTS/text_to_stream.py
--rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.43/RealtimeTTS/threadsafe_generators.py
--rw-rw-rw-   0        0        0       42 2024-03-21 19:29:46.798023 RealTimeTTS-0.3.43/setup.cfg
--rw-rw-rw-   0        0        0     1295 2024-03-21 19:16:44.000000 RealTimeTTS-0.3.43/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-21 19:29:46.795017 RealTimeTTS-0.3.43/tests/
--rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.43/tests/test_callbacks.py
--rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.43/tests/test_on_audio_chunk_callback.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.331675 RealTimeTTS-0.3.44/
+-rw-rw-rw-   0        0        0    19233 2024-04-08 00:16:32.330673 RealTimeTTS-0.3.44/PKG-INFO
+-rw-rw-rw-   0        0        0    18114 2024-04-08 00:07:46.000000 RealTimeTTS-0.3.44/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.329673 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/
+-rw-rw-rw-   0        0        0    19233 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      768 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      182 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 00:16:32.000000 RealTimeTTS-0.3.44/RealTimeTTS.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.242551 RealTimeTTS-0.3.44/RealtimeTTS/
+-rw-rw-rw-   0        0        0      422 2023-12-28 10:50:12.000000 RealTimeTTS-0.3.44/RealtimeTTS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.325669 RealTimeTTS-0.3.44/RealtimeTTS/engines/
+-rw-rw-rw-   0        0        0      397 2023-12-28 10:50:55.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/__init__.py
+-rw-rw-rw-   0        0        0     9413 2024-03-15 16:54:18.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/azure_engine.py
+-rw-rw-rw-   0        0        0     4490 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/base_engine.py
+-rw-rw-rw-   0        0        0   506471 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/chinese.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_default_voice.json
+-rw-rw-rw-   0        0        0    38627 2024-04-07 23:58:16.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_engine.py
+-rw-rw-rw-   0        0        0    10331 2023-12-01 16:58:58.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/elevenlabs_engine.py
+-rw-rw-rw-   0        0        0   505425 2023-11-17 22:30:40.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/female.json
+-rw-rw-rw-   0        0        0   506653 2023-12-07 22:51:46.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/male.json
+-rw-rw-rw-   0        0        0     3477 2023-12-28 10:13:43.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/openai_engine.py
+-rw-rw-rw-   0        0        0     4834 2023-12-07 10:47:05.000000 RealTimeTTS-0.3.44/RealtimeTTS/engines/system_engine.py
+-rw-rw-rw-   0        0        0    10159 2024-04-08 00:13:32.000000 RealTimeTTS-0.3.44/RealtimeTTS/stream_player.py
+-rw-rw-rw-   0        0        0    27936 2024-04-08 00:03:01.000000 RealTimeTTS-0.3.44/RealtimeTTS/text_to_stream.py
+-rw-rw-rw-   0        0        0    10179 2023-11-29 16:17:54.000000 RealTimeTTS-0.3.44/RealtimeTTS/threadsafe_generators.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 00:16:32.331675 RealTimeTTS-0.3.44/setup.cfg
+-rw-rw-rw-   0        0        0     1295 2024-04-08 00:16:23.000000 RealTimeTTS-0.3.44/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 00:16:32.327670 RealTimeTTS-0.3.44/tests/
+-rw-rw-rw-   0        0        0     1361 2023-11-03 15:39:11.000000 RealTimeTTS-0.3.44/tests/test_callbacks.py
+-rw-rw-rw-   0        0        0      637 2024-02-21 18:39:01.000000 RealTimeTTS-0.3.44/tests/test_on_audio_chunk_callback.py
```

### Comparing `RealTimeTTS-0.3.43/PKG-INFO` & `RealTimeTTS-0.3.44/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.43
+Version: 0.3.44
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## Updates
 
-Latest Version: v0.3.43
+Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -83,15 +83,15 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.1.1+cu118 torchaudio==2.1.1+cu118 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
@@ -126,15 +126,15 @@
 
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
-- to clone a voice submit the filename of a wave file containing the source voice as cloning_reference_wav to the CoquiEngine constructor
+- to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
 - in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
@@ -251,15 +251,17 @@
 
 ```python
 stream.stop()
 ```
 
 ## Requirements Explained
 
-- Python 3.6+
+- **Python Version**: 
+  - **Required**: Python >= 3.9, < 3.12
+  - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
 - **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
   
 - **PyAudio (>=0.2.13)**: to create an output audio stream
   
 - **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
 
@@ -302,14 +304,32 @@
 - **Description**: This optional callback function is called when the audio stream stops. Ideal for resource cleanup or post-processing tasks.
 
 #### `on_character` (callable)
 - **Type**: Callable function
 - **Required**: No
 - **Description**: This optional callback function is called when a single character is processed.
 
+#### `output_device_index` (int)
+- **Type**: Integer
+- **Required**: No
+- **Default**: None
+- **Description**: Specifies the output device index to use. None uses the default device.
+
+#### `tokenizer` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: nltk
+- **Description**: Tokenizer to use for sentence splitting (currently "nltk" and "stanza" are supported).
+
+#### `language` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: en
+- **Description**: Language to use for sentence splitting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.43/README.md` & `RealTimeTTS-0.3.44/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## Updates
 
-Latest Version: v0.3.43
+Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -59,15 +59,15 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.1.1+cu118 torchaudio==2.1.1+cu118 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
@@ -102,15 +102,15 @@
 
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
-- to clone a voice submit the filename of a wave file containing the source voice as cloning_reference_wav to the CoquiEngine constructor
+- to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
 - in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
@@ -227,15 +227,17 @@
 
 ```python
 stream.stop()
 ```
 
 ## Requirements Explained
 
-- Python 3.6+
+- **Python Version**: 
+  - **Required**: Python >= 3.9, < 3.12
+  - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
 - **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
   
 - **PyAudio (>=0.2.13)**: to create an output audio stream
   
 - **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
 
@@ -278,14 +280,32 @@
 - **Description**: This optional callback function is called when the audio stream stops. Ideal for resource cleanup or post-processing tasks.
 
 #### `on_character` (callable)
 - **Type**: Callable function
 - **Required**: No
 - **Description**: This optional callback function is called when a single character is processed.
 
+#### `output_device_index` (int)
+- **Type**: Integer
+- **Required**: No
+- **Default**: None
+- **Description**: Specifies the output device index to use. None uses the default device.
+
+#### `tokenizer` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: nltk
+- **Description**: Tokenizer to use for sentence splitting (currently "nltk" and "stanza" are supported).
+
+#### `language` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: en
+- **Description**: Language to use for sentence splitting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.43/RealTimeTTS.egg-info/PKG-INFO` & `RealTimeTTS-0.3.44/RealTimeTTS.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RealTimeTTS
-Version: 0.3.43
+Version: 0.3.44
 Summary: *Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.
 Home-page: https://github.com/KoljaB/RealTimeTTS
 Author: Kolja Beigel
 Author-email: kolja.beigel@web.de
 Keywords: real-time,text-to-speech,TTS,streaming,audio,voice,synthesis,sentence-segmentation,low-latency,character-streaming,dynamic feedback,audio-output,text-input,TTS-engine,audio-playback,stream-player,sentence-fragment,audio-feedback,interactive,python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -46,15 +46,15 @@
   - ensures continuous operation with a fallback mechanism
   - switches to alternative engines in case of disruptions guaranteeing consistent performance and reliability, which is vital for critical and professional use cases
 
 > **Hint**: *check out [RealtimeSTT](https://github.com/KoljaB/RealtimeSTT), the input counterpart of this library, for speech-to-text capabilities. Together, they form a powerful realtime audio wrapper around large language models.*
 
 ## Updates
 
-Latest Version: v0.3.43
+Latest Version: v0.3.44
 
 See [release history](https://github.com/KoljaB/RealtimeTTS/releases).
 
 ## Tech Stack
 
 This library uses:
 
@@ -83,15 +83,15 @@
 Installation into virtual environment with GPU support:
 
 ```bash
 python -m venv env_realtimetts
 env_realtimetts\Scripts\activate.bat
 python.exe -m pip install --upgrade pip
 pip install RealtimeTTS
-pip install torch==2.1.1+cu118 torchaudio==2.1.1+cu118 --index-url https://download.pytorch.org/whl/cu118
+pip install torch==2.2.1+cu118 torchaudio==2.2.1 --index-url https://download.pytorch.org/whl/cu118
 ```
 
 More information about [CUDA installation](#cuda-installation).
 
 ## Engine Requirements
 
 Different engines supported by RealtimeTTS have unique requirements. Ensure you fulfill these requirements based on the engine you choose.
@@ -126,15 +126,15 @@
 
 ### CoquiEngine
 
 Delivers high quality, local, neural TTS with voice-cloning.  
 
 Downloads a neural TTS model first. In most cases it be fast enought for Realtime using GPU synthesis. Needs around 4-5 GB VRAM.
 
-- to clone a voice submit the filename of a wave file containing the source voice as cloning_reference_wav to the CoquiEngine constructor
+- to clone a voice submit the filename of a wave file containing the source voice as "voice" parameter to the CoquiEngine constructor
 - in my experience voice cloning works best with a 22050 Hz mono 16bit WAV file containing a short (~10-30 sec) sample 
 
 On most systems GPU support will be needed to run fast enough for realtime, otherwise you will experience stuttering.
 
 ## Quick Start
 
 Here's a basic usage example:
@@ -251,15 +251,17 @@
 
 ```python
 stream.stop()
 ```
 
 ## Requirements Explained
 
-- Python 3.6+
+- **Python Version**: 
+  - **Required**: Python >= 3.9, < 3.12
+  - **Reason**: The library depends on the GitHub library "TTS" from coqui, which requires Python versions in this range.
 
 - **requests (>=2.31.0)**: to send HTTP requests for API calls and voice list retrieval
   
 - **PyAudio (>=0.2.13)**: to create an output audio stream
   
 - **stream2sentence (>=0.1.1)**: to split the incoming text stream into sentences 
 
@@ -302,14 +304,32 @@
 - **Description**: This optional callback function is called when the audio stream stops. Ideal for resource cleanup or post-processing tasks.
 
 #### `on_character` (callable)
 - **Type**: Callable function
 - **Required**: No
 - **Description**: This optional callback function is called when a single character is processed.
 
+#### `output_device_index` (int)
+- **Type**: Integer
+- **Required**: No
+- **Default**: None
+- **Description**: Specifies the output device index to use. None uses the default device.
+
+#### `tokenizer` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: nltk
+- **Description**: Tokenizer to use for sentence splitting (currently "nltk" and "stanza" are supported).
+
+#### `language` (string)
+- **Type**: String
+- **Required**: No
+- **Default**: en
+- **Description**: Language to use for sentence splitting.
+
 #### `level` (int)
 - **Type**: Integer
 - **Required**: No
 - **Default**: `logging.WARNING`
 - **Description**: Sets the logging level for the internal logger. This can be any integer constant from Python's built-in `logging` module.
 
 #### Example Usage:
```

### Comparing `RealTimeTTS-0.3.43/RealTimeTTS.egg-info/SOURCES.txt` & `RealTimeTTS-0.3.44/RealTimeTTS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/azure_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/azure_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/base_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/base_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/chinese.json` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/chinese.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/coqui_default_voice.json` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_default_voice.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/coqui_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/coqui_engine.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,21 +5,25 @@
 from tqdm import tqdm
 import numpy as np
 import traceback
 import requests
 import logging
 import pyaudio
 import torch
+import time
 import json
 import sys
 import io
 import os
 import re
 
 
+TIME_SLEEP_DEVICE_RESET = 2
+
+
 class QueueWriter(io.TextIOBase):
     """
     Custom file-like object to write text to a multiprocessing queue.
     """
     def __init__(self, queue):
         super().__init__()
         self.queue = queue
@@ -65,16 +69,17 @@
                  full_sentences=False,
                  level=logging.WARNING,
                  use_mps=False,
                  use_deepspeed=False,
                  prepare_text_for_synthesis_callback=None,
                  add_sentence_filter=False,
                  pretrained=False,
-                 comma_silence_duration=0.15,
-                 sentence_silence_duration=0.35,
+                 comma_silence_duration=0.3,
+                 sentence_silence_duration=0.6,
+                 default_silence_duration=0.3
                  ):
         """
         Initializes a coqui voice realtime text to speech engine object.
 
         Args:
             model_name (str):
               Name of the coqui model to use.
@@ -149,14 +154,15 @@
         self.enable_text_splitting = enable_text_splitting
         self.full_sentences = full_sentences
         self.use_mps = use_mps
         self.use_deepspeed = use_deepspeed
         self.add_sentence_filter = add_sentence_filter
         self.comma_silence_duration = comma_silence_duration
         self.sentence_silence_duration = sentence_silence_duration
+        self.default_silence_duration = default_silence_duration
 
         self.cloning_reference_wav = voice
         self.speed = speed
         self.specific_model = specific_model
         if not local_models_path:
             local_models_path = os.environ.get("COQUI_MODEL_PATH")
             if local_models_path and len(local_models_path) > 0:
@@ -239,15 +245,16 @@
                 self.use_mps,
                 self.model_path,
                 self.use_deepspeed,
                 self.voices_path,
                 self.voices_list,
                 self.pretrained,
                 self.comma_silence_duration,
-                self.sentence_silence_duration
+                self.sentence_silence_duration,
+                self.default_silence_duration
             ))
         self.synthesize_process.start()
 
         logging.debug('Waiting for coqui model start')
         self.main_synthesize_ready_event.wait()
         logging.info('Coqui synthesis model ready')
 
@@ -277,15 +284,16 @@
             use_mps,
             local_model_path,
             use_deepspeed,
             voices_path,
             predefined_voices,
             pretrained,
             comma_silence_duration,
-            sentence_silence_duration):
+            sentence_silence_duration,
+            default_silence_duration):
         """
         Worker process for the coqui text to speech synthesis model.
 
         Args:
             conn (multiprocessing.Connection):
               Connection to the parent process.
             model_name (str): Name of the coqui model to use.
@@ -437,47 +445,51 @@
             chunk = chunk[None, : int(chunk.shape[0])]
             chunk = np.clip(chunk, -1, 1)
             chunk = chunk.astype(np.float32)
             return chunk
 
         def load_model(checkpoint, tts):
             global config
-            if tts:
-                import gc
-                del tts
-                torch.cuda.empty_cache()
-                gc.collect()
-                from numba import cuda
-                current_device = cuda.get_current_device()
-                current_device.reset()
-                tts = None
-                import time
-                time.sleep(10)
-
-            torch.set_num_threads(int(str(thread_count)))
-            if torch.cuda.is_available():
-                device = torch.device("cuda")
-            elif use_mps and torch.backends.mps.is_available() and torch.backends.mps.is_built():
-                device = torch.device("mps")
-            else:
-                device = torch.device("cpu")
+            try:
+                if tts:
+                    import gc
+                    del tts
+                    torch.cuda.empty_cache()
+                    gc.collect()
+                    from numba import cuda
+                    current_device = cuda.get_current_device()
+                    current_device.reset()
+                    tts = None
+                    import time
+                    time.sleep(TIME_SLEEP_DEVICE_RESET)
+
+                torch.set_num_threads(int(str(thread_count)))
+                if torch.cuda.is_available():
+                    device = torch.device("cuda")
+                elif use_mps and torch.backends.mps.is_available() and torch.backends.mps.is_built():
+                    device = torch.device("mps")
+                else:
+                    device = torch.device("cpu")
 
-            config = load_config((os.path.join(checkpoint, "config.json")))
-            tts = setup_tts_model(config)
-            logging.debug(f"  xtts load_checkpoint({checkpoint})")
-
-            tts.load_checkpoint(
-                config,
-                checkpoint_dir=checkpoint,
-                checkpoint_path=None,
-                vocab_path=None,
-                eval=True,
-                use_deepspeed=use_deepspeed,
-            )
-            tts.to(device)
+                config = load_config((os.path.join(checkpoint, "config.json")))
+                tts = setup_tts_model(config)
+                logging.debug(f"  xtts load_checkpoint({checkpoint})")
+
+                tts.load_checkpoint(
+                    config,
+                    checkpoint_dir=checkpoint,
+                    checkpoint_path=None,
+                    vocab_path=None,
+                    eval=True,
+                    use_deepspeed=use_deepspeed,
+                )
+                tts.to(device)
+            except Exception as e:
+                print(f"Error loading model for checkpoint {checkpoint}: {e}")
+                raise
             return tts
 
         logging.debug(f"Initializing coqui model {model_name}")
         logging.debug(f" - cloning reference {cloning_reference_wav}")
         logging.debug(f" - language {language}")
         logging.debug(f" - user data dir {get_user_data_dir('tts')}")
         logging.debug(f" - local model path {local_model_path}")
@@ -528,14 +540,21 @@
                 elif command == 'synthesize':
 
                     text = data['text']
                     language = data['language']
 
                     logging.debug(f'Starting inference for text: {text}')
 
+                    print(f"XTTS Synthesizing: {text}")
+                    time_start = time.time()
+                    seconds_to_first_chunk = 0.0
+                    full_generated_seconds = 0.0
+                    raw_inference_start = 0.0
+                    first_chunk_length_seconds = 0.0
+
                     chunks = tts.inference_stream(
                         text,
                         language,
                         gpt_cond_latent,
                         speaker_embedding,
                         stream_chunk_size=stream_chunk_size,
                         overlap_wav_len=overlap_wav_len,
@@ -549,35 +568,72 @@
                     )
 
                     if full_sentences:
                         chunklist = []
 
                         for i, chunk in enumerate(chunks):
                             chunk = postprocess_wave(chunk)
+                            chunk_bytes = chunk.tobytes()
+                            chunklist.append(chunk_bytes)
+                            chunk_duration = len(chunk_bytes) / (4 * 24000)
+                            full_generated_seconds += chunk_duration
+                            if i == 0:
+                                first_chunk_length_seconds = chunk_duration
+                                raw_inference_start = time.time()
+                                seconds_to_first_chunk = raw_inference_start - time_start
+
+                        for i, chunk in enumerate(chunks):
+                            chunk = postprocess_wave(chunk)
                             chunklist.append(chunk.tobytes())
 
                         for chunk in chunklist:
                             conn.send(('success', chunk))
                     else:
                         for i, chunk in enumerate(chunks):
                             chunk = postprocess_wave(chunk)
-                            conn.send(('success', chunk.tobytes()))
+                            chunk_bytes = chunk.tobytes()
+                            conn.send(('success', chunk_bytes))
+                            chunk_duration = len(chunk_bytes) / (4 * 24000)  # 4 bytes per sample, 24000 Hz
+                            full_generated_seconds += chunk_duration
+                            if i == 0:
+                                first_chunk_length_seconds = chunk_duration
+                                raw_inference_start = time.time()
+                                seconds_to_first_chunk = raw_inference_start - time_start
+
+                    time_end = time.time()
+                    seconds = time_end - time_start
+
+                    if full_generated_seconds > 0 and (full_generated_seconds - first_chunk_length_seconds) > 0:
+
+                        realtime_factor = seconds / full_generated_seconds
+                        raw_inference_time = seconds - seconds_to_first_chunk
+                        raw_inference_factor = raw_inference_time / (full_generated_seconds - first_chunk_length_seconds) 
+
+                        # print(
+                        #     f"XTTS synthesized {full_generated_seconds:.2f}s"
+                        #     f" audio in {seconds:.2f}s"
+                        #     f" realtime factor: {realtime_factor:.2f}x"
+                        # )
+                        # print(
+                        #     f"seconds to first chunk: {seconds_to_first_chunk:.2f}s"
+                        #     f" raw_inference_factor: {raw_inference_factor:.2f}x"
+                        # )
 
                     # Send silent audio
                     sample_rate = config.audio.sample_rate
 
                     end_sentence_delimeters = ".!?…。¡¿"
                     mid_sentence_delimeters = ";:,\n()[]{}-“”„”—/|《》"
 
                     if text[-1] in end_sentence_delimeters:
                         silence_duration = sentence_silence_duration
                     elif text[-1] in mid_sentence_delimeters:
                         silence_duration = comma_silence_duration
                     else:
-                        silence_duration = 0
+                        silence_duration = default_silence_duration
 
                     silent_samples = int(sample_rate * silence_duration)
                     silent_chunk = np.zeros(silent_samples, dtype=np.float32)
                     conn.send(('success', silent_chunk.tobytes()))
 
                     conn.send(('finished', ''))
```

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/elevenlabs_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/elevenlabs_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/female.json` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/female.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/male.json` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/male.json`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/openai_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/openai_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/engines/system_engine.py` & `RealTimeTTS-0.3.44/RealtimeTTS/engines/system_engine.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/stream_player.py` & `RealTimeTTS-0.3.44/RealtimeTTS/stream_player.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,24 +16,27 @@
     Defines the configuration for an audio stream.
     """
 
     def __init__(
             self,
             format: int = pyaudio.paInt16,
             channels: int = 1,
-            rate: int = 16000):
+            rate: int = 16000,
+            output_device_index=None):
         """
         Args:
             format (int): Audio format, defaults to pyaudio.paInt16
             channels (int): Number of channels, defaults to 1 (mono)
             rate (int): Sample rate, defaults to 16000
+            output_device_index (int): Output device index, defaults to None
         """
         self.format = format
         self.channels = channels
         self.rate = rate
+        self.output_device_index = output_device_index
 
 
 class AudioStream:
     """
     Handles audio stream operations
     - opening, starting, stopping, and closing
     """
@@ -49,31 +52,37 @@
 
     def open_stream(self):
         """Opens an audio stream."""
 
         # check for mpeg format
         pyChannels = self.config.channels
         pySampleRate = self.config.rate
+        pyOutput_device_index = self.config.output_device_index
 
         if self.config.format == pyaudio.paCustomFormat:
             pyFormat = self.pyaudio_instance.get_format_from_width(2)
             logging.debug("Opening stream for mpeg audio chunks, "
                           f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
                           f"pySampleRate: {pySampleRate}")
         else:
             pyFormat = self.config.format
             logging.debug("Opening stream for wave audio chunks, "
                           f"pyFormat: {pyFormat}, pyChannels: {pyChannels}, "
                           f"pySampleRate: {pySampleRate}")
 
-        self.stream = self.pyaudio_instance.open(
-            format=pyFormat,
-            channels=pyChannels,
-            rate=pySampleRate,
-            output=True)
+        try:
+            self.stream = self.pyaudio_instance.open(
+                format=pyFormat,
+                channels=pyChannels,
+                rate=pySampleRate,
+                output_device_index=pyOutput_device_index,
+                output=True)
+        except Exception as e:
+            print(f"Error opening stream: {e}")
+            exit(0)
 
     def start_stream(self):
         """Starts the audio stream."""
         if self.stream and not self.stream.is_active():
             self.stream.start_stream()
 
     def stop_stream(self):
```

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/text_to_stream.py` & `RealTimeTTS-0.3.44/RealtimeTTS/text_to_stream.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,14 +22,15 @@
                  engine: Union[BaseEngine, List[BaseEngine]],
                  log_characters: bool = False,
                  on_text_stream_start=None,
                  on_text_stream_stop=None,
                  on_audio_stream_start=None,
                  on_audio_stream_stop=None,
                  on_character=None,
+                 output_device_index=None,
                  tokenizer: str = "nltk",
                  language: str = "en",
                  level=logging.WARNING,
                  ):
         """
         Initializes the TextToAudioStream.
 
@@ -43,21 +44,27 @@
               gets called when the text stream stops.
             on_audio_stream_start (callable, optional): Callback function that
               gets called when the audio stream starts.
             on_audio_stream_stop (callable, optional): Callback function that
               gets called when the audio stream stops.
             on_character (callable, optional): Callback function that gets
               called when a single character is processed.
+            output_device_index (int, optional): The index of the output device
+                to use for audio playback.
+            tokenizer (str, optional): Tokenizer to use for sentence splitting
+                (currently "nltk" and "stanza" are supported).
+            language (str, optional): Language to use for sentence splitting.
             level (int, optional): Logging level. Defaults to logging.WARNING.
         """
         self.log_characters = log_characters
         self.on_text_stream_start = on_text_stream_start
         self.on_text_stream_stop = on_text_stream_stop
         self.on_audio_stream_start = on_audio_stream_start
         self.on_audio_stream_stop = on_audio_stream_stop
+        self.output_device_index = output_device_index
         self.output_wavfile = None
         self.chunk_callback = None
         self.wf = None
         self.abort_events = []
         self.tokenizer = tokenizer
         self.language = language
         self.player = None
@@ -105,15 +112,22 @@
         self.engine = engine
 
         # Extract stream information (format, channels, rate) from the engine
         format, channels, rate = self.engine.get_stream_info()
 
         # Check if the engine doesn't support consuming generators directly
         if not self.engine.can_consume_generators:
-            self.player = StreamPlayer(self.engine.queue, AudioConfiguration(format, channels, rate), on_playback_start=self._on_audio_stream_start)
+            self.player = StreamPlayer(
+                self.engine.queue,
+                AudioConfiguration(
+                    format,
+                    channels,
+                    rate,
+                    self.output_device_index),
+                on_playback_start=self._on_audio_stream_start)
         else:
             self.engine.on_playback_start = self._on_audio_stream_start
             self.player = None
 
         logging.info(f"loaded engine {self.engine.engine_name}")
```

### Comparing `RealTimeTTS-0.3.43/RealtimeTTS/threadsafe_generators.py` & `RealTimeTTS-0.3.44/RealtimeTTS/threadsafe_generators.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/setup.py` & `RealTimeTTS-0.3.44/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 # Read requirements.txt
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setuptools.setup(
     name="RealTimeTTS",
-    version="0.3.43",
+    version="0.3.44",
     author="Kolja Beigel",
     author_email="kolja.beigel@web.de",
     description="*Stream text into audio with an easy-to-use, highly configurable library delivering voice output with minimal latency.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/KoljaB/RealTimeTTS",
     packages=setuptools.find_packages(),
```

### Comparing `RealTimeTTS-0.3.43/tests/test_callbacks.py` & `RealTimeTTS-0.3.44/tests/test_callbacks.py`

 * *Files identical despite different names*

### Comparing `RealTimeTTS-0.3.43/tests/test_on_audio_chunk_callback.py` & `RealTimeTTS-0.3.44/tests/test_on_audio_chunk_callback.py`

 * *Files identical despite different names*

