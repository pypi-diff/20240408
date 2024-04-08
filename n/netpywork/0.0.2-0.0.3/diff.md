# Comparing `tmp/netpywork-0.0.2.tar.gz` & `tmp/netpywork-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netpywork-0.0.2.tar", last modified: Mon Apr  8 12:15:28 2024, max compression
+gzip compressed data, was "netpywork-0.0.3.tar", last modified: Mon Apr  8 14:04:04 2024, max compression
```

## Comparing `netpywork-0.0.2.tar` & `netpywork-0.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-08 12:15:28.062473 netpywork-0.0.2/
--rw-rw-rw-   0        0        0     2995 2024-04-08 12:15:28.061472 netpywork-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2080 2024-04-08 12:09:20.000000 netpywork-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-04-08 12:15:28.044300 netpywork-0.0.2/netpywork/
--rw-rw-rw-   0        0        0      223 2024-04-08 12:13:31.000000 netpywork-0.0.2/netpywork/__init__.py
--rw-rw-rw-   0        0        0     3982 2024-04-08 12:13:15.000000 netpywork-0.0.2/netpywork/client.py
--rw-rw-rw-   0        0        0       84 2024-04-08 12:15:06.000000 netpywork-0.0.2/netpywork/constants.py
--rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.2/netpywork/protocol.py
--rw-rw-rw-   0        0        0     1204 2024-04-08 12:12:57.000000 netpywork-0.0.2/netpywork/sequence_manager.py
--rw-rw-rw-   0        0        0     5559 2024-04-08 12:13:14.000000 netpywork-0.0.2/netpywork/server.py
--rw-rw-rw-   0        0        0     3787 2024-04-08 12:12:58.000000 netpywork-0.0.2/netpywork/utils.py
-drwxrwxrwx   0        0        0        0 2024-04-08 12:15:28.057507 netpywork-0.0.2/netpywork.egg-info/
--rw-rw-rw-   0        0        0     2995 2024-04-08 12:15:27.000000 netpywork-0.0.2/netpywork.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      306 2024-04-08 12:15:27.000000 netpywork-0.0.2/netpywork.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-08 12:15:27.000000 netpywork-0.0.2/netpywork.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-08 12:15:27.000000 netpywork-0.0.2/netpywork.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-08 12:15:28.063468 netpywork-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      674 2024-04-08 12:13:00.000000 netpywork-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.947058 netpywork-0.0.3/
+-rw-rw-rw-   0        0        0     3070 2024-04-08 14:04:03.946060 netpywork-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     2110 2024-04-08 13:25:46.000000 netpywork-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.931098 netpywork-0.0.3/netpywork/
+-rw-rw-rw-   0        0        0      304 2024-04-08 13:22:33.000000 netpywork-0.0.3/netpywork/__init__.py
+-rw-rw-rw-   0        0        0     4081 2024-04-08 13:15:31.000000 netpywork-0.0.3/netpywork/client.py
+-rw-rw-rw-   0        0        0       84 2024-04-08 14:03:16.000000 netpywork-0.0.3/netpywork/constants.py
+-rw-rw-rw-   0        0        0       93 2024-04-08 12:13:40.000000 netpywork-0.0.3/netpywork/protocol.py
+-rw-rw-rw-   0        0        0     2284 2024-04-08 14:01:27.000000 netpywork-0.0.3/netpywork/sequence_manager.py
+-rw-rw-rw-   0        0        0     5656 2024-04-08 13:15:27.000000 netpywork-0.0.3/netpywork/server.py
+-rw-rw-rw-   0        0        0     3789 2024-04-08 13:51:29.000000 netpywork-0.0.3/netpywork/utils.py
+drwxrwxrwx   0        0        0        0 2024-04-08 14:04:03.943068 netpywork-0.0.3/netpywork.egg-info/
+-rw-rw-rw-   0        0        0     3070 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      306 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-08 14:04:03.000000 netpywork-0.0.3/netpywork.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-08 14:04:03.948105 netpywork-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      719 2024-04-08 13:45:44.000000 netpywork-0.0.3/setup.py
```

### Comparing `netpywork-0.0.2/PKG-INFO` & `netpywork-0.0.3/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library that simplifies UDP and TCP server and client
-Home-page: UNKNOWN
+Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
 Description: # netpywork
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
@@ -15,14 +15,15 @@
         - Callbacks for `On Receive` and `On Connect` for client
         - Sending messages from server to client both with tcp and udp by specifing the address to send to `(see example below)`
         - Sending *large* `UDP` messages
         
         # Example
         ```Python
         import netpywork as networking
+        
         def server_receive(msg,proto):
             if(proto == networking.protocol.UDP):
                 msg: networking.udp_msg = msg
                 print("Server UDP:",msg.length,msg.data,msg.address)
             if(proto == networking.protocol.TCP):
                 msg: networking.tcp_msg = msg
                 print("Server TCP:",msg.length,msg.data,msg.address)
@@ -52,18 +53,19 @@
             server.run()
             client.connect()
             
             client.send_reliable("Hello :)".encode())
             client.send_unreliable(("Hello!!!").encode())
             server.send_reliable("Hi1".encode(),client.address)
             server.send_unreliable("Hi2".encode(),client.address)
+        
             client.close()
             server.close()
             
-            input()
+            input("Press any key to exit...")
         if __name__ == "__main__":
             main()
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `netpywork-0.0.2/README.md` & `netpywork-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 - Callbacks for `On Receive` and `On Connect` for client
 - Sending messages from server to client both with tcp and udp by specifing the address to send to `(see example below)`
 - Sending *large* `UDP` messages
 
 # Example
 ```Python
 import netpywork as networking
+
 def server_receive(msg,proto):
     if(proto == networking.protocol.UDP):
         msg: networking.udp_msg = msg
         print("Server UDP:",msg.length,msg.data,msg.address)
     if(proto == networking.protocol.TCP):
         msg: networking.tcp_msg = msg
         print("Server TCP:",msg.length,msg.data,msg.address)
@@ -44,14 +45,15 @@
     server.run()
     client.connect()
     
     client.send_reliable("Hello :)".encode())
     client.send_unreliable(("Hello!!!").encode())
     server.send_reliable("Hi1".encode(),client.address)
     server.send_unreliable("Hi2".encode(),client.address)
+
     client.close()
     server.close()
     
-    input()
+    input("Press any key to exit...")
 if __name__ == "__main__":
     main()
 ```
