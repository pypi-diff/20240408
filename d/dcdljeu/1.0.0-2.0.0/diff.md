# Comparing `tmp/dcdljeu-1.0.0.tar.gz` & `tmp/dcdljeu-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dcdljeu-1.0.0.tar", max compression
+gzip compressed data, was "dcdljeu-2.0.0.tar", max compression
```

## Comparing `dcdljeu-1.0.0.tar` & `dcdljeu-2.0.0.tar`

### file list

```diff
@@ -1,5 +1,7 @@
--rw-r--r--   0        0        0      431 2024-04-04 16:57:22.309610 dcdljeu-1.0.0/README.md
--rwxr-xr-x   0        0        0    12103 2024-04-04 16:53:31.910519 dcdljeu-1.0.0/dcdljeu/ceb.py
--rwxr-xr-x   0        0        0     8965 2024-04-04 16:25:18.719025 dcdljeu-1.0.0/dcdljeu/mlpl.py
--rw-r--r--   0        0        0      374 2024-04-04 17:01:40.222891 dcdljeu-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      872 1970-01-01 00:00:00.000000 dcdljeu-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1218 2024-04-08 12:51:27.997723 dcdljeu-2.0.0/README.md
+-rwxr-xr-x   0        0        0    10649 2024-04-07 11:34:35.392936 dcdljeu-2.0.0/dcdljeu/ceb.py
+-rwxr-xr-x   0        0        0     8826 2024-04-07 11:31:42.509878 dcdljeu-2.0.0/dcdljeu/mlpl.py
+-rwxr-xr-x   0        0        0   932965 2024-04-04 16:48:19.177232 dcdljeu-2.0.0/dcdljeu/tlm_dcdl.txt
+-rwxr-xr-x   0        0        0  1865940 2023-02-18 17:36:02.000000 dcdljeu-2.0.0/dcdljeu/tlm_dcdl_sort.txt
+-rw-r--r--   0        0        0      374 2024-04-08 12:52:37.526390 dcdljeu-2.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1659 1970-01-01 00:00:00.000000 dcdljeu-2.0.0/PKG-INFO
```

### Comparing `dcdljeu-1.0.0/dcdljeu/ceb.py` & `dcdljeu-2.0.0/dcdljeu/ceb.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,14 +21,15 @@
     elif op in "/:":
         try:
             return cn1/cn2
         except ZeroDivisionError:
             return 0
     else:
         raise ValueError("Invalid op :"+str(op))
+    
 def solve(nombres,nat,verbose=True,return_one_solution=False,allow_float=False,avoid_doubles=True,shortest_sol=True):
     try:
         tt=time.time()
         def info(txt):
             tt2=time.time()-tt
             #print(tt2)
             i=int(tt2)
@@ -95,14 +96,15 @@
                 return (solutions,nts)
             pistes=npistes
             a+=1
     except KeyboardInterrupt as err:
         raise err
         print("KeyboardInterrupt")
         return (solutions,nts)
+    
 def generer(n=6,solver=False,printer_solver=True,return_one_solution_solver=False,resoluble=False):
     n25=random.randrange(100)<71
     nondouble=random.randrange(100)<52
     nat=random.randrange(101,1000)
 
     tentative=0
     while True:
@@ -138,14 +140,15 @@
                 return (nombres,nat)
             else:
                 pass
 
         tentative+=1
         if tentative/10==int(tentative/10):
             pass
+        
 def demo(times="inf"):
 
     if times=="inf":times=99999
     n=0
     while True:
         try:
         #try:
@@ -173,47 +176,17 @@
             else:break
     tt=time.time()
     print("Solveur en cours...")
     d=solve(tirage,nat)
     print("\nFini en "+str(round(time.time()-tt,3))+" seconde(s), il y a "+str(len(d[0]))+" solutions pour trouver "+" et ".join(map(str,d[1]))+(" (Le Compte est bon)" if d[1]==[nat] else "")+".")
     time.sleep(1)
     n+=1
