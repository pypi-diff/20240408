# Comparing `tmp/lyyddforward-1.7.tar.gz` & `tmp/lyyddforward-1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lyyddforward-1.7.tar", last modified: Tue Jan 16 01:11:56 2024, max compression
+gzip compressed data, was "lyyddforward-1.8.tar", last modified: Mon Apr  8 05:06:48 2024, max compression
```

## Comparing `lyyddforward-1.7.tar` & `lyyddforward-1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-01-16 01:11:56.619441 lyyddforward-1.7/
--rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyddforward-1.7/LICENSE
--rw-rw-rw-   0        0        0      288 2024-01-16 01:11:56.618439 lyyddforward-1.7/PKG-INFO
--rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyddforward-1.7/README.md
-drwxrwxrwx   0        0        0        0 2024-01-16 01:11:56.616438 lyyddforward-1.7/lyyddforward.egg-info/
--rw-rw-rw-   0        0        0      288 2024-01-16 01:11:56.000000 lyyddforward-1.7/lyyddforward.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      221 2024-01-16 01:11:56.000000 lyyddforward-1.7/lyyddforward.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-01-16 01:11:56.000000 lyyddforward-1.7/lyyddforward.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-01-16 01:11:56.000000 lyyddforward-1.7/lyyddforward.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-01-16 01:11:56.000000 lyyddforward-1.7/lyyddforward.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    53523 2024-01-16 01:11:50.000000 lyyddforward-1.7/lyyddforward.py
--rw-rw-rw-   0        0        0       42 2024-01-16 01:11:56.619441 lyyddforward-1.7/setup.cfg
--rw-rw-rw-   0        0        0      369 2024-01-16 01:11:55.000000 lyyddforward-1.7/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-08 05:06:48.104708 lyyddforward-1.8/
+-rw-rw-rw-   0        0        0     1090 2023-09-21 00:20:00.000000 lyyddforward-1.8/LICENSE
+-rw-rw-rw-   0        0        0      159 2024-04-08 05:06:48.104708 lyyddforward-1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      253 2023-09-21 00:18:05.000000 lyyddforward-1.8/README.md
+drwxrwxrwx   0        0        0        0 2024-04-08 05:06:48.103703 lyyddforward-1.8/lyyddforward.egg-info/
+-rw-rw-rw-   0        0        0      159 2024-04-08 05:06:47.000000 lyyddforward-1.8/lyyddforward.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      221 2024-04-08 05:06:48.000000 lyyddforward-1.8/lyyddforward.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-08 05:06:47.000000 lyyddforward-1.8/lyyddforward.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-04-08 05:06:47.000000 lyyddforward-1.8/lyyddforward.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-04-08 05:06:47.000000 lyyddforward-1.8/lyyddforward.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    62127 2024-04-08 05:06:42.000000 lyyddforward-1.8/lyyddforward.py
+-rw-rw-rw-   0        0        0       42 2024-04-08 05:06:48.104708 lyyddforward-1.8/setup.cfg
+-rw-rw-rw-   0        0        0      369 2024-04-08 05:06:46.000000 lyyddforward-1.8/setup.py
```

### Comparing `lyyddforward-1.7/LICENSE` & `lyyddforward-1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `lyyddforward-1.7/lyyddforward.py` & `lyyddforward-1.8/lyyddforward.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,71 +3,156 @@
 from pypinyin import lazy_pinyin
 import re
 import requests
 import json
 from PIL import Image
 import base64
 import io
+import inspect
 import warnings
+import sqlite3
 from datetime import datetime
 from lyylog import log
 from sqlalchemy import create_engine, text, exc
 import lyytext
 from pdf2image import convert_from_path
 from urllib.parse import urlparse, unquote
 import lyyimage
 import lyyddsender
 import subprocess
 import lyyprocess
+import http.client
+
 """
 markdown_json发送前：
 data= {'msgtype': 'markdown', 'markdown': {'title': '图片', 'text': '![](@lAPPM25bqxb_A7PNApTNAcI)', 'at': {},'name':"luofei",'chinesename':'洛飞"}}
 wss收到的图片和文本格式：
 {'msg': '{"type":"text","markdown":{"from":"洛飞笔记","id":"77315199515","text":"充策略] 2023-12-28 11:09:47德业，建议取关一半。","image":""}}', 'mb': '77315199515'}
 {'msg': '{"type":"image","markdown":{"from":"傅峙峰","id":"77091290576","text":"","image":"https://static.d0P8eefTNBTwpng?auth_bizType=IM&bizType=im"}}', 'mb': '77091290576'}    
 {'msgtype': 'markdown', 'markdown': {'at': {'atMobiles': [], 'isAtAll': False}, 'text': '二个高标都板确认', 'title': '二个高标都板，突破7板，新的'}, 'name': 'dachenglupang', 'chinesename': '大成路旁', 'mb': 1756, 'cmd': 'mengxia'}
 
 """
 
 
-def try_to_ocr(msg_json, deny_ocr_text_patterns_list, ocr_engine, retry=True):
-    print("ocr engine=`", ocr_engine)
-    if ocr_engine == "tesseract":
+
+def get_img_size_from_url(url):
+    regex=r'_\d{2,4}_(\d{2,4})\.png'
+    match = re.search(regex,url)
+    if match:
+        width=match.group(1)
+        print("Width=",width)
+
+u="https://static.dingtalk.com/media/lALPD1za8UFzIqnNAsXNA0A_832_709.png?auth_bizType=IM&bizType=im"
+get_img_size_from_url(u)
+
+def is_weekday_time():
+    # 获取当前日期和时间
+    now = datetime.now()
+
+    # 判断是否是周一到周五
+    weekday = now.weekday() < 5
+
+    # 判断是否在9点到11点之间
+    time_interval = (920<=(now.hour*10 +now.minute) <=1000)
+
+    return weekday and time_interval
+def process_ocr(msg_json, text_rule_dict, deny_ocr_text_patterns_list,ocr_engine,retry=True,debug=False):
+    try: 
+        if "img" not in msg_json.keys() or msg_json["chinesename"]  in deny_ocr_text_patterns_list:
+            print("if ocr:","img" not in msg_json.keys() , msg_json["chinesename"]  in deny_ocr_text_patterns_list)
+            return None
+
+        print("有img字段且未在禁止ocr名单中，尝试ocr")
+        ocr_result_text = lyyimage.ocr_panddle_jd_server(msg_json['img'] )
+        if ocr_result_text is None:
+            return
+        ocr_result_text = process_format_msg_text(ocr_result_text, text_rule_dict)
+
+        print(f"来自{msg_json['chinesename']}群的图片ocr结束，过滤看是否有用：，无用则直接跳过回到正常图片处理流程")
+
+        if lyytext.ocr_text_is_useful(ocr_result_text, deny_ocr_text_patterns_list):
+            print("排除了其它不保留的OCR情况。开始处理")
+            msg_json_with_ocr_text = msg_json
+            msg_json_with_ocr_text["markdown"]["text"] = ocr_result_text
+            del msg_json_with_ocr_text["img"]
+            # lyyddforward.dd_to_db(engine, ocr_result_text, 消息中文群名, 来源群拼音,                                     msg_json['groupid'], msg_json['cmd'])
+
+            if len(ocr_result_text) < 4:
+                log("---------ok ocr result--------" + ocr_result_text + ",img=" + str(msg_json))
+                return
+            else:
+                print("<<<<OK ocr_yext=",msg_json_with_ocr_text)
+                return msg_json_with_ocr_text
+    except Exception as e:
+        return None
+
+
+
+
+def try_to_ocr_by_ocr_panddle_jd_server(img_link, ocr_red_text=False, debug=False):
+    # 目标URL
+    url = "http://117.72.45.252:10028/ocr"
+    print("img urlll=",img_link)
+    # 要发送的数据
+    post_data = {"img_url": img_link}
+
+    # 发送POST请求
+    response = requests.post(url, json=post_data)
+
+    # 检查响应是否成功
+    if response.status_code == 200:
+        if debug:
+            print(response.text)
+        # 解析JSON响应
+        result = response.json()
+        ocr_text = result.get("ocr_text")
+        if len(ocr_text) != 0 and not ocr_text.startswith("error"):            
+            return result.get("ocr_text")
+    
+    # 如果响应不成功，打印错误信息
+    print(f"Error: {response.status_code}, response={response}")
+    return None
+
+
+                
+def try_to_ocr_old(msg_json, deny_ocr_text_patterns_list,ocr_engine,retry=True,debug=False):
+    if ocr_engine  =="tesseract":
         ocr_function = lyyimage.ocr_img_file_to_text_by_tesseract