```

### Comparing `netpywork-0.0.2/netpywork/client.py` & `netpywork-0.0.3/netpywork/client.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,44 +42,46 @@
         server_address = self.__tcp_socket.getpeername()
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         self.__seq_manager.delete_addr(server_address)
 
         self.__udp_thread.join()
         self.__udp_socket.close()
+
+        self.__seq_manager.stop()
     def send_reliable(self,msg: bytes):
         utils.send_tcp(self.__tcp_socket,msg)
     def send_unreliable(self,msg: bytes):
         msg_len = len(msg)
         if(msg_len <= utils.MAX_UDP_PACKET_SIZE):
-            utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),msg,self.__udp_seq,0,True)
+            utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),msg,self.__udp_seq,0,1)
         else:
             parts = []
             while (len(msg) > utils.MAX_UDP_PACKET_SIZE):
                 parts.append(msg[0:utils.MAX_UDP_PACKET_SIZE])
                 msg = msg[utils.MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
-                utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),parts[i],self.__udp_seq,i, i == len(parts) - 1)
+                utils.send_udp(self.__udp_socket,self.address[1],(self.ip,self.port),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __run_udp(self):
         while self.__is_running:
             try:
                 message: udp_msg = utils.read_udp_msg(self.__udp_socket)
                 self.__seq_manager.add_seq(message.address,message.seq_no,message.data,message.seq_id)
-                if(message.is_end):
+                if(message.amount == self.__seq_manager.get_amount(message.address,message.seq_no)):
                     # TODO : move to logging
                     # print("UDP",)
                     data = self.__seq_manager.get_result(message.address,message.seq_no)
                     result_msg = udp_msg()
                     result_msg.data = data
                     result_msg.address = message.address
                     result_msg.length = len(data)
                     result_msg.port = message.port
-                    result_msg.is_end = True
+                    result_msg.amount = message.amount
                     result_msg.seq_no = message.seq_no
                     if(self.on_receive):
                         self.on_receive(result_msg,protocol.UDP)
             except:
                 continue
     def __run_tcp(self):
         while self.__is_running:
```

### Comparing `netpywork-0.0.2/netpywork/server.py` & `netpywork-0.0.3/netpywork/server.py`

 * *Files 4% similar despite different names*

```diff
@@ -40,30 +40,31 @@
         self.__is_running = False
         self.__tcp_socket.close()
         self.__tcp_thread.join()
         for client in self.__clients:
             self.__seq_manager.delete_addr(client.getpeername())
         self.__udp_thread.join()
         self.__udp_socket.close()
+        self.__seq_manager.stop()
     def send_reliable(self,msg: bytes,address:tuple):
         utils.send_tcp(self.__addr_to_sock[address],msg)
     def __get_actual_address(self,address):
         return self.__addr_to_sock[address].getpeername()
     def send_unreliable(self,msg: bytes,address:tuple):
         msg_len = len(msg)
         if(msg_len <= utils.MAX_UDP_PACKET_SIZE):
-            utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),msg,self.__udp_seq,0,True)
+            utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),msg,self.__udp_seq,0,1)
         else:
             parts = []
             while (len(msg) > utils.MAX_UDP_PACKET_SIZE):
                 parts.append(msg[0:utils.MAX_UDP_PACKET_SIZE])
                 msg = msg[utils.MAX_UDP_PACKET_SIZE:]
             parts.append(msg)
             for i in range(len(parts)):
