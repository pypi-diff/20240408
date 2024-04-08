# Comparing `tmp/circuitsapi-0.0.2.tar.gz` & `tmp/circuitsapi-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "circuitsapi-0.0.2.tar", last modified: Fri Apr  5 18:02:33 2024, max compression
+gzip compressed data, was "circuitsapi-0.0.3.tar", last modified: Mon Apr  8 16:51:12 2024, max compression
```

## Comparing `circuitsapi-0.0.2.tar` & `circuitsapi-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2024-04-05 18:02:33.238216 circuitsapi-0.0.2/
--rw-rw-rw-   0        0        0     5540 2024-04-05 18:02:33.236195 circuitsapi-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     4835 2024-04-05 17:51:01.000000 circuitsapi-0.0.2/README.md
--rw-rw-rw-   0        0        0      775 2024-04-05 18:01:59.000000 circuitsapi-0.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-05 18:02:33.239230 circuitsapi-0.0.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-05 18:02:33.192458 circuitsapi-0.0.2/src/
-drwxrwxrwx   0        0        0        0 2024-04-05 18:02:33.205678 circuitsapi-0.0.2/src/circuitsapi/
--rw-rw-rw-   0        0        0      173 2024-04-05 16:32:20.000000 circuitsapi-0.0.2/src/circuitsapi/__init__.py
--rw-rw-rw-   0        0        0    18789 2024-04-05 16:31:46.000000 circuitsapi-0.0.2/src/circuitsapi/client.py
--rw-rw-rw-   0        0        0     1792 2024-03-30 18:22:40.000000 circuitsapi-0.0.2/src/circuitsapi/exceptions.py
--rw-rw-rw-   0        0        0     2843 2024-04-03 08:48:12.000000 circuitsapi-0.0.2/src/circuitsapi/helpers.py
--rw-rw-rw-   0        0        0     1448 2024-04-02 16:55:51.000000 circuitsapi-0.0.2/src/circuitsapi/request.py
-drwxrwxrwx   0        0        0        0 2024-04-05 18:02:33.235175 circuitsapi-0.0.2/src/circuitsapi.egg-info/
--rw-rw-rw-   0        0        0     5540 2024-04-05 18:02:33.000000 circuitsapi-0.0.2/src/circuitsapi.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      356 2024-04-05 18:02:33.000000 circuitsapi-0.0.2/src/circuitsapi.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-05 18:02:33.000000 circuitsapi-0.0.2/src/circuitsapi.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      108 2024-04-05 18:02:33.000000 circuitsapi-0.0.2/src/circuitsapi.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-05 18:02:33.000000 circuitsapi-0.0.2/src/circuitsapi.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.325513 circuitsapi-0.0.3/
+-rw-rw-rw-   0        0        0     1092 2024-04-05 20:02:02.000000 circuitsapi-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0     6742 2024-04-08 16:51:12.323970 circuitsapi-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6014 2024-04-08 16:29:36.000000 circuitsapi-0.0.3/README.md
+-rw-rw-rw-   0        0        0      775 2024-04-08 16:50:58.000000 circuitsapi-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-08 16:51:12.325513 circuitsapi-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.244824 circuitsapi-0.0.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.282830 circuitsapi-0.0.3/src/circuitsapi/
+-rw-rw-rw-   0        0        0      173 2024-04-05 16:32:20.000000 circuitsapi-0.0.3/src/circuitsapi/__init__.py
+-rw-rw-rw-   0        0        0    18968 2024-04-08 16:29:26.000000 circuitsapi-0.0.3/src/circuitsapi/client.py
+-rw-rw-rw-   0        0        0     1792 2024-03-30 18:22:40.000000 circuitsapi-0.0.3/src/circuitsapi/exceptions.py
+-rw-rw-rw-   0        0        0     2843 2024-04-03 08:48:12.000000 circuitsapi-0.0.3/src/circuitsapi/helpers.py
+-rw-rw-rw-   0        0        0     1448 2024-04-02 16:55:51.000000 circuitsapi-0.0.3/src/circuitsapi/request.py
+drwxrwxrwx   0        0        0        0 2024-04-08 16:51:12.318393 circuitsapi-0.0.3/src/circuitsapi.egg-info/
+-rw-rw-rw-   0        0        0     6742 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      364 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-08 16:51:12.000000 circuitsapi-0.0.3/src/circuitsapi.egg-info/top_level.txt
```

### Comparing `circuitsapi-0.0.2/PKG-INFO` & `circuitsapi-0.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 Metadata-Version: 2.1
 Name: circuitsapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: CircuitsAPI is a system to transmit data to Rec Room circuits.
 Author: Jegarde
 Project-URL: Homepage, https://github.com/Jegarde/CircuitsAPI
 Project-URL: Bug Tracker, https://github.com/Jegarde/CircuitsAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: aiohttp==3.9.2
 Requires-Dist: recnetpy==0.2.71
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: recnetlogin==0.1.1
 
 ![promo](https://github.com/Jegarde/CircuitsAPI/assets/13438202/554a02af-6862-44d9-aa80-da78fccdb409)
 
 ## THIS PROJECT IS IN PRE-ALPHA STAGE
 This system has not been properly tested. It is constantly being updated with breaking changes. Do not use this system in a production environment. Only use it for testing and experimenting.
 
+Detailed documentation and instructions coming later.
+
+Feel free to contact @Jegarde on Discord for inquiries.
+
 ## What is this?
 A system to communicate with CV2 using Python.
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/fad38801-641f-439f-ab36-249bc22d08e9" width="400">
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/70d09f93-8f40-4dff-8c26-f1577d91ba6f" width="350">
 
 ## Limitations
 - You must sacrifice the following permission roles: host, moderator & contributor. Co-owner will be the only role you can grant others without triggering the system. 
 - Room owner & co-owners will not be able to receive data by this system.
 - You can only send a single bit at once. This system is not applicable for big data transmissions.
 - CV2 pongs require messing with the instance's matchmaking state.
 - The circuits are currently made in Rooms v2 to prevent the system being used in existing production rooms due to instability.
   - It will be ported over to Rooms v1 once it's stable enough.
 
-## Rec Room Setup
-1. Clone the template room: https://rec.net/room/CircuitsAPI.
-2. **IMPORTANT:** Remove any privileged permissions from the following roles from the room: host, moderator & contributor. Otherwise you may risk troublemakers abusing the privileges.
-3. Add `circuitsapi` as a room tag to indicate it's supported by the system.
-4. Activate the 'Receiver' circuit board.
-
 ## Installation
-1. Download and unpack the [repository](https://github.com/Jegarde/CircuitsAPI/archive/refs/heads/pre-alpha.zip).
-2. Install the Python requirements. `pip install -U -r requirements.txt`
-3. Include the `circuitsapi` directory in your project. That is the library.
+The recommended method is installing via [pip](https://pypi.org/project/pip/).
+
+`pip install -U circuitsapi`
+
+For instructions on installing Python and pip, see [The Hitchhiker's Guide to Python](https://docs.python-guide.org/starting/installation/).
 
 ## Setup
+Clone the template room: https://rec.net/room/CircuitsAPI.
+
 Request a developer key from https://devportal.rec.net/. This will be passed as the `dev_token` argument in the client.
 
 Setup RecNetLogin: https://github.com/Jegarde/RecNet-Login/?tab=readme-ov-file#setup.
 
 ## Quickstart
-Here's the basics of setting up the client:
+Here's the basics of setting up the client: 
 ```py
 import circuitsapi
+import asyncio
 
-# Let's initialize the CircuitsAPI client!
-# dev_token is the developer key from https://devportal.rec.net/.
-# rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
-async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
-    # Connect to a supported room
-    room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
-
-    # Connect to a specific user to send data to
-    user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
-
-    # Send binary
-    await user.send_binary(101101)
-
-    # Send signals to the receiver ports
-    await user.send_bit_0()
-    await user.send_bit_1()
-    await user.send_end_signal()
+async def main():
+    # Let's initialize the CircuitsAPI client!
+    # dev_token is the developer key from https://devportal.rec.net/.
+    # rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
+    async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
+        # Connect to a supported room
+        room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
+    
+        # Connect to a specific user to send data to
+        user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
+    
+        # Send signals to the receiver ports
+        await user.send_bit_1()
+        await user.send_bit_0()
+        await user.send_end_signal()
+
+        # Send binary
+        await user.send_binary(101101)
+
+asyncio.run(main())
 ```
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6ed9b3b4-a14f-4ef2-8a8b-79d76fa0e29f" height="300">
+
 Here's the functions you can use if you hook up the in-game 'Receiver' to the 'Packet Handler':
 ```py
-# Assuming you have connected to an user
+# Assuming you are connected to an user
 
 # Sending text
 await user.send_text_packet("Hello, World!")
 
 # Sending integers
 await user.send_int_packet(69420)
 
@@ -91,25 +102,53 @@
 Here's some miscellaneous functions:
 ```py
 # Returns true if the player is in the specified room
 # Requires 'rn.match.read' scope in access token.
 await user.check_is_player_in_room()
 
 # Returns the player's room instance data
+# Requires 'rn.match.read' scope in access token.
 await user.get_instance()
 
 # Returns player IDs of those who have taken images in the past 10 minutes
 # If you want to connect to users, you can ask them to take pictures and have the server check for those pictures
 await room.find_players()
 ```
 
+## Example Usage
+This [example script](https://github.com/Jegarde/CircuitsAPI/blob/pre-alpha/examples/helloworld.py) is compatible with the [template room](https://rec.net/room/CircuitsAPI).
+
+## Experimental Features
+
+### Run-length encoding
+You can compress data with [run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
+
+Ex. "aaabbbceeeeee" -> "3a3b1c6e"
+
+This is only efficient if the data has lots of repetition.
+
+```py
+# Shortened code
+from circuitsapi import run_length_encoding
+await user.send_text_packet(run_length_encoding("aaabbbccc"))  # encodes to 3a3b3c
+```
+
+In-game decoder:
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6005cf1e-7ae0-475a-9e9c-d5a2fcfecbf5" height="200">
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/b025e943-971d-4f90-9cd1-f49d04786ec9" height="200">
+
+
+
+
 ## How does this work?
 There's CV2 chips for checking if a player is a host, mod or a contributor and you can modify a player's roles through the API. This allows us to send remote signals to the specified player while CV2 is constantly checking for each players' roles.
 
-RR Transmitter uses the following signals:
+CircuitsAPI uses the following signals:
 ```
 Host = Add on bit
 Mod = Add off bit
 Contributor = Repeat previous bit
 No role = End of binary number
 ```
```

### Comparing `circuitsapi-0.0.2/README.md` & `circuitsapi-0.0.3/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,67 +1,77 @@
 ![promo](https://github.com/Jegarde/CircuitsAPI/assets/13438202/554a02af-6862-44d9-aa80-da78fccdb409)
 
 ## THIS PROJECT IS IN PRE-ALPHA STAGE
 This system has not been properly tested. It is constantly being updated with breaking changes. Do not use this system in a production environment. Only use it for testing and experimenting.
 
+Detailed documentation and instructions coming later.
+
+Feel free to contact @Jegarde on Discord for inquiries.
+
 ## What is this?
 A system to communicate with CV2 using Python.
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/fad38801-641f-439f-ab36-249bc22d08e9" width="400">
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/70d09f93-8f40-4dff-8c26-f1577d91ba6f" width="350">
 
 ## Limitations
 - You must sacrifice the following permission roles: host, moderator & contributor. Co-owner will be the only role you can grant others without triggering the system. 
 - Room owner & co-owners will not be able to receive data by this system.
 - You can only send a single bit at once. This system is not applicable for big data transmissions.
 - CV2 pongs require messing with the instance's matchmaking state.
 - The circuits are currently made in Rooms v2 to prevent the system being used in existing production rooms due to instability.
   - It will be ported over to Rooms v1 once it's stable enough.
 
-## Rec Room Setup
-1. Clone the template room: https://rec.net/room/CircuitsAPI.
-2. **IMPORTANT:** Remove any privileged permissions from the following roles from the room: host, moderator & contributor. Otherwise you may risk troublemakers abusing the privileges.
-3. Add `circuitsapi` as a room tag to indicate it's supported by the system.
-4. Activate the 'Receiver' circuit board.
-
 ## Installation
-1. Download and unpack the [repository](https://github.com/Jegarde/CircuitsAPI/archive/refs/heads/pre-alpha.zip).
-2. Install the Python requirements. `pip install -U -r requirements.txt`
-3. Include the `circuitsapi` directory in your project. That is the library.
+The recommended method is installing via [pip](https://pypi.org/project/pip/).
+
+`pip install -U circuitsapi`
+
+For instructions on installing Python and pip, see [The Hitchhiker's Guide to Python](https://docs.python-guide.org/starting/installation/).
 
 ## Setup
+Clone the template room: https://rec.net/room/CircuitsAPI.
+
 Request a developer key from https://devportal.rec.net/. This will be passed as the `dev_token` argument in the client.
 
 Setup RecNetLogin: https://github.com/Jegarde/RecNet-Login/?tab=readme-ov-file#setup.
 
 ## Quickstart
-Here's the basics of setting up the client:
+Here's the basics of setting up the client: 
 ```py
 import circuitsapi
+import asyncio
 
-# Let's initialize the CircuitsAPI client!
-# dev_token is the developer key from https://devportal.rec.net/.
-# rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
-async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
-    # Connect to a supported room
-    room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
-
-    # Connect to a specific user to send data to
-    user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
-
-    # Send binary
-    await user.send_binary(101101)
-
-    # Send signals to the receiver ports
-    await user.send_bit_0()
-    await user.send_bit_1()
-    await user.send_end_signal()
+async def main():
+    # Let's initialize the CircuitsAPI client!
+    # dev_token is the developer key from https://devportal.rec.net/.
+    # rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
+    async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
+        # Connect to a supported room
+        room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
+    
+        # Connect to a specific user to send data to
+        user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
+    
+        # Send signals to the receiver ports
+        await user.send_bit_1()
+        await user.send_bit_0()
+        await user.send_end_signal()
+
+        # Send binary
+        await user.send_binary(101101)
+
+asyncio.run(main())
 ```
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6ed9b3b4-a14f-4ef2-8a8b-79d76fa0e29f" height="300">
+
 Here's the functions you can use if you hook up the in-game 'Receiver' to the 'Packet Handler':
 ```py
-# Assuming you have connected to an user
+# Assuming you are connected to an user
 
 # Sending text
 await user.send_text_packet("Hello, World!")
 
 # Sending integers
 await user.send_int_packet(69420)
 
@@ -72,25 +82,53 @@
 Here's some miscellaneous functions:
 ```py
 # Returns true if the player is in the specified room
 # Requires 'rn.match.read' scope in access token.
 await user.check_is_player_in_room()
 
 # Returns the player's room instance data
+# Requires 'rn.match.read' scope in access token.
 await user.get_instance()
 
 # Returns player IDs of those who have taken images in the past 10 minutes
 # If you want to connect to users, you can ask them to take pictures and have the server check for those pictures
 await room.find_players()
 ```
 
+## Example Usage
+This [example script](https://github.com/Jegarde/CircuitsAPI/blob/pre-alpha/examples/helloworld.py) is compatible with the [template room](https://rec.net/room/CircuitsAPI).
+
+## Experimental Features
+
+### Run-length encoding
+You can compress data with [run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
+
+Ex. "aaabbbceeeeee" -> "3a3b1c6e"
+
+This is only efficient if the data has lots of repetition.
+
+```py
+# Shortened code
+from circuitsapi import run_length_encoding
+await user.send_text_packet(run_length_encoding("aaabbbccc"))  # encodes to 3a3b3c
+```
+
+In-game decoder:
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6005cf1e-7ae0-475a-9e9c-d5a2fcfecbf5" height="200">
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/b025e943-971d-4f90-9cd1-f49d04786ec9" height="200">
+
+
+
+
 ## How does this work?
 There's CV2 chips for checking if a player is a host, mod or a contributor and you can modify a player's roles through the API. This allows us to send remote signals to the specified player while CV2 is constantly checking for each players' roles.
 
-RR Transmitter uses the following signals:
+CircuitsAPI uses the following signals:
 ```
 Host = Add on bit
 Mod = Add off bit
 Contributor = Repeat previous bit
 No role = End of binary number
 ```
```

### Comparing `circuitsapi-0.0.2/pyproject.toml` & `circuitsapi-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "circuitsapi"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
     { name="Jegarde"}
 ]
 description = "CircuitsAPI is a system to transmit data to Rec Room circuits."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `circuitsapi-0.0.2/src/circuitsapi/client.py` & `circuitsapi-0.0.3/src/circuitsapi/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,25 +32,23 @@
         self.access_token = None
         self.access_to_matchmaking = False
 
         # host account ID
         self.host_account_id = 0
 
         # Determine login method
-        self.used_recnetlogin = False
         if isinstance(rr_auth, str):
             self.headers["Authorization"] = "Bearer " + rr_auth
             self.access_token = rr_auth
         else:
             # Attempt to login with RecNetLogin
             rnl = RecNetLogin()
             token = rnl.get_token()
             self.headers["Authorization"] = "Bearer " + token
             self.access_token = token
-            self.used_recnetlogin = True
 
         # clients
         self.session: aiohttp.ClientSession | None = None
         self.RecNet: recnetpy.Client | None = None
         self.auth_task: asyncio.Task = None
 
         # debug mode for printing
@@ -60,31 +58,40 @@
         self.initialized = False
 
     async def initialize(self):
         """Initialize the client for usage. Must be ran.
         """
         if self.initialized: return
         
+        # Initialize aiohttp and recnetpy
         self.session = aiohttp.ClientSession(headers=self.headers, cookies=self.cookies)
         self.RecNet = recnetpy.Client(api_key=self.dev_token)
-
-        # Wait for auth
-        while True: 
-            if self.access_token: break
             
+        # Read token properties
         decoded_token = self.__decode_token(self.access_token)
         self.host_account_id = int(decoded_token.get("sub", "0"))
         self.access_to_matchmaking = "rn.match.read" in decoded_token.get("scope", [])
 
+        # Matchmaking data lets you access room instances.
         if not self.access_to_matchmaking:
             print("WARNING: Your access token is lacking the 'rn.match.read' scope. This will limit functionality.")
 
         self.initialized = True
 
-    async def send_request(self, method: str, url: str, payload: str | dict = {}):
+    async def send_request(self, method: str, url: str, payload: str | dict = {}) -> aiohttp.ClientResponse:
+        """Sends an API request
+
+        Args:
+            method (str): Request method
+            url (str): Request URL
+            payload (str | dict, optional): Request payload. Defaults to {}.
+
+        Returns:
+            aiohttp.ClientResponse: aiohttp response
+        """
         request = Request(self.session, method, url, payload)
         response = await request.send_request()
         print(f"{method.upper()} {url} DATA: {payload} - {response.status}")
         return response
 
     async def connect_to_room(self, room: str | int):
         """Create a connection to a room. You will then be able to target a specific user to transmit data.
@@ -108,17 +115,14 @@
         Returns:
             dict: Decoded bearer token
         """
         
         decoded = jwt.decode(token, options={"verify_signature": False})
         return decoded
 
-    async def db_print(self, *args) -> None:
-        if self.debug: print("Transmitter -", args)
-
     # asynchronous context manager enter
     async def __aenter__(self):
         await self.initialize()
         return self
 
     # asynchronous context manager exit
     async def __aexit__(self, *args):
@@ -411,15 +415,15 @@
         await self.__transmit_bit(1)
 
 
     async def send_end_signal(self):
         """Executes 'END' port in 'Receiver' circuit board
         """
 
-        await self.__packet_completed(self)
+        await self.__packet_completed()
                 
 
     async def send_binary(self, binary: int):
         """Sends a binary number executing 'Bit 1' and 'Bit 0' ports in 'Receiver' circuit board.
         Once the binary number has been fully sent, 'END' port will be executed.
 
         Args:
```

### Comparing `circuitsapi-0.0.2/src/circuitsapi/exceptions.py` & `circuitsapi-0.0.3/src/circuitsapi/exceptions.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.2/src/circuitsapi/helpers.py` & `circuitsapi-0.0.3/src/circuitsapi/helpers.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.2/src/circuitsapi/request.py` & `circuitsapi-0.0.3/src/circuitsapi/request.py`

 * *Files identical despite different names*

### Comparing `circuitsapi-0.0.2/src/circuitsapi.egg-info/PKG-INFO` & `circuitsapi-0.0.3/src/circuitsapi.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,86 +1,97 @@
 Metadata-Version: 2.1
 Name: circuitsapi
-Version: 0.0.2
+Version: 0.0.3
 Summary: CircuitsAPI is a system to transmit data to Rec Room circuits.
 Author: Jegarde
 Project-URL: Homepage, https://github.com/Jegarde/CircuitsAPI
 Project-URL: Bug Tracker, https://github.com/Jegarde/CircuitsAPI/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+License-File: LICENSE
 Requires-Dist: PyJWT==2.7.0
 Requires-Dist: python-dotenv==1.0.0
 Requires-Dist: aiohttp==3.9.2
 Requires-Dist: recnetpy==0.2.71
 Requires-Dist: python-dateutil==2.8.2
 Requires-Dist: recnetlogin==0.1.1
 
 ![promo](https://github.com/Jegarde/CircuitsAPI/assets/13438202/554a02af-6862-44d9-aa80-da78fccdb409)
 
 ## THIS PROJECT IS IN PRE-ALPHA STAGE
 This system has not been properly tested. It is constantly being updated with breaking changes. Do not use this system in a production environment. Only use it for testing and experimenting.
 
+Detailed documentation and instructions coming later.
+
+Feel free to contact @Jegarde on Discord for inquiries.
+
 ## What is this?
 A system to communicate with CV2 using Python.
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/fad38801-641f-439f-ab36-249bc22d08e9" width="400">
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/70d09f93-8f40-4dff-8c26-f1577d91ba6f" width="350">
 
 ## Limitations
 - You must sacrifice the following permission roles: host, moderator & contributor. Co-owner will be the only role you can grant others without triggering the system. 
 - Room owner & co-owners will not be able to receive data by this system.
 - You can only send a single bit at once. This system is not applicable for big data transmissions.
 - CV2 pongs require messing with the instance's matchmaking state.
 - The circuits are currently made in Rooms v2 to prevent the system being used in existing production rooms due to instability.
   - It will be ported over to Rooms v1 once it's stable enough.
 
-## Rec Room Setup
-1. Clone the template room: https://rec.net/room/CircuitsAPI.
-2. **IMPORTANT:** Remove any privileged permissions from the following roles from the room: host, moderator & contributor. Otherwise you may risk troublemakers abusing the privileges.
-3. Add `circuitsapi` as a room tag to indicate it's supported by the system.
-4. Activate the 'Receiver' circuit board.
-
 ## Installation
-1. Download and unpack the [repository](https://github.com/Jegarde/CircuitsAPI/archive/refs/heads/pre-alpha.zip).
-2. Install the Python requirements. `pip install -U -r requirements.txt`
-3. Include the `circuitsapi` directory in your project. That is the library.
+The recommended method is installing via [pip](https://pypi.org/project/pip/).
+
+`pip install -U circuitsapi`
+
+For instructions on installing Python and pip, see [The Hitchhiker's Guide to Python](https://docs.python-guide.org/starting/installation/).
 
 ## Setup
+Clone the template room: https://rec.net/room/CircuitsAPI.
+
 Request a developer key from https://devportal.rec.net/. This will be passed as the `dev_token` argument in the client.
 
 Setup RecNetLogin: https://github.com/Jegarde/RecNet-Login/?tab=readme-ov-file#setup.
 
 ## Quickstart
-Here's the basics of setting up the client:
+Here's the basics of setting up the client: 
 ```py
 import circuitsapi
+import asyncio
 
-# Let's initialize the CircuitsAPI client!
-# dev_token is the developer key from https://devportal.rec.net/.
-# rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
-async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
-    # Connect to a supported room
-    room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
-
-    # Connect to a specific user to send data to
-    user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
-
-    # Send binary
-    await user.send_binary(101101)
-
-    # Send signals to the receiver ports
-    await user.send_bit_0()
-    await user.send_bit_1()
-    await user.send_end_signal()
+async def main():
+    # Let's initialize the CircuitsAPI client!
+    # dev_token is the developer key from https://devportal.rec.net/.
+    # rr_auth is the RecNet access token. If left empty, CircuitsAPI defaults to RecNetLogin: https://github.com/Jegarde/RecNet-Login/
+    async with circuitsapi.Client(dev_token="", rr_auth=None) as client:
+        # Connect to a supported room
+        room = await client.connect_to_room(room="CircuitsAPI")  # You can also use the room ID
+    
+        # Connect to a specific user to send data to
+        user = await room.connect_to_user(user="Jegarde")  # You can also use the account ID
+    
+        # Send signals to the receiver ports
+        await user.send_bit_1()
+        await user.send_bit_0()
+        await user.send_end_signal()
+
+        # Send binary
+        await user.send_binary(101101)
+
+asyncio.run(main())
 ```
 
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6ed9b3b4-a14f-4ef2-8a8b-79d76fa0e29f" height="300">
+
 Here's the functions you can use if you hook up the in-game 'Receiver' to the 'Packet Handler':
 ```py
-# Assuming you have connected to an user
+# Assuming you are connected to an user
 
 # Sending text
 await user.send_text_packet("Hello, World!")
 
 # Sending integers
 await user.send_int_packet(69420)
 
@@ -91,25 +102,53 @@
 Here's some miscellaneous functions:
 ```py
 # Returns true if the player is in the specified room
 # Requires 'rn.match.read' scope in access token.
 await user.check_is_player_in_room()
 
 # Returns the player's room instance data
+# Requires 'rn.match.read' scope in access token.
 await user.get_instance()
 
 # Returns player IDs of those who have taken images in the past 10 minutes
 # If you want to connect to users, you can ask them to take pictures and have the server check for those pictures
 await room.find_players()
 ```
 
+## Example Usage
+This [example script](https://github.com/Jegarde/CircuitsAPI/blob/pre-alpha/examples/helloworld.py) is compatible with the [template room](https://rec.net/room/CircuitsAPI).
+
+## Experimental Features
+
+### Run-length encoding
+You can compress data with [run-length encoding](https://en.wikipedia.org/wiki/Run-length_encoding).
+
+Ex. "aaabbbceeeeee" -> "3a3b1c6e"
+
+This is only efficient if the data has lots of repetition.
+
+```py
+# Shortened code
+from circuitsapi import run_length_encoding
+await user.send_text_packet(run_length_encoding("aaabbbccc"))  # encodes to 3a3b3c
+```
+
+In-game decoder:
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/6005cf1e-7ae0-475a-9e9c-d5a2fcfecbf5" height="200">
+
+<img src="https://github.com/Jegarde/CircuitsAPI/assets/13438202/b025e943-971d-4f90-9cd1-f49d04786ec9" height="200">
+
+
+
+
 ## How does this work?
 There's CV2 chips for checking if a player is a host, mod or a contributor and you can modify a player's roles through the API. This allows us to send remote signals to the specified player while CV2 is constantly checking for each players' roles.
 
-RR Transmitter uses the following signals:
+CircuitsAPI uses the following signals:
 ```
 Host = Add on bit
 Mod = Add off bit
 Contributor = Repeat previous bit
 No role = End of binary number
 ```
```

