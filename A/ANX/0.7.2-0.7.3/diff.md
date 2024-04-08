# Comparing `tmp/ANX-0.7.2.tar.gz` & `tmp/ANX-0.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ANX-0.7.2.tar", last modified: Tue Apr  2 03:01:02 2024, max compression
+gzip compressed data, was "ANX-0.7.3.tar", last modified: Mon Apr  8 11:35:14 2024, max compression
```

## Comparing `ANX-0.7.2.tar` & `ANX-0.7.3.tar`

### file list

```diff
@@ -1,165 +1,166 @@
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.659266 ANX-0.7.2/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.610915 ANX-0.7.2/ANX.egg-info/
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-02 03:01:02.000000 ANX-0.7.2/ANX.egg-info/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)     4860 2024-04-02 03:01:02.000000 ANX-0.7.2/ANX.egg-info/SOURCES.txt
--rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-02 03:01:02.000000 ANX-0.7.2/ANX.egg-info/dependency_links.txt
--rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-02 03:01:02.000000 ANX-0.7.2/ANX.egg-info/requires.txt
--rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-02 03:01:02.000000 ANX-0.7.2/ANX.egg-info/top_level.txt
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.611718 ANX-0.7.2/AndroidQQ/
--rw-r--r--   0 1a         (501) staff       (20)    33802 2024-03-12 14:39:25.000000 ANX-0.7.2/AndroidQQ/Android.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.612279 ANX-0.7.2/AndroidQQ/Echo/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/Echo/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/Echo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     4040 2024-04-02 03:00:23.000000 ANX-0.7.2/AndroidQQ/Tcp.py
--rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.616454 ANX-0.7.2/AndroidQQ/http/
--rw-r--r--   0 1a         (501) staff       (20)     2017 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/http/ClientKey.py
--rw-r--r--   0 1a         (501) staff       (20)      119 2024-03-05 18:40:23.000000 ANX-0.7.2/AndroidQQ/http/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1961 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/http/accounts.py
--rw-r--r--   0 1a         (501) staff       (20)     3760 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/http/friends.py
--rw-r--r--   0 1a         (501) staff       (20)     6591 2024-03-05 18:40:23.000000 ANX-0.7.2/AndroidQQ/http/game_credit.py
--rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/http/headers.py
--rw-r--r--   0 1a         (501) staff       (20)     7078 2024-03-17 04:57:20.000000 ANX-0.7.2/AndroidQQ/http/level.py
--rw-r--r--   0 1a         (501) staff       (20)     9985 2024-02-13 12:05:01.000000 ANX-0.7.2/AndroidQQ/http/music.py
--rw-r--r--   0 1a         (501) staff       (20)     1539 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/http/qqsignin.py
--rw-r--r--   0 1a         (501) staff       (20)     1279 2024-03-01 14:47:52.000000 ANX-0.7.2/AndroidQQ/http/weishi.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.617034 ANX-0.7.2/AndroidQQ/im/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.617370 ANX-0.7.2/AndroidQQ/im/oidb/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.617792 ANX-0.7.2/AndroidQQ/im/oidb/OidbSvc_0xc96/
--rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.618535 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x88d/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x88d/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.619143 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/
--rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.619846 ANX-0.7.2/AndroidQQ/im/oidb/cmd0xeb8/
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.620833 ANX-0.7.2/AndroidQQ/im/oidb/oidb_0xc05/
--rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.621967 ANX-0.7.2/AndroidQQ/im/oidb/oidb_sso/
--rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/oidb_sso/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.622783 ANX-0.7.2/AndroidQQ/im/oidb/qqconnect/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/qqconnect/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.623606 ANX-0.7.2/AndroidQQ/im/oidb/scanlogin/
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/scanlogin/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.624006 ANX-0.7.2/AndroidQQ/log/
--rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/log/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.628888 ANX-0.7.2/AndroidQQ/pack/
--rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/Heartbeat_Alive.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
--rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
--rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/OidbSvc_0x88d_1.py
--rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xc05.py
--rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xc96.py
--rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xeb8.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.630761 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/
--rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/delUgc.py
--rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/like.py
--rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/publishmood.py
--rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
--rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/StatSvc_register.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.631227 ANX-0.7.2/AndroidQQ/pack/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.2/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/friendlist.py
--rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.2/AndroidQQ/pack/test.py
--rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.632287 ANX-0.7.2/AndroidQQ/proto/
--rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.2/AndroidQQ/proto/IM_r_pb2.py
--rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/proto/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.2/AndroidQQ/proto/wtlogin_pb2.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.635894 ANX-0.7.2/AndroidQQ/struct/
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.637709 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/
--rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
--rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/MessageSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.638616 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_COMM/
--rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.643225 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/
--rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
--rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
--rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
--rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
--rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
--rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
--rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
--rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.646821 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/
--rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
--rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
--rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
--rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
--rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
--rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
--rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/OidbSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.651380 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/
--rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
--rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
--rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
--rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
--rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.652252 ANX-0.7.2/AndroidQQ/struct/QQService/
--rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
--rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/QQService/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/StatSvc.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.653416 ANX-0.7.2/AndroidQQ/struct/SummaryCard/
--rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
--rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
--rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/SummaryCard/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.2/AndroidQQ/struct/Tlv.py
--rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/Tlv_res.py
--rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.653783 ANX-0.7.2/AndroidQQ/struct/cooperation/
--rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/cooperation/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.654802 ANX-0.7.2/AndroidQQ/struct/cooperation/qzone/
--rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/cooperation/qzone/WNSStream.py
--rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/cooperation/qzone/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.655297 ANX-0.7.2/AndroidQQ/struct/feedcomponent/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/feedcomponent/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/feedcomponent/model.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.655874 ANX-0.7.2/AndroidQQ/struct/friendlist/
--rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/friendlist/AddFriendReq.py
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/friendlist/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.2/AndroidQQ/struct/head.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.656570 ANX-0.7.2/AndroidQQ/struct/push/
--rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/push/SvcReqRegister.py
--rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/push/SvcRespRegister.py
--rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/struct/push/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.2/AndroidQQ/struct/wtlogin.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.657978 ANX-0.7.2/AndroidQQ/utils/
--rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/utils/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/utils/build_device.py
--rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/utils/ecdh.py
--rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/utils/sso_server.py
--rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/utils/tool.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.658228 ANX-0.7.2/AndroidQQ/wlogin_sdk/
--rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/wlogin_sdk/__init__.py
-drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-02 03:01:02.658672 ANX-0.7.2/AndroidQQ/wlogin_sdk/request/
--rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.2/AndroidQQ/wlogin_sdk/request/__init__.py
--rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-02 03:01:02.659021 ANX-0.7.2/PKG-INFO
--rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.2/README.md
--rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-02 03:01:02.659361 ANX-0.7.2/setup.cfg
--rw-r--r--   0 1a         (501) staff       (20)      573 2024-04-02 03:00:48.000000 ANX-0.7.2/setup.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366819 ANX-0.7.3/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.336644 ANX-0.7.3/ANX.egg-info/
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)     4882 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/SOURCES.txt
+-rw-r--r--   0 1a         (501) staff       (20)        1 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/dependency_links.txt
+-rw-r--r--   0 1a         (501) staff       (20)      108 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/requires.txt
+-rw-r--r--   0 1a         (501) staff       (20)       10 2024-04-08 11:35:14.000000 ANX-0.7.3/ANX.egg-info/top_level.txt
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.337351 ANX-0.7.3/AndroidQQ/
+-rw-r--r--   0 1a         (501) staff       (20)    34763 2024-04-08 06:20:56.000000 ANX-0.7.3/AndroidQQ/Android.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.337700 ANX-0.7.3/AndroidQQ/Echo/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/Echo/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/Echo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3878 2024-04-07 22:37:06.000000 ANX-0.7.3/AndroidQQ/Tcp.py
+-rw-r--r--   0 1a         (501) staff       (20)       71 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339696 ANX-0.7.3/AndroidQQ/http/
+-rw-r--r--   0 1a         (501) staff       (20)     2195 2024-04-08 06:23:23.000000 ANX-0.7.3/AndroidQQ/http/ClientKey.py
+-rw-r--r--   0 1a         (501) staff       (20)      138 2024-04-08 05:21:16.000000 ANX-0.7.3/AndroidQQ/http/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2009 2024-04-08 05:37:11.000000 ANX-0.7.3/AndroidQQ/http/accounts.py
+-rw-r--r--   0 1a         (501) staff       (20)      820 2024-04-08 05:31:10.000000 ANX-0.7.3/AndroidQQ/http/cip.py
+-rw-r--r--   0 1a         (501) staff       (20)     4061 2024-04-08 05:46:08.000000 ANX-0.7.3/AndroidQQ/http/friends.py
+-rw-r--r--   0 1a         (501) staff       (20)     4697 2024-04-08 05:55:05.000000 ANX-0.7.3/AndroidQQ/http/game_credit.py
+-rw-r--r--   0 1a         (501) staff       (20)      422 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/http/headers.py
+-rw-r--r--   0 1a         (501) staff       (20)     7243 2024-04-08 05:40:22.000000 ANX-0.7.3/AndroidQQ/http/level.py
+-rw-r--r--   0 1a         (501) staff       (20)    10305 2024-04-08 05:54:43.000000 ANX-0.7.3/AndroidQQ/http/music.py
+-rw-r--r--   0 1a         (501) staff       (20)     1499 2024-04-08 05:42:12.000000 ANX-0.7.3/AndroidQQ/http/qqsignin.py
+-rw-r--r--   0 1a         (501) staff       (20)     1325 2024-04-08 05:50:32.000000 ANX-0.7.3/AndroidQQ/http/weishi.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339828 ANX-0.7.3/AndroidQQ/im/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.339914 ANX-0.7.3/AndroidQQ/im/oidb/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.340159 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/
+-rw-r--r--   0 1a         (501) staff       (20)     2797 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       34 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.341126 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2139 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.341549 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/
+-rw-r--r--   0 1a         (501) staff       (20)     1343 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1542 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342045 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342511 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/
+-rw-r--r--   0 1a         (501) staff       (20)       30 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2603 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.342963 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/
+-rw-r--r--   0 1a         (501) staff       (20)       27 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1468 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.343402 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     2618 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.344059 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1385 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.344385 ANX-0.7.3/AndroidQQ/log/
+-rw-r--r--   0 1a         (501) staff       (20)       33 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/log/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.347595 ANX-0.7.3/AndroidQQ/pack/
+-rw-r--r--   0 1a         (501) staff       (20)      395 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/Heartbeat_Alive.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py
+-rw-r--r--   0 1a         (501) staff       (20)      733 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py
+-rw-r--r--   0 1a         (501) staff       (20)     1368 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0x88d_1.py
+-rw-r--r--   0 1a         (501) staff       (20)      986 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc05.py
+-rw-r--r--   0 1a         (501) staff       (20)     1141 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc96.py
+-rw-r--r--   0 1a         (501) staff       (20)      872 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xeb8.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.348992 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/
+-rw-r--r--   0 1a         (501) staff       (20)       94 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1124 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/delUgc.py
+-rw-r--r--   0 1a         (501) staff       (20)     2637 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/like.py
+-rw-r--r--   0 1a         (501) staff       (20)     2631 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/publishmood.py
+-rw-r--r--   0 1a         (501) staff       (20)     2152 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1116 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/StatSvc_register.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.349367 ANX-0.7.3/AndroidQQ/pack/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     1349 2024-03-07 10:14:41.000000 ANX-0.7.3/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)       29 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      402 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1383 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/friendlist.py
+-rw-r--r--   0 1a         (501) staff       (20)      543 2024-03-06 13:46:02.000000 ANX-0.7.3/AndroidQQ/pack/test.py
+-rw-r--r--   0 1a         (501) staff       (20)    46467 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.349963 ANX-0.7.3/AndroidQQ/proto/
+-rw-r--r--   0 1a         (501) staff       (20)     4301 2024-02-12 04:07:38.000000 ANX-0.7.3/AndroidQQ/proto/IM_r_pb2.py
+-rw-r--r--   0 1a         (501) staff       (20)       67 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/proto/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1308 2023-10-29 17:25:21.000000 ANX-0.7.3/AndroidQQ/proto/wtlogin_pb2.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.352025 ANX-0.7.3/AndroidQQ/struct/
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.352940 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/
+-rw-r--r--   0 1a         (501) staff       (20)      444 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/DestQQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1061 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      853 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py
+-rw-r--r--   0 1a         (501) staff       (20)     1028 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      894 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/MessageSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.353500 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/
+-rw-r--r--   0 1a         (501) staff       (20)      373 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/UgcRightInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       28 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_COMM/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.356959 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/
+-rw-r--r--   0 1a         (501) staff       (20)       70 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     3064 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py
+-rw-r--r--   0 1a         (501) staff       (20)     1565 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py
+-rw-r--r--   0 1a         (501) staff       (20)      565 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      895 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1789 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      451 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_arkshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      673 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py
+-rw-r--r--   0 1a         (501) staff       (20)      728 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py
+-rw-r--r--   0 1a         (501) staff       (20)      249 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_user.py
+-rw-r--r--   0 1a         (501) staff       (20)     1163 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.359140 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/
+-rw-r--r--   0 1a         (501) staff       (20)      479 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/Source.py
+-rw-r--r--   0 1a         (501) staff       (20)      187 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      656 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py
+-rw-r--r--   0 1a         (501) staff       (20)     1161 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py
+-rw-r--r--   0 1a         (501) staff       (20)     1300 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      560 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)     3031 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py
+-rw-r--r--   0 1a         (501) staff       (20)      503 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_rsp.py
+-rw-r--r--   0 1a         (501) staff       (20)      594 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/OidbSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.361811 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/
+-rw-r--r--   0 1a         (501) staff       (20)      504 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfBusiControl.py
+-rw-r--r--   0 1a         (501) staff       (20)      630 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      714 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      526 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)     1180 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py
+-rw-r--r--   0 1a         (501) staff       (20)      489 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/RetryInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       87 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.362100 ANX-0.7.3/AndroidQQ/struct/QQService/
+-rw-r--r--   0 1a         (501) staff       (20)     1112 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)      878 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/QQService/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1115 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/StatSvc.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.362754 ANX-0.7.3/AndroidQQ/struct/SummaryCard/
+-rw-r--r--   0 1a         (501) staff       (20)     2861 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py
+-rw-r--r--   0 1a         (501) staff       (20)      493 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/UserLocaleInfo.py
+-rw-r--r--   0 1a         (501) staff       (20)       61 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/SummaryCard/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    15568 2024-03-05 18:40:23.000000 ANX-0.7.3/AndroidQQ/struct/Tlv.py
+-rw-r--r--   0 1a         (501) staff       (20)     4784 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/Tlv_res.py
+-rw-r--r--   0 1a         (501) staff       (20)      131 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.363479 ANX-0.7.3/AndroidQQ/struct/cooperation/
+-rw-r--r--   0 1a         (501) staff       (20)       23 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.363964 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/
+-rw-r--r--   0 1a         (501) staff       (20)     4558 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/WNSStream.py
+-rw-r--r--   0 1a         (501) staff       (20)       26 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.364217 ANX-0.7.3/AndroidQQ/struct/feedcomponent/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/feedcomponent/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     1482 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/feedcomponent/model.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.364605 ANX-0.7.3/AndroidQQ/struct/friendlist/
+-rw-r--r--   0 1a         (501) staff       (20)     2842 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/friendlist/AddFriendReq.py
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/friendlist/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)     7428 2024-03-07 10:14:48.000000 ANX-0.7.3/AndroidQQ/struct/head.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.365079 ANX-0.7.3/AndroidQQ/struct/push/
+-rw-r--r--   0 1a         (501) staff       (20)     3536 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/SvcReqRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)     2084 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/SvcRespRegister.py
+-rw-r--r--   0 1a         (501) staff       (20)       31 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/struct/push/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)    27313 2024-03-05 18:40:23.000000 ANX-0.7.3/AndroidQQ/struct/wtlogin.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.365872 ANX-0.7.3/AndroidQQ/utils/
+-rw-r--r--   0 1a         (501) staff       (20)       20 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      523 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/build_device.py
+-rw-r--r--   0 1a         (501) staff       (20)     1140 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/ecdh.py
+-rw-r--r--   0 1a         (501) staff       (20)     1379 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/sso_server.py
+-rw-r--r--   0 1a         (501) staff       (20)      735 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/utils/tool.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366014 ANX-0.7.3/AndroidQQ/wlogin_sdk/
+-rw-r--r--   0 1a         (501) staff       (20)       25 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/wlogin_sdk/__init__.py
+drwxr-xr-x   0 1a         (501) staff       (20)        0 2024-04-08 11:35:14.366275 ANX-0.7.3/AndroidQQ/wlogin_sdk/request/
+-rw-r--r--   0 1a         (501) staff       (20)        0 2024-02-12 04:39:43.000000 ANX-0.7.3/AndroidQQ/wlogin_sdk/request/__init__.py
+-rw-r--r--   0 1a         (501) staff       (20)      125 2024-04-08 11:35:14.366469 ANX-0.7.3/PKG-INFO
+-rw-r--r--   0 1a         (501) staff       (20)       34 2023-08-04 12:41:32.000000 ANX-0.7.3/README.md
+-rw-r--r--   0 1a         (501) staff       (20)       38 2024-04-08 11:35:14.366889 ANX-0.7.3/setup.cfg
+-rw-r--r--   0 1a         (501) staff       (20)      601 2024-04-08 11:35:10.000000 ANX-0.7.3/setup.py
```

### Comparing `ANX-0.7.2/ANX.egg-info/SOURCES.txt` & `ANX-0.7.3/ANX.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 AndroidQQ/Tcp.py
 AndroidQQ/__init__.py
 AndroidQQ/Echo/Tcp.py
 AndroidQQ/Echo/__init__.py
 AndroidQQ/http/ClientKey.py
 AndroidQQ/http/__init__.py
 AndroidQQ/http/accounts.py
