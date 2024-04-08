# Comparing `tmp/Jetski-0.0.2.tar.gz` & `tmp/Jetski-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Jetski-0.0.2.tar", last modified: Sat Apr  6 16:21:13 2024, max compression
+gzip compressed data, was "Jetski-0.0.3.tar", last modified: Mon Apr  8 19:17:24 2024, max compression
```

## Comparing `Jetski-0.0.2.tar` & `Jetski-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.678070 Jetski-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.640484 Jetski-0.0.2/Jetski/
--rw-rw-rw-   0        0        0     7848 2024-04-06 15:40:58.000000 Jetski-0.0.2/Jetski/Jetski.py
--rw-rw-rw-   0        0        0       48 2024-04-02 10:30:56.000000 Jetski-0.0.2/Jetski/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-06 16:21:13.675577 Jetski-0.0.2/Jetski.egg-info/
--rw-rw-rw-   0        0        0     1648 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      197 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-04-06 16:21:13.000000 Jetski-0.0.2/Jetski.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1092 2024-03-19 09:16:49.000000 Jetski-0.0.2/LICENSE.txt
--rw-rw-rw-   0        0        0     1648 2024-04-06 16:21:13.677564 Jetski-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      648 2024-04-06 16:02:48.000000 Jetski-0.0.2/README.rst
--rw-rw-rw-   0        0        0       86 2024-04-06 16:21:13.680543 Jetski-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     1341 2024-04-06 15:59:55.000000 Jetski-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:17:24.390015 Jetski-0.0.3/
+drwxrwxrwx   0        0        0        0 2024-04-08 19:17:24.365728 Jetski-0.0.3/Jetski/
+-rw-rw-rw-   0        0        0     8703 2024-04-08 18:59:12.000000 Jetski-0.0.3/Jetski/Jetski.py
+-rw-rw-rw-   0        0        0       48 2024-04-02 10:30:56.000000 Jetski-0.0.3/Jetski/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 19:17:24.388515 Jetski-0.0.3/Jetski.egg-info/
+-rw-rw-rw-   0        0        0     2226 2024-04-08 19:17:24.000000 Jetski-0.0.3/Jetski.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      197 2024-04-08 19:17:24.000000 Jetski-0.0.3/Jetski.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 19:17:24.000000 Jetski-0.0.3/Jetski.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-04-08 19:17:24.000000 Jetski-0.0.3/Jetski.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1092 2024-03-19 09:16:49.000000 Jetski-0.0.3/LICENSE.txt
+-rw-rw-rw-   0        0        0     2226 2024-04-08 19:17:24.389544 Jetski-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1200 2024-04-08 19:11:11.000000 Jetski-0.0.3/README.rst
+-rw-rw-rw-   0        0        0       86 2024-04-08 19:17:24.392515 Jetski-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1341 2024-04-08 19:09:40.000000 Jetski-0.0.3/setup.py
```

### Comparing `Jetski-0.0.2/Jetski/Jetski.py` & `Jetski-0.0.3/Jetski/Jetski.py`

 * *Files 4% similar despite different names*

```diff
@@ -68,16 +68,17 @@
             if (3 <= numOfJetskis <= 5):
                 bill = bill * 0.8
             return bill
         else:
             print("Are you sure you rented a jetski with us?")
             return None
     
-    # Save
-    def save_file(self, data=[], filename="JetskiInformation.json"):
+    # Save   
+    def save_file(self, n=0, data={"Stock": 0, "Customers": {}}, filename="JetskiInformation.json"):
+        data["Stock"] = n
         with open(filename, "w") as file:
             json.dump(data, file)
             
     # Load
     def load_file(self, filename="JetskiInformation.json"):
         try:
             with open(filename, "r") as file:
@@ -111,105 +112,117 @@
         return self.jetskis
 
     def returnJetski(self):
         if self.rentalBasis and self.rentalTime and self.jetskis:
             return self.rentalTime, self.rentalBasis, self.jetskis
         else:
             return 0,0,0
-        
+
 def main():
     shop = JetskiRental()
-    mydata = shop.load_file()
-    
-    while True:
-        print("Menu:")
-        print("1: Display informations")
-        print("2: To rent jetskis")
-        print("3: To return jetskis")
-        print("4: Exit and Save")
-        choice = input("Enter your choice (1-4): ")
+    n = int(input("Enter the number of your shop's jetskis: "))
+    if n>0:
+        shop.save_file(n)
+        mydata = shop.load_file()
         
