# Comparing `tmp/adrmdr-0.1.6-py3-none-any.whl.zip` & `tmp/adrmdr-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 192025 bytes, number of entries: 9
+Zip file size: 192112 bytes, number of entries: 9
 -rw-rw-rw-  2.0 fat      834 b- defN 23-Oct-25 05:36 adrmdr/__init__.py
--rw-rw-rw-  2.0 fat   275355 b- defN 24-Apr-01 08:56 adrmdr/adrmdr.py
+-rw-rw-rw-  2.0 fat   275563 b- defN 24-Apr-08 00:43 adrmdr/adrmdr.py
 -rw-rw-rw-  2.0 fat   187510 b- defN 23-Nov-07 02:41 adrmdr/def.py
--rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      707 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      694 b- defN 24-Apr-01 08:58 adrmdr-0.1.6.dist-info/RECORD
-9 files, 466312 bytes uncompressed, 190839 bytes compressed:  59.1%
+-rw-rw-rw-  2.0 fat     1074 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      707 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       39 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat        7 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      694 b- defN 24-Apr-08 00:45 adrmdr-0.1.7.dist-info/RECORD
+9 files, 466520 bytes uncompressed, 190926 bytes compressed:  59.1%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: adrmdr/adrmdr.py
 Comment: 
 
 Filename: adrmdr/def.py
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/LICENSE
+Filename: adrmdr-0.1.7.dist-info/LICENSE
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/METADATA
+Filename: adrmdr-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/WHEEL
+Filename: adrmdr-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/entry_points.txt
+Filename: adrmdr-0.1.7.dist-info/entry_points.txt
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/top_level.txt
+Filename: adrmdr-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: adrmdr-0.1.6.dist-info/RECORD
+Filename: adrmdr-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## adrmdr/adrmdr.py

```diff
@@ -64,15 +64,15 @@
 
 
 global version_now
 global usergroup
 global setting_cfg
 global csdir
 global peizhidir
-version_now="0.1.6" 
+version_now="0.1.7" 
 usergroup="用户组=0"
 setting_cfg=""
 csdir =str (os .path .abspath (__file__ )).replace (str (__file__ ),"")
 if csdir=="":
     csdir =str (os .path .dirname (__file__ ))#
     csdir =csdir +csdir.split ("adrmdr")[0 ][-1 ]#
 
@@ -1269,15 +1269,16 @@
 			data.loc[(data["经营企业使用单位报告状态"]=="审核通过"), "有效报告"] = 1   			
 			
 			
 		if ini["模式"]=="药品":
 			data['用药开始时间'] = pd.to_datetime(data['用药开始时间'], format='%Y-%m-%d', errors='coerce') 			
 			data["时隔"]=pd.to_datetime(data["事件发生日期"])-pd.to_datetime(data["用药开始时间"])
 			data["时隔"]=data["时隔"].astype(str)
-			data["报告时限"] = pd.to_datetime(data["报告日期"]) - pd.to_datetime(data["事件发生日期"])
+			#data["报告时限"] = pd.to_datetime(data["报告日期"]) - pd.to_datetime(data["事件发生日期"])
+			data["报告时限"] = pd.to_datetime(data["国家中心接收时间"]) - pd.to_datetime(data["报告日期"])
 			data["报告时限"] = data["报告时限"].dt.days
 			data.loc[(data["报告时限"]>15)&(data["报告类型-严重程度"]=="严重"), "超时标记"] = 1
 			data.loc[(data["报告时限"]>30)&(data["报告类型-严重程度"]=="一般"), "超时标记"] = 1
 			data.loc[(data["报告时限"]>15)&(data["报告类型-新的"]=="新的"), "超时标记"] = 1
 			data.loc[(data["报告时限"]>1)&(data["报告类型-严重程度"]=="死亡"), "超时标记"] = 1  			
 
 			data.loc[~data["市评价时间"].isnull(), "有效报告"] = 1
@@ -5952,15 +5953,15 @@
 		pass
 
 
 	##############提示框########################
 	text = ScrolledText(root, height=400, width=400, bg="#FFFFFF")
 	text.pack(padx=5, pady=5)
 	text.insert(
-		END, "\n 本程序适用于整理和分析国家医疗器械不良事件信息系统、国家药品不良反应监测系统和国家化妆品不良反应监测系统中导出的监测数据。如您有改进建议，请点击其-意见反馈。\n\n 20240306 增加了国家药品新系统的兼容性。\n\n 20240329 修复了初始打开文件看不到xlsx格式的问题。"
+		END, "\n 本程序适用于整理和分析国家医疗器械不良事件信息系统、国家药品不良反应监测系统和国家化妆品不良反应监测系统中导出的监测数据。如您有改进建议，请点击其-意见反馈。\n\n 20240306 增加了国家药品新系统的兼容性。\n\n 20240329 修复了初始打开文件看不到xlsx格式的问题。\n\n 20240402 修改药品超时报告统计规则为国家中心接收时间-报告日期。"
 	)
 	text.insert(END, "\n\n")
 
 	#序列好验证、配置表生成与自动更新。
 	setting_cfg=read_setting_cfg()
 	generate_random_file()
 	setting_cfg=open_setting_cfg()
```