+AndroidQQ/http/cip.py
 AndroidQQ/http/friends.py
 AndroidQQ/http/game_credit.py
 AndroidQQ/http/headers.py
 AndroidQQ/http/level.py
 AndroidQQ/http/music.py
 AndroidQQ/http/qqsignin.py
 AndroidQQ/http/weishi.py
```

### Comparing `ANX-0.7.2/AndroidQQ/Android.py` & `ANX-0.7.3/AndroidQQ/Android.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 import AndroidQQ.struct.OidbSvc as OidbSvc
 import AndroidQQ.struct.StatSvc as StatSvc
 import AndroidQQ.pack.friendlist as friendlist
 import AndroidQQ.struct.wtlogin as wt_login
 from AndroidQQ.Tcp import start_client, disconnect_client
 from AndroidQQ.http import qq_level_index, WriteMindJar, change_psw_getsms, Friends, bot_uin, delete_qq_friend, \
-    GetLevelStatus, GetLevelTask, RefreshTask, credit_score
+    GetLevelStatus, GetLevelTask, RefreshTask, credit_score, GetHttpIp
 from AndroidQQ.http.music import Music
 from AndroidQQ.http.weishi import weishi_up_
 from AndroidQQ.pack import *
 from AndroidQQ.pack.MQUpdateSvc_com_qq_ti_web_scanlogin import *
 from AndroidQQ.pack.SQQzoneSvc import SQQzoneSvc_shuoshuo, SQQzoneSvc_shuoshuo_rsp, SQQzoneSvc_publishmood, \
     SQQzoneSvc_publishmood_rsp, SQQzoneSvc_delUgc, SQQzoneSvc_delUgc_rsp
 from AndroidQQ.pack.SummaryCard import SummaryCard_ReqSummaryCard, SummaryCard_ReqSummaryCard_rsp