-        if choice == '1':
-            customer = Customer()
-            myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)"])
-            if mydata['Customers']=={}:
-                myTable.add_row(["-","-","-","-","-","-"])
-            else:
-                for key,value in mydata['Customers'].items():
-                    list_time  = value[2]
+        while True:
+            print("========= Menu =========")
+            print("1: Display informations")
+            print("2: To rent jetskis")
+            print("3: To return jetskis")
+            print("4: Exit and Save")
+            choice = input("Enter your choice (1-4): ")
+            
+            if choice == '1':
+                customer = Customer()
+                myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)"])
+                if mydata['Customers']=={}:
+                    myTable.add_row(["-","-","-","-","-","-"])
+                else:
+                    for key,value in mydata['Customers'].items():
+                        list_time  = value[2]
+                        customer.rentalTime = datetime.datetime(*list_time)
+                        myTable.add_row([key, 
+                                        value[1], 
+                                        value[0],
+                                        customer.rentalTime,
+                                        "-",
+                                        "-",
+                                        ])
+                print(myTable)
+                print(f"Stocks: {mydata['Stock']}")
+                
+            elif choice == '2':
+                customer = Customer()
+                name = input("Enter your name: ")
+                jetskis = customer.requestJetski()
+                if mydata["Stock"]>=jetskis and jetskis>=1:
+                    mydata["Stock"] -= jetskis
+                    rentalBasis = int(input("Choose the rentalBasis: 1(1 hr), 2(4 hrs), 3(8 hrs): "))
+                    rentalTime = datetime.datetime.now()
+                    date_list = list(rentalTime.timetuple())
+                    del date_list[5:]
+                    mydata['Customers'][name] = [jetskis, rentalBasis, date_list]
+                    
+                    # Table
+                    myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"])
+                    list_time  = mydata["Customers"][name][2]
                     customer.rentalTime = datetime.datetime(*list_time)