-    elif ocr_engine == "baidu-api":
+    elif ocr_engine  =="baidu-api" and  is_weekday_time():
+        print("current ocr engine=`","百度OCR")
+
         ocr_function = lyyimage.百度OCR
     else:
-        ocr_function = lyyimage.ocr_img_file_to_text
+        ocr_function = lyyimage.ocr_panddle_jd_server
+        print("current ocr engine=`","ocr_panddle")
+        #ocr_function = lyyimage.ocr_panddle
+
     msg_json_with_ocr_text = msg_json
     file_url = get_to_ocr_image_pdf_url(msg_json["img"])
-    file = download_file(file_url)
+    try:
+        file = download_file(file_url)
+    except Exception as e:
+        print("download file error=",e)
+        return None
     print("download is as " + file)
     if ".pdf" in file:
         ocr_text_result = ocr_pdf_file(file)
     elif ".jpg" in file or ".png" in file or ".bmp" in file or ".jpeg" in file:
         try:
-            ocr_red_text = True if msg_json['chinesename'] in deny_ocr_text_patterns_list else False
-            ocr_text_result = ocr_function(file, ocr_red_text=ocr_red_text, debug=True)
-            print("ocr reasult =", str(ocr_text_result))
-            if ocr_text_result and lyytext.count_digits(ocr_text_result) > 20 and not lyytext.deny_ocr_text_patterns(deny_ocr_text_patterns_list, ocr_text_result, debug=True):
-                msg_json_with_ocr_text['markdown']['text'] = ocr_text_result
-                del msg_json_with_ocr_text['img']
-                return ocr_text_result
+            ocr_red_text = True if msg_json['chinesename'] in deny_ocr_text_patterns_list else False               
+            ocr_text_result = ocr_function(file, ocr_red_text=ocr_red_text, debug=debug)
 
+            return ocr_text_result
         except Exception as e:
-            print("in ocr function, error msg=", str(e), "if retry then retry:", retry)
+            log("in ocr function, error msg="+ str(e)+"if retry then retry:"+ str(retry))
             if retry:
+                ocr_engine  ="ocr_panddle" if ocr_engine  =="baidu-api" else "baidu-api"
+                try_to_ocr(msg_json, deny_ocr_text_patterns_list, ocr_engine,retry=False)
 
-                lyyprocess.kill_process_by_name("Umi-OCR.exe")
-                lyyprocess.subprocess.Popen([r"D:\Soft\Umi-OCR_Paddle_v2.0.1\Umi-OCR.exe"])
-                time.sleep(5)
-                try_to_ocr(msg_json, deny_ocr_text_patterns_list, retry=False)
-
-
-def forward_msg_group_by_group(df, msg_json, debug=False):
+def forward_msg_group_by_group(df,msg_json,debug=False):
 
     for index, row in df.iterrows():
         to = row['to']
         fromgroup = row['from']
         fromuser = row['fromuser']
         from_group_name = row['from_group_name']
         # prefix = row['prefix']
@@ -103,58 +188,62 @@
                 title = prefix if prefix is not None else "图片"
                 result = dd.send_markdown_img(title, msg_json['img'])
 
             else:
                 if debug: print(f"{msg_json['chinesename']} 不是图片")
                 if markdown_text and prefix is not None and "https" not in markdown_text:
                     markdown_text = prefix + "：" + markdown_text
-                msg_json_full = msg_json_from_text_or_imgurl(markdown_text)
-                result = lyy_send_msg_json_by_pass_hosts(钉钉webhook, 钉钉sign, msg_json_full)
+                msg_json_full = msg_json_from_text_or_imgurl(
+                    markdown_text)
+                result = lyy_send_msg_json_by_pass_hosts(
+                    钉钉webhook, 钉钉sign, msg_json_full)
         return result
 
 
-def download_file(url):
-    print("in download file")
+
+def download_file(url,debug=False):
+    if debug: print("in download file")
     response = requests.get(url)
     filename = get_filename_from_url(url)
-    print("to saved as " + filename)
+    if debug: print("to saved as "+filename)
     with open(filename, 'wb') as output_file:
         output_file.write(response.content)
+    if debug: print("in download_file,  finished")
     return filename
 
-
-def get_to_ocr_image_pdf_url(text, debug=False):
+def get_to_ocr_image_pdf_url(text,debug=False):
     if debug: print("enter get_to_ocr_image_pdf_url")
     pattern = r'https?://[\w/\-?=%.]+\.(pdf|png|jpeg|jpg|bmp)'
     if debug: print("try to search")
-    match = re.search(pattern, text)
-    if match:
-        if debug: print("找到匹配=", match.group())
+    match = re.search(pattern,text)
+    if match:        
+        if debug: print("找到匹配=",match.group())
         return match.group()
     else:
         if debug: print("没有匹配，返回False")
         return False
 
-
 def get_filename_from_url(url):
     print("get_filename_from_url")
-    extension = url[-4:]
-    return "tmp" + extension
+    extension =  url[-4:]
+    return "tmp"+extension
+
 
 
 def ocr_pdf_file(pdf_file_path):
     images = convert_from_path(pdf_file_path)
     result_text_list = []
     for i, image in enumerate(images):
         image.save(f'image{i}.png', 'PNG')
         ocr_text_result = lyyimage.ocr_img_file_to_text(f'image{i}.png')
         result_text_list.append(ocr_text_result)
     return "\n".join(result_text_list)
 
 
+
 def lyytimer时间没超(时间文本):
     nowtime_full = str(datetime.now())
     现在时 = nowtime_full[11:13]
     现在分 = nowtime_full[14:16]
     现在时间 = nowtime_full[11:16]
 
     # print(现在时)
@@ -226,203 +315,262 @@
         if int(现在时) < int(时间范围的起始时间):
 
             return False
         else:
             return True
 
 
-def process_QYbot_msg(self, qybot_msg, debug=False):
-    """
-    socket server接收到元素：<message=厕所镜子&webhook=6215350562012f&sign=SECeba7ab6bc9e752f3468701>
-    """
-    msg_and_ddinfo = qybot_msg.split("&webhook=", 1)
-    msg_text = msg_and_ddinfo[0].replace("message=", "").replace("imgurl=", "")
-    if debug: print(msg_and_ddinfo[1])
-    webhook, sign = msg_and_ddinfo[1].split("&sign=", 1)
-    #send_ding_message(webhook,sign,msg_text,是否图片=False,is_send_all=False)
-    msg_json = msg_json_from_text_or_imgurl(msg_text)
-    print("in process_QYbot_msg, jsg_json=" + str(msg_json))
-
-    msg = msg_json_from_text_or_imgurl(msg_text)
-    print("after, msg=" + str(msg))
-    result = lyy_send_msg_json_by_pass_hosts(webhook, sign, msg)
 
-    self.insert_text_in_text3(qybot_msg + "\nresult=" + result)
+def process_format_msg_text(msg, text_rule_dict,debug=False):
+    #if debug: print("enter fun process_msg_text,text_rule_dict=",text_rule_dict)
+    #根据字典中的设置对文本对待处理
+    #1. 删除re模式 2.删除文本 3.替换文本 4.删除首尾
+    #参数1如果是str直接处理
+
+    markdown_text=msg if isinstance(msg,str) else msg['markdown']['text']
+    if markdown_text.startswith("http")  :
+        return markdown_text
 