@@ -101,28 +101,48 @@
     Guid: bytes = get_random_bin(16)
     login_time: int = int(time.time())
     UN_Tlv_list: UN_Tlv_list = UN_Tlv_list()
     device: device = device()
     cookies: cookies = cookies()
     Tips: str = None
     proxy_str: str = None
+    proxy_proxies: dict = None
     emp_time: str = None
 
 
 class AndroidQQ:
     def __init__(self, **kwargs):
         """
         :param client_type: QQ or Watch
         :param kwargs:
         """
-        self.proxy = kwargs.get('proxy', [])  # 元组[121.236.248.165,40033]
 
         self.info = info_model()
+        self.proxy = kwargs.get('proxy', [])  # 元组[121.236.248.165,40033]
         if self.proxy:
-            self.info.proxy_str = f'{self.proxy[0]}:{self.proxy[1]}'
+            proxy_host = self.proxy[0]
+            proxy_port = self.proxy[1]
+            # 检查是否提供了用户名和密码
+            proxy_user = self.proxy[2] if len(self.proxy) > 2 else None
+            proxy_pass = self.proxy[3] if len(self.proxy) > 3 else None
+
+            # 如果有用户名和密码，则在代理字符串中包含这些认证信息
+            if proxy_user and proxy_pass:
+                proxy_str = f'{proxy_user}:{proxy_pass}@{proxy_host}:{proxy_port}'
+            else:
+                proxy_str = f'{proxy_host}:{proxy_port}'
+
+            self.info.proxy_str = proxy_str
+            self.info.proxy_proxies = {
+                'http': f'socks5h://{proxy_str}',
+                'https': f'socks5h://{proxy_str}'
+            }
+        else:
+            self.info.proxy_str = None
+            self.info.proxy_proxies = None
 
         # self.info.device.Bssid_bytes = bytes.fromhex(get_md5('00:14:bf:3a:8a:50'.encode()))
         client_type = kwargs.setdefault('client_type', 'QQ')
         self.info.device.Imei = '862542082770767'
         self.info.device.Mac = '89:C2:A9:C5:FA:E9'
         self.info.device.Bssid = '00:14:bf:3a:8a:50'
 