-                utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),parts[i],self.__udp_seq,i, i == len(parts) - 1)
+                utils.send_udp(self.__udp_socket,self.__tcp_socket.getsockname()[1],self.__get_actual_address(address),parts[i],self.__udp_seq,i,len(parts))
         self.__udp_seq += 1
     def __has_client(self,address):
         for client in self.__clients:
             client_address = client.getpeername()
             if(address == client_address):
                 return True
         return False
@@ -78,24 +79,24 @@
     def __run_udp(self):
         while self.__is_running:
             try:
                 message: udp_msg = utils.read_udp_msg(self.__udp_socket)
                 if(not self.__has_client(message.address)):
                     continue
                 self.__seq_manager.add_seq(message.address,message.seq_no,message.data,message.seq_id)
-                if(message.is_end):
+                if(message.amount == self.__seq_manager.get_amount(message.address,message.seq_no)):
                     # TODO : move to logging
                     # print("UDP",)
                     data = self.__seq_manager.get_result(message.address,message.seq_no)
                     result_msg = udp_msg()
                     result_msg.data = data
                     result_msg.address = message.address
                     result_msg.length = len(data)
                     result_msg.port = message.port
-                    result_msg.is_end = True
+                    result_msg.amount = message.amount
                     result_msg.seq_no = message.seq_no
                     if(self.on_receive):
                         self.on_receive(result_msg,protocol.UDP)
             except:
                 continue
     def __run_tcp(self):
         while self.__is_running:
```

### Comparing `netpywork-0.0.2/netpywork/utils.py` & `netpywork-0.0.3/netpywork/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,24 +7,24 @@
 
     Port 2 bytes
 
     Seq_no 4 bytes
 
     Seq_id 2 bytes
 
-    End 1 byte
+    Amount of ids 2 bytes
 
     Msg ? bytes
     """
     port:int = -1
     length: int = -1
     address: tuple = ()
     seq_no: int = -1
     seq_id: int = -1
-    is_end: bool = False
+    amount: int = -1
     data: bytes = None
 
 class tcp_msg:
     """
     TCP Message header:
 
     Length 4 bytes
@@ -36,15 +36,15 @@
     length:int = -1
     port:int = -1
     address: tuple = ()
     data:bytes = None
     closing:bool = False
 
 class utils:
-    MAX_UDP_PACKET_SIZE = 65507 - 4 - 2 - 1 - 2 - 4
+    MAX_UDP_PACKET_SIZE = 65507 - 4 - 2 - 4 - 2 - 2
     def peek_udp(sock: socket.socket,size: int):
             buffer = bytearray(size)
             # Windows workaround as it errors out with errorcode 10040 even though it peeked the msg
             try:
                 sock.recv_into(buffer,size,socket.MSG_PEEK)
             except OSError as ex:
                 if(ex.errno != 10040):
@@ -64,20 +64,20 @@
         result,result_address = socket.recvfrom(length)
         result = bytearray(result)
         utils.read_message(result,4)
         port = int.from_bytes(utils.read_message(result,2),"big")
         full_address = (result_address[0],port)
         seqno = int.from_bytes(utils.read_message(result,4),"big")
         seqid = int.from_bytes(utils.read_message(result,2),"big")