-        #if not while_true:break
-def _demo():
-        while True:
-            try:
-            #try:
-                tirage=input("\nLe tirage de nombres : ")
-                if not tirage:break
-                tirage=list(map(int,tirage.split(" ")))
-                #print("W")
-                #print(repr(tirage))
-            except Exception:pass
-            else:break
-        if not tirage:
-            
-            tirage,nat=generer(6)
-            print("Tirage de nombres: "+str(" ".join(map(str,tirage))),"Recherche du nombre: "+str(nat))
-            time.sleep(1)
-        else:
-            while True:
-                try:
-                    tirage.remove("")
-                except:break
-            while True:
-                try:
-                    nat=int(input("Recherche du nombre : "))
-                except Exception:pass
-                else:break
-        tt=time.time()
-        print("Solveur en cours...")
-        d=solve(tirage,nat)
-        print("\nFini en "+str(round(time.time()-tt,3))+" seconde(s), il y a "+str(len(d[0]))+" solutions pour trouver "+" et ".join(map(str,d[1]))+(" (Le Compte est bon)" if d[1]==[nat] else "")+".")
-        time.sleep(1)
-def ceb_to_bytes(ceb,file=None):
+
+
+def to_scratch(ceb,file=None):
     bceb=b""
     pair=[]
     nbr_pairs=0
     ceb=(list(ceb[0]),ceb[1],ceb[2])
     nombres=ceb[0].copy()
     for nombre in nombres:
         idn=NOMBRES_POSSIBLES.index(nombre)
@@ -247,25 +220,26 @@
         del nombres[cm2]
         nombres.append(calculate(int(cn1),bsigne,int(cn2)))
         #print(nombres)
         cc=(cm1,OPS.index(signe),cm2)
         code=cc[0]*20+cc[1]*5+cc[2]
         bceb+=BS[code]
     try:
-        nceb=bytes_to_ceb(bceb)
+        nceb=from_scratch(bceb)
     except Exception as err:
         print(err,file=sys.stderr)
     else:
         if ceb!=nceb:
             print("ERROR ceb:",ceb,"nceb:",nceb,file=sys.stderr)
                 
         return bceb
     return b
-def cebs_to_print(fichier_exercices,fichier_corrige,cebs_or_nbr_cebs=3,n=6,solver=True,resoluble=True):
-    cebs=cebs_or_nbr_cebs
+
+def to_file(fichier_exercices,fichier_corrige,nbr=3,n=6,solver=True,resoluble=True):
+    cebs=nbr
     if not isinstance(cebs,(list,tuple)):
         new_cebs=[]
         for id in range(cebs):
             print(str(id)+"/"+str(cebs))
             #print("n",n,"solver",solver)
             data=generer(n,solver,False,True,resoluble)
             new_cebs.append(data)
@@ -300,18 +274,17 @@
     f.write(espace_page.join(pages))
     f.close()
     f=open(fichier_corrige,"w")
     f.write(espace_page.join(pages_corr))
     f.close()
     #mypkg.open_file_with_browser(fichier_exercices)
     #mypkg.open_file_with_browser(fichier_corrige)
-    time.sleep(1)
-    os.remove(fichier_exercices)
-    os.remove(fichier_corrige)
-def bytes_to_ceb(ceb):
+
+    
+def from_scratch(ceb):
     b=ceb
     bs=list(map(lambda b:b[0],BS))
     nombres=[]
     idx=0
     for _ in range(3):
         idx_nn=bs.index(b[idx])
         n1=int(idx_nn/14)
@@ -344,31 +317,25 @@
     cebs=[]
     b=b""
     for idx in range(nbr_de_cebs):
         print(str(idx)+"/"+str(nbr_de_cebs))
         data=generer(6,True,False,True,resoluble=resoluble)
         #print(data[2][0])
         cebs.append((data[0],data[1],data[2][0][0]))
-        b+=ceb_to_bytes(cebs[-1])+BS[-1]
+        b+=to_scratch(cebs[-1])+BS[-1]
     if file:
         f=open(file,"wb")
         f.write(b)
         f.close()
         #mypkg.open_file_with_browser(file)
         if not input("Tapez Enter pour supprimer le fichier, tapez un texte pour le garder"):
 
             os.remove(file)
         #print("w")
     #print(cebs)
     #print(cebs)
     return (b,cebs)