+    #if debug: print("#批量删除特定re模式")
+    #if debug: print("in process_msg_text, text_rule_dict=",text_rule_dict['global_remove_patterns'].keys())
+    
+    markdown_text = lyytext.batch_remove_regex_strings_by_list(text_rule_dict['global_remove_patterns'].keys(),markdown_text,debug=debug)
 
-def process_msg_text(msg, process_text_rule_dict, debug=False):
-    #参数1如果是str直接处理
-    markdown_text = msg if isinstance(msg, str) else msg['markdown']['text']
+    #if debug: print("#删除特定文本")
+    markdown_text = lyytext.batch_format_remove_subtext(markdown_text,text_rule_dict["global_remove_subtext"].keys(),debug=debug)
+
+    #if debug: print("#替换特定文本")
+    markdown_text = lyytext.batch_replace_text_by_dict(markdown_text, text_rule_dict['global_replace_patterns'],debug=debug)
+
+    #if debug: print("#去除收尾特定字符。")
+    markdown_text = lyytext.batch_strip_text(markdown_text,text_rule_dict["strip_characters"].keys(),debug=debug)
+    #if debug: print("in process_msg_text, result=",markdown_text)
+    return markdown_text
+
+def get_img_url_from_server(img_url="@lALPM25brIffogLNASPNAl8"):
+    conn = http.client.HTTPConnection("127.0.0.1", 12888)
+    conn.request("GET", f"/?{img_url}")
+    response = conn.getresponse()
+    data = response.read().decode("utf-8")
+    return data
+
+def extracet_img_packet(text):
+    pattern = r'!\[screenshot\]\(@([a-zA-Z0-9\-\_]+?)\)'
+    # 使用正则表达式搜索
+    matches = re.search(pattern, text)
+
+    # 检查是否有匹配
+    if matches:
+        # 提取匹配的组
+        extracted_text = matches.group(1)
+
+        log("找到图片包,imgpacket=",extracted_text)
+        url = get_img_url_from_server(extracted_text)
+        return(extracted_text)  # 输出: lALPM2OzMXg0v_7NBOLNArI
 
-    markdown_text = re.sub(r'\n+', '\n', markdown_text)
-    #print("keyword_to_replace=",remove_subtext_list,end=" ")
-    if "img" not in msg:
-        if debug: print("#批量删除特定re模式")
-        markdown_text = lyytext.batch_remove_regex_strings_by_list(process_text_rule_dict['global_remove_patterns'].keys(), markdown_text, debug=debug)
-        if debug: print("markdown_text=", markdown_text)
-        # markdown_text = lyyddforward.format_remove_subtext_by_patterns(
-        #     markdown_text, global_remove_patterns_list)
-        if debug: print("#删除特定文本")
-        markdown_text = lyytext.format_remove_subtext(markdown_text, process_text_rule_dict["global_remove_subtext"].keys(), debug=debug)
-
-        if debug: print("#替换特定文本")
-        markdown_text = lyytext.format_replace_text(markdown_text, process_text_rule_dict['global_replace_patterns'], debug=debug)
-        # #查找re模式，替换成特定文本
-        # markdown_text = lyyddforward.format_replace_text_by_patterns(
-        #     markdown_text, replace_text_patterns_dict)
-        if debug: print("#去除收尾特定字符。")
-        markdown_text = lyytext.batch_strip_text(markdown_text, process_text_rule_dict["strip_characters"], debug=debug)
-    return markdown_text.strip(".").strip()
+    else:
+        print("No match found")
+        return text
 
 
-def format_mengxia(msg_json, number, number_pinyin_dict, number_chinese_dict, debug=False):
-    #{'type': 'text', 'msg': '[52秒] [请用手机APP收听](https://static.dingtalk.com/media/lAXPDf0i9wsXJoXOd3xZy84aeXqv.mp3) \r\n 语音消息 ', 'url': '', 'name': ''}
+def format_xmpro(original_data, pinyin2token,token,dict_group_pinyin):
+    if isinstance(original_data,str):
+        original_data=json.loads(original_data)
     json_new = {'msgtype': 'markdown', 'markdown': {'at': {}}}