@@ -723,15 +743,15 @@
         return qq_bkn(self.info.cookies.skey)
 
     def get_qq_level(self):
         """
         获取qq等级
         :return .get('levelInfo')
         """
-        return qq_level_index(self.get_cookie("ti.qq.com"))
+        return qq_level_index(self.info, self.get_cookie("ti.qq.com"))
 
     def get_lv_task_status(self, query: bool = False):
         """获取等级任务状态"""
         return GetLevelStatus(self.info, self.get_cookie("ti.qq.com"), query)
 
     def get_lv_task(self):
         """获取等级任务"""
@@ -739,21 +759,21 @@
 
     def refresh_task(self, task_id: str):
         """刷新任务状态"""
         return RefreshTask(self.info, self.get_cookie("ti.qq.com"), task_id)
 
     def sign_in(self):
         """签到"""
-        return WriteMindJar(self.get_cookie("ti.qq.com"), self.info.cookies.skey, self.info.proxy_str)
+        return WriteMindJar(self.info, self.get_cookie("ti.qq.com"), self.info.cookies.skey)
 
     def change_psw_getsms(self, mobile):
         """修改密码，获取验证码
         :param mobile: 手机号
         """
-        return change_psw_getsms(self.info.uin, self.get_cookie("accounts.qq.com"), mobile)
+        return change_psw_getsms(self.info, self.get_cookie("accounts.qq.com"), mobile)
 
     def weishi_up(self):
         """微视任务"""
         return weishi_up_(self.info)
 
     def Music_task(self):
         """音乐"""
@@ -782,15 +802,15 @@
 
         return self.tcp_task(req_func, rsp_func)
 
     def lv_Friend(self):
         """加好友任务"""
         selected = random.sample(bot_uin, 3)
         try:
-            Friend = Friends(self.get_bkn(), self.info.uin, self.get_cookie('qun.qq.com'))
+            Friend = Friends(self.info, self.get_bkn(), self.info.uin, self.get_cookie('qun.qq.com'))
             success = 0
             for f_uin in selected:
                 rsp = Friend.del_friend(f_uin)
                 if not rsp.status:
                     continue
                 rsp = Friend.add_friend(f_uin)
                 if not rsp.status:
@@ -802,15 +822,15 @@
                        finishedAccelerateDays=finished_accelerate_days)
 
         except Exception as e:
             return Box(status=False, message=f'好友活跃任务异常{e}')
 
         finally:
             for f_uin in selected:
-                delete_qq_friend(self.info.uin, f_uin, self.get_bkn(), self.get_cookie('qzone.qq.com'))
+                delete_qq_friend(self.info, self.info.uin, f_uin, self.get_bkn(), self.get_cookie('qzone.qq.com'))
 
     def lv_cm_show(self):
         """"厘米秀装扮"""
         try:
             self.qq_show_replace('女性_兔兔发箍')
             self.qq_show_replace('女性带眼镜')
             task = self.refresh_task('27').get('response', {}).get('task', {})
@@ -845,15 +865,15 @@
 
         except Exception as e:
             return Box(status=False, message=f'音乐任务异常{e}')
 
     def lv_Qzone(self):
         """空间任务"""
         try:
-            rsp = self.Qzone_publishmood('偶尔的停顿和修整，对于人生是非常必要的。')['response']
+            rsp = self.Qzone_publishmood('当遇到你时，大脑连上CSGO都会掉帧。')['response']
             tid = rsp.get('Busi', {}).get('tid', '')
             self.get_qq_level()
             self.Qzone_delUgc(tid)
             task = self.refresh_task('2').get('response', {}).get('task', {})
             if not task:
                 return Box(status=False, message='刷新任务异常')
             button_text = task.get('button_text')
@@ -883,15 +903,16 @@
     def lv_extra_task_up(self, lv_music=True):
         """升级所有额外任务"""
         rsp = self.exchange_emp()
         if rsp['status'] != 0:
             return Box(status=False, message='emp' + rsp['message'])
 
         rsp = self.no_tail_login()
-        if rsp['status'] != 0:
+        status = rsp['status']
+        if status != 0:
             return Box(status=False, message=rsp['message'])
 
         task_functions = {
             '连续登录QQ': self.lv_continuous_login,
             '发布一条空间说说': self.lv_Qzone,
             '去日签卡打一次卡': self.lv_clock_in,
             '去QQ音乐听歌30分钟+0.5天': self.lv_music,
@@ -918,10 +939,14 @@
         if execute_task:
             task_status = self.get_lv_task_status(True)
 
         done_count = task_status.get('done_count', None)
         logger.info(f'{self.info.uin}已完成任务数量{done_count}')
         return Box(status=True, level=level, done_count=done_count, task_status=task_status)
 
+    def get_http_ip(self):
+        """获取http代理"""
+        return GetHttpIp(self.info)
+
     def get_credit(self):
         """获取信用分"""
-        return Box(credit_score(self.info.uin, self.info.cookies.client_key).query_common_credit())
+        return Box(credit_score(self.info, self.info.cookies.client_key).query_common_credit())
```

### Comparing `ANX-0.7.2/AndroidQQ/Tcp.py` & `ANX-0.7.3/AndroidQQ/Tcp.py`

 * *Files 3% similar despite different names*

```diff
@@ -83,36 +83,34 @@
             #     disconnect_client(client, clients, client_info)
             #     log.info('断开连接')
             # else:
             #     # log.info(f"从客户端收到的数据: {data.hex()}")
             #     repackage(data, client)
 
 
-def start_client(_func=None, proxy=list):
+def start_client(_func=None, proxy=None):
     if proxy is None:
         proxy = []
     if ip_list:
         random_item = random.choice(ip_list)
         host = random_item['1']
         port = random_item['2']
     else:
         # 没初始化ip列表前用这个快速连接
         host = '36.155.245.16'
         port = 8080
+    client = socks.socksocket()
 
     if len(proxy) >= 2:
         # 对于需要设置代理的客户端，创建一个配置了代理的socket对象
+
         if len(proxy) == 2:
-            socks.set_default_proxy(socks.SOCKS5, proxy[0], proxy[1])
+            client.set_proxy(socks.SOCKS5, proxy[0], proxy[1])
         else:
-            socks.set_default_proxy(socks.SOCKS5, proxy[0], int(proxy[1]), username=proxy[2], password=proxy[3])
-        client = socks.socksocket()
-    else:
-        # 不需要代理的客户端，使用普通的socket对象
-        client = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
+            client.set_proxy(socks.SOCKS5, proxy[0], int(proxy[1]), username=proxy[2], password=proxy[3])
 
     try:
         client.connect((host, port))
     except socket.error as e:
         log.info(f"连接到 {host}:{port} 失败，错误信息: {e}")
         return None
```

### Comparing `ANX-0.7.2/AndroidQQ/http/ClientKey.py` & `ANX-0.7.3/AndroidQQ/http/ClientKey.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import time
 
 import requests
 
 
-def ClientKeyToCookies(uin, client_key):
+def ClientKeyToCookies(info, uin, client_key):
     try:
         response = requests.get(url="https://ssl.ptlogin2.qq.com/jump",
                                 params={
                                     "keyindex": "19",
                                     "clientuin": uin,
                                     "clientkey": client_key,
                                     "u1": "https://connect.qq.com",
@@ -17,17 +17,20 @@
                                     "style": "35",
                                     "pt_ua": "60C3D6175A88C661094CF87DC58D1C55",
                                     "pt_browser": "others",
                                     "pt_3rd_aid": "1101083114",
                                     "pt_openlogin_data": f"appid=716027609&pt_3rd_aid=1101083114&daid=383&pt_skey_valid=0&style=35&s_url=https%3A%2F%2Fconnect.qq.com&refer_cgi=authorize&which=&sdkp=pcweb&sdkv=v1.0&time={str(int(time.time()))}&loginty=3&h5sig=OnX6dkcSfE3T5i4O7UxIp2gnmDJnviaXNxQcfA9X1Xg&response_type=code&client_id=1101083114&redirect_uri=https%3A%2F%2Fh5.weishi.qq.com%2Fweishi%2Faccount%2Flogin%3Fr_url%3Dhttp%253A%252F%252Fmedia.weishi.qq.com%252F%26loginfrom%3Dqc%26retry%3D1&state=state&pt_flex=1&loginfrom=&h5sig=OnX6dkcSfE3T5i4O7UxIp2gnmDJnviaXNxQcfA9X1Xg&loginty=3&",
                                 }
                                 ,
-                                allow_redirects=False)
+                                allow_redirects=False,
+                                proxies=info.proxy_proxies
+                                )
         Location = response.headers['Location']
         if Location is None:
             return {'status': False, 'message': '没找到Location'}
-        response = requests.get(url=Location, allow_redirects=False)
+        response = requests.get(url=Location, allow_redirects=False, proxies=info.proxy_proxies
+                                )
         cookie_str = '; '.join([f'{c.name}={c.value}' for c in response.cookies])
 
         return {'status': True, 'cookie': cookie_str}
     except Exception as e:
-        return {'status': False, 'message': f'获取cookie异常:{e}'}
+        return {'status': False, 'message': f'ClientKeyToCookies获取cookie异常:{e}'}
```

### Comparing `ANX-0.7.2/AndroidQQ/http/accounts.py` & `ANX-0.7.3/AndroidQQ/http/accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 import requests
 
 from AndroidQQ.http import User_Agent
 from AndroidQQ.utils import qq_bkn
 
 
-def change_psw_getsms(Uin, Cookie: str, mobile: str):
+def change_psw_getsms(info, Cookie: str, mobile: str):
     match = re.search(r'skey=([^;]+)', Cookie)
     if match:
         skey = match.group(1)
     else:
         skey = None
 
     try:
@@ -32,29 +32,32 @@
                 "User-Agent": User_Agent,
                 "Content-Type": "application/json",
                 "Origin": 'https://accounts.qq.com',
                 "X-Requested-With": "com.tencent.mobileqq",
                 "Sec-Fetch-Site": "same-origin",
                 "Sec-Fetch-Mode": "cors",
                 "Sec-Fetch-Dest": "empty",
-                "Referer": "https://accounts.qq.com/cn2/change_psw/mobile/mobile_change_psw_way?source_id=3259&uin=" + Uin,
+                "Referer": "https://accounts.qq.com/cn2/change_psw/mobile/mobile_change_psw_way?source_id=3259&uin=" + info.uin,
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": Cookie,
+
             },
             data=json.dumps({
                 "com": {
                     "version": "8.9.83",
                     "scene": 304,
                     "src": 1,
                     "platform": 2
                 },
                 "areaCode": "+86",
                 "way": 3,
                 "mobile": mobile
-            })
+            }),
+            proxies=info.proxy_proxies
+
         )
 
         return response.json()
     except requests.exceptions.RequestException:
         print('发送短信失败')
         return {}
```

### Comparing `ANX-0.7.2/AndroidQQ/http/friends.py` & `ANX-0.7.3/AndroidQQ/http/friends.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from AndroidQQ.http import User_Agent
 
 bot_uin = [66600000, 2854196306, 2854213893, 2854211892, 2854204259]
 
 
 # 66600000 2854196306 2854213893 2854211892 2854204259
 
-def delete_qq_friend(uin, fuin, bkn, cookie):
+def delete_qq_friend(info, uin, fuin, bkn, cookie):
     """空间包删除好友"""
 
     try:
         rsp = requests.post(
             url='https://h5.qzone.qq.com/proxy/domain/w.qzone.qq.com/cgi-bin/tfriend/friend_delete_qqfriend.cgi?g_tk=' + bkn,
             data={
                 'uin': uin,
@@ -25,25 +25,27 @@
                 'qzreferrer': f'http://user.qzone.qq.com/{uin}/myhome/friends'
             },
             headers={
                 "User-Agent": User_Agent,
                 "Content-Type": "application/x-www-form-urlencoded",
                 "Origin": "https://h5.qzone.qq.com",
                 "Referer": "https://h5.qzone.qq.com/",
-                'Cookie': cookie
+                'Cookie': cookie,
 
-            }
+            },
+            proxies=info.proxy_proxies
         )
         return Box(status=True, message=f'空间请求删除好友', echo=rsp.json())
     except Exception as e:
         return Box(status=False, message=f'空间删除好友异常{e}')
 
 
 class Friends:
-    def __init__(self, bkn, uin, cookie):
+    def __init__(self, info, bkn, uin, cookie):
+        self.info = info
         self.bkn = bkn
         self.uin = uin
         self.cookie = cookie
         pass
 
     def add_friend(self, robot_uin):
         try:
@@ -55,36 +57,41 @@
                                 headers={
                                     "User-Agent": User_Agent,
                                     "Content-Type": "application/x-www-form-urlencoded",
                                     "Origin": "https://web.qun.qq.com",
                                     "X-Requested-With": "com.tencent.mobileqq",
                                     "Referer": "https://web.qun.qq.com/",
                                     "Cookie": self.cookie
-                                })
+                                },
+                                proxies=self.info.proxy_proxies
+                                )
 
             return Box(status=True, message=f'已请求添加好友', echo=rsp.json())
 
         except Exception as e:
             return Box(status=False, message=f'添加好友异常{e}')
 
     def del_friend(self, robot_uin):
+        """删除好友"""
         try:
             rsp = requests.post(url='https://qun.qq.com/cgi-bin/qunapp/robots_removefriend?bkn=' + self.bkn,
                                 data={
                                     'robot_uin': robot_uin,
                                     'bkn': self.bkn
                                 },
                                 headers={
                                     "User-Agent": User_Agent,
                                     "Content-Type": "application/x-www-form-urlencoded",
                                     "Origin": "https://web.qun.qq.com",
                                     "X-Requested-With": "com.tencent.mobileqq",
                                     "Referer": "https://web.qun.qq.com/",
                                     "Cookie": self.cookie
-                                })
+                                },
+                                proxies=self.info.proxy_proxies
+                                )
 
             return Box(status=True, message=f'已申请删除好友', echo=rsp.json())
 
         except Exception as e:
             return Box(status=False, message=f'删除好友异常{e}')
```

### Comparing `ANX-0.7.2/AndroidQQ/http/level.py` & `ANX-0.7.3/AndroidQQ/http/level.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from bs4 import BeautifulSoup
 
 from AndroidQQ import log
 
 from .headers import *
 
 
-def qq_level_index(cookie: str):
+def qq_level_index(info, cookie: str):
     """获取QQ等级的具体信息 多了需要代理"""
     try:
         response = requests.get(
             url="https://ti.qq.com/qqlevel/index",
             params={
                 "_wv": "3",
                 "_wwv": "1",
@@ -33,14 +33,15 @@
                 "Sec-Fetch-Mode": "navigate",
                 "Sec-Fetch-User": "?1",
                 "Sec-Fetch-Dest": "document",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": cookie,
             },
+            proxies=info.proxy_proxies
         )
         soup = BeautifulSoup(response.content, 'html.parser')
         scripts = soup.find_all('script')
         data_string = None
         for script in scripts:
             if script.string and '__INITIAL_STATE__' in script.string:
                 data_string = script.string
@@ -55,14 +56,15 @@
     except requests.exceptions.RequestException:
         log.error('HTTP 请求失败')
         return {}
 
 
 def GetLevelTask(info, cookie):
     """获取任务,具有更新效果"""
+
     try:
         rsp = requests.post(
 
             url="https://ti.qq.com/qqlevel/trpc/levelTask/Get",
             params={
                 "bkn": qq_bkn(info.cookies.skey),
             },
@@ -83,14 +85,15 @@
                 "Sec-Fetch-Mode": "navigate",
                 "Sec-Fetch-User": "?1",
                 "Sec-Fetch-Dest": "document",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": cookie,
             },
+            proxies=info.proxy_proxies
         )
         return rsp.json()
     except Exception as e:
         log.error(f'获取等级任务列表失败{e}')
         return {}
 
 