-        is_end = int.from_bytes(utils.read_message(result,1),"big") == 1
+        amount = int.from_bytes(utils.read_message(result,2),"big")
         result = utils.read_message(result)
         udp_message = udp_msg()
         udp_message.address = full_address
         udp_message.data = result
-        udp_message.is_end = is_end
+        udp_message.amount = amount
         udp_message.length = length
         udp_message.port = port
         udp_message.seq_no = seqno
         udp_message.seq_id = seqid
         return udp_message
     def read_tcp_msg(socket: socket.socket):
         length = socket.recv(4)
@@ -97,15 +97,15 @@
         tcp_message.port = address[1]
         return tcp_message
     def send_tcp(sock: socket.socket,msg: bytes,keep_con:bool = True):
         # Length msg + 1 byte for keep con
         length = (len(msg)+1).to_bytes(4,"big")
         closing = (1 if not keep_con else 0).to_bytes(1,"big")
         sock.send(length + closing + msg)
-    def send_udp(sock: socket.socket,port:int,address: tuple,msg: bytes,seq_no: int,seq_id:int ,is_end:bool):
-        # Length msg + 2 byte for port + 4 bytes for seq + 4 bytes for seq id+ 1 byte for is end
-        length = (len(msg) + 2 + 4 + 1 + 4).to_bytes(4,"big")
+    def send_udp(sock: socket.socket,port:int,address: tuple,msg: bytes,seq_no: int,seq_id:int ,amount:int):
+        # Length msg + 2 byte for port + 4 bytes for seq + 2 bytes for seq id + 2 bytes for amount of seq
+        length = (len(msg) + 2 + 4 + 2 + 2).to_bytes(4,"big")
         port = port.to_bytes(2,"big")
-        end = (1 if is_end else 0).to_bytes(1,"big")
         seqno = seq_no.to_bytes(4,"big")
         seqid = seq_id.to_bytes(2,"big")
-        sock.sendto(length + port + seqno + seqid + end + msg,address)
+        amount = amount.to_bytes(2,"big")
+        sock.sendto(length + port + seqno + seqid + amount + msg,address)
```

### Comparing `netpywork-0.0.2/netpywork.egg-info/PKG-INFO` & `netpywork-0.0.3/netpywork.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: netpywork
-Version: 0.0.2
+Version: 0.0.3
 Summary: Python library that simplifies UDP and TCP server and client
-Home-page: UNKNOWN
+Home-page: https://github.com/MurkyYT/netpywork
 Author: Murky
 Author-email: shooterkingof@gmail.com
 License: UNKNOWN
 Description: # netpywork
         **netpywork** is a library that makes using tcp and udp server and client easier
         
         # Features
@@ -15,14 +15,15 @@
         - Callbacks for `On Receive` and `On Connect` for client
         - Sending messages from server to client both with tcp and udp by specifing the address to send to `(see example below)`
         - Sending *large* `UDP` messages
         
         # Example
         ```Python
         import netpywork as networking
+        
         def server_receive(msg,proto):
             if(proto == networking.protocol.UDP):
                 msg: networking.udp_msg = msg
                 print("Server UDP:",msg.length,msg.data,msg.address)
             if(proto == networking.protocol.TCP):
                 msg: networking.tcp_msg = msg
                 print("Server TCP:",msg.length,msg.data,msg.address)
@@ -52,18 +53,19 @@
             server.run()
             client.connect()
             
             client.send_reliable("Hello :)".encode())
             client.send_unreliable(("Hello!!!").encode())
             server.send_reliable("Hi1".encode(),client.address)
             server.send_unreliable("Hi2".encode(),client.address)
+        
             client.close()
             server.close()
             
-            input()
+            input("Press any key to exit...")
         if __name__ == "__main__":
             main()
         ```
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `netpywork-0.0.2/setup.py` & `netpywork-0.0.3/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 'Programming Language :: Python :: 3',
 'License :: OSI Approved :: MIT License',
 'Operating System :: OS Independent',
 ],
 long_description=long_description,
 long_description_content_type='text/markdown',
 python_requires='>=3.8',
+url="https://github.com/MurkyYT/netpywork",
 )
```