+    if original_data['msgtype']=="text":
+        json_new['markdown']['text']=original_data['text']['content']   
+        json_new['markdown']['title'] = original_data['text']['title'] if "title" in original_data['text'] else original_data['text']['content'] [:20]
+
+    
+    elif original_data['msgtype']=="markdown":
+        if "![screenshot](@" in original_data['markdown']['text']:
+            #flsk_msg_json =  {'msgtype': 'markdown', 'markdown': {'title': '#### 扑影: 茅台     ![screenshot](@lALPM2OzMXg0v_7NBOLNArI)         > 2024-04-08 上午 10:33:39   ', 'text': '####  扑影: 茅台     ![screenshot](@lALPM2OzMXg0v_7NBOLNArI)         > 2024-04-08 上午 10:33:39   '}, 'at': {'atMobiles': [], 'isAtAll': False}}
+            print("format_xmpro, startswith screenshot")
+            url = extracet_img_packet(original_data['markdown']['text'])
+            json_new['markdown']['text'] = json_new['img']=url
+            json_new ['title']="图片"
+        else:
+            print("markdown, but not screenshot")
+            json_new['markdown']['text'] = original_data['markdown']['text']
+            json_new['markdown']['title'] = original_data['markdown']['title']
+
+    elif original_data['msgtype']== 'actionCard':
+        print("you got an actionCard")
+        json_new['markdown']['text'] = original_data['actionCard']['text']
+        json_new ['markdown']['title']=original_data['actionCard']['title']
+
+    else:
+        #flsk_msg_json =  {'actionCard': {'title': 'certificate.pem', 'text': 'certificate.pem', 'hideAvatar': '0', 'btnOrientation': '1', 'singleTitle': '立即查看', 'singleURL': ''}, 'msgtype': 'actionCard'}
+        log("format_xmpro, msg_type不是markdown又不是text,original_data=",str(original_data))
+    
+
+    json_new['name']= token
+    json_new['chinesename'] = dict_group_pinyin.get(json_new['name'])
+    json_new['groupid']=0
+    json_new['cmd'] = "showmsg"
+    return json_new
+# {'msgtype': 'markdown', 'markdown': {'at': {}, 'text': 'd d a ', 'title': 'd d a '}, 'name': '7823f3682963d60828b772cd8d08206b219bcbd51bb823045bf4e8e607a34fad***SECa5ec4cb87b097f4b48d0249be3b3505e6dd8c29a8fb2bb68639e09348ef8de93***好的', 'chinesename': None, 'cmd': 'showmsg'}
+    # data_type = original_data['msg']['type']
+    # data_text = original_data['msg']['text']
+    # data_title = original_data['msg']['title']
+    #text:1,image:2,link:102,file:501,voice:3,richtext:3100
+
+    #msg_json =  {'msgtype': 'markdown', 'markdown': {'title': '[ͼƬ]', 'text': '![screenshot](https://static.dingtalk.com/media/lQLPJxuMEduq0pE0eLCK5L7vMiTxswYACJrskR4A_120_52.png?auth_bizType=IM&bizType=im)'}, 'at': {'atMobiles': [], 'isAtAll': False}}
+    # [23:56:15]jsonStr={"msg":{"id":"18782752867960","type":1200,"title":"DING]() ","text":"DING]() "},"source":{"type":2,"uid":"4184562838","nick":"1","cid":"56752603742","name":"震哥ad"}}
+    #[00:05:52]jsonStr={"msg":{"id":"18798625399052","type":1200,"title":"[图片]  ","text":"![](@lADPD0eJ-qyq9jnNBQDNA-E)    "},"source":{"type":2,"uid":"4184562838","nick":"1","cid":"56752603742","name":"震哥ad"}}
+
+def format_mengxia(msg_json, number, number_pinyin_dict,number_chinese_dict,debug=False):
+     #{'type': 'text', 'msg': '[52秒] [请用手机APP收听](https://static.dingtalk.com/media/lAXPDf0i9wsXJoXOd3xZy84aeXqv.mp3) \r\n 语音消息 ', 'url': '', 'name': ''}
+    json_new = {'msgtype': 'markdown', 'markdown': {'text':'','title':'','at': {}}}
     if msg_json['type'] == "text":
-        json_new['markdown']['text'] = msg_json["msg"]
-    elif msg_json['type'] == "pic" or msg_json['type'] == "file":
-        json_new['markdown']['text'] = msg_json["url"]
-        json_new['img'] = msg_json['url']
+        json_new['markdown']['text']= msg_json["msg"].replace("\\/","/").replace(r"/////",r"//")
+    elif msg_json['type'] == "pic" :
+        json_new['markdown']['text']= msg_json["url"].replace("\\/","/").replace(r"/////",r"//")
+        json_new['img']=json_new['markdown']['text']
+    elif msg_json['type'] == "file":
+        json_new['markdown']['text']= msg_json["url"].replace("\\/","/").replace(r"/////",r"//")
     else:
         log("in get_msg_content_from_json, 出现第3种情况 ", +str(msg_json))
     #生成标准json，如果黑名单，返回None，后续会跳过处理。
     if len(json_new['markdown']['text']) < 3:
         return None
-    json_new['markdown']['text'] = json_new['markdown']['text'].replace("\\/", "/")
-
     if "title" in msg_json.keys():
         json_new['markdown']['title'] = msg_json['title']
     else:
         json_new['markdown']['title'] = json_new['markdown']['text'][:14]
+    
     json_new['groupid'] = number
     json_new['cmd'] = "mengxia"
     # print("try to get pinyin from number_pinyin_dict")
-    if number in number_pinyin_dict.keys():
-        json_new['name'] = number_pinyin_dict[number]
-        json_new['chinesename'] = number_chinese_dict[number]
+
+    if "name" in msg_json.keys() and "chinesename" in msg_json.keys():
+        json_new['name']=msg_json.get("name")
+        json_new['chinesename']=msg_json.get("chinesename")
 
     else:
-        log(f"此number{number}没有。message={msg_json}")
-        json_new['name'] = "weizhiqunzu"
-        json_new['chinesename'] = "未知群组"
+        if number in number_pinyin_dict.keys():
+            json_new['name'] = number_pinyin_dict[number]
+            json_new['chinesename'] = number_chinese_dict[number]
 
-    return json_new
+        else:
+            log(f"此number{number}没有。message={msg_json}")
+            json_new['name'] = "weizhiqunzu"
+            json_new['chinesename'] = "未知群组"
 
+    return json_new
 
 def get_chinesename_sign_dict(ddforward_file=r"D:\UserData\resource\ddForward\ddForward.ini"):
     cfdd = configparser.ConfigParser()
     cfdd.read(ddforward_file, encoding="utf-8")
     config_dict = {}
     for section in cfdd.sections():
         group_name = get_config_value(cfdd, section, "from_group_name")
         webhook_sign = get_config_value(cfdd, section, "to")
         config_dict[group_name] = webhook_sign
     return config_dict
 