@@ -120,14 +123,16 @@
                 "Sec-Fetch-Mode": "navigate",
                 "Sec-Fetch-User": "?1",
                 "Sec-Fetch-Dest": "document",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": cookie,
             },
+            proxies=info.proxy_proxies
+
         )
         return rsp.json()
     except Exception as e:
         log.error(f'刷新任务失败{e}')
         return {}
 
 
@@ -188,14 +193,16 @@
                 "Sec-Fetch-Mode": "navigate",
                 "Sec-Fetch-User": "?1",
                 "Sec-Fetch-Dest": "document",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": cookie,
             },
+            proxies=info.proxy_proxies
+
         )
         return format_conversion(rsp.json()) if query else rsp.json().get('response', {})
     except Exception as e:
         log.error(f'获取等级任务列表失败{e}')
         return {}
```

### Comparing `ANX-0.7.2/AndroidQQ/http/music.py` & `ANX-0.7.3/AndroidQQ/http/music.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,14 +51,15 @@
         self.qm_keyst = None
         self.cookies = None
         self.uin = info.uin
         self.client_key = info.cookies.client_key
         self.code = None
         self.g_tk = None
         self.psrf_qqopenid = None
+        self.info = info
 
     def get_Location_code(self):
         if not self.client_key:
             return {'status': False, 'message': '没有获取到clientkey'}
         try:
             response = requests.get(url="https://ssl.ptlogin2.qq.com/jump",
                                     params={
@@ -72,15 +73,16 @@
                                         "style": "35",
                                         "pt_ua": "76BA0A6746DFE83A98D8D2F11E2D88FF",
                                         "pt_browser": "others",
                                         "pt_3rd_aid": "100497308",
                                         'pt_openlogin_data': f'appid=716027609&pt_3rd_aid=100497308&daid=383&pt_skey_valid=1&style=35&s_url=https%3A%2F%2Fconnect.qq.com&refer_cgi=authorize&which=&sdkp=pcweb&sdkv=v1.0&time={str(int(time.time()))}&loginty=3&h5sig=eGKHXAcp1AAAlR38DBo6E_oj3OrsS53GtW1_bmkcOzY&response_type=code&client_id=100497308&redirect_uri=https%3A%2F%2Fy.qq.com%2Fm%2Flogin%2Fredirect.html%3Fis_qq_connect%3D1%26login_type%3D1%26surl%3Dhttps%253A%252F%252Fi.y.qq.com%252Fn2%252Fm%252Fclient%252Factcenter%252Findex.html%253Ffrom_tag%253Dqq%2526openid%253D&state=state&display=mobile&scope=get_user_info%2Cget_app_friends&pt_flex=1&loginfrom=&h5sig=eGKHXAcp1AAAlR38DBo6E_oj3OrsS53GtW1_bmkcOzY&loginty=3&'
                                     }
                                     ,
-                                    allow_redirects=False)
+                                    allow_redirects=False,
+                                    proxies=self.info.proxy_proxies)
             Location = response.headers['Location']
             if Location is None:
                 return {'status': False, 'message': '没找到Location'}
             parsed_url = urlparse(Location)
             query_params = parse_qs(parsed_url.query)
             self.code = query_params.get('code')[0]
             if self.code is None:
@@ -100,15 +102,16 @@
                 }
             }
             post_json = json.dumps(post_data)
 
             rsp = requests.post(
                 url='https://u.y.qq.com/cgi-bin/musicu.fcg',
                 data=post_json,
-                allow_redirects=False
+                allow_redirects=False,
+                proxies=self.info.proxy_proxies
             )
 
             self.cookies = '; '.join([f'{c.name}={c.value}' for c in rsp.cookies])
             self.qm_keyst = re.search(r'qm_keyst=([^;]+)', self.cookies).group(1)
             self.g_tk = qq_bkn(self.qm_keyst)
             self.psrf_qqopenid = rsp.cookies.get('psrf_qqopenid')
             return {'status': True}
@@ -161,15 +164,18 @@
                     "Cookie": self.cookies,
                     "Content-Type": "application/json"
                 }
 
                 response = requests.request("POST", url,
                                             params=querystring,
                                             data=data,
-                                            headers=headers)
+                                            headers=headers,
+                                            proxies=self.info.proxy_proxies
+
+                                            )
 
                 code = response.json()['code']
                 if code != 0:
                     return {'status': False, 'code': code, 'message': '获取任务失败'}
                 return {'status': True, 'code': code, 'message': '获取任务失败'}
 
 
@@ -191,15 +197,17 @@
 
                 response = requests.post(
                     url='https://stat.y.qq.com/android/fcgi-bin/imusic_tj',
                     headers={
                         'User-Agent': 'QQMusic 9020807(android 9)',
                         'Content-Encoding': 'gzip',
                     },
-                    data=compressed_xml
+                    data=compressed_xml,
+                    proxies=self.info.proxy_proxies
+
                 )
                 if response.status_code == 200:
                     body = response.content
                     if body and body[-1] == 0xD7:
                         succNum += 1
                 if succNum >= 3:
                     break
```

### Comparing `ANX-0.7.2/AndroidQQ/http/qqsignin.py` & `ANX-0.7.3/AndroidQQ/http/qqsignin.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,16 @@
 import requests
 import json
 
 from AndroidQQ.http import User_Agent
 from AndroidQQ.utils import qq_bkn
 
 
-def WriteMindJar(cookie: str, skey: str, proxy=None):
+def WriteMindJar(info, cookie: str, skey: str):
     """心灵罐子签到"""
-    proxies = {
-        'https': proxy
-    }
     try:
         response = requests.post(
             url="https://ti.qq.com/qqsignin/mindjar/trpc/WriteMindJar",
             params={
                 "bkn": qq_bkn(skey),
             },
             headers={
@@ -29,15 +26,15 @@
                 "Sec-Fetch-Dest": "empty",
                 "Referer": "https://ti.qq.com/signin/public/index.html?_wv=1090528161&_wwv=13",
                 "Accept-Encoding": "gzip, deflate",
                 "Accept-Language": "zh-CN,zh;q=0.9,en-US;q=0.8,en;q=0.7",
                 "Cookie": cookie,
             },
             data=json.dumps({}),
-            proxies=proxies
+            proxies=info.proxy_proxies
         )
         return response.json()
     except requests.exceptions.ProxyError as e:
         return {"errcode": -2, "errmsg": f'代理异常{e}'}
     except requests.exceptions.RequestException:
         return {"errcode": -1, "errmsg": '请求异常'}