## Comparing `adrmdr-0.1.6.dist-info/LICENSE` & `adrmdr-0.1.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `adrmdr-0.1.6.dist-info/METADATA` & `adrmdr-0.1.7.dist-info/METADATA`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: adrmdr
-Version: 0.1.6
+Version: 0.1.7
 Summary: RTS
 Home-page: https://github.com/dfjsodjfwsysucai
 Author: sysucai
 Author-email: 411703730@qq.com
 Platform: Any platform -- don't need Windows
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

## Comparing `adrmdr-0.1.6.dist-info/RECORD` & `adrmdr-0.1.7.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 adrmdr/__init__.py,sha256=WOQVHRGH7qnH1l6p-PLsGWBoJHpWy73c9uDsjm2baJs,834
-adrmdr/adrmdr.py,sha256=vKFZdoSM_5uY993vqAq9BIP3OK_--fJcfufvr3Ta-5A,275355
+adrmdr/adrmdr.py,sha256=0YhN_XH64mGXgB2TOgjGOAWZu9JEzXFMnZNtNHr8iDo,275563
 adrmdr/def.py,sha256=5-BLEpcel4Y0lrgluNgpuj_wvrmgj20GQdwZtv4ACXc,187510
-adrmdr-0.1.6.dist-info/LICENSE,sha256=nC_P4SgMa07filsYB3QtksztRZ6EIwTDALA1pdyg__c,1074
-adrmdr-0.1.6.dist-info/METADATA,sha256=5OYDWyf0QVfSHeZTJJfScKYR41lFKHT1MondUU2f05M,707
-adrmdr-0.1.6.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-adrmdr-0.1.6.dist-info/entry_points.txt,sha256=-5hzbwj_1Wzf99wpjyLuGUCDb7tEaO4Fi0PuwlRc3Yw,39
-adrmdr-0.1.6.dist-info/top_level.txt,sha256=LHrx2R0xwMuSXcbeVRkxYrpOnQCiVSdnYPa-3UmkVWE,7
-adrmdr-0.1.6.dist-info/RECORD,,
+adrmdr-0.1.7.dist-info/LICENSE,sha256=nC_P4SgMa07filsYB3QtksztRZ6EIwTDALA1pdyg__c,1074
+adrmdr-0.1.7.dist-info/METADATA,sha256=c-sJzWK-vOaqWvxcdyU7ZpG1nG3K9WE9xYTKTuPq_Do,707
+adrmdr-0.1.7.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+adrmdr-0.1.7.dist-info/entry_points.txt,sha256=-5hzbwj_1Wzf99wpjyLuGUCDb7tEaO4Fi0PuwlRc3Yw,39
+adrmdr-0.1.7.dist-info/top_level.txt,sha256=LHrx2R0xwMuSXcbeVRkxYrpOnQCiVSdnYPa-3UmkVWE,7
+adrmdr-0.1.7.dist-info/RECORD,,
```

