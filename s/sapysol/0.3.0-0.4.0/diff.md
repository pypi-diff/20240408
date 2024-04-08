# Comparing `tmp/sapysol-0.3.0.tar.gz` & `tmp/sapysol-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapysol-0.3.0.tar", max compression
+gzip compressed data, was "sapysol-0.4.0.tar", max compression
```

## Comparing `sapysol-0.3.0.tar` & `sapysol-0.4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.3.0/LICENSE
--rw-r--r--   0        0        0     3727 2024-04-05 20:58:10.770800 sapysol-0.3.0/README.md
--rw-r--r--   0        0        0      529 2024-04-02 11:09:02.178062 sapysol-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2602 2024-04-08 07:29:59.627437 sapysol-0.3.0/sapysol/__init__.py
--rw-r--r--   0        0        0     8367 2024-04-08 11:42:21.533995 sapysol-0.3.0/sapysol/helpers.py
--rw-r--r--   0        0        0     7970 2024-04-08 07:21:58.647655 sapysol-0.3.0/sapysol/ix.py
--rw-r--r--   0        0        0     5921 2024-04-08 07:30:51.470374 sapysol-0.3.0/sapysol/jupag.py
--rw-r--r--   0        0        0     4775 2024-04-04 22:25:05.883961 sapysol-0.3.0/sapysol/snippets/batcher.py
--rw-r--r--   0        0        0     4668 2024-04-08 07:29:48.650854 sapysol-0.3.0/sapysol/snippets/token_selloff.py
--rw-r--r--   0        0        0     4454 2024-04-05 20:16:05.330344 sapysol-0.3.0/sapysol/snippets/wallets_balance.py
--rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.3.0/sapysol/sysvar/clock.py
--rw-r--r--   0        0        0     7102 2024-04-06 18:57:26.944570 sapysol-0.3.0/sapysol/token.py
--rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.3.0/sapysol/tokenMetadata2022.py
--rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.3.0/sapysol/tokenMetadataMetaplex.py
--rw-r--r--   0        0        0     7233 2024-04-05 20:08:23.397989 sapysol-0.3.0/sapysol/token_cache.py
--rw-r--r--   0        0        0    13796 2024-04-06 18:47:21.503484 sapysol-0.3.0/sapysol/tx.py
--rw-r--r--   0        0        0     4963 2024-04-08 07:29:31.640984 sapysol-0.3.0/sapysol/wallet.py
--rw-r--r--   0        0        0     4610 1970-01-01 00:00:00.000000 sapysol-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4644 2024-04-08 12:29:18.740757 sapysol-0.4.0/README.md
+-rw-r--r--   0        0        0      529 2024-04-08 11:49:07.574452 sapysol-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2690 2024-04-08 12:49:12.656562 sapysol-0.4.0/sapysol/__init__.py
+-rw-r--r--   0        0        0     9019 2024-04-08 12:48:28.490259 sapysol-0.4.0/sapysol/helpers.py
+-rw-r--r--   0        0        0     7970 2024-04-08 07:21:58.647655 sapysol-0.4.0/sapysol/ix.py
+-rw-r--r--   0        0        0     5921 2024-04-08 07:30:51.470374 sapysol-0.4.0/sapysol/jupag.py
+-rw-r--r--   0        0        0     4775 2024-04-04 22:25:05.883961 sapysol-0.4.0/sapysol/snippets/batcher.py
+-rw-r--r--   0        0        0     4668 2024-04-08 07:29:48.650854 sapysol-0.4.0/sapysol/snippets/token_selloff.py
+-rw-r--r--   0        0        0     4454 2024-04-05 20:16:05.330344 sapysol-0.4.0/sapysol/snippets/wallets_balance.py
+-rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.4.0/sapysol/sysvar/clock.py
+-rw-r--r--   0        0        0     7102 2024-04-06 18:57:26.944570 sapysol-0.4.0/sapysol/token.py
+-rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.4.0/sapysol/tokenMetadata2022.py
+-rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.4.0/sapysol/tokenMetadataMetaplex.py
+-rw-r--r--   0        0        0     7233 2024-04-05 20:08:23.397989 sapysol-0.4.0/sapysol/token_cache.py
+-rw-r--r--   0        0        0    13796 2024-04-06 18:47:21.503484 sapysol-0.4.0/sapysol/tx.py
+-rw-r--r--   0        0        0     4963 2024-04-08 07:29:31.640984 sapysol-0.4.0/sapysol/wallet.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 sapysol-0.4.0/PKG-INFO
```

### Comparing `sapysol-0.3.0/LICENSE` & `sapysol-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/README.md` & `sapysol-0.4.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -21,32 +21,51 @@
 `sapysol` uses `Client` instead of `AsyncClient` for few reasons:
 * First - without `async` you can put more logic to Python constructors and other non-async functions;
 * Second - what is the point of `async` if you really use `await` in 100% of cases?
 
 Please use `threading` if you need parallel execution.
 
 ```py
+# ========================================
 # Sending SOL to another wallet
 from solana.rpc.api import Client 
 from sapysol        import *
 
 connection: Client          = Client("https://api.mainnet-beta.solana.com")
 wallet:     SapysolWallet   = SapysolWallet(connection=connection, keypair="path/to/file.json")
 result:     SapysolTxStatus = wallet.SendSol(destinationAddress="11111111111111111111111111111111", amountSol=0.5)
 assert(result==SapysolTxStatus.SUCCESS)
 
+# ========================================
+# Jupiter swap
+from solana.rpc.api import Client
+from sapysol        import *
+from sapysol.jupag  import SapysolJupag
+
+connection: Client = Client("https://api.mainnet-beta.solana.com")
+quote = SapysolJupag.GetSwapQuote(connection    = connection,
+                                  tokenFrom     = "So11111111111111111111111111111111111111112",
+                                  tokenTo       = "DezXAZ8z7PnrnRJjz3wXBoRgixCa6xjnB7YaB1pPB263", # BONK
+                                  inAmount      = 1 * LAMPORTS_PER_SOL)
+txB64 = SapysolJupag.GetSwapTxBase64(walletAddress=wallet.KEYPAIR.pubkey(), coinQuote=quote)
+tx: SapysolTx = SapysolTx(connection=connection, payer=wallet.KEYPAIR)
+tx.FromBase64(txB64)
+result: SapysolTxStatus = tx.SendAndWait()
+assert(result==SapysolTxStatus.SUCCESS)
+
+# ========================================
 # TODO - other simple use cases
 ```
 
 TODO
 
 # Contributing
 
 All contributions are welcome! Although the devil is in the details:
-* One of the main requirements is to [b]keep the same coding style[/b] for all future changes.
+* One of the main requirements is to **keep the same coding style** for all future changes.
 * `sapysol` is designed as a wrapper, one layer above `solders`/`solana-py`, don't expect it to do very narrow or specific tasks. If you need custom behavior in your case just go one level down and implement that using `solders`/`solana-py` in your local scripts.
 
 # Tests
 
 TODO
 
 # Contact
```

### Comparing `sapysol-0.3.0/pyproject.toml` & `sapysol-0.4.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sapysol"
-version = "0.3.0"
+version = "0.4.0"
 description = "SuperArmor's Solana Python wrapper."
 authors = ["Anton Platonov <anton@platonov.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `sapysol-0.3.0/sapysol/__init__.py` & `sapysol-0.4.0/sapysol/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,35 +14,38 @@
 # SuperArmor's Python Solana library.
 # (c) SuperArmor
 #
 # module: main
 #
 # =============================================================================
 # 
-from sapysol.helpers import EnsurePathExists,             \
-                            SetupLogging,                 \
-                            NestedAttributeExists,        \
-                            GetModulePath,                \
-                            ListToChunks,                 \
-                            SapysolPubkey,                \
-                            MakePubkey,                   \
-                            SapysolKeypair,               \
-                            MakeKeypair,                  \
-                            FetchAccount,                 \
-                            FetchAccounts,                \
+from sapysol.helpers import EnsurePathExists,       \
+                            SetupLogging,           \
+                            NestedAttributeExists,  \
+                            GetModulePath,          \
+                            ListToChunks,           \
+                            SapysolPubkey,          \
+                            MakePubkey,             \
+                            SapysolKeypair,         \
+                            MakeKeypair,            \
+                            GetFilesFromPath,       \
+                            GetKeypairsFromPath,    \
+                            GetPubkeysFromKeypairs, \
+                            FetchAccount,           \
+                            FetchAccounts,          \
                             DivmodJsBignumber
 
-from sapysol.ix import AtaInstruction,               \
-                       GetAta,                       \
-                       GetOrCreateAtaIx,             \
-                       GetTransferTokenIxInternal,   \
-                       GetTransferTokenIx,           \
-                       WrapSolInstructions,          \
-                       UnwrapSolInstruction,         \
-                       ComputeBudgetIx,              \
+from sapysol.ix import AtaInstruction,              \
+                       GetAta,                      \
+                       GetOrCreateAtaIx,            \
+                       GetTransferTokenIxInternal,  \
+                       GetTransferTokenIx,          \
+                       WrapSolInstructions,         \
+                       UnwrapSolInstruction,        \
+                       ComputeBudgetIx,             \
                        ComputePriceIx 
 
 from sapysol.token import SapysolToken
 
 from sapysol.tokenMetadataMetaplex import *
 from sapysol.tokenMetadata2022     import *
```

### Comparing `sapysol-0.3.0/sapysol/helpers.py` & `sapysol-0.4.0/sapysol/helpers.py`

 * *Files 6% similar despite different names*

```diff
@@ -139,14 +139,28 @@
             return Keypair.from_json(keypair)
         except:
             pass
     return None
 
 # ================================================================================
 #
+def GetFilesFromPath(path: str, endsWith: str=".json") -> List[str]:
+    files = os.listdir(path)
+    return [os.path.join(dir, f) for f in files if os.path.isfile(os.path.join(dir, f)) and f.lower().endswith(endsWith)]
+
+def GetKeypairsFromPath(path: str, endsWith: str=".json") -> List[Keypair]:
+    files    = GetFilesFromPath(path=path, endsWith=endsWith)
+    keypairs = [MakeKeypair(f) for f in files]
+    return keypairs
+
+def GetPubkeysFromKeypairs(keypairList: List[SapysolKeypair]) -> List[Pubkey]:
+    return [ MakeKeypair(x).pubkey() for x in keypairList ]
+
+# ================================================================================
+#
 def FetchAccounts(connection:    Client, 
                   pubkeys:       List[SapysolPubkey],
                   chunkSize:     int           = 100,
                   requiredOwner: SapysolPubkey = None,
                   commitment:    Commitment    = None,
                   parseToJson:   bool          = False) -> Union[List[Account], List[AccountJSON]]:
     results = []
```

### Comparing `sapysol-0.3.0/sapysol/ix.py` & `sapysol-0.4.0/sapysol/ix.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/jupag.py` & `sapysol-0.4.0/sapysol/jupag.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/snippets/batcher.py` & `sapysol-0.4.0/sapysol/snippets/batcher.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/snippets/token_selloff.py` & `sapysol-0.4.0/sapysol/snippets/token_selloff.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/snippets/wallets_balance.py` & `sapysol-0.4.0/sapysol/snippets/wallets_balance.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/sysvar/clock.py` & `sapysol-0.4.0/sapysol/sysvar/clock.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/token.py` & `sapysol-0.4.0/sapysol/token.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/tokenMetadata2022.py` & `sapysol-0.4.0/sapysol/tokenMetadata2022.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/tokenMetadataMetaplex.py` & `sapysol-0.4.0/sapysol/tokenMetadataMetaplex.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/token_cache.py` & `sapysol-0.4.0/sapysol/token_cache.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/tx.py` & `sapysol-0.4.0/sapysol/tx.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/sapysol/wallet.py` & `sapysol-0.4.0/sapysol/wallet.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.3.0/PKG-INFO` & `sapysol-0.4.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapysol
-Version: 0.3.0
+Version: 0.4.0
 Summary: SuperArmor's Solana Python wrapper.
 License: MIT
 Author: Anton Platonov
 Author-email: anton@platonov.io
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -46,32 +46,51 @@
 `sapysol` uses `Client` instead of `AsyncClient` for few reasons:
 * First - without `async` you can put more logic to Python constructors and other non-async functions;
 * Second - what is the point of `async` if you really use `await` in 100% of cases?
 
 Please use `threading` if you need parallel execution.
 
 ```py
+# ========================================
 # Sending SOL to another wallet
 from solana.rpc.api import Client 
 from sapysol        import *
 
 connection: Client          = Client("https://api.mainnet-beta.solana.com")
 wallet:     SapysolWallet   = SapysolWallet(connection=connection, keypair="path/to/file.json")
 result:     SapysolTxStatus = wallet.SendSol(destinationAddress="11111111111111111111111111111111", amountSol=0.5)
 assert(result==SapysolTxStatus.SUCCESS)
 
+# ========================================
+# Jupiter swap
+from solana.rpc.api import Client
+from sapysol        import *
+from sapysol.jupag  import SapysolJupag
+
+connection: Client = Client("https://api.mainnet-beta.solana.com")
+quote = SapysolJupag.GetSwapQuote(connection    = connection,
+                                  tokenFrom     = "So11111111111111111111111111111111111111112",
+                                  tokenTo       = "DezXAZ8z7PnrnRJjz3wXBoRgixCa6xjnB7YaB1pPB263", # BONK
+                                  inAmount      = 1 * LAMPORTS_PER_SOL)
+txB64 = SapysolJupag.GetSwapTxBase64(walletAddress=wallet.KEYPAIR.pubkey(), coinQuote=quote)
+tx: SapysolTx = SapysolTx(connection=connection, payer=wallet.KEYPAIR)
+tx.FromBase64(txB64)
+result: SapysolTxStatus = tx.SendAndWait()
+assert(result==SapysolTxStatus.SUCCESS)
+
+# ========================================
 # TODO - other simple use cases
 ```
 
 TODO
 
 # Contributing
 
 All contributions are welcome! Although the devil is in the details:
-* One of the main requirements is to [b]keep the same coding style[/b] for all future changes.
+* One of the main requirements is to **keep the same coding style** for all future changes.
 * `sapysol` is designed as a wrapper, one layer above `solders`/`solana-py`, don't expect it to do very narrow or specific tasks. If you need custom behavior in your case just go one level down and implement that using `solders`/`solana-py` in your local scripts.
 
 # Tests
 
 TODO
 
 # Contact
```