-                    myTable.add_row([key, 
-                                    value[1], 
-                                    value[0],
+                    myTable.add_row([name, 
+                                    mydata["Customers"][name][1], 
+                                    mydata["Customers"][name][0],
                                     customer.rentalTime,
-                                    "-",
-                                    "-",
+                                    "-","-","-","-"
                                     ])
-            print(myTable)
-            print(f"Stocks:{mydata['Stock']}")
-            
-        elif choice == '2':
-            customer = Customer()
-            name = input("Enter your name: ")
-            jetskis = customer.requestJetski()
-            if mydata["Stock"]>=jetskis and jetskis>=1:
-                mydata["Stock"] -= jetskis
-                rentalBasis = int(input("Choose the rentalBasis: 1(1 hr), 2(4 hrs), 3(8 hrs): "))
-                rentalTime = datetime.datetime.now()
-                date_list = list(rentalTime.timetuple())
-                del date_list[5:]
-                mydata['Customers'][name] = [jetskis, rentalBasis, date_list]
-                shop.save_file(mydata)
-                myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"])
+                    print(myTable)
+                    
+                    shop.save_file(n=mydata["Stock"], data=mydata)
+                
+            elif choice == '3':
+                customer = Customer()
+                name = input("Enter your name: ")
+                customer.jetskis = mydata["Customers"][name][0]
+                customer.rentalBasis = mydata["Customers"][name][1]
                 list_time  = mydata["Customers"][name][2]
                 customer.rentalTime = datetime.datetime(*list_time)
+                request = customer.returnJetski()
+                bill = shop.returnJetski(request)
+                
+                if 3 <= mydata["Customers"][name][0] <= 5: 
+                    discount = bill/0.8 - bill
+                else:
+                    discount = 0
+                
+                End = datetime.datetime.now()
+                Endlist = list(End.timetuple())
+                del Endlist[5:]
+                EndrentalTime = datetime.datetime(*Endlist)
+
+                periodTime = datetime.datetime.now()-customer.rentalTime
+                periodhour = round(periodTime.seconds / 3600)
+                myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"]) 
                 myTable.add_row([name, 
                                 mydata["Customers"][name][1], 
                                 mydata["Customers"][name][0],
                                 customer.rentalTime,
-                                "-","-","-","-"
+                                EndrentalTime,
+                                periodhour,
+                                discount,
+                                bill
                                 ])
                 print(myTable)
-            
-        elif choice == '3':
-            customer = Customer()
-            name = input("Enter your name: ")
-            customer.jetskis = mydata["Customers"][name][0]
-            customer.rentalBasis = mydata["Customers"][name][1]
-            list_time  = mydata["Customers"][name][2]
-            customer.rentalTime = datetime.datetime(*list_time)
-            request = customer.returnJetski()
-            bill = shop.returnJetski(request)
-            
-            if 3 <= mydata["Customers"][name][0] <= 5: 
-                discount = bill/0.8 - bill
+                
+                mydata["Stock"] += mydata["Customers"][name][0]
+                del mydata["Customers"][name]
+                shop.save_file(n=mydata["Stock"], data=mydata)
+                
+            elif choice == '4':
+                print("Exiting the program.")
+                break
             else:
-                discount = 0
-            
-            End = datetime.datetime.now()
-            Endlist = list(End.timetuple())
-            del Endlist[5:]
-            EndrentalTime = datetime.datetime(*Endlist)
-
-            periodTime = datetime.datetime.now()-customer.rentalTime
-            periodhour = round(periodTime.seconds / 3600)
-            myTable = prettytable.PrettyTable(["Customer", "Type", "Amount", "Start", "End", "Period(hrs)", "Discount($)", "Price($)"]) 
-            myTable.add_row([name, 
-                             mydata["Customers"][name][1], 
-                             mydata["Customers"][name][0],
-                             customer.rentalTime,
-                             EndrentalTime,
-                             periodhour,
-                             discount,
-                             bill
-                             ])
-            print(myTable)
-            
-            mydata["Stock"] += mydata["Customers"][name][0]
-            del mydata["Customers"][name]
-            shop.save_file(mydata)
-        else:
-            break
+                print("Invalid choice! Please try again.")
+    else:
+        print("Invalid number!")
     
 #Test   
 if __name__ == '__main__':
     main()
```

### Comparing `Jetski-0.0.2/Jetski.egg-info/PKG-INFO` & `Jetski-0.0.3/Jetski.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Jetski
-Version: 0.0.2
+Version: 0.0.3
 Summary: Jetski Rental System by Tarid Suwansri
 Home-page: https://github.com/TaridSuwansri/Jetski
-Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip
+Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.3.zip
 Author: Tarid Suwansri
 Author-email: taridsuwansri@gmail.com
 License: MIT
 Keywords: Jetski,Mathematics,Tarid,Suwansri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
@@ -36,19 +36,45 @@
 .. code:: bash
 
    pip install Jetski
 
 Usage
 -----
 
+Start by importing both classes and datetime module.
+
 .. code:: python
 
-   from Jetski import JetskiRental
+   from Jetski import JetskiRental, Customer
+   import datetime
+
+Then, create JetskiRental and Customer objects and test example of rent.
+
+.. code:: python
+
+   shop = JetskiRental(10)
+   customer = Customer()
+
+   jetskis = customer.requestJetski()
+
+   customer.rentalBasis = 1
+
+   customer.rentalTime = datetime.datetime.now() + datetime.timedelta(hours=-2)
+
+   request = customer.returnJetski()
+
+   shop.displaystock()
+
+   shop.rentJetskiOnHourlyBasis(jetskis)
+
+   shop.displaystock()
+
+   bill = shop.returnJetski(request)
 
-   shop = JetskiRental()
+   print(f"Your bill is {bill}.")
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `Jetski-0.0.2/LICENSE.txt` & `Jetski-0.0.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `Jetski-0.0.2/PKG-INFO` & `Jetski-0.0.3/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: Jetski
-Version: 0.0.2
+Version: 0.0.3
 Summary: Jetski Rental System by Tarid Suwansri
 Home-page: https://github.com/TaridSuwansri/Jetski
-Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip
+Download-URL: https://github.com/TaridSuwansri/Jetski/archive/v0.0.3.zip
 Author: Tarid Suwansri
 Author-email: taridsuwansri@gmail.com
 License: MIT
 Keywords: Jetski,Mathematics,Tarid,Suwansri
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Topic :: Utilities
@@ -36,19 +36,45 @@
 .. code:: bash
 
    pip install Jetski
 
 Usage
 -----
 
+Start by importing both classes and datetime module.
+
 .. code:: python
 
-   from Jetski import JetskiRental
+   from Jetski import JetskiRental, Customer
+   import datetime
+
+Then, create JetskiRental and Customer objects and test example of rent.
+
+.. code:: python
+
+   shop = JetskiRental(10)
+   customer = Customer()
+
+   jetskis = customer.requestJetski()
+
+   customer.rentalBasis = 1
+
+   customer.rentalTime = datetime.datetime.now() + datetime.timedelta(hours=-2)
+
+   request = customer.returnJetski()
+
+   shop.displaystock()
+
+   shop.rentJetskiOnHourlyBasis(jetskis)
+
+   shop.displaystock()
+
+   bill = shop.returnJetski(request)
 
-   shop = JetskiRental()
+   print(f"Your bill is {bill}.")
 
 Contributing
 ------------
 
 Pull requests are welcome. For major changes, please open an issue first
 to discuss what you would like to change.
```

### Comparing `Jetski-0.0.2/setup.py` & `Jetski-0.0.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 DESCRIPTION = '\n\n'.join(LOAD_TEXT(_) for _ in [
     'README.rst'
 ])
 
 setup(
   name = 'Jetski',      
   packages = ['Jetski'], 
-  version = '0.0.2',
+  version = '0.0.3',
   license='MIT', 
   description = 'Jetski Rental System by Tarid Suwansri',
   long_description=DESCRIPTION,
   author = 'Tarid Suwansri',                 
   author_email = 'taridsuwansri@gmail.com',     
   url = 'https://github.com/TaridSuwansri/Jetski',  
-  download_url = 'https://github.com/TaridSuwansri/Jetski/archive/v0.0.2.zip',  
+  download_url = 'https://github.com/TaridSuwansri/Jetski/archive/v0.0.3.zip',  
   keywords = ['Jetski', 'Mathematics','Tarid','Suwansri'],
   classifiers=[
     'Development Status :: 3 - Alpha',     
     'Intended Audience :: Education',     
     'Topic :: Utilities',
     'License :: OSI Approved :: MIT License',   
     'Programming Language :: Python :: 3',
```