-
 def get_dict_from_file(file_path):
     # 读取文件内容
-    with open(file_path, 'r', encoding="utf-8") as file:
+    with open(file_path, 'r',encoding="utf-8") as file:
         content = file.read()
     # 将文本内容转换为字典
     data = {}
     lines = content.split('\n')
     for line in lines:
         if ":" in line:  # 忽略空行
             key, value = line.split(':')
-            data[int(key.strip())] = value.strip().replace('"', '').replace(',', '')
+            data[int(key.strip())] = value.strip().replace('"','').replace(',','')
     # 将字典转换为 JSON 格式并打印
     return data
 
-
-def get_chinese_from_pinyin(pinyin, dict_group_pinyin, debug=False):
+def get_chinese_from_pinyin(pinyin,dict_group_pinyin,debug=False):
 
     for key, val in dict_group_pinyin.items():
         if pinyin in key:
             return val
     log(f"pinyin没找到匹配的chinese，请检查。pinyin={pinyin} ")
     return "未知群组"
     if debug: print(f"{str(dict_token_pinyin)}")
 
 
-def get_pinyin_from_token(token, dict_token_pinyin):
+def get_pinyin_from_token(token,dict_token_pinyin):
     for key, val in dict_token_pinyin.items():
         if token in val:
             return key
     log(f"token没找到匹配的拼音，请检查。token={token}, {str(dict_token_pinyin)}")
 
-    # def format_flask(json_data,group_name_replace_dict_flask,dict_groupid_chinese):
-    #     if "img" not in json_data.keys():
-    #         txt_content=json_data['markdown']['text']
-    #         img=get_http_imgurl_from_text(txt_content)
-    #         if img is not None:
-    #             json_data['img']=img
-    #             json_data['markdown']['title']="图片"
-    #         else:#真的不是图片
-    #             json_data['markdown']['title']=txt_content[:14]
-    #     print("in format_flask, json = ",json_data)
-
-    return json_data
 
 
-def format_flask2(json_data, group_name_replace_dict_flask, dict_groupid_chinese):
-    msg_json = {"msgtype": "markdown", "markdown": {"title": "[]", "text": ""}, "at": {}}
+# def format_flask(json_data,group_name_replace_dict_flask,dict_groupid_chinese):
+#     if "img" not in json_data.keys():
+#         txt_content=json_data['markdown']['text']
+#         img=get_http_imgurl_from_text(txt_content)
+#         if img is not None:
+#             json_data['img']=img
+#             json_data['markdown']['title']="图片"
+#         else:#真的不是图片
+#             json_data['markdown']['title']=txt_content[:14]
+#     print("in format_flask, json = ",json_data)
+
+#    return json_data
+def format_flask2(json_data,group_name_replace_dict_flask,dict_groupid_chinese):
+    msg_json={"msgtype": "markdown", "markdown": {"title": "[]", "text": ""}, "at": {}}
     if "source" in json_data.keys():
-        msg_json['chinesename'] = 群中文名 = json_data['source']['name']
-        群号 = json_data['source']['cid']
-        msg_json['fromuser'] = json_data['source']['uid']
-        msg_json['groupid'] = 群号
+        msg_json['chinesename'] =群中文名=json_data['source']['name']
+        群号=json_data['source']['cid']
+        msg_json['fromuser']=json_data['source']['uid']
+        msg_json['groupid']=群号
     else:
         msg_json['chinesename'] = json_data['from']
         msg_json['fromuser'] = json_data['uid']
-
-    if json_data['groupid'] in dict_groupid_chinese.keys():
-        msg_json['chinesename'] = dict_groupid_chinese[json_data['groupid']]
-    elif json_data['chinesename'] in group_name_replace_dict_flask.keys():
-        msg_json['chinesename'] = group_name_replace_dict_flask[json_data['chinesename']]
+    
+    if json_data['groupid']  in dict_groupid_chinese.keys():
+        msg_json['chinesename'] =dict_groupid_chinese[json_data['groupid'] ]
+    elif  json_data['chinesename']  in group_name_replace_dict_flask.keys():
+        msg_json['chinesename'] =group_name_replace_dict_flask[json_data['chinesename'] ]
 
     if "img" in json_data.keys():
-        txt_content = msg_json['img'] = json_data['img']
-        msg_json['markdown']['title'] = "图片"
+        txt_content=msg_json['img']= json_data['img']
+        msg_json['markdown']['title']="图片"
     else:
-        txt_content = json_data['msg']['text']
-        img = get_http_imgurl_from_text(txt_content)
+        txt_content=json_data['msg']['text']
+        img=get_http_imgurl_from_text(txt_content)
         # img=extract_link(txt_content)
         if img is not None:
-            msg_json['img'] = img
-            msg_json['markdown']['title'] = "图片"
-        else:  #真的不是图片
-            msg_json['markdown']['title'] = txt_content[:14]
-
-    msg_json['markdown']['text'] = txt_content
-    msg_json['groupid'] = 群号
+            msg_json['img']=img
+            msg_json['markdown']['title']="图片"
+        else:#真的不是图片
+            msg_json['markdown']['title']=txt_content[:14]
 
-    msg_json['cmd'] = "showmsg"
-    msg_json['name'] = get_pinyin(msg_json['chinesename'])
+    msg_json['markdown']['text']=txt_content
+    msg_json['groupid']= 群号
+    
+    msg_json['cmd']="showmsg"
+    msg_json['name']=get_pinyin(msg_json['chinesename'])
     return msg_json
 
 