```

### Comparing `ANX-0.7.2/AndroidQQ/http/weishi.py` & `ANX-0.7.3/AndroidQQ/http/weishi.py`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from AndroidQQ.http.ClientKey import ClientKeyToCookies
 
 
 def weishi_up_(info):
     if not info.cookies.client_key:
         return {'status': False, 'message': '没有获取到clientkey'}
 
-    rsp = ClientKeyToCookies(info.uin, info.cookies.client_key)
+    rsp = ClientKeyToCookies(info, info.uin, info.cookies.client_key)
     if not rsp['status']:
         return rsp
     try:
         cookies = rsp['cookie']
         params = {
             "req_body": {
                 "blockID": "2",
@@ -28,15 +28,16 @@
             headers={
                 "User-Agent": User_Agent,
                 "Content-Type": "multipart/form-data",
                 "Origin": "https://isee.weishi.qq.com",
                 "Referer": "https://isee.weishi.qq.com/",
                 "Cookie": cookies,
                 "wesee_fe_map_ext": "{}",
-            }
+            },
+            proxies=info.proxy_proxies
 
         )
         return {'status': True, 'rsp': rsp.json()}
     except Exception as e:
         return {'status': False, 'message': f'微视任务失败{e}'}
```

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/OidbSvc_0xc96/OidbSvc_0xc96_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x88d/oidb_0x88d_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/PushInfo_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/cmd0x922/cmd0x922_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/cmd0xeb8/cmd0xeb8_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/oidb_0xc05/oidb_0xc05_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/oidb_sso/oidb_sso_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/qqconnect/qqconnect_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py` & `ANX-0.7.3/AndroidQQ/im/oidb/scanlogin/scanlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py` & `ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_ti_web_scanlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py` & `ANX-0.7.3/AndroidQQ/pack/MQUpdateSvc_com_qq_vip_zb_web_OidbSvc_0xdfa_0.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/OidbSvc_0x88d_1.py` & `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0x88d_1.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xc05.py` & `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc05.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xc96.py` & `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xc96.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/OidbSvc_0xeb8.py` & `ANX-0.7.3/AndroidQQ/pack/OidbSvc_0xeb8.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/delUgc.py` & `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/delUgc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/like.py` & `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/like.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/publishmood.py` & `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/publishmood.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py` & `ANX-0.7.3/AndroidQQ/pack/SQQzoneSvc/shuoshuo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/StatSvc_register.py` & `ANX-0.7.3/AndroidQQ/pack/StatSvc_register.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.3/AndroidQQ/pack/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/friendlist.py` & `ANX-0.7.3/AndroidQQ/pack/friendlist.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/test.py` & `ANX-0.7.3/AndroidQQ/pack/test.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py` & `ANX-0.7.3/AndroidQQ/pack/trpc_metaverse_mob_proxy_svr_MobProxy_SsoHandle.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/proto/IM_r_pb2.py` & `ANX-0.7.3/AndroidQQ/proto/IM_r_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/proto/wtlogin_pb2.py` & `ANX-0.7.3/AndroidQQ/proto/wtlogin_pb2.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py` & `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py` & `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py` & `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/QQHeadUrlResp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Avatarlnfo/__init__.py` & `ANX-0.7.3/AndroidQQ/struct/Avatarlnfo/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/MessageSvc.py` & `ANX-0.7.3/AndroidQQ/struct/MessageSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_comm.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_operation.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/cell_userinfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/mobile_applist_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_outshare.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/s_picurl.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_FEEDS/single_feed.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/cmshow_active_result.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_delugc_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_like_rsp.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py` & `ANX-0.7.3/AndroidQQ/struct/NS_MOBILE_OPERATION/operation_publishmood_req.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/OidbSvc.py` & `ANX-0.7.3/AndroidQQ/struct/OidbSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py` & `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfClientIpInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py` & `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfDownstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py` & `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfTokenInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py` & `ANX-0.7.3/AndroidQQ/struct/QMF_PROTOCAL/QmfUpstream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py` & `ANX-0.7.3/AndroidQQ/struct/QQService/SvcReqGetDevLoginInfo.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/QQService/__init__.py` & `ANX-0.7.3/AndroidQQ/struct/QQService/__init__.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/StatSvc.py` & `ANX-0.7.3/AndroidQQ/struct/StatSvc.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py` & `ANX-0.7.3/AndroidQQ/struct/SummaryCard/ReqSummaryCard.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Tlv.py` & `ANX-0.7.3/AndroidQQ/struct/Tlv.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/Tlv_res.py` & `ANX-0.7.3/AndroidQQ/struct/Tlv_res.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/cooperation/qzone/WNSStream.py` & `ANX-0.7.3/AndroidQQ/struct/cooperation/qzone/WNSStream.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/feedcomponent/model.py` & `ANX-0.7.3/AndroidQQ/struct/feedcomponent/model.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/friendlist/AddFriendReq.py` & `ANX-0.7.3/AndroidQQ/struct/friendlist/AddFriendReq.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/head.py` & `ANX-0.7.3/AndroidQQ/struct/head.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/push/SvcReqRegister.py` & `ANX-0.7.3/AndroidQQ/struct/push/SvcReqRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/push/SvcRespRegister.py` & `ANX-0.7.3/AndroidQQ/struct/push/SvcRespRegister.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/struct/wtlogin.py` & `ANX-0.7.3/AndroidQQ/struct/wtlogin.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/utils/build_device.py` & `ANX-0.7.3/AndroidQQ/utils/build_device.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/utils/ecdh.py` & `ANX-0.7.3/AndroidQQ/utils/ecdh.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/utils/sso_server.py` & `ANX-0.7.3/AndroidQQ/utils/sso_server.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/AndroidQQ/utils/tool.py` & `ANX-0.7.3/AndroidQQ/utils/tool.py`

 * *Files identical despite different names*

### Comparing `ANX-0.7.2/setup.py` & `ANX-0.7.3/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import setuptools
 
 with open("requirements.txt", "r") as f:
     requirements = f.read().splitlines()
 setuptools.setup(
     name='ANX',
-    version='0.7.2',
+    version='0.7.3',
     url='https://github.com/grayrail000/AndroidQQ',
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     license='',
     author='1x',
     author_email='',
     description='',
     install_requires=[
         'AndTools',
         'protobuf==4.23.4',
```