-def atest():
-    tt=time.time()
-    try:
-        for result in solve([8, 10, 75, 5, 100, 3],646):pass
-    except Exception as err:raise err
-    finally:
-        print(time.time()-tt)
+
 
 #id=str(random.randrange(1000))
 #cebs_to_print("ceb_ex"+id+".txt","ceb_corr"+id+".txt",24)
 #solve(*generer())
```

### Comparing `dcdljeu-1.0.0/dcdljeu/mlpl.py` & `dcdljeu-2.0.0/dcdljeu/mlpl.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,50 +3,64 @@
 LETTRES="ABCDEFGHIJKLMNOPQRSTUVWXYZ"
 LETTRES_SCRABBLE=list("A"*9+"B"*2+"C"*2+"D"*3+"E"*15+"F"*2+"G"*2+"H"*2+"I"*8+"J"*1+"K"*1+"L"*5+"M"*3+
                       "N"*6+"O"*6+"P"*2+"Q"*1+"R"* 6+"S"*6+"T"*6+"U"*6+"V"*2+"W"*1+"X"*1+"Y"*1+"Z"*1)
 VOYELLES="AEIOUY"
 BS=[]
 ID_BS=[]
 FILE_BS="bs.txt"
+
+import time
+import random
+import os
+
 f=open(FILE_BS,"rb")
 for b in f.read():
     BS.append(bytes([b]))
     ID_BS.append(b)
 f.close()
-import time,random,os,ceb
+
+
 def get_tlm():
+    """Obtenir la liste des mots"""
     f=open(FILE_TLM)
     mots=f.read().splitlines()
     f.close()
     return mots
+
 def renew_tlm_sort():
     mots=get_tlm()
     f=open(FILE_TLM_SORT,"w")
-    f.write("".join(map(lambda mot:"\n"+"".join(sorted(mot))+":"+mot,mots)).upper())
+    f.write(
+        "".join(
+            map(lambda mot:"\n"+"".join(sorted(mot))+":"+mot,mots)).upper())
     f.close()
+    
 try:
     f=open(FILE_TLM_SORT)
 except:
     renew_tlm_sort()
+    
 def tlm_to_scratch():
     mots=get_tlm()
     scratch="".join(map(lambda mot:mot.upper()+";",mots))
     print("Texte généré")
     return scratch
+
 def solve(lettres,n=10,Printer=True):
     global mots_trouves,lmot
     tt=time.time()
-    def info(txt):
+    def info_with_timer(txt):
         ttt=str(int(round(time.time()-tt,3)*1000))
         ttt=ttt[:-3]+"."+ttt[-3:]
         ttt=("0"*(6-len(ttt)))+ttt      
         print("["+ttt+"] "+txt)
+        
     if not Printer:
-        info=lambda *args:None
-    info("Tirage: "+lettres)
+        info_with_timer=lambda *args:None
+    info_with_timer("Tirage: "+lettres)
     mots_trouves=[]
     for _ in range(len(lettres)+1):
         mots_trouves.append([])
     all_lettres=[sorted(lettres.upper())]
     
     #print(all_lettres)
     #new_lettres=[]
@@ -56,15 +70,15 @@
     Breaker=False
     max=0
     while True:
         new_lettres=[]
         l=len(all_lettres[0])
         if l+(n-1)<max or not l:
             return (mots_trouves,max)
-        info("Recherche pour "+str(l)+" lettres...")
+        info_with_timer("Recherche pour "+str(l)+" lettres...")
         for lettres in all_lettres:
             #if lettres==list("ADEINNOSU"):print("CC")
             #print(list(map(len,all_lettres)))
             idx=0
             while True:
                 try:
                     #print(len(lettres))
@@ -76,46 +90,38 @@
                     mot_trouve=txt[idx:txt.index("\n",idx)]
                     lmot=len(mot_trouve)
                     
                     if mot_trouve not in mots_trouves[lmot]:
                         #if lettres==list("ADEINNOSU"):print("NO")
                         if lmot>max:
                             max=lmot
-                        info(str(lmot)+" lettres: "+mot_trouve)
+                        info_with_timer(str(lmot)+" lettres: "+mot_trouve)
                         mots_trouves[lmot].append(mot_trouve)
             a_lettre=""
             for idx in range(len(lettres)):
                 lettre=lettres[idx]
                 if lettre==a_lettre:
                     continue
                 a_lettre=lettre
                 lettresc=lettres.copy()
                 del lettresc[idx]
                 new_lettres.append(lettresc)
             #print(new_lettres)
         #print(new_lettres)
         all_lettres=new_lettres
     print("WW")