-def format_wss(msg_json, group_name_replace_dict_wss={}, debug=False):
+def format_wss(msg_json,group_name_replace_dict_wss={},debug=False):
     if msg_json['type'] == "text":
         if debug: print("1.type is text")
         msg_json_result = convert_txt_to_markdown(msg_json['markdown']['text'])
         if debug: print("2.new json")
     else:
         if debug: print("1.type is image")
         msg_json_result = convert_img_to_markdown(msg_json['markdown']['image'])
 
     from_chinese_name = msg_json['markdown']['from']
-    if debug: print(f"3.get chinesename={from_chinese_name}")
+    if debug:print(f"3.get chinesename={from_chinese_name}")
     msg_json_result['groupid'] = msg_json['markdown']['id']
-    if debug: print(f"5.groupid={msg_json_result['groupid'] }")
+    if debug:print(f"5.groupid={msg_json_result['groupid'] }")
 
     msg_json_result['chinesename'] = group_name_replace_dict_wss[from_chinese_name] if from_chinese_name in group_name_replace_dict_wss.keys() else from_chinese_name
-
-    msg_json_result['name'] = "".join(get_pinyin(msg_json_result['chinesename']))
-    if debug: print(f"4.get name={msg_json_result['name'] }")
+    
+    msg_json_result['name'] = "".join(get_pinyin(msg_json_result['chinesename'] ))
+    if debug:print(f"4.get name={msg_json_result['name'] }")
 
     msg_json_result['cmd'] = "showwss"
     return msg_json_result
 
 
 def convert_txt_to_markdown(txt):
     mk = {
@@ -449,47 +597,48 @@
     }
     mk['markdown']['text'] = image_url
     mk['markdown']['title'] = "图片"
     mk['img'] = image_url
     return mk
 
 
-def get_config_value(config, section, option):
-    try:
-        value = config.get(section, option)
-        return value
-    except (configparser.NoSectionError, configparser.NoOptionError):
-        return ""
-
 
 # 解析 INI 配置文件
 def parse_ini_config(ini_config_file):
     ini_config = configparser.ConfigParser()
     ini_config.read(ini_config_file, encoding="utf-8")
     return ini_config
 
 
-def config2dict(config, section, option, sep="|", sub_sep="*", debug=False):
+def get_config_value(config, section, option,debug=False):
+    try:
+        txt = config.get(section, option)
+        
+    except (configparser.NoSectionError, configparser.NoOptionError):
+        if debug: print(f"读取字典{config}/{section}/{option}失败，使用默认空值")
+        txt = ""
+    return txt
+
+def config2dict(config, section:str, option:str, sep="|", sub_sep="*", debug=False):
     #单值
     txt = get_config_value(config, section, option)
-    if debug: print("config item = ", txt)
     #txt = "47904542011*特定群名|47696677108*特定输出|52625333512*涨停猫|47904542011*输入群"
     txt_list = txt.strip(sep).split(sep)
 
     result = {}
     for item in txt_list:
-        key_value = item.split(sub_sep, 1)
+        key_value = item.split(sub_sep,1)
         if len(key_value) == 1:
             key = key_value[0]
             if debug: print("只有一项，赋空值")
             result[key] = ""
         else:
             key, value = key_value
             result[key] = value
-    if debug: print("xresult = ", result)
+    if debug: print(f"config2dict 读取字典{config}/{section}/{option} = ", result)
     return result
 
 
 def get_pinyin(string):
 
     def is_chinese(char):
         return 'u4e00' <= char <= '\u9fa5'
@@ -694,26 +843,25 @@
     signature = base64.b64encode(hmac_code).decode()
     headers = {"Content-Type": "application/json"}
     payload = {"msgtype": "text", "text": {"content": content}, "at": {"isAtAll": False}}
     params = {"access_token": access_token, "timestamp": timestamp, "sign": signature}
     if display: print(headers, payload, params)
     return headers, payload, params
 
-
-def get_http_imgurl_from_text(msg_text, debug=False):
+def get_http_imgurl_from_text(msg_text,debug=False):
     # 定义正则表达式模式
     pattern = r'(https?://(tc|gchat|static).*(jpg|auth_bizType=IM|png|jpg|/0))'
     match = re.search(pattern, msg_text)
     if match:
         matched_text = match.group()
         if debug: print(f"匹配成功", match.group())
         return matched_text
 
 
-def msg_json_from_text_or_imgurl(msg_text, debug=False):
+def msg_json_from_text_or_imgurl(msg_text,debug=False):
     # 定义正则表达式模式
     pattern = r'(https://(gchat|static).*(jpg|auth_bizType=IM|png|jpg|/0))'
     match = re.search(pattern, msg_text)
     if match:
         matched_text = match.group()
         if debug: print(f"匹配成功", match.group())
 
@@ -1162,45 +1310,95 @@
             # ActionCard类型
             data = {"title": self.title, "actionURL": self.url}
             return data
         else:
             logging.error("CardItem是ActionCard的子控件时，title、url不能为空；是FeedCard的子控件时，title、url、pic_url不能为空！")
             raise ValueError("CardItem是ActionCard的子控件时，title、url不能为空；是FeedCard的子控件时，title、url、pic_url不能为空！")
 