+    
 def demo(n_solver=2,alternes_mlpl_dcdl=False):
-    while True:
-        lettres=input("Lettres ?")
-        if not lettres:
-            lettres=generer()
-            print("Lettres:"+lettres)
-            time.sleep(1)
-        try:
-            d=solve(lettres,n_solver)
-        except KeyboardInterrupt:
-            print("KeyboardInterrupt")
-        else:
-            print("Fini")
-        if alternes_mlpl_dcdl:
-            ceb2.demo(1)
-        #except NameError or UnboundLocalError:
-        #    pass
+    lettres=input("Lettres ?")
+    if not lettres:
+        lettres=generer()
+        print("Lettres:"+lettres)
+        time.sleep(1)
+    d=solve(lettres,n_solver)
+    
 def generer(nbr_de_voyelles=5,n=10,solver=False,n_solver=2,Printer_solver=True):
     if nbr_de_voyelles=="random":
         nbr_de_voyelles=random.randrange(3,7)
     #print("nn",n_solver)
     while True:
         tirage=""
         voyelles=0
@@ -128,31 +134,34 @@
                 if voyelles>nbr_de_voyelles:
                     break
             tirage+=lettre
         if voyelles==nbr_de_voyelles:
             if solver:
                 return (tirage,solve(tirage,n_solver,Printer_solver))
             return tirage
+        
 def generer_bytes(nbr_de_voyelles=5,nbr_de_mlpls=1000,file=None):
     mlpls=[]
     b=b""
     for idx in range(nbr_de_mlpls):
         print(str(idx)+"/"+str(nbr_de_mlpls))
         data=generer(nbr_de_voyelles,solver=True,n_solver=1,Printer_solver=False)
         mlpls.append((data))
-        b+=mlpl_to_bytes(mlpls[-1])+BS[-1]
+        b+=to_scratch(mlpls[-1])+BS[-1]
     if file:
         f=open(file,"wb")
         f.write(b)
         f.close()
         #mypkg.open_file_with_browser(file)
         if not input("Tapez Enter pour supprimer le fichier, tapez un texte pour le garder"):
             os.remove(file)
     return (b,mlpls)
-def mlpl_to_bytes(mlpl,file=None):
+
+def to_scratch(mlpl,file=None):
+    """To turn for scratch"""
     """mlpl_to_bytes(("ABCDEFGHIJ",([[],[],[],[],[],[],[],["FICHAGE"]],7)),"YOUR_FILE.txt")"""
     bs=b''
     lettres=sorted(mlpl[0].upper())
     solutions,max=mlpl[1]
     max-=1
     int1=int(max/5)
     int2=max-int1*5
@@ -204,15 +213,17 @@
         #tirages_mc.append(tirage_mc)
     if file:
         f=open(file,"wb")
         f.write(bs+BS[-1])
         f.close()
         #mypkg.open_file_with_browser(file)
     return bs
-def bytes_to_mlpl(bs):
+
+def from_scratch(bs):
+    """From scratch to python"""
     f=open(FILE_TLM_SORT)
     tfts=f.read()
     f.close()
     b1=ID_BS.index(bs[0])
     b2=ID_BS.index(bs[1])
     int1=int(b1/len(LETTRES))
     int2=int(b2/len(LETTRES))
@@ -275,18 +286,13 @@
         if idx>=len(bs):break
     print(bs)
     solutions=[]
     for _ in range(max):
         solutions.append([])
     solutions.append(mots)
     return ("".join(lettres),(solutions,max))
-def pmanche():
-    demo(2,True)
-def mots2lafin():
-    demo(1)
-print("")
         #print("YO")
 #tt=time.time()
 #LETTRES="abcdefghij"
 #d=solve(LETTRES,len(LETTRES)-5)
 #print("Fin en : "+str(time.time()-tt))
 #d=mlpl_to_bytes(("ABCDEFGHIJ",(([],[],[],[],[],[],[],["FICHAGE"]),7)),"f.txt")
```