+def dd_to_db(msg_json, 替换字典, cmd,groupid="0", debug=False):
+    mysql_text = lyytext.batch_replace_text_by_dict(msg_json["markdown"]["text"], 替换字典)
+    dd_to_SQLite(engine,mysql_text, msg_json['chinesename'], msg_json['name'], cmd,groupid=groupid, debug=debug)
+    dd_to_MySql(engine,mysql_text, msg_json['chinesename'], msg_json['name'], cmd,groupid=groupid, debug=debug)
+
+def dd_to_SQLite(msg_json, msg_text, conn_text=None, debug=False):
+    if debug: print("in dd_to_SQLite",msg_json)
+    中文群名= msg_json["chinesename"]
+    群拼音=msg_json["name"]
+    cmd=msg_json["cmd"]
+    groupid = msg_json["groupid"]
+
+    conn = sqlite3.connect(conn_text)
+
+    if debug: print("    # SQLite创建数据库dddata.db")
+    
+    cursor = conn.cursor()
+    current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+    if debug: print("    # SQLite创建表stock_info")
+    cursor.execute("""
+        CREATE TABLE IF NOT EXISTS stock_info (
+            id INTEGER PRIMARY KEY AUTOINCREMENT,
+            time TEXT,
+            name TEXT,
+            chinesename TEXT,
+            new TEXT,
+            groupid TEXT,
+            message TEXT
+        )
+    """)
+    if debug: print("sqlite准备查询")
+
+    cursor.execute("INSERT INTO stock_info (time, name, chinesename, new, groupid, message) VALUES (?, ?, ?, ?, ?, ?)", (current_time, 群拼音, 中文群名, cmd, groupid, msg_text))
+    affected_rows = cursor.rowcount
+    conn.commit()
+    cursor.close()
+    conn.close()
+    return affected_rows
+
 
-def dd_to_MySql(engine, msg_text, 中文群名, 群拼音, cmd, groupid="0", debug=False):
+
+def dd_to_MySql(engine,msg_text, 中文群名, 群拼音, cmd,groupid="0", debug=False):
+    debug=True
     # 创建MySQL连接
     # conn = engine.connect()
     # if "http" not in msg_text:
     #     from dd01msg import recovery_text_mysql
     #     msg_text = recovery_text_mysql(msg_text,mysql替换文本对数组)
-
+    if len(msg_text)<1:
+        if debug: print("in dd_to_MySql, msg_text<1")
+        return
     current_time = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
 
-    # 插入数据到 MySQL
-    insert_query = text("INSERT INTO stock_info (time, name, chinesename, new,groupid, message) VALUES (:time, :name, :chinesename, :new,:groupid, :message)")
-    params = {'time': current_time, 'name': 群拼音, 'chinesename': 中文群名, 'new': cmd, 'groupid': groupid, 'message': msg_text}
+    if debug: print("# 插入数据到 MySQL")
+    insert_query = text("INSERT INTO stock_info (time, name, chinesename, new, groupid, message) VALUES (:time, :name, :chinesename, :new, :groupid, :message) ON DUPLICATE KEY UPDATE time = IF(groupid = :groupid AND message = :message AND time >= NOW() - INTERVAL 1 MINUTE, VALUES(time), time);")
+    params = {
+        'time': current_time,
+        'name': 群拼音,
+        'chinesename': 中文群名,
+        'new':cmd,
+        'groupid': groupid,
+        'message': msg_text
+
+    }
 
     try:
         with engine.begin() as connection:
             result = connection.execute(insert_query, params)
             affected_rows = result.rowcount  # 获取成功插入的行数
-            print(f"Affected rows: {affected_rows}")
+            if debug: print(f"mysql Affected rows: {affected_rows}")
             if affected_rows > 0:
-                # 插入成功
+                if debug: print("# 插入成功")
                 return affected_rows
             else:
                 # 插入失败
                 return 0
     except Exception as e:
         log("Insert ddmsg to MySQL error. errormsg =" + str(e))
-        return 0
 
 
-def remove_from_MySql(engine, msg_text, 中文群名, 群拼音, cmd, groupid="0", debug=False):
+def remove_from_MySql(engine,msg_text, 中文群名, 群拼音, cmd,groupid="0", debug=False):
 
     # 插入数据到 MySQL
     if debug: print(f"try to delete no specify user's message,pinyin={群拼音},msg={msg_text}")
     insert_query = text(f'delete from stock_info where name="{群拼音}" and message="{msg_text}"')
 
     try:
         with engine.begin() as connection:
@@ -1212,14 +1410,15 @@
             else:
                 return 0
     except Exception as e:
         log("delete ddmsg to MySQL error. errormsg =" + str(e))
         return 0
 
 
+
 if __name__ == '__main__':
 
     webhook = "62153505b1635f6f0a0b0ed41fb0f2e0dff5fd9373ce093be85b3f2db262012f"
     sign = "SECeba7ab6bc8fc2341a25034a5d5e703995279ebedb42455f9d4920752f3468701"
     webhook = "62e08928ef4864af0ccff2cc446d2bbd89591493871565db4d9cc2a7f0304a08"
     sign = "SEC37d6650050af983c66c842dbc9c631f879be6629f4e35cb9d95e024f19f6a114"
     t = '.\r\r![screenshot](https://static.dingtalk.com/media/lADPD1Iyci_hm4bNAr7NBLA_1200_702.jpg_620x10000q90g.jpg?auth_bizType=IM)\r\r.'
```

