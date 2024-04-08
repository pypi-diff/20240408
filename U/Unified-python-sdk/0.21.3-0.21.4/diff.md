# Comparing `tmp/Unified-python-sdk-0.21.3.tar.gz` & `tmp/Unified-python-sdk-0.21.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Unified-python-sdk-0.21.3.tar", last modified: Sat Apr  6 00:25:45 2024, max compression
+gzip compressed data, was "Unified-python-sdk-0.21.4.tar", last modified: Mon Apr  8 15:59:40 2024, max compression
```

## Comparing `Unified-python-sdk-0.21.3.tar` & `Unified-python-sdk-0.21.4.tar`

### file list

```diff
@@ -1,438 +1,438 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.246194 Unified-python-sdk-0.21.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-06 00:25:45.242194 Unified-python-sdk-0.21.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)    53215 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 00:25:45.246194 Unified-python-sdk-0.21.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.182193 Unified-python-sdk-0.21.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.182193 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-06 00:25:44.000000 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-06 00:25:45.000000 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 00:25:44.000000 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-06 00:25:44.000000 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-06 00:25:44.000000 Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.194193 Unified-python-sdk-0.21.3/src/unified_to/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.194193 Unified-python-sdk-0.21.3/src/unified_to/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    19759 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/account.py
--rw-r--r--   0 runner    (1001) docker     (127)   103146 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/accounting.py
--rw-r--r--   0 runner    (1001) docker     (127)    19415 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/activity.py
--rw-r--r--   0 runner    (1001) docker     (127)     6500 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/apicall.py
--rw-r--r--   0 runner    (1001) docker     (127)    19607 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/application.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/applicationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)   141775 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/ats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/call.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/candidate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19835 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    77080 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/commerce.py
--rw-r--r--   0 runner    (1001) docker     (127)    28545 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/company.py
--rw-r--r--   0 runner    (1001) docker     (127)    19281 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)    57246 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/contact.py
--rw-r--r--   0 runner    (1001) docker     (127)   112757 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/crm.py
--rw-r--r--   0 runner    (1001) docker     (127)    19761 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/customer.py
--rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/deal.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/document.py
--rw-r--r--   0 runner    (1001) docker     (127)    19466 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/employee.py
--rw-r--r--   0 runner    (1001) docker     (127)     6742 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/enrich.py
--rw-r--r--   0 runner    (1001) docker     (127)    19200 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/event.py
--rw-r--r--   0 runner    (1001) docker     (127)    19373 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    19260 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/group.py
--rw-r--r--   0 runner    (1001) docker     (127)    50375 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/hris.py
--rw-r--r--   0 runner    (1001) docker     (127)    10112 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/interview.py
--rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/inventory.py
--rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3532 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)    19438 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/item.py
--rw-r--r--   0 runner    (1001) docker     (127)    19066 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/job.py
--rw-r--r--   0 runner    (1001) docker     (127)    19133 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/lead.py
--rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/link.py
--rw-r--r--   0 runner    (1001) docker     (127)    19400 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/list.py
--rw-r--r--   0 runner    (1001) docker     (127)    19701 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3794 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/login.py
--rw-r--r--   0 runner    (1001) docker     (127)    38376 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/martech.py
--rw-r--r--   0 runner    (1001) docker     (127)    19531 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/member.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.194193 Unified-python-sdk-0.21.3/src/unified_to/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.194193 Unified-python-sdk-0.21.3/src/unified_to/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.230194 Unified-python-sdk-0.21.3/src/unified_to/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createhrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createhrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/createunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingorganization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatscompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrispayslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethristimeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentpayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedapicall.py
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedintegrationauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedintegrationlogin.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingcontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountinginvoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingorganizations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingtaxrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsactivities.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsapplications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsapplicationstatuses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatscandidates.py
--rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatscompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsdocuments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsinterviews.py
--rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsjobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsscorecards.py
--rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommercecollections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommerceinventories.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommerceitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommercelocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmcompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmcontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmdeals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmevents.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmleads.py
--rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmpipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listenrichcompanies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listenrichpeople.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrisemployees.py
--rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrisgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrispayslips.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhristimeoffs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listmartechlists.py
--rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listmartechmembers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpassthroughs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentlinks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentpayments.py
--rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentpayouts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/liststoragefiles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingcustomers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingtickets.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listuccalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listuccontacts.py
--rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedapicalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedconnections.py
--rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedintegrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedintegrationworkspaces.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedissues.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedwebhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchhrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchhrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchmartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchmartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchstoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchunifiedwebhooktrigger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removehrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removehrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removemartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removemartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removestoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeunifiedwebhook.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatehrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatehrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatemartechlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatemartechmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepassthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepaymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepaymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatestoragefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateuccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateunifiedconnection.py
--rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateunifiedwebhooktrigger.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.242194 Unified-python-sdk-0.21.3/src/unified_to/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingcontactpaymentmethod.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountinginvoice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountinglineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingorganization.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtaxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtransactionlineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/apicall.py
--rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsactivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsapplication.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsapplicationanswer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscandidate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscompensation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsdocument.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsinterview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsjob.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsjobquestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsscorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsscorecardquestion.py
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/atstelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commercecollection.py
--rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceinventory.py
--rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemmedia.py
--rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemoption.py
--rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemprice.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemvariant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/commercelocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/connection.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmcontact.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmdeal.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmlead.py
--rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmpipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichcompany.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichperson.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichpersonworkhistory.py
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisemployee.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisgroup.py
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrispayslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrispayslipdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hristelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/hristimeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/integration.py
--rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/integrationsupport.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/issue.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketinglist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketingmember.py
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentlink.py
--rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentlinklineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentpayment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentpayout.py
--rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingcontact_billing_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingcontact_shipping_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingorganization_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_atscandidate_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_atscompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_commercelocation_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_connection_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_connection_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_connection_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmcompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmcontact_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_call.py
--rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_email.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_meeting.py
--rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_note.py
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_task.py
--rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmlead_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_enrichcompany_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_enrichperson_address.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_hrisemployee_address.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_integration_categories.py
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_integrationsupport_webhook_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_created.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_deleted.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_updated.py
--rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_storagepermission_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_uccall_telephone.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/storagefile.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/storagepermission.py
--rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingcustomer.py
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingemail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingnote.py
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingtelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingticket.py
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/uccall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/uccontact.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/ucemail.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/uctelephone.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/models/shared/webhook.py
--rw-r--r--   0 runner    (1001) docker     (127)    19493 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/note.py
--rw-r--r--   0 runner    (1001) docker     (127)     6899 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/organization.py
--rw-r--r--   0 runner    (1001) docker     (127)    16274 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/passthrough.py
--rw-r--r--   0 runner    (1001) docker     (127)    50726 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/payment.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/payout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6662 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/payslip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3634 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/person.py
--rw-r--r--   0 runner    (1001) docker     (127)    19401 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/pipeline.py
--rw-r--r--   0 runner    (1001) docker     (127)     6700 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)    19468 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/scorecard.py
--rw-r--r--   0 runner    (1001) docker     (127)     8643 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    19376 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    19754 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/taxrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    19627 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)    57770 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/ticketing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6663 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/timeoff.py
--rw-r--r--   0 runner    (1001) docker     (127)    20022 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)    22276 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/uc.py
--rw-r--r--   0 runner    (1001) docker     (127)    55968 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/unified.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 00:25:45.242194 Unified-python-sdk-0.21.3/src/unified_to/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30022 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    18780 2024-04-06 00:25:33.000000 Unified-python-sdk-0.21.3/src/unified_to/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.494471 Unified-python-sdk-0.21.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-08 15:59:40.490471 Unified-python-sdk-0.21.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)    53215 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 15:59:40.494471 Unified-python-sdk-0.21.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.430470 Unified-python-sdk-0.21.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.434471 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    92456 2024-04-08 15:59:40.000000 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20913 2024-04-08 15:59:40.000000 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 15:59:40.000000 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-08 15:59:40.000000 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-08 15:59:40.000000 Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.442470 Unified-python-sdk-0.21.4/src/unified_to/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.442470 Unified-python-sdk-0.21.4/src/unified_to/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19424 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)   101255 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/accounting.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19126 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/activity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6424 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/apicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19296 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/application.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/applicationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)   139526 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/ats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6817 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/call.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19492 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75778 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/commerce.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28048 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/company.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19071 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56361 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/contact.py
+-rw-r--r--   0 runner    (1001) docker     (127)   111137 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/crm.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19426 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/deal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/document.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19171 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/employee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6592 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/enrich.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18937 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/event.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19086 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18989 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49529 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/hris.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9875 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/interview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19445 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/inventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3495 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19143 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/item.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18819 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/lead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19134 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/link.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19113 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19374 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37786 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/martech.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19228 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/member.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.442470 Unified-python-sdk-0.21.4/src/unified_to/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.442470 Unified-python-sdk-0.21.4/src/unified_to/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.478471 Unified-python-sdk-0.21.4/src/unified_to/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createhrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createhrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1227 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1187 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/createunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingorganization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1385 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1417 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatscompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1304 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1395 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrispayslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethristimeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentpayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedapicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6718 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedintegrationauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedintegrationlogin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2514 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingcontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountinginvoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingorganizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingtaxrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3488 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsactivities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsapplications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2290 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsapplicationstatuses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatscandidates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2275 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatscompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsdocuments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2498 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsinterviews.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsjobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3098 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsscorecards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2328 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommercecollections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommerceinventories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommerceitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommercelocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmcompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2860 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmcontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmdeals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmevents.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmleads.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2279 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmpipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listenrichcompanies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listenrichpeople.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrisemployees.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2265 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrisgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrispayslips.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhristimeoffs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listmartechlists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2481 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listmartechmembers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpassthroughs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentlinks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentpayments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentpayouts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/liststoragefiles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2321 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingcustomers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2475 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2707 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingtickets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listuccalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listuccontacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedapicalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedconnections.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2947 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedintegrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2597 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedintegrationworkspaces.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedissues.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedwebhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1356 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1387 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchhrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchhrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchmartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchmartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1221 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchstoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1357 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1209 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchunifiedwebhooktrigger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1048 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1060 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1047 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removehrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removehrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removemartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removemartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removestoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1050 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeunifiedwebhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1255 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1309 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatehrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatehrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatemartechlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatemartechmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepassthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepaymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepaymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatestoragefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateuccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateunifiedconnection.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateunifiedwebhooktrigger.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.490471 Unified-python-sdk-0.21.4/src/unified_to/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)     7130 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4584 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingcontactpaymentmethod.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5500 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountinginvoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountinglineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2806 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingorganization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtaxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1693 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtransactionlineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/apicall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3146 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsactivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1766 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsapplication.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsapplicationanswer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4363 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscandidate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2392 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscompensation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2977 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsdocument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsinterview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4995 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsjob.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsjobquestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2998 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsscorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsscorecardquestion.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/atstelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commercecollection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1886 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceinventory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3401 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemmedia.py
+-rw-r--r--   0 runner    (1001) docker     (127)      878 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemoption.py
+-rw-r--r--   0 runner    (1001) docker     (127)      835 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemprice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemvariant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/commercelocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/connection.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmcontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3637 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmdeal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4383 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmlead.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2015 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5834 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichcompany.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5554 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichperson.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichpersonworkhistory.py
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      742 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisemployee.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisgroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrispayslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2164 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrispayslipdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hristelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3079 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/hristimeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4073 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/integration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6456 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/integrationsupport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketinglist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2331 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketingmember.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentlink.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3704 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentlinklineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2736 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentpayment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentpayout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingcontact_billing_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingcontact_shipping_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingorganization_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_atscandidate_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_atscompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_commercelocation_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5059 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_connection_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)      473 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_connection_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3824 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_connection_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmcompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmcontact_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_call.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_meeting.py
+-rw-r--r--   0 runner    (1001) docker     (127)      747 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_task.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1778 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmlead_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_enrichcompany_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_enrichperson_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_hrisemployee_address.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_integration_categories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_integrationsupport_webhook_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_deleted.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_property_integrationsupport_webhook_events_updated.py
+-rw-r--r--   0 runner    (1001) docker     (127)      241 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_storagepermission_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_uccall_telephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3234 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/storagefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/storagepermission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2124 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingcustomer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1920 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingnote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingtelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3459 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/uccall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/uccontact.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/ucemail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/uctelephone.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/models/shared/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19190 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/note.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6715 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/organization.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16091 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/passthrough.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49832 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/payment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/payout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6522 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/payslip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3562 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/person.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19114 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/scorecard.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8660 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1439 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19089 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19419 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/taxrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19308 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56813 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/ticketing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6523 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/timeoff.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19655 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21943 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/uc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55159 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/unified.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 15:59:40.490471 Unified-python-sdk-0.21.4/src/unified_to/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18531 2024-04-08 15:59:30.000000 Unified-python-sdk-0.21.4/src/unified_to/webhook.py
```

### Comparing `Unified-python-sdk-0.21.3/LICENSE.md` & `Unified-python-sdk-0.21.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/PKG-INFO` & `Unified-python-sdk-0.21.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Unified-python-sdk
-Version: 0.21.3
+Version: 0.21.4
 Summary: Python Client SDK for Unified.to
 Home-page: https://github.com/unified-to/unified-python-sdk.git
 Author: Unified API Inc
 License: UNKNOWN
 Description: <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://github.com/unified-to/unified-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/unified-to/unified-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.3 Summary: Python
+Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.4 Summary: Python
 Client SDK for Unified.to Home-page: https://github.com/unified-to/unified-
 python-sdk.git Author: Unified API Inc License: UNKNOWN Description:
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_n_i_f_i_e_d_-_t_o_/_u_n_i_f_i_e_d_-
 _p_y_t_h_o_n_-_s_d_k_/_s_p_e_a_k_e_a_s_y___s_d_k___g_e_n_e_r_a_t_i_o_n_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 ## SDK Installation ```bash pip install Unified-python-sdk ``` ## SDK Example
```

### Comparing `Unified-python-sdk-0.21.3/README.md` & `Unified-python-sdk-0.21.4/README.md`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/setup.py` & `Unified-python-sdk-0.21.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Unified-python-sdk',
-    version='0.21.3',
+    version='0.21.4',
     author='Unified API Inc',
     description='Python Client SDK for Unified.to',
     url='https://github.com/unified-to/unified-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/PKG-INFO` & `Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Unified-python-sdk
-Version: 0.21.3
+Version: 0.21.4
 Summary: Python Client SDK for Unified.to
 Home-page: https://github.com/unified-to/unified-python-sdk.git
 Author: Unified API Inc
 License: UNKNOWN
 Description: <div align="left">
             <a href="https://speakeasyapi.dev/"><img src="https://custom-icon-badges.demolab.com/badge/-Built%20By%20Speakeasy-212015?style=for-the-badge&logoColor=FBE331&logo=speakeasy&labelColor=545454" /></a>
             <a href="https://github.com/unified-to/unified-python-sdk/actions"><img src="https://img.shields.io/github/actions/workflow/status/unified-to/unified-python-sdk/speakeasy_sdk_generation.yml?style=for-the-badge" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.3 Summary: Python
+Metadata-Version: 2.1 Name: Unified-python-sdk Version: 0.21.4 Summary: Python
 Client SDK for Unified.to Home-page: https://github.com/unified-to/unified-
 python-sdk.git Author: Unified API Inc License: UNKNOWN Description:
 _[_h_t_t_p_s_:_/_/_c_u_s_t_o_m_-_i_c_o_n_-_b_a_d_g_e_s_._d_e_m_o_l_a_b_._c_o_m_/_b_a_d_g_e_/_-_B_u_i_l_t_%_2_0_B_y_%_2_0_S_p_e_a_k_e_a_s_y_-
 _2_1_2_0_1_5_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_&_l_o_g_o_C_o_l_o_r_=_F_B_E_3_3_1_&_l_o_g_o_=_s_p_e_a_k_e_a_s_y_&_l_a_b_e_l_C_o_l_o_r_=_5_4_5_4_5_4_]
 _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/_w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_u_n_i_f_i_e_d_-_t_o_/_u_n_i_f_i_e_d_-
 _p_y_t_h_o_n_-_s_d_k_/_s_p_e_a_k_e_a_s_y___s_d_k___g_e_n_e_r_a_t_i_o_n_._y_m_l_?_s_t_y_l_e_=_f_o_r_-_t_h_e_-_b_a_d_g_e_]
 ## SDK Installation ```bash pip install Unified-python-sdk ``` ## SDK Example
```

### Comparing `Unified-python-sdk-0.21.3/src/Unified_python_sdk.egg-info/SOURCES.txt` & `Unified-python-sdk-0.21.4/src/Unified_python_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/_hooks/sdkhooks.py` & `Unified-python-sdk-0.21.4/src/unified_to/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/_hooks/types.py` & `Unified-python-sdk-0.21.4/src/unified_to/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/account.py` & `Unified-python-sdk-0.21.4/src/unified_to/account.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_account(self, request: operations.CreateAccountingAccountRequest) -> operations.CreateAccountingAccountResponse:
         r"""Create an account"""
         hook_ctx = HookContext(operation_id='createAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingAccountRequest, base_url, '/accounting/{connection_id}/account', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingAccountRequest, "accounting_account", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_accounting_account(self, request: operations.GetAccountingAccountRequest) -> operations.GetAccountingAccountResponse:
         r"""Retrieve an account"""
         hook_ctx = HookContext(operation_id='getAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingAccountRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_accounting_accounts(self, request: operations.ListAccountingAccountsRequest) -> operations.ListAccountingAccountsResponse:
         r"""List all accounts"""
         hook_ctx = HookContext(operation_id='listAccountingAccounts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingAccountsRequest, base_url, '/accounting/{connection_id}/account', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingAccountsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_accounting_account(self, request: operations.PatchAccountingAccountRequest) -> operations.PatchAccountingAccountResponse:
         r"""Update an account"""
         hook_ctx = HookContext(operation_id='patchAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingAccountRequest, "accounting_account", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_accounting_account(self, request: operations.RemoveAccountingAccountRequest) -> operations.RemoveAccountingAccountResponse:
         r"""Remove an account"""
         hook_ctx = HookContext(operation_id='removeAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_accounting_account(self, request: operations.UpdateAccountingAccountRequest) -> operations.UpdateAccountingAccountResponse:
         r"""Update an account"""
         hook_ctx = HookContext(operation_id='updateAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingAccountRequest, "accounting_account", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/accounting.py` & `Unified-python-sdk-0.21.4/src/unified_to/accounting.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_account(self, request: operations.CreateAccountingAccountRequest) -> operations.CreateAccountingAccountResponse:
         r"""Create an account"""
         hook_ctx = HookContext(operation_id='createAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingAccountRequest, base_url, '/accounting/{connection_id}/account', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingAccountRequest, "accounting_account", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_accounting_contact(self, request: operations.CreateAccountingContactRequest) -> operations.CreateAccountingContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingContactRequest, base_url, '/accounting/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_accounting_invoice(self, request: operations.CreateAccountingInvoiceRequest) -> operations.CreateAccountingInvoiceResponse:
         r"""Create a invoice"""
         hook_ctx = HookContext(operation_id='createAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
@@ -187,15 +187,15 @@
     
     
     def create_accounting_taxrate(self, request: operations.CreateAccountingTaxrateRequest) -> operations.CreateAccountingTaxrateResponse:
         r"""Create a taxrate"""
         hook_ctx = HookContext(operation_id='createAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
@@ -244,15 +244,15 @@
     
     
     def create_accounting_transaction(self, request: operations.CreateAccountingTransactionRequest) -> operations.CreateAccountingTransactionResponse:
         r"""Create a transaction"""
         hook_ctx = HookContext(operation_id='createAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
@@ -301,22 +301,22 @@
     
     
     def get_accounting_account(self, request: operations.GetAccountingAccountRequest) -> operations.GetAccountingAccountResponse:
         r"""Retrieve an account"""
         hook_ctx = HookContext(operation_id='getAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingAccountRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -356,22 +356,22 @@
     
     
     def get_accounting_contact(self, request: operations.GetAccountingContactRequest) -> operations.GetAccountingContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -411,22 +411,22 @@
     
     
     def get_accounting_invoice(self, request: operations.GetAccountingInvoiceRequest) -> operations.GetAccountingInvoiceResponse:
         r"""Retrieve a invoice"""
         hook_ctx = HookContext(operation_id='getAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingInvoiceRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -466,22 +466,22 @@
     
     
     def get_accounting_organization(self, request: operations.GetAccountingOrganizationRequest) -> operations.GetAccountingOrganizationResponse:
         r"""Retrieve an organization"""
         hook_ctx = HookContext(operation_id='getAccountingOrganization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingOrganizationRequest, base_url, '/accounting/{connection_id}/organization/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/organization/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingOrganizationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -521,22 +521,22 @@
     
     
     def get_accounting_taxrate(self, request: operations.GetAccountingTaxrateRequest) -> operations.GetAccountingTaxrateResponse:
         r"""Retrieve a taxrate"""
         hook_ctx = HookContext(operation_id='getAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingTaxrateRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -576,22 +576,22 @@
     
     
     def get_accounting_transaction(self, request: operations.GetAccountingTransactionRequest) -> operations.GetAccountingTransactionResponse:
         r"""Retrieve a transaction"""
         hook_ctx = HookContext(operation_id='getAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingTransactionRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -631,22 +631,22 @@
     
     
     def list_accounting_accounts(self, request: operations.ListAccountingAccountsRequest) -> operations.ListAccountingAccountsResponse:
         r"""List all accounts"""
         hook_ctx = HookContext(operation_id='listAccountingAccounts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingAccountsRequest, base_url, '/accounting/{connection_id}/account', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingAccountsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -686,22 +686,22 @@
     
     
     def list_accounting_contacts(self, request: operations.ListAccountingContactsRequest) -> operations.ListAccountingContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listAccountingContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingContactsRequest, base_url, '/accounting/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -741,22 +741,22 @@
     
     
     def list_accounting_invoices(self, request: operations.ListAccountingInvoicesRequest) -> operations.ListAccountingInvoicesResponse:
         r"""List all invoices"""
         hook_ctx = HookContext(operation_id='listAccountingInvoices', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingInvoicesRequest, base_url, '/accounting/{connection_id}/invoice', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingInvoicesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -796,22 +796,22 @@
     
     
     def list_accounting_organizations(self, request: operations.ListAccountingOrganizationsRequest) -> operations.ListAccountingOrganizationsResponse:
         r"""List all organizations"""
         hook_ctx = HookContext(operation_id='listAccountingOrganizations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingOrganizationsRequest, base_url, '/accounting/{connection_id}/organization', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/organization', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingOrganizationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -851,22 +851,22 @@
     
     
     def list_accounting_taxrates(self, request: operations.ListAccountingTaxratesRequest) -> operations.ListAccountingTaxratesResponse:
         r"""List all taxrates"""
         hook_ctx = HookContext(operation_id='listAccountingTaxrates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingTaxratesRequest, base_url, '/accounting/{connection_id}/taxrate', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingTaxratesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -906,22 +906,22 @@
     
     
     def list_accounting_transactions(self, request: operations.ListAccountingTransactionsRequest) -> operations.ListAccountingTransactionsResponse:
         r"""List all transactions"""
         hook_ctx = HookContext(operation_id='listAccountingTransactions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingTransactionsRequest, base_url, '/accounting/{connection_id}/transaction', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingTransactionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -961,15 +961,15 @@
     
     
     def patch_accounting_account(self, request: operations.PatchAccountingAccountRequest) -> operations.PatchAccountingAccountResponse:
         r"""Update an account"""
         hook_ctx = HookContext(operation_id='patchAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingAccountRequest, "accounting_account", False, True, 'json')
@@ -1018,15 +1018,15 @@
     
     
     def patch_accounting_contact(self, request: operations.PatchAccountingContactRequest) -> operations.PatchAccountingContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -1075,15 +1075,15 @@
     
     
     def patch_accounting_invoice(self, request: operations.PatchAccountingInvoiceRequest) -> operations.PatchAccountingInvoiceResponse:
         r"""Update a invoice"""
         hook_ctx = HookContext(operation_id='patchAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
@@ -1132,15 +1132,15 @@
     
     
     def patch_accounting_taxrate(self, request: operations.PatchAccountingTaxrateRequest) -> operations.PatchAccountingTaxrateResponse:
         r"""Update a taxrate"""
         hook_ctx = HookContext(operation_id='patchAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
@@ -1189,15 +1189,15 @@
     
     
     def patch_accounting_transaction(self, request: operations.PatchAccountingTransactionRequest) -> operations.PatchAccountingTransactionResponse:
         r"""Update a transaction"""
         hook_ctx = HookContext(operation_id='patchAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
@@ -1246,15 +1246,15 @@
     
     
     def remove_accounting_account(self, request: operations.RemoveAccountingAccountRequest) -> operations.RemoveAccountingAccountResponse:
         r"""Remove an account"""
         hook_ctx = HookContext(operation_id='removeAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1300,15 +1300,15 @@
     
     
     def remove_accounting_contact(self, request: operations.RemoveAccountingContactRequest) -> operations.RemoveAccountingContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1354,15 +1354,15 @@
     
     
     def remove_accounting_invoice(self, request: operations.RemoveAccountingInvoiceRequest) -> operations.RemoveAccountingInvoiceResponse:
         r"""Remove a invoice"""
         hook_ctx = HookContext(operation_id='removeAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1408,15 +1408,15 @@
     
     
     def remove_accounting_taxrate(self, request: operations.RemoveAccountingTaxrateRequest) -> operations.RemoveAccountingTaxrateResponse:
         r"""Remove a taxrate"""
         hook_ctx = HookContext(operation_id='removeAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1462,15 +1462,15 @@
     
     
     def remove_accounting_transaction(self, request: operations.RemoveAccountingTransactionRequest) -> operations.RemoveAccountingTransactionResponse:
         r"""Remove a transaction"""
         hook_ctx = HookContext(operation_id='removeAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1516,15 +1516,15 @@
     
     
     def update_accounting_account(self, request: operations.UpdateAccountingAccountRequest) -> operations.UpdateAccountingAccountResponse:
         r"""Update an account"""
         hook_ctx = HookContext(operation_id='updateAccountingAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingAccountRequest, base_url, '/accounting/{connection_id}/account/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/account/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingAccountRequest, "accounting_account", False, True, 'json')
@@ -1573,15 +1573,15 @@
     
     
     def update_accounting_contact(self, request: operations.UpdateAccountingContactRequest) -> operations.UpdateAccountingContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -1630,15 +1630,15 @@
     
     
     def update_accounting_invoice(self, request: operations.UpdateAccountingInvoiceRequest) -> operations.UpdateAccountingInvoiceResponse:
         r"""Update a invoice"""
         hook_ctx = HookContext(operation_id='updateAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
@@ -1687,15 +1687,15 @@
     
     
     def update_accounting_taxrate(self, request: operations.UpdateAccountingTaxrateRequest) -> operations.UpdateAccountingTaxrateResponse:
         r"""Update a taxrate"""
         hook_ctx = HookContext(operation_id='updateAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
@@ -1744,15 +1744,15 @@
     
     
     def update_accounting_transaction(self, request: operations.UpdateAccountingTransactionRequest) -> operations.UpdateAccountingTransactionResponse:
         r"""Update a transaction"""
         hook_ctx = HookContext(operation_id='updateAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/activity.py` & `Unified-python-sdk-0.21.4/src/unified_to/activity.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_activity(self, request: operations.CreateAtsActivityRequest) -> operations.CreateAtsActivityResponse:
         r"""Create an activity"""
         hook_ctx = HookContext(operation_id='createAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsActivityRequest, base_url, '/ats/{connection_id}/activity', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsActivityRequest, "ats_activity", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_activity(self, request: operations.GetAtsActivityRequest) -> operations.GetAtsActivityResponse:
         r"""Retrieve an activity"""
         hook_ctx = HookContext(operation_id='getAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsActivityRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_activities(self, request: operations.ListAtsActivitiesRequest) -> operations.ListAtsActivitiesResponse:
         r"""List all activities"""
         hook_ctx = HookContext(operation_id='listAtsActivities', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsActivitiesRequest, base_url, '/ats/{connection_id}/activity', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsActivitiesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_activity(self, request: operations.PatchAtsActivityRequest) -> operations.PatchAtsActivityResponse:
         r"""Update an activity"""
         hook_ctx = HookContext(operation_id='patchAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsActivityRequest, "ats_activity", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_activity(self, request: operations.RemoveAtsActivityRequest) -> operations.RemoveAtsActivityResponse:
         r"""Remove an activity"""
         hook_ctx = HookContext(operation_id='removeAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_activity(self, request: operations.UpdateAtsActivityRequest) -> operations.UpdateAtsActivityResponse:
         r"""Update an activity"""
         hook_ctx = HookContext(operation_id='updateAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsActivityRequest, "ats_activity", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/apicall.py` & `Unified-python-sdk-0.21.4/src/unified_to/apicall.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def get_unified_apicall(self, request: operations.GetUnifiedApicallRequest) -> operations.GetUnifiedApicallResponse:
         r"""Retrieve specific API Call by its ID"""
         hook_ctx = HookContext(operation_id='getUnifiedApicall', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedApicallRequest, base_url, '/unified/apicall/{id}', request)
+        url = utils.generate_url(base_url, '/unified/apicall/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -77,15 +77,15 @@
         url = base_url + '/unified/apicall'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedApicallsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/application.py` & `Unified-python-sdk-0.21.4/src/unified_to/application.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_application(self, request: operations.CreateAtsApplicationRequest) -> operations.CreateAtsApplicationResponse:
         r"""Create an application"""
         hook_ctx = HookContext(operation_id='createAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsApplicationRequest, base_url, '/ats/{connection_id}/application', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsApplicationRequest, "ats_application", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_application(self, request: operations.GetAtsApplicationRequest) -> operations.GetAtsApplicationResponse:
         r"""Retrieve an application"""
         hook_ctx = HookContext(operation_id='getAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsApplicationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_applications(self, request: operations.ListAtsApplicationsRequest) -> operations.ListAtsApplicationsResponse:
         r"""List all applications"""
         hook_ctx = HookContext(operation_id='listAtsApplications', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsApplicationsRequest, base_url, '/ats/{connection_id}/application', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsApplicationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_application(self, request: operations.PatchAtsApplicationRequest) -> operations.PatchAtsApplicationResponse:
         r"""Update an application"""
         hook_ctx = HookContext(operation_id='patchAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsApplicationRequest, "ats_application", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_application(self, request: operations.RemoveAtsApplicationRequest) -> operations.RemoveAtsApplicationResponse:
         r"""Remove an application"""
         hook_ctx = HookContext(operation_id='removeAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_application(self, request: operations.UpdateAtsApplicationRequest) -> operations.UpdateAtsApplicationResponse:
         r"""Update an application"""
         hook_ctx = HookContext(operation_id='updateAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsApplicationRequest, "ats_application", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/applicationstatus.py` & `Unified-python-sdk-0.21.4/src/unified_to/applicationstatus.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def list_ats_applicationstatuses(self, request: operations.ListAtsApplicationstatusesRequest) -> operations.ListAtsApplicationstatusesResponse:
         r"""List all application statuses"""
         hook_ctx = HookContext(operation_id='listAtsApplicationstatuses', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsApplicationstatusesRequest, base_url, '/ats/{connection_id}/applicationstatus', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/applicationstatus', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsApplicationstatusesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/ats.py` & `Unified-python-sdk-0.21.4/src/unified_to/ats.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_activity(self, request: operations.CreateAtsActivityRequest) -> operations.CreateAtsActivityResponse:
         r"""Create an activity"""
         hook_ctx = HookContext(operation_id='createAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsActivityRequest, base_url, '/ats/{connection_id}/activity', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsActivityRequest, "ats_activity", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_ats_application(self, request: operations.CreateAtsApplicationRequest) -> operations.CreateAtsApplicationResponse:
         r"""Create an application"""
         hook_ctx = HookContext(operation_id='createAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsApplicationRequest, base_url, '/ats/{connection_id}/application', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsApplicationRequest, "ats_application", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_ats_candidate(self, request: operations.CreateAtsCandidateRequest) -> operations.CreateAtsCandidateResponse:
         r"""Create a candidate"""
         hook_ctx = HookContext(operation_id='createAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsCandidateRequest, "ats_candidate", False, True, 'json')
@@ -187,15 +187,15 @@
     
     
     def create_ats_document(self, request: operations.CreateAtsDocumentRequest) -> operations.CreateAtsDocumentResponse:
         r"""Create a document"""
         hook_ctx = HookContext(operation_id='createAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsDocumentRequest, base_url, '/ats/{connection_id}/document', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsDocumentRequest, "ats_document", False, True, 'json')
@@ -244,15 +244,15 @@
     
     
     def create_ats_interview(self, request: operations.CreateAtsInterviewRequest) -> operations.CreateAtsInterviewResponse:
         r"""Create a interview"""
         hook_ctx = HookContext(operation_id='createAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsInterviewRequest, base_url, '/ats/{connection_id}/interview', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsInterviewRequest, "ats_interview", False, True, 'json')
@@ -301,15 +301,15 @@
     
     
     def create_ats_job(self, request: operations.CreateAtsJobRequest) -> operations.CreateAtsJobResponse:
         r"""Create a job"""
         hook_ctx = HookContext(operation_id='createAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsJobRequest, base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsJobRequest, "ats_job", False, True, 'json')
@@ -358,15 +358,15 @@
     
     
     def create_ats_scorecard(self, request: operations.CreateAtsScorecardRequest) -> operations.CreateAtsScorecardResponse:
         r"""Create a scorecard"""
         hook_ctx = HookContext(operation_id='createAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsScorecardRequest, "ats_scorecard", False, True, 'json')
@@ -415,22 +415,22 @@
     
     
     def get_ats_activity(self, request: operations.GetAtsActivityRequest) -> operations.GetAtsActivityResponse:
         r"""Retrieve an activity"""
         hook_ctx = HookContext(operation_id='getAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsActivityRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -470,22 +470,22 @@
     
     
     def get_ats_application(self, request: operations.GetAtsApplicationRequest) -> operations.GetAtsApplicationResponse:
         r"""Retrieve an application"""
         hook_ctx = HookContext(operation_id='getAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsApplicationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -525,22 +525,22 @@
     
     
     def get_ats_candidate(self, request: operations.GetAtsCandidateRequest) -> operations.GetAtsCandidateResponse:
         r"""Retrieve a candidate"""
         hook_ctx = HookContext(operation_id='getAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsCandidateRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -580,22 +580,22 @@
     
     
     def get_ats_company(self, request: operations.GetAtsCompanyRequest) -> operations.GetAtsCompanyResponse:
         r"""Retrieve a company"""
         hook_ctx = HookContext(operation_id='getAtsCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsCompanyRequest, base_url, '/ats/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsCompanyRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -635,22 +635,22 @@
     
     
     def get_ats_document(self, request: operations.GetAtsDocumentRequest) -> operations.GetAtsDocumentResponse:
         r"""Retrieve a document"""
         hook_ctx = HookContext(operation_id='getAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsDocumentRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -690,22 +690,22 @@
     
     
     def get_ats_interview(self, request: operations.GetAtsInterviewRequest) -> operations.GetAtsInterviewResponse:
         r"""Retrieve a interview"""
         hook_ctx = HookContext(operation_id='getAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsInterviewRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -745,22 +745,22 @@
     
     
     def get_ats_job(self, request: operations.GetAtsJobRequest) -> operations.GetAtsJobResponse:
         r"""Retrieve a job"""
         hook_ctx = HookContext(operation_id='getAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsJobRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -800,22 +800,22 @@
     
     
     def get_ats_scorecard(self, request: operations.GetAtsScorecardRequest) -> operations.GetAtsScorecardResponse:
         r"""Retrieve a scorecard"""
         hook_ctx = HookContext(operation_id='getAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsScorecardRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -855,22 +855,22 @@
     
     
     def list_ats_activities(self, request: operations.ListAtsActivitiesRequest) -> operations.ListAtsActivitiesResponse:
         r"""List all activities"""
         hook_ctx = HookContext(operation_id='listAtsActivities', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsActivitiesRequest, base_url, '/ats/{connection_id}/activity', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsActivitiesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -910,22 +910,22 @@
     
     
     def list_ats_applications(self, request: operations.ListAtsApplicationsRequest) -> operations.ListAtsApplicationsResponse:
         r"""List all applications"""
         hook_ctx = HookContext(operation_id='listAtsApplications', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsApplicationsRequest, base_url, '/ats/{connection_id}/application', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsApplicationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -965,22 +965,22 @@
     
     
     def list_ats_applicationstatuses(self, request: operations.ListAtsApplicationstatusesRequest) -> operations.ListAtsApplicationstatusesResponse:
         r"""List all application statuses"""
         hook_ctx = HookContext(operation_id='listAtsApplicationstatuses', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsApplicationstatusesRequest, base_url, '/ats/{connection_id}/applicationstatus', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/applicationstatus', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsApplicationstatusesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1020,22 +1020,22 @@
     
     
     def list_ats_candidates(self, request: operations.ListAtsCandidatesRequest) -> operations.ListAtsCandidatesResponse:
         r"""List all candidates"""
         hook_ctx = HookContext(operation_id='listAtsCandidates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsCandidatesRequest, base_url, '/ats/{connection_id}/candidate', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsCandidatesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1075,22 +1075,22 @@
     
     
     def list_ats_companies(self, request: operations.ListAtsCompaniesRequest) -> operations.ListAtsCompaniesResponse:
         r"""List all companies"""
         hook_ctx = HookContext(operation_id='listAtsCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsCompaniesRequest, base_url, '/ats/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1130,22 +1130,22 @@
     
     
     def list_ats_documents(self, request: operations.ListAtsDocumentsRequest) -> operations.ListAtsDocumentsResponse:
         r"""List all documents"""
         hook_ctx = HookContext(operation_id='listAtsDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsDocumentsRequest, base_url, '/ats/{connection_id}/document', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsDocumentsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1185,22 +1185,22 @@
     
     
     def list_ats_interviews(self, request: operations.ListAtsInterviewsRequest) -> operations.ListAtsInterviewsResponse:
         r"""List all interviews"""
         hook_ctx = HookContext(operation_id='listAtsInterviews', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsInterviewsRequest, base_url, '/ats/{connection_id}/interview', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsInterviewsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1240,22 +1240,22 @@
     
     
     def list_ats_jobs(self, request: operations.ListAtsJobsRequest) -> operations.ListAtsJobsResponse:
         r"""List all jobs"""
         hook_ctx = HookContext(operation_id='listAtsJobs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsJobsRequest, base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsJobsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1295,22 +1295,22 @@
     
     
     def list_ats_scorecards(self, request: operations.ListAtsScorecardsRequest) -> operations.ListAtsScorecardsResponse:
         r"""List all scorecards"""
         hook_ctx = HookContext(operation_id='listAtsScorecards', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsScorecardsRequest, base_url, '/ats/{connection_id}/scorecard', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsScorecardsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1350,15 +1350,15 @@
     
     
     def patch_ats_activity(self, request: operations.PatchAtsActivityRequest) -> operations.PatchAtsActivityResponse:
         r"""Update an activity"""
         hook_ctx = HookContext(operation_id='patchAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsActivityRequest, "ats_activity", False, True, 'json')
@@ -1407,15 +1407,15 @@
     
     
     def patch_ats_application(self, request: operations.PatchAtsApplicationRequest) -> operations.PatchAtsApplicationResponse:
         r"""Update an application"""
         hook_ctx = HookContext(operation_id='patchAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsApplicationRequest, "ats_application", False, True, 'json')
@@ -1464,15 +1464,15 @@
     
     
     def patch_ats_candidate(self, request: operations.PatchAtsCandidateRequest) -> operations.PatchAtsCandidateResponse:
         r"""Update a candidate"""
         hook_ctx = HookContext(operation_id='patchAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsCandidateRequest, "ats_candidate", False, True, 'json')
@@ -1521,15 +1521,15 @@
     
     
     def patch_ats_document(self, request: operations.PatchAtsDocumentRequest) -> operations.PatchAtsDocumentResponse:
         r"""Update a document"""
         hook_ctx = HookContext(operation_id='patchAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsDocumentRequest, "ats_document", False, True, 'json')
@@ -1578,15 +1578,15 @@
     
     
     def patch_ats_interview(self, request: operations.PatchAtsInterviewRequest) -> operations.PatchAtsInterviewResponse:
         r"""Update a interview"""
         hook_ctx = HookContext(operation_id='patchAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsInterviewRequest, "ats_interview", False, True, 'json')
@@ -1635,15 +1635,15 @@
     
     
     def patch_ats_job(self, request: operations.PatchAtsJobRequest) -> operations.PatchAtsJobResponse:
         r"""Update a job"""
         hook_ctx = HookContext(operation_id='patchAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsJobRequest, "ats_job", False, True, 'json')
@@ -1692,15 +1692,15 @@
     
     
     def patch_ats_scorecard(self, request: operations.PatchAtsScorecardRequest) -> operations.PatchAtsScorecardResponse:
         r"""Update a scorecard"""
         hook_ctx = HookContext(operation_id='patchAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsScorecardRequest, "ats_scorecard", False, True, 'json')
@@ -1749,15 +1749,15 @@
     
     
     def remove_ats_activity(self, request: operations.RemoveAtsActivityRequest) -> operations.RemoveAtsActivityResponse:
         r"""Remove an activity"""
         hook_ctx = HookContext(operation_id='removeAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1803,15 +1803,15 @@
     
     
     def remove_ats_application(self, request: operations.RemoveAtsApplicationRequest) -> operations.RemoveAtsApplicationResponse:
         r"""Remove an application"""
         hook_ctx = HookContext(operation_id='removeAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1857,15 +1857,15 @@
     
     
     def remove_ats_candidate(self, request: operations.RemoveAtsCandidateRequest) -> operations.RemoveAtsCandidateResponse:
         r"""Remove a candidate"""
         hook_ctx = HookContext(operation_id='removeAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1911,15 +1911,15 @@
     
     
     def remove_ats_document(self, request: operations.RemoveAtsDocumentRequest) -> operations.RemoveAtsDocumentResponse:
         r"""Remove a document"""
         hook_ctx = HookContext(operation_id='removeAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1965,15 +1965,15 @@
     
     
     def remove_ats_interview(self, request: operations.RemoveAtsInterviewRequest) -> operations.RemoveAtsInterviewResponse:
         r"""Remove a interview"""
         hook_ctx = HookContext(operation_id='removeAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -2019,15 +2019,15 @@
     
     
     def remove_ats_job(self, request: operations.RemoveAtsJobRequest) -> operations.RemoveAtsJobResponse:
         r"""Remove a job"""
         hook_ctx = HookContext(operation_id='removeAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -2073,15 +2073,15 @@
     
     
     def remove_ats_scorecard(self, request: operations.RemoveAtsScorecardRequest) -> operations.RemoveAtsScorecardResponse:
         r"""Remove a scorecard"""
         hook_ctx = HookContext(operation_id='removeAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -2127,15 +2127,15 @@
     
     
     def update_ats_activity(self, request: operations.UpdateAtsActivityRequest) -> operations.UpdateAtsActivityResponse:
         r"""Update an activity"""
         hook_ctx = HookContext(operation_id='updateAtsActivity', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsActivityRequest, base_url, '/ats/{connection_id}/activity/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/activity/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsActivityRequest, "ats_activity", False, True, 'json')
@@ -2184,15 +2184,15 @@
     
     
     def update_ats_application(self, request: operations.UpdateAtsApplicationRequest) -> operations.UpdateAtsApplicationResponse:
         r"""Update an application"""
         hook_ctx = HookContext(operation_id='updateAtsApplication', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsApplicationRequest, base_url, '/ats/{connection_id}/application/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/application/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsApplicationRequest, "ats_application", False, True, 'json')
@@ -2241,15 +2241,15 @@
     
     
     def update_ats_candidate(self, request: operations.UpdateAtsCandidateRequest) -> operations.UpdateAtsCandidateResponse:
         r"""Update a candidate"""
         hook_ctx = HookContext(operation_id='updateAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsCandidateRequest, "ats_candidate", False, True, 'json')
@@ -2298,15 +2298,15 @@
     
     
     def update_ats_document(self, request: operations.UpdateAtsDocumentRequest) -> operations.UpdateAtsDocumentResponse:
         r"""Update a document"""
         hook_ctx = HookContext(operation_id='updateAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsDocumentRequest, "ats_document", False, True, 'json')
@@ -2355,15 +2355,15 @@
     
     
     def update_ats_interview(self, request: operations.UpdateAtsInterviewRequest) -> operations.UpdateAtsInterviewResponse:
         r"""Update a interview"""
         hook_ctx = HookContext(operation_id='updateAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsInterviewRequest, "ats_interview", False, True, 'json')
@@ -2412,15 +2412,15 @@
     
     
     def update_ats_job(self, request: operations.UpdateAtsJobRequest) -> operations.UpdateAtsJobResponse:
         r"""Update a job"""
         hook_ctx = HookContext(operation_id='updateAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsJobRequest, "ats_job", False, True, 'json')
@@ -2469,15 +2469,15 @@
     
     
     def update_ats_scorecard(self, request: operations.UpdateAtsScorecardRequest) -> operations.UpdateAtsScorecardResponse:
         r"""Update a scorecard"""
         hook_ctx = HookContext(operation_id='updateAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsScorecardRequest, "ats_scorecard", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/auth.py` & `Unified-python-sdk-0.21.4/src/unified_to/auth.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     def get_unified_integration_auth(self, request: operations.GetUnifiedIntegrationAuthRequest) -> operations.GetUnifiedIntegrationAuthResponse:
         r"""Create connection indirectly
         Returns an authorization URL for the specified integration.  Once a successful authorization occurs, a new connection is created.
         """
         hook_ctx = HookContext(operation_id='getUnifiedIntegrationAuth', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedIntegrationAuthRequest, base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
+        url = utils.generate_url(base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUnifiedIntegrationAuthRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'text/plain'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -73,22 +73,22 @@
     def get_unified_integration_login(self, request: operations.GetUnifiedIntegrationLoginRequest) -> operations.GetUnifiedIntegrationLoginResponse:
         r"""Sign in a user
         Returns an authentication URL for the specified integration.  Once a successful authentication occurs, the name and email are returned inside a jwt parameter, which is a JSON web token that is base-64 encoded.
         """
         hook_ctx = HookContext(operation_id='getUnifiedIntegrationLogin', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedIntegrationLoginRequest, base_url, '/unified/integration/login/{workspace_id}/{integration_type}', request)
+        url = utils.generate_url(base_url, '/unified/integration/login/{workspace_id}/{integration_type}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUnifiedIntegrationLoginRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'text/plain'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/call.py` & `Unified-python-sdk-0.21.4/src/unified_to/call.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def list_uc_calls(self, request: operations.ListUcCallsRequest) -> operations.ListUcCallsResponse:
         r"""List all calls"""
         hook_ctx = HookContext(operation_id='listUcCalls', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUcCallsRequest, base_url, '/uc/{connection_id}/call', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/call', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUcCallsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/candidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/candidate.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_candidate(self, request: operations.CreateAtsCandidateRequest) -> operations.CreateAtsCandidateResponse:
         r"""Create a candidate"""
         hook_ctx = HookContext(operation_id='createAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsCandidateRequest, "ats_candidate", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_candidate(self, request: operations.GetAtsCandidateRequest) -> operations.GetAtsCandidateResponse:
         r"""Retrieve a candidate"""
         hook_ctx = HookContext(operation_id='getAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsCandidateRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_candidates(self, request: operations.ListAtsCandidatesRequest) -> operations.ListAtsCandidatesResponse:
         r"""List all candidates"""
         hook_ctx = HookContext(operation_id='listAtsCandidates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsCandidatesRequest, base_url, '/ats/{connection_id}/candidate', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsCandidatesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_candidate(self, request: operations.PatchAtsCandidateRequest) -> operations.PatchAtsCandidateResponse:
         r"""Update a candidate"""
         hook_ctx = HookContext(operation_id='patchAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsCandidateRequest, "ats_candidate", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_candidate(self, request: operations.RemoveAtsCandidateRequest) -> operations.RemoveAtsCandidateResponse:
         r"""Remove a candidate"""
         hook_ctx = HookContext(operation_id='removeAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_candidate(self, request: operations.UpdateAtsCandidateRequest) -> operations.UpdateAtsCandidateResponse:
         r"""Update a candidate"""
         hook_ctx = HookContext(operation_id='updateAtsCandidate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsCandidateRequest, base_url, '/ats/{connection_id}/candidate/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/candidate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsCandidateRequest, "ats_candidate", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/collection.py` & `Unified-python-sdk-0.21.4/src/unified_to/collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_commerce_collection(self, request: operations.CreateCommerceCollectionRequest) -> operations.CreateCommerceCollectionResponse:
         r"""Create a collection"""
         hook_ctx = HookContext(operation_id='createCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceCollectionRequest, "commerce_collection", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_commerce_collection(self, request: operations.GetCommerceCollectionRequest) -> operations.GetCommerceCollectionResponse:
         r"""Retrieve a collection"""
         hook_ctx = HookContext(operation_id='getCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceCollectionRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_commerce_collections(self, request: operations.ListCommerceCollectionsRequest) -> operations.ListCommerceCollectionsResponse:
         r"""List all collections"""
         hook_ctx = HookContext(operation_id='listCommerceCollections', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceCollectionsRequest, base_url, '/commerce/{connection_id}/collection', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceCollectionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_commerce_collection(self, request: operations.PatchCommerceCollectionRequest) -> operations.PatchCommerceCollectionResponse:
         r"""Update a collection"""
         hook_ctx = HookContext(operation_id='patchCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceCollectionRequest, "commerce_collection", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_commerce_collection(self, request: operations.RemoveCommerceCollectionRequest) -> operations.RemoveCommerceCollectionResponse:
         r"""Remove a collection"""
         hook_ctx = HookContext(operation_id='removeCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_commerce_collection(self, request: operations.UpdateCommerceCollectionRequest) -> operations.UpdateCommerceCollectionResponse:
         r"""Update a collection"""
         hook_ctx = HookContext(operation_id='updateCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceCollectionRequest, "commerce_collection", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/commerce.py` & `Unified-python-sdk-0.21.4/src/unified_to/commerce.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_commerce_collection(self, request: operations.CreateCommerceCollectionRequest) -> operations.CreateCommerceCollectionResponse:
         r"""Create a collection"""
         hook_ctx = HookContext(operation_id='createCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceCollectionRequest, "commerce_collection", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_commerce_inventory(self, request: operations.CreateCommerceInventoryRequest) -> operations.CreateCommerceInventoryResponse:
         r"""Create an inventory"""
         hook_ctx = HookContext(operation_id='createCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_commerce_item(self, request: operations.CreateCommerceItemRequest) -> operations.CreateCommerceItemResponse:
         r"""Create an item"""
         hook_ctx = HookContext(operation_id='createCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceItemRequest, base_url, '/commerce/{connection_id}/item', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceItemRequest, "commerce_item", False, True, 'json')
@@ -187,15 +187,15 @@
     
     
     def create_commerce_location(self, request: operations.CreateCommerceLocationRequest) -> operations.CreateCommerceLocationResponse:
         r"""Create a location"""
         hook_ctx = HookContext(operation_id='createCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceLocationRequest, base_url, '/commerce/{connection_id}/location', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceLocationRequest, "commerce_location", False, True, 'json')
@@ -244,22 +244,22 @@
     
     
     def get_commerce_collection(self, request: operations.GetCommerceCollectionRequest) -> operations.GetCommerceCollectionResponse:
         r"""Retrieve a collection"""
         hook_ctx = HookContext(operation_id='getCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceCollectionRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -299,22 +299,22 @@
     
     
     def get_commerce_inventory(self, request: operations.GetCommerceInventoryRequest) -> operations.GetCommerceInventoryResponse:
         r"""Retrieve an inventory"""
         hook_ctx = HookContext(operation_id='getCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceInventoryRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -354,22 +354,22 @@
     
     
     def get_commerce_item(self, request: operations.GetCommerceItemRequest) -> operations.GetCommerceItemResponse:
         r"""Retrieve an item"""
         hook_ctx = HookContext(operation_id='getCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceItemRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -409,22 +409,22 @@
     
     
     def get_commerce_location(self, request: operations.GetCommerceLocationRequest) -> operations.GetCommerceLocationResponse:
         r"""Retrieve a location"""
         hook_ctx = HookContext(operation_id='getCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceLocationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -464,22 +464,22 @@
     
     
     def list_commerce_collections(self, request: operations.ListCommerceCollectionsRequest) -> operations.ListCommerceCollectionsResponse:
         r"""List all collections"""
         hook_ctx = HookContext(operation_id='listCommerceCollections', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceCollectionsRequest, base_url, '/commerce/{connection_id}/collection', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceCollectionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -519,22 +519,22 @@
     
     
     def list_commerce_inventories(self, request: operations.ListCommerceInventoriesRequest) -> operations.ListCommerceInventoriesResponse:
         r"""List all inventories"""
         hook_ctx = HookContext(operation_id='listCommerceInventories', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceInventoriesRequest, base_url, '/commerce/{connection_id}/inventory', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceInventoriesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -574,22 +574,22 @@
     
     
     def list_commerce_items(self, request: operations.ListCommerceItemsRequest) -> operations.ListCommerceItemsResponse:
         r"""List all items"""
         hook_ctx = HookContext(operation_id='listCommerceItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceItemsRequest, base_url, '/commerce/{connection_id}/item', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceItemsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -629,22 +629,22 @@
     
     
     def list_commerce_locations(self, request: operations.ListCommerceLocationsRequest) -> operations.ListCommerceLocationsResponse:
         r"""List all locations"""
         hook_ctx = HookContext(operation_id='listCommerceLocations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceLocationsRequest, base_url, '/commerce/{connection_id}/location', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceLocationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -684,15 +684,15 @@
     
     
     def patch_commerce_collection(self, request: operations.PatchCommerceCollectionRequest) -> operations.PatchCommerceCollectionResponse:
         r"""Update a collection"""
         hook_ctx = HookContext(operation_id='patchCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceCollectionRequest, "commerce_collection", False, True, 'json')
@@ -741,15 +741,15 @@
     
     
     def patch_commerce_inventory(self, request: operations.PatchCommerceInventoryRequest) -> operations.PatchCommerceInventoryResponse:
         r"""Update an inventory"""
         hook_ctx = HookContext(operation_id='patchCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
@@ -798,15 +798,15 @@
     
     
     def patch_commerce_item(self, request: operations.PatchCommerceItemRequest) -> operations.PatchCommerceItemResponse:
         r"""Update an item"""
         hook_ctx = HookContext(operation_id='patchCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceItemRequest, "commerce_item", False, True, 'json')
@@ -855,15 +855,15 @@
     
     
     def patch_commerce_location(self, request: operations.PatchCommerceLocationRequest) -> operations.PatchCommerceLocationResponse:
         r"""Update a location"""
         hook_ctx = HookContext(operation_id='patchCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceLocationRequest, "commerce_location", False, True, 'json')
@@ -912,15 +912,15 @@
     
     
     def remove_commerce_collection(self, request: operations.RemoveCommerceCollectionRequest) -> operations.RemoveCommerceCollectionResponse:
         r"""Remove a collection"""
         hook_ctx = HookContext(operation_id='removeCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -966,15 +966,15 @@
     
     
     def remove_commerce_inventory(self, request: operations.RemoveCommerceInventoryRequest) -> operations.RemoveCommerceInventoryResponse:
         r"""Remove an inventory"""
         hook_ctx = HookContext(operation_id='removeCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1020,15 +1020,15 @@
     
     
     def remove_commerce_item(self, request: operations.RemoveCommerceItemRequest) -> operations.RemoveCommerceItemResponse:
         r"""Remove an item"""
         hook_ctx = HookContext(operation_id='removeCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1074,15 +1074,15 @@
     
     
     def remove_commerce_location(self, request: operations.RemoveCommerceLocationRequest) -> operations.RemoveCommerceLocationResponse:
         r"""Remove a location"""
         hook_ctx = HookContext(operation_id='removeCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1128,15 +1128,15 @@
     
     
     def update_commerce_collection(self, request: operations.UpdateCommerceCollectionRequest) -> operations.UpdateCommerceCollectionResponse:
         r"""Update a collection"""
         hook_ctx = HookContext(operation_id='updateCommerceCollection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceCollectionRequest, base_url, '/commerce/{connection_id}/collection/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/collection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceCollectionRequest, "commerce_collection", False, True, 'json')
@@ -1185,15 +1185,15 @@
     
     
     def update_commerce_inventory(self, request: operations.UpdateCommerceInventoryRequest) -> operations.UpdateCommerceInventoryResponse:
         r"""Update an inventory"""
         hook_ctx = HookContext(operation_id='updateCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
@@ -1242,15 +1242,15 @@
     
     
     def update_commerce_item(self, request: operations.UpdateCommerceItemRequest) -> operations.UpdateCommerceItemResponse:
         r"""Update an item"""
         hook_ctx = HookContext(operation_id='updateCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceItemRequest, "commerce_item", False, True, 'json')
@@ -1299,15 +1299,15 @@
     
     
     def update_commerce_location(self, request: operations.UpdateCommerceLocationRequest) -> operations.UpdateCommerceLocationResponse:
         r"""Update a location"""
         hook_ctx = HookContext(operation_id='updateCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceLocationRequest, "commerce_location", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/company.py` & `Unified-python-sdk-0.21.4/src/unified_to/company.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_company(self, request: operations.CreateCrmCompanyRequest) -> operations.CreateCrmCompanyResponse:
         r"""Create a company"""
         hook_ctx = HookContext(operation_id='createCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmCompanyRequest, base_url, '/crm/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmCompanyRequest, "crm_company", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_company(self, request: operations.GetAtsCompanyRequest) -> operations.GetAtsCompanyResponse:
         r"""Retrieve a company"""
         hook_ctx = HookContext(operation_id='getAtsCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsCompanyRequest, base_url, '/ats/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsCompanyRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def get_crm_company(self, request: operations.GetCrmCompanyRequest) -> operations.GetCrmCompanyResponse:
         r"""Retrieve a company"""
         hook_ctx = HookContext(operation_id='getCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmCompanyRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,22 +183,22 @@
     
     
     def list_ats_companies(self, request: operations.ListAtsCompaniesRequest) -> operations.ListAtsCompaniesResponse:
         r"""List all companies"""
         hook_ctx = HookContext(operation_id='listAtsCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsCompaniesRequest, base_url, '/ats/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -238,22 +238,22 @@
     
     
     def list_crm_companies(self, request: operations.ListCrmCompaniesRequest) -> operations.ListCrmCompaniesResponse:
         r"""List all companies"""
         hook_ctx = HookContext(operation_id='listCrmCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmCompaniesRequest, base_url, '/crm/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -293,22 +293,22 @@
     
     
     def list_enrich_companies(self, request: operations.ListEnrichCompaniesRequest) -> operations.ListEnrichCompaniesResponse:
         r"""Retrieve enrichment information for a company"""
         hook_ctx = HookContext(operation_id='listEnrichCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListEnrichCompaniesRequest, base_url, '/enrich/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/enrich/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListEnrichCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -348,15 +348,15 @@
     
     
     def patch_crm_company(self, request: operations.PatchCrmCompanyRequest) -> operations.PatchCrmCompanyResponse:
         r"""Update a company"""
         hook_ctx = HookContext(operation_id='patchCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmCompanyRequest, "crm_company", False, True, 'json')
@@ -405,15 +405,15 @@
     
     
     def remove_crm_company(self, request: operations.RemoveCrmCompanyRequest) -> operations.RemoveCrmCompanyResponse:
         r"""Remove a company"""
         hook_ctx = HookContext(operation_id='removeCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -459,15 +459,15 @@
     
     
     def update_crm_company(self, request: operations.UpdateCrmCompanyRequest) -> operations.UpdateCrmCompanyResponse:
         r"""Update a company"""
         hook_ctx = HookContext(operation_id='updateCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmCompanyRequest, "crm_company", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/connection.py` & `Unified-python-sdk-0.21.4/src/unified_to/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     
     
     def get_unified_connection(self, request: operations.GetUnifiedConnectionRequest) -> operations.GetUnifiedConnectionResponse:
         r"""Retrieve connection"""
         hook_ctx = HookContext(operation_id='getUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -134,15 +134,15 @@
         url = base_url + '/unified/connection'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedConnectionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -182,15 +182,15 @@
     
     
     def patch_unified_connection(self, request: operations.PatchUnifiedConnectionRequest) -> operations.PatchUnifiedConnectionResponse:
         r"""Update connection"""
         hook_ctx = HookContext(operation_id='patchUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchUnifiedConnectionRequest, "connection", False, True, 'json')
@@ -239,15 +239,15 @@
     
     
     def remove_unified_connection(self, request: operations.RemoveUnifiedConnectionRequest) -> operations.RemoveUnifiedConnectionResponse:
         r"""Remove connection"""
         hook_ctx = HookContext(operation_id='removeUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -293,15 +293,15 @@
     
     
     def update_unified_connection(self, request: operations.UpdateUnifiedConnectionRequest) -> operations.UpdateUnifiedConnectionResponse:
         r"""Update connection"""
         hook_ctx = HookContext(operation_id='updateUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUnifiedConnectionRequest, "connection", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/contact.py` & `Unified-python-sdk-0.21.4/src/unified_to/contact.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_contact(self, request: operations.CreateAccountingContactRequest) -> operations.CreateAccountingContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingContactRequest, base_url, '/accounting/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_crm_contact(self, request: operations.CreateCrmContactRequest) -> operations.CreateCrmContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmContactRequest, base_url, '/crm/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmContactRequest, "crm_contact", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_uc_contact(self, request: operations.CreateUcContactRequest) -> operations.CreateUcContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateUcContactRequest, base_url, '/uc/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUcContactRequest, "uc_contact", False, True, 'json')
@@ -187,22 +187,22 @@
     
     
     def get_accounting_contact(self, request: operations.GetAccountingContactRequest) -> operations.GetAccountingContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -242,22 +242,22 @@
     
     
     def get_crm_contact(self, request: operations.GetCrmContactRequest) -> operations.GetCrmContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -297,22 +297,22 @@
     
     
     def get_uc_contact(self, request: operations.GetUcContactRequest) -> operations.GetUcContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUcContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -352,22 +352,22 @@
     
     
     def list_accounting_contacts(self, request: operations.ListAccountingContactsRequest) -> operations.ListAccountingContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listAccountingContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingContactsRequest, base_url, '/accounting/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -407,22 +407,22 @@
     
     
     def list_crm_contacts(self, request: operations.ListCrmContactsRequest) -> operations.ListCrmContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listCrmContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmContactsRequest, base_url, '/crm/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -462,22 +462,22 @@
     
     
     def list_uc_contacts(self, request: operations.ListUcContactsRequest) -> operations.ListUcContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listUcContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUcContactsRequest, base_url, '/uc/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUcContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -517,15 +517,15 @@
     
     
     def patch_accounting_contact(self, request: operations.PatchAccountingContactRequest) -> operations.PatchAccountingContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -574,15 +574,15 @@
     
     
     def patch_crm_contact(self, request: operations.PatchCrmContactRequest) -> operations.PatchCrmContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmContactRequest, "crm_contact", False, True, 'json')
@@ -631,15 +631,15 @@
     
     
     def patch_uc_contact(self, request: operations.PatchUcContactRequest) -> operations.PatchUcContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchUcContactRequest, "uc_contact", False, True, 'json')
@@ -688,15 +688,15 @@
     
     
     def remove_accounting_contact(self, request: operations.RemoveAccountingContactRequest) -> operations.RemoveAccountingContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -742,15 +742,15 @@
     
     
     def remove_crm_contact(self, request: operations.RemoveCrmContactRequest) -> operations.RemoveCrmContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -796,15 +796,15 @@
     
     
     def remove_uc_contact(self, request: operations.RemoveUcContactRequest) -> operations.RemoveUcContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -850,15 +850,15 @@
     
     
     def update_accounting_contact(self, request: operations.UpdateAccountingContactRequest) -> operations.UpdateAccountingContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateAccountingContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingContactRequest, base_url, '/accounting/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingContactRequest, "accounting_contact", False, True, 'json')
@@ -907,15 +907,15 @@
     
     
     def update_crm_contact(self, request: operations.UpdateCrmContactRequest) -> operations.UpdateCrmContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmContactRequest, "crm_contact", False, True, 'json')
@@ -964,15 +964,15 @@
     
     
     def update_uc_contact(self, request: operations.UpdateUcContactRequest) -> operations.UpdateUcContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUcContactRequest, "uc_contact", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/crm.py` & `Unified-python-sdk-0.21.4/src/unified_to/crm.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_company(self, request: operations.CreateCrmCompanyRequest) -> operations.CreateCrmCompanyResponse:
         r"""Create a company"""
         hook_ctx = HookContext(operation_id='createCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmCompanyRequest, base_url, '/crm/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmCompanyRequest, "crm_company", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_crm_contact(self, request: operations.CreateCrmContactRequest) -> operations.CreateCrmContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmContactRequest, base_url, '/crm/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmContactRequest, "crm_contact", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_crm_deal(self, request: operations.CreateCrmDealRequest) -> operations.CreateCrmDealResponse:
         r"""Create a deal"""
         hook_ctx = HookContext(operation_id='createCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmDealRequest, base_url, '/crm/{connection_id}/deal', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmDealRequest, "crm_deal", False, True, 'json')
@@ -187,15 +187,15 @@
     
     
     def create_crm_event(self, request: operations.CreateCrmEventRequest) -> operations.CreateCrmEventResponse:
         r"""Create a event"""
         hook_ctx = HookContext(operation_id='createCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmEventRequest, base_url, '/crm/{connection_id}/event', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmEventRequest, "crm_event", False, True, 'json')
@@ -244,15 +244,15 @@
     
     
     def create_crm_lead(self, request: operations.CreateCrmLeadRequest) -> operations.CreateCrmLeadResponse:
         r"""Create a lead"""
         hook_ctx = HookContext(operation_id='createCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmLeadRequest, base_url, '/crm/{connection_id}/lead', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmLeadRequest, "crm_lead", False, True, 'json')
@@ -301,15 +301,15 @@
     
     
     def create_crm_pipeline(self, request: operations.CreateCrmPipelineRequest) -> operations.CreateCrmPipelineResponse:
         r"""Create a pipeline"""
         hook_ctx = HookContext(operation_id='createCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmPipelineRequest, "crm_pipeline", False, True, 'json')
@@ -358,22 +358,22 @@
     
     
     def get_crm_company(self, request: operations.GetCrmCompanyRequest) -> operations.GetCrmCompanyResponse:
         r"""Retrieve a company"""
         hook_ctx = HookContext(operation_id='getCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmCompanyRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -413,22 +413,22 @@
     
     
     def get_crm_contact(self, request: operations.GetCrmContactRequest) -> operations.GetCrmContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -468,22 +468,22 @@
     
     
     def get_crm_deal(self, request: operations.GetCrmDealRequest) -> operations.GetCrmDealResponse:
         r"""Retrieve a deal"""
         hook_ctx = HookContext(operation_id='getCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmDealRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -523,22 +523,22 @@
     
     
     def get_crm_event(self, request: operations.GetCrmEventRequest) -> operations.GetCrmEventResponse:
         r"""Retrieve a event"""
         hook_ctx = HookContext(operation_id='getCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmEventRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -578,22 +578,22 @@
     
     
     def get_crm_lead(self, request: operations.GetCrmLeadRequest) -> operations.GetCrmLeadResponse:
         r"""Retrieve a lead"""
         hook_ctx = HookContext(operation_id='getCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmLeadRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -633,22 +633,22 @@
     
     
     def get_crm_pipeline(self, request: operations.GetCrmPipelineRequest) -> operations.GetCrmPipelineResponse:
         r"""Retrieve a pipeline"""
         hook_ctx = HookContext(operation_id='getCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmPipelineRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -688,22 +688,22 @@
     
     
     def list_crm_companies(self, request: operations.ListCrmCompaniesRequest) -> operations.ListCrmCompaniesResponse:
         r"""List all companies"""
         hook_ctx = HookContext(operation_id='listCrmCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmCompaniesRequest, base_url, '/crm/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -743,22 +743,22 @@
     
     
     def list_crm_contacts(self, request: operations.ListCrmContactsRequest) -> operations.ListCrmContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listCrmContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmContactsRequest, base_url, '/crm/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -798,22 +798,22 @@
     
     
     def list_crm_deals(self, request: operations.ListCrmDealsRequest) -> operations.ListCrmDealsResponse:
         r"""List all deals"""
         hook_ctx = HookContext(operation_id='listCrmDeals', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmDealsRequest, base_url, '/crm/{connection_id}/deal', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmDealsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -853,22 +853,22 @@
     
     
     def list_crm_events(self, request: operations.ListCrmEventsRequest) -> operations.ListCrmEventsResponse:
         r"""List all events"""
         hook_ctx = HookContext(operation_id='listCrmEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmEventsRequest, base_url, '/crm/{connection_id}/event', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmEventsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -908,22 +908,22 @@
     
     
     def list_crm_leads(self, request: operations.ListCrmLeadsRequest) -> operations.ListCrmLeadsResponse:
         r"""List all leads"""
         hook_ctx = HookContext(operation_id='listCrmLeads', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmLeadsRequest, base_url, '/crm/{connection_id}/lead', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmLeadsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -963,22 +963,22 @@
     
     
     def list_crm_pipelines(self, request: operations.ListCrmPipelinesRequest) -> operations.ListCrmPipelinesResponse:
         r"""List all pipelines"""
         hook_ctx = HookContext(operation_id='listCrmPipelines', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmPipelinesRequest, base_url, '/crm/{connection_id}/pipeline', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmPipelinesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -1018,15 +1018,15 @@
     
     
     def patch_crm_company(self, request: operations.PatchCrmCompanyRequest) -> operations.PatchCrmCompanyResponse:
         r"""Update a company"""
         hook_ctx = HookContext(operation_id='patchCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmCompanyRequest, "crm_company", False, True, 'json')
@@ -1075,15 +1075,15 @@
     
     
     def patch_crm_contact(self, request: operations.PatchCrmContactRequest) -> operations.PatchCrmContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmContactRequest, "crm_contact", False, True, 'json')
@@ -1132,15 +1132,15 @@
     
     
     def patch_crm_deal(self, request: operations.PatchCrmDealRequest) -> operations.PatchCrmDealResponse:
         r"""Update a deal"""
         hook_ctx = HookContext(operation_id='patchCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmDealRequest, "crm_deal", False, True, 'json')
@@ -1189,15 +1189,15 @@
     
     
     def patch_crm_event(self, request: operations.PatchCrmEventRequest) -> operations.PatchCrmEventResponse:
         r"""Update a event"""
         hook_ctx = HookContext(operation_id='patchCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmEventRequest, "crm_event", False, True, 'json')
@@ -1246,15 +1246,15 @@
     
     
     def patch_crm_lead(self, request: operations.PatchCrmLeadRequest) -> operations.PatchCrmLeadResponse:
         r"""Update a lead"""
         hook_ctx = HookContext(operation_id='patchCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmLeadRequest, "crm_lead", False, True, 'json')
@@ -1303,15 +1303,15 @@
     
     
     def patch_crm_pipeline(self, request: operations.PatchCrmPipelineRequest) -> operations.PatchCrmPipelineResponse:
         r"""Update a pipeline"""
         hook_ctx = HookContext(operation_id='patchCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmPipelineRequest, "crm_pipeline", False, True, 'json')
@@ -1360,15 +1360,15 @@
     
     
     def remove_crm_company(self, request: operations.RemoveCrmCompanyRequest) -> operations.RemoveCrmCompanyResponse:
         r"""Remove a company"""
         hook_ctx = HookContext(operation_id='removeCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1414,15 +1414,15 @@
     
     
     def remove_crm_contact(self, request: operations.RemoveCrmContactRequest) -> operations.RemoveCrmContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1468,15 +1468,15 @@
     
     
     def remove_crm_deal(self, request: operations.RemoveCrmDealRequest) -> operations.RemoveCrmDealResponse:
         r"""Remove a deal"""
         hook_ctx = HookContext(operation_id='removeCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1522,15 +1522,15 @@
     
     
     def remove_crm_event(self, request: operations.RemoveCrmEventRequest) -> operations.RemoveCrmEventResponse:
         r"""Remove a event"""
         hook_ctx = HookContext(operation_id='removeCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1576,15 +1576,15 @@
     
     
     def remove_crm_lead(self, request: operations.RemoveCrmLeadRequest) -> operations.RemoveCrmLeadResponse:
         r"""Remove a lead"""
         hook_ctx = HookContext(operation_id='removeCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1630,15 +1630,15 @@
     
     
     def remove_crm_pipeline(self, request: operations.RemoveCrmPipelineRequest) -> operations.RemoveCrmPipelineResponse:
         r"""Remove a pipeline"""
         hook_ctx = HookContext(operation_id='removeCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -1684,15 +1684,15 @@
     
     
     def update_crm_company(self, request: operations.UpdateCrmCompanyRequest) -> operations.UpdateCrmCompanyResponse:
         r"""Update a company"""
         hook_ctx = HookContext(operation_id='updateCrmCompany', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmCompanyRequest, base_url, '/crm/{connection_id}/company/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/company/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmCompanyRequest, "crm_company", False, True, 'json')
@@ -1741,15 +1741,15 @@
     
     
     def update_crm_contact(self, request: operations.UpdateCrmContactRequest) -> operations.UpdateCrmContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateCrmContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmContactRequest, base_url, '/crm/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmContactRequest, "crm_contact", False, True, 'json')
@@ -1798,15 +1798,15 @@
     
     
     def update_crm_deal(self, request: operations.UpdateCrmDealRequest) -> operations.UpdateCrmDealResponse:
         r"""Update a deal"""
         hook_ctx = HookContext(operation_id='updateCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmDealRequest, "crm_deal", False, True, 'json')
@@ -1855,15 +1855,15 @@
     
     
     def update_crm_event(self, request: operations.UpdateCrmEventRequest) -> operations.UpdateCrmEventResponse:
         r"""Update a event"""
         hook_ctx = HookContext(operation_id='updateCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmEventRequest, "crm_event", False, True, 'json')
@@ -1912,15 +1912,15 @@
     
     
     def update_crm_lead(self, request: operations.UpdateCrmLeadRequest) -> operations.UpdateCrmLeadResponse:
         r"""Update a lead"""
         hook_ctx = HookContext(operation_id='updateCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmLeadRequest, "crm_lead", False, True, 'json')
@@ -1969,15 +1969,15 @@
     
     
     def update_crm_pipeline(self, request: operations.UpdateCrmPipelineRequest) -> operations.UpdateCrmPipelineResponse:
         r"""Update a pipeline"""
         hook_ctx = HookContext(operation_id='updateCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmPipelineRequest, "crm_pipeline", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/customer.py` & `Unified-python-sdk-0.21.4/src/unified_to/customer.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ticketing_customer(self, request: operations.CreateTicketingCustomerRequest) -> operations.CreateTicketingCustomerResponse:
         r"""Create a customer"""
         hook_ctx = HookContext(operation_id='createTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ticketing_customer(self, request: operations.GetTicketingCustomerRequest) -> operations.GetTicketingCustomerResponse:
         r"""Retrieve a customer"""
         hook_ctx = HookContext(operation_id='getTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingCustomerRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ticketing_customers(self, request: operations.ListTicketingCustomersRequest) -> operations.ListTicketingCustomersResponse:
         r"""List all customers"""
         hook_ctx = HookContext(operation_id='listTicketingCustomers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingCustomersRequest, base_url, '/ticketing/{connection_id}/customer', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingCustomersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ticketing_customer(self, request: operations.PatchTicketingCustomerRequest) -> operations.PatchTicketingCustomerResponse:
         r"""Update a customer"""
         hook_ctx = HookContext(operation_id='patchTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ticketing_customer(self, request: operations.RemoveTicketingCustomerRequest) -> operations.RemoveTicketingCustomerResponse:
         r"""Remove a customer"""
         hook_ctx = HookContext(operation_id='removeTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ticketing_customer(self, request: operations.UpdateTicketingCustomerRequest) -> operations.UpdateTicketingCustomerResponse:
         r"""Update a customer"""
         hook_ctx = HookContext(operation_id='updateTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/deal.py` & `Unified-python-sdk-0.21.4/src/unified_to/deal.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_deal(self, request: operations.CreateCrmDealRequest) -> operations.CreateCrmDealResponse:
         r"""Create a deal"""
         hook_ctx = HookContext(operation_id='createCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmDealRequest, base_url, '/crm/{connection_id}/deal', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmDealRequest, "crm_deal", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_crm_deal(self, request: operations.GetCrmDealRequest) -> operations.GetCrmDealResponse:
         r"""Retrieve a deal"""
         hook_ctx = HookContext(operation_id='getCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmDealRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_crm_deals(self, request: operations.ListCrmDealsRequest) -> operations.ListCrmDealsResponse:
         r"""List all deals"""
         hook_ctx = HookContext(operation_id='listCrmDeals', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmDealsRequest, base_url, '/crm/{connection_id}/deal', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmDealsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_crm_deal(self, request: operations.PatchCrmDealRequest) -> operations.PatchCrmDealResponse:
         r"""Update a deal"""
         hook_ctx = HookContext(operation_id='patchCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmDealRequest, "crm_deal", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_crm_deal(self, request: operations.RemoveCrmDealRequest) -> operations.RemoveCrmDealResponse:
         r"""Remove a deal"""
         hook_ctx = HookContext(operation_id='removeCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_crm_deal(self, request: operations.UpdateCrmDealRequest) -> operations.UpdateCrmDealResponse:
         r"""Update a deal"""
         hook_ctx = HookContext(operation_id='updateCrmDeal', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmDealRequest, base_url, '/crm/{connection_id}/deal/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/deal/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmDealRequest, "crm_deal", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/document.py` & `Unified-python-sdk-0.21.4/src/unified_to/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_document(self, request: operations.CreateAtsDocumentRequest) -> operations.CreateAtsDocumentResponse:
         r"""Create a document"""
         hook_ctx = HookContext(operation_id='createAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsDocumentRequest, base_url, '/ats/{connection_id}/document', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsDocumentRequest, "ats_document", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_document(self, request: operations.GetAtsDocumentRequest) -> operations.GetAtsDocumentResponse:
         r"""Retrieve a document"""
         hook_ctx = HookContext(operation_id='getAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsDocumentRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_documents(self, request: operations.ListAtsDocumentsRequest) -> operations.ListAtsDocumentsResponse:
         r"""List all documents"""
         hook_ctx = HookContext(operation_id='listAtsDocuments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsDocumentsRequest, base_url, '/ats/{connection_id}/document', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsDocumentsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_document(self, request: operations.PatchAtsDocumentRequest) -> operations.PatchAtsDocumentResponse:
         r"""Update a document"""
         hook_ctx = HookContext(operation_id='patchAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsDocumentRequest, "ats_document", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_document(self, request: operations.RemoveAtsDocumentRequest) -> operations.RemoveAtsDocumentResponse:
         r"""Remove a document"""
         hook_ctx = HookContext(operation_id='removeAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_document(self, request: operations.UpdateAtsDocumentRequest) -> operations.UpdateAtsDocumentResponse:
         r"""Update a document"""
         hook_ctx = HookContext(operation_id='updateAtsDocument', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsDocumentRequest, base_url, '/ats/{connection_id}/document/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/document/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsDocumentRequest, "ats_document", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/employee.py` & `Unified-python-sdk-0.21.4/src/unified_to/employee.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_hris_employee(self, request: operations.CreateHrisEmployeeRequest) -> operations.CreateHrisEmployeeResponse:
         r"""Create an employee"""
         hook_ctx = HookContext(operation_id='createHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisEmployeeRequest, "hris_employee", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_hris_employee(self, request: operations.GetHrisEmployeeRequest) -> operations.GetHrisEmployeeResponse:
         r"""Retrieve an employee"""
         hook_ctx = HookContext(operation_id='getHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisEmployeeRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_hris_employees(self, request: operations.ListHrisEmployeesRequest) -> operations.ListHrisEmployeesResponse:
         r"""List all employees"""
         hook_ctx = HookContext(operation_id='listHrisEmployees', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisEmployeesRequest, base_url, '/hris/{connection_id}/employee', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisEmployeesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_hris_employee(self, request: operations.PatchHrisEmployeeRequest) -> operations.PatchHrisEmployeeResponse:
         r"""Update an employee"""
         hook_ctx = HookContext(operation_id='patchHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisEmployeeRequest, "hris_employee", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_hris_employee(self, request: operations.RemoveHrisEmployeeRequest) -> operations.RemoveHrisEmployeeResponse:
         r"""Remove an employee"""
         hook_ctx = HookContext(operation_id='removeHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_hris_employee(self, request: operations.UpdateHrisEmployeeRequest) -> operations.UpdateHrisEmployeeResponse:
         r"""Update an employee"""
         hook_ctx = HookContext(operation_id='updateHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisEmployeeRequest, "hris_employee", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/enrich.py` & `Unified-python-sdk-0.21.4/src/unified_to/enrich.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def list_enrich_companies(self, request: operations.ListEnrichCompaniesRequest) -> operations.ListEnrichCompaniesResponse:
         r"""Retrieve enrichment information for a company"""
         hook_ctx = HookContext(operation_id='listEnrichCompanies', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListEnrichCompaniesRequest, base_url, '/enrich/{connection_id}/company', request)
+        url = utils.generate_url(base_url, '/enrich/{connection_id}/company', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListEnrichCompaniesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_enrich_people(self, request: operations.ListEnrichPeopleRequest) -> operations.ListEnrichPeopleResponse:
         r"""Retrieve enrichment information for a person"""
         hook_ctx = HookContext(operation_id='listEnrichPeople', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListEnrichPeopleRequest, base_url, '/enrich/{connection_id}/person', request)
+        url = utils.generate_url(base_url, '/enrich/{connection_id}/person', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListEnrichPeopleRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/event.py` & `Unified-python-sdk-0.21.4/src/unified_to/event.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_event(self, request: operations.CreateCrmEventRequest) -> operations.CreateCrmEventResponse:
         r"""Create a event"""
         hook_ctx = HookContext(operation_id='createCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmEventRequest, base_url, '/crm/{connection_id}/event', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmEventRequest, "crm_event", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_crm_event(self, request: operations.GetCrmEventRequest) -> operations.GetCrmEventResponse:
         r"""Retrieve a event"""
         hook_ctx = HookContext(operation_id='getCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmEventRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_crm_events(self, request: operations.ListCrmEventsRequest) -> operations.ListCrmEventsResponse:
         r"""List all events"""
         hook_ctx = HookContext(operation_id='listCrmEvents', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmEventsRequest, base_url, '/crm/{connection_id}/event', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmEventsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_crm_event(self, request: operations.PatchCrmEventRequest) -> operations.PatchCrmEventResponse:
         r"""Update a event"""
         hook_ctx = HookContext(operation_id='patchCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmEventRequest, "crm_event", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_crm_event(self, request: operations.RemoveCrmEventRequest) -> operations.RemoveCrmEventResponse:
         r"""Remove a event"""
         hook_ctx = HookContext(operation_id='removeCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_crm_event(self, request: operations.UpdateCrmEventRequest) -> operations.UpdateCrmEventResponse:
         r"""Update a event"""
         hook_ctx = HookContext(operation_id='updateCrmEvent', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmEventRequest, base_url, '/crm/{connection_id}/event/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/event/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmEventRequest, "crm_event", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/file.py` & `Unified-python-sdk-0.21.4/src/unified_to/file.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_storage_file(self, request: operations.CreateStorageFileRequest) -> operations.CreateStorageFileResponse:
         r"""Create a file"""
         hook_ctx = HookContext(operation_id='createStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateStorageFileRequest, base_url, '/storage/{connection_id}/file', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateStorageFileRequest, "storage_file", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_storage_file(self, request: operations.GetStorageFileRequest) -> operations.GetStorageFileResponse:
         r"""Retrieve a file"""
         hook_ctx = HookContext(operation_id='getStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetStorageFileRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_storage_files(self, request: operations.ListStorageFilesRequest) -> operations.ListStorageFilesResponse:
         r"""List all files"""
         hook_ctx = HookContext(operation_id='listStorageFiles', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListStorageFilesRequest, base_url, '/storage/{connection_id}/file', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListStorageFilesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_storage_file(self, request: operations.PatchStorageFileRequest) -> operations.PatchStorageFileResponse:
         r"""Update a file"""
         hook_ctx = HookContext(operation_id='patchStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchStorageFileRequest, "storage_file", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_storage_file(self, request: operations.RemoveStorageFileRequest) -> operations.RemoveStorageFileResponse:
         r"""Remove a file"""
         hook_ctx = HookContext(operation_id='removeStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_storage_file(self, request: operations.UpdateStorageFileRequest) -> operations.UpdateStorageFileResponse:
         r"""Update a file"""
         hook_ctx = HookContext(operation_id='updateStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateStorageFileRequest, "storage_file", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/group.py` & `Unified-python-sdk-0.21.4/src/unified_to/group.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_hris_group(self, request: operations.CreateHrisGroupRequest) -> operations.CreateHrisGroupResponse:
         r"""Create a group"""
         hook_ctx = HookContext(operation_id='createHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateHrisGroupRequest, base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisGroupRequest, "hris_group", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_hris_group(self, request: operations.GetHrisGroupRequest) -> operations.GetHrisGroupResponse:
         r"""Retrieve a group"""
         hook_ctx = HookContext(operation_id='getHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisGroupRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_hris_groups(self, request: operations.ListHrisGroupsRequest) -> operations.ListHrisGroupsResponse:
         r"""List all groups"""
         hook_ctx = HookContext(operation_id='listHrisGroups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisGroupsRequest, base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisGroupsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_hris_group(self, request: operations.PatchHrisGroupRequest) -> operations.PatchHrisGroupResponse:
         r"""Update a group"""
         hook_ctx = HookContext(operation_id='patchHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisGroupRequest, "hris_group", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_hris_group(self, request: operations.RemoveHrisGroupRequest) -> operations.RemoveHrisGroupResponse:
         r"""Remove a group"""
         hook_ctx = HookContext(operation_id='removeHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_hris_group(self, request: operations.UpdateHrisGroupRequest) -> operations.UpdateHrisGroupResponse:
         r"""Update a group"""
         hook_ctx = HookContext(operation_id='updateHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisGroupRequest, "hris_group", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/hris.py` & `Unified-python-sdk-0.21.4/src/unified_to/hris.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_hris_employee(self, request: operations.CreateHrisEmployeeRequest) -> operations.CreateHrisEmployeeResponse:
         r"""Create an employee"""
         hook_ctx = HookContext(operation_id='createHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisEmployeeRequest, "hris_employee", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_hris_group(self, request: operations.CreateHrisGroupRequest) -> operations.CreateHrisGroupResponse:
         r"""Create a group"""
         hook_ctx = HookContext(operation_id='createHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateHrisGroupRequest, base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateHrisGroupRequest, "hris_group", False, True, 'json')
@@ -130,22 +130,22 @@
     
     
     def get_hris_employee(self, request: operations.GetHrisEmployeeRequest) -> operations.GetHrisEmployeeResponse:
         r"""Retrieve an employee"""
         hook_ctx = HookContext(operation_id='getHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisEmployeeRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -185,22 +185,22 @@
     
     
     def get_hris_group(self, request: operations.GetHrisGroupRequest) -> operations.GetHrisGroupResponse:
         r"""Retrieve a group"""
         hook_ctx = HookContext(operation_id='getHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisGroupRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -240,22 +240,22 @@
     
     
     def get_hris_payslip(self, request: operations.GetHrisPayslipRequest) -> operations.GetHrisPayslipResponse:
         r"""Retrieve a payslip"""
         hook_ctx = HookContext(operation_id='getHrisPayslip', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisPayslipRequest, base_url, '/hris/{connection_id}/payslip/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/payslip/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisPayslipRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -295,22 +295,22 @@
     
     
     def get_hris_timeoff(self, request: operations.GetHrisTimeoffRequest) -> operations.GetHrisTimeoffResponse:
         r"""Retrieve a timeoff"""
         hook_ctx = HookContext(operation_id='getHrisTimeoff', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisTimeoffRequest, base_url, '/hris/{connection_id}/timeoff/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/timeoff/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisTimeoffRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -350,22 +350,22 @@
     
     
     def list_hris_employees(self, request: operations.ListHrisEmployeesRequest) -> operations.ListHrisEmployeesResponse:
         r"""List all employees"""
         hook_ctx = HookContext(operation_id='listHrisEmployees', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisEmployeesRequest, base_url, '/hris/{connection_id}/employee', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisEmployeesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -405,22 +405,22 @@
     
     
     def list_hris_groups(self, request: operations.ListHrisGroupsRequest) -> operations.ListHrisGroupsResponse:
         r"""List all groups"""
         hook_ctx = HookContext(operation_id='listHrisGroups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisGroupsRequest, base_url, '/hris/{connection_id}/group', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisGroupsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -460,22 +460,22 @@
     
     
     def list_hris_payslips(self, request: operations.ListHrisPayslipsRequest) -> operations.ListHrisPayslipsResponse:
         r"""List all payslip"""
         hook_ctx = HookContext(operation_id='listHrisPayslips', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisPayslipsRequest, base_url, '/hris/{connection_id}/payslip', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/payslip', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisPayslipsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -515,22 +515,22 @@
     
     
     def list_hris_timeoffs(self, request: operations.ListHrisTimeoffsRequest) -> operations.ListHrisTimeoffsResponse:
         r"""List all timeoffs"""
         hook_ctx = HookContext(operation_id='listHrisTimeoffs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisTimeoffsRequest, base_url, '/hris/{connection_id}/timeoff', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/timeoff', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisTimeoffsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -570,15 +570,15 @@
     
     
     def patch_hris_employee(self, request: operations.PatchHrisEmployeeRequest) -> operations.PatchHrisEmployeeResponse:
         r"""Update an employee"""
         hook_ctx = HookContext(operation_id='patchHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisEmployeeRequest, "hris_employee", False, True, 'json')
@@ -627,15 +627,15 @@
     
     
     def patch_hris_group(self, request: operations.PatchHrisGroupRequest) -> operations.PatchHrisGroupResponse:
         r"""Update a group"""
         hook_ctx = HookContext(operation_id='patchHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchHrisGroupRequest, "hris_group", False, True, 'json')
@@ -684,15 +684,15 @@
     
     
     def remove_hris_employee(self, request: operations.RemoveHrisEmployeeRequest) -> operations.RemoveHrisEmployeeResponse:
         r"""Remove an employee"""
         hook_ctx = HookContext(operation_id='removeHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -738,15 +738,15 @@
     
     
     def remove_hris_group(self, request: operations.RemoveHrisGroupRequest) -> operations.RemoveHrisGroupResponse:
         r"""Remove a group"""
         hook_ctx = HookContext(operation_id='removeHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -792,15 +792,15 @@
     
     
     def update_hris_employee(self, request: operations.UpdateHrisEmployeeRequest) -> operations.UpdateHrisEmployeeResponse:
         r"""Update an employee"""
         hook_ctx = HookContext(operation_id='updateHrisEmployee', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateHrisEmployeeRequest, base_url, '/hris/{connection_id}/employee/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/employee/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisEmployeeRequest, "hris_employee", False, True, 'json')
@@ -849,15 +849,15 @@
     
     
     def update_hris_group(self, request: operations.UpdateHrisGroupRequest) -> operations.UpdateHrisGroupResponse:
         r"""Update a group"""
         hook_ctx = HookContext(operation_id='updateHrisGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateHrisGroupRequest, base_url, '/hris/{connection_id}/group/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/group/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateHrisGroupRequest, "hris_group", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/integration.py` & `Unified-python-sdk-0.21.4/src/unified_to/integration.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,22 +18,22 @@
     def get_unified_integration_auth(self, request: operations.GetUnifiedIntegrationAuthRequest) -> operations.GetUnifiedIntegrationAuthResponse:
         r"""Create connection indirectly
         Returns an authorization URL for the specified integration.  Once a successful authorization occurs, a new connection is created.
         """
         hook_ctx = HookContext(operation_id='getUnifiedIntegrationAuth', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedIntegrationAuthRequest, base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
+        url = utils.generate_url(base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUnifiedIntegrationAuthRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'text/plain'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -74,22 +74,22 @@
     def list_unified_integration_workspaces(self, request: operations.ListUnifiedIntegrationWorkspacesRequest) -> operations.ListUnifiedIntegrationWorkspacesResponse:
         r"""Returns all activated integrations in a workspace
         No authentication required as this is to be used by front-end interface
         """
         hook_ctx = HookContext(operation_id='listUnifiedIntegrationWorkspaces', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUnifiedIntegrationWorkspacesRequest, base_url, '/unified/integration/workspace/{workspace_id}', request)
+        url = utils.generate_url(base_url, '/unified/integration/workspace/{workspace_id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIntegrationWorkspacesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -136,15 +136,15 @@
         url = base_url + '/unified/integration'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIntegrationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/interview.py` & `Unified-python-sdk-0.21.4/src/unified_to/interview.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_interview(self, request: operations.CreateAtsInterviewRequest) -> operations.CreateAtsInterviewResponse:
         r"""Create a interview"""
         hook_ctx = HookContext(operation_id='createAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsInterviewRequest, base_url, '/ats/{connection_id}/interview', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsInterviewRequest, "ats_interview", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_interview(self, request: operations.GetAtsInterviewRequest) -> operations.GetAtsInterviewResponse:
         r"""Retrieve a interview"""
         hook_ctx = HookContext(operation_id='getAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsInterviewRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_interviews(self, request: operations.ListAtsInterviewsRequest) -> operations.ListAtsInterviewsResponse:
         r"""List all interviews"""
         hook_ctx = HookContext(operation_id='listAtsInterviews', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsInterviewsRequest, base_url, '/ats/{connection_id}/interview', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsInterviewsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_interview(self, request: operations.PatchAtsInterviewRequest) -> operations.PatchAtsInterviewResponse:
         r"""Update a interview"""
         hook_ctx = HookContext(operation_id='patchAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsInterviewRequest, "ats_interview", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_interview(self, request: operations.RemoveAtsInterviewRequest) -> operations.RemoveAtsInterviewResponse:
         r"""Remove a interview"""
         hook_ctx = HookContext(operation_id='removeAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_interview(self, request: operations.UpdateAtsInterviewRequest) -> operations.UpdateAtsInterviewResponse:
         r"""Update a interview"""
         hook_ctx = HookContext(operation_id='updateAtsInterview', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsInterviewRequest, base_url, '/ats/{connection_id}/interview/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/interview/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsInterviewRequest, "ats_interview", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/inventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/inventory.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_commerce_inventory(self, request: operations.CreateCommerceInventoryRequest) -> operations.CreateCommerceInventoryResponse:
         r"""Create an inventory"""
         hook_ctx = HookContext(operation_id='createCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_commerce_inventory(self, request: operations.GetCommerceInventoryRequest) -> operations.GetCommerceInventoryResponse:
         r"""Retrieve an inventory"""
         hook_ctx = HookContext(operation_id='getCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceInventoryRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_commerce_inventories(self, request: operations.ListCommerceInventoriesRequest) -> operations.ListCommerceInventoriesResponse:
         r"""List all inventories"""
         hook_ctx = HookContext(operation_id='listCommerceInventories', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceInventoriesRequest, base_url, '/commerce/{connection_id}/inventory', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceInventoriesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_commerce_inventory(self, request: operations.PatchCommerceInventoryRequest) -> operations.PatchCommerceInventoryResponse:
         r"""Update an inventory"""
         hook_ctx = HookContext(operation_id='patchCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_commerce_inventory(self, request: operations.RemoveCommerceInventoryRequest) -> operations.RemoveCommerceInventoryResponse:
         r"""Remove an inventory"""
         hook_ctx = HookContext(operation_id='removeCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_commerce_inventory(self, request: operations.UpdateCommerceInventoryRequest) -> operations.UpdateCommerceInventoryResponse:
         r"""Update an inventory"""
         hook_ctx = HookContext(operation_id='updateCommerceInventory', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceInventoryRequest, base_url, '/commerce/{connection_id}/inventory/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/inventory/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceInventoryRequest, "commerce_inventory", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/invoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/invoice.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_invoice(self, request: operations.CreateAccountingInvoiceRequest) -> operations.CreateAccountingInvoiceResponse:
         r"""Create a invoice"""
         hook_ctx = HookContext(operation_id='createAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_accounting_invoice(self, request: operations.GetAccountingInvoiceRequest) -> operations.GetAccountingInvoiceResponse:
         r"""Retrieve a invoice"""
         hook_ctx = HookContext(operation_id='getAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingInvoiceRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_accounting_invoices(self, request: operations.ListAccountingInvoicesRequest) -> operations.ListAccountingInvoicesResponse:
         r"""List all invoices"""
         hook_ctx = HookContext(operation_id='listAccountingInvoices', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingInvoicesRequest, base_url, '/accounting/{connection_id}/invoice', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingInvoicesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_accounting_invoice(self, request: operations.PatchAccountingInvoiceRequest) -> operations.PatchAccountingInvoiceResponse:
         r"""Update a invoice"""
         hook_ctx = HookContext(operation_id='patchAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_accounting_invoice(self, request: operations.RemoveAccountingInvoiceRequest) -> operations.RemoveAccountingInvoiceResponse:
         r"""Remove a invoice"""
         hook_ctx = HookContext(operation_id='removeAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_accounting_invoice(self, request: operations.UpdateAccountingInvoiceRequest) -> operations.UpdateAccountingInvoiceResponse:
         r"""Update a invoice"""
         hook_ctx = HookContext(operation_id='updateAccountingInvoice', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingInvoiceRequest, base_url, '/accounting/{connection_id}/invoice/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/invoice/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingInvoiceRequest, "accounting_invoice", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/issue.py` & `Unified-python-sdk-0.21.4/src/unified_to/issue.py`

 * *Files 8% similar despite different names*

```diff
@@ -23,15 +23,15 @@
         url = base_url + '/unified/issue'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIssuesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/item.py` & `Unified-python-sdk-0.21.4/src/unified_to/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_commerce_item(self, request: operations.CreateCommerceItemRequest) -> operations.CreateCommerceItemResponse:
         r"""Create an item"""
         hook_ctx = HookContext(operation_id='createCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceItemRequest, base_url, '/commerce/{connection_id}/item', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceItemRequest, "commerce_item", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_commerce_item(self, request: operations.GetCommerceItemRequest) -> operations.GetCommerceItemResponse:
         r"""Retrieve an item"""
         hook_ctx = HookContext(operation_id='getCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceItemRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_commerce_items(self, request: operations.ListCommerceItemsRequest) -> operations.ListCommerceItemsResponse:
         r"""List all items"""
         hook_ctx = HookContext(operation_id='listCommerceItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceItemsRequest, base_url, '/commerce/{connection_id}/item', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceItemsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_commerce_item(self, request: operations.PatchCommerceItemRequest) -> operations.PatchCommerceItemResponse:
         r"""Update an item"""
         hook_ctx = HookContext(operation_id='patchCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceItemRequest, "commerce_item", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_commerce_item(self, request: operations.RemoveCommerceItemRequest) -> operations.RemoveCommerceItemResponse:
         r"""Remove an item"""
         hook_ctx = HookContext(operation_id='removeCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_commerce_item(self, request: operations.UpdateCommerceItemRequest) -> operations.UpdateCommerceItemResponse:
         r"""Update an item"""
         hook_ctx = HookContext(operation_id='updateCommerceItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceItemRequest, base_url, '/commerce/{connection_id}/item/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/item/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceItemRequest, "commerce_item", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/job.py` & `Unified-python-sdk-0.21.4/src/unified_to/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_job(self, request: operations.CreateAtsJobRequest) -> operations.CreateAtsJobResponse:
         r"""Create a job"""
         hook_ctx = HookContext(operation_id='createAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsJobRequest, base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsJobRequest, "ats_job", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_job(self, request: operations.GetAtsJobRequest) -> operations.GetAtsJobResponse:
         r"""Retrieve a job"""
         hook_ctx = HookContext(operation_id='getAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsJobRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_jobs(self, request: operations.ListAtsJobsRequest) -> operations.ListAtsJobsResponse:
         r"""List all jobs"""
         hook_ctx = HookContext(operation_id='listAtsJobs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsJobsRequest, base_url, '/ats/{connection_id}/job', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsJobsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_job(self, request: operations.PatchAtsJobRequest) -> operations.PatchAtsJobResponse:
         r"""Update a job"""
         hook_ctx = HookContext(operation_id='patchAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsJobRequest, "ats_job", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_job(self, request: operations.RemoveAtsJobRequest) -> operations.RemoveAtsJobResponse:
         r"""Remove a job"""
         hook_ctx = HookContext(operation_id='removeAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_job(self, request: operations.UpdateAtsJobRequest) -> operations.UpdateAtsJobResponse:
         r"""Update a job"""
         hook_ctx = HookContext(operation_id='updateAtsJob', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsJobRequest, base_url, '/ats/{connection_id}/job/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/job/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsJobRequest, "ats_job", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/lead.py` & `Unified-python-sdk-0.21.4/src/unified_to/lead.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_lead(self, request: operations.CreateCrmLeadRequest) -> operations.CreateCrmLeadResponse:
         r"""Create a lead"""
         hook_ctx = HookContext(operation_id='createCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmLeadRequest, base_url, '/crm/{connection_id}/lead', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmLeadRequest, "crm_lead", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_crm_lead(self, request: operations.GetCrmLeadRequest) -> operations.GetCrmLeadResponse:
         r"""Retrieve a lead"""
         hook_ctx = HookContext(operation_id='getCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmLeadRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_crm_leads(self, request: operations.ListCrmLeadsRequest) -> operations.ListCrmLeadsResponse:
         r"""List all leads"""
         hook_ctx = HookContext(operation_id='listCrmLeads', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmLeadsRequest, base_url, '/crm/{connection_id}/lead', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmLeadsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_crm_lead(self, request: operations.PatchCrmLeadRequest) -> operations.PatchCrmLeadResponse:
         r"""Update a lead"""
         hook_ctx = HookContext(operation_id='patchCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmLeadRequest, "crm_lead", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_crm_lead(self, request: operations.RemoveCrmLeadRequest) -> operations.RemoveCrmLeadResponse:
         r"""Remove a lead"""
         hook_ctx = HookContext(operation_id='removeCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_crm_lead(self, request: operations.UpdateCrmLeadRequest) -> operations.UpdateCrmLeadResponse:
         r"""Update a lead"""
         hook_ctx = HookContext(operation_id='updateCrmLead', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmLeadRequest, base_url, '/crm/{connection_id}/lead/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/lead/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmLeadRequest, "crm_lead", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/link.py` & `Unified-python-sdk-0.21.4/src/unified_to/link.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_payment_link(self, request: operations.CreatePaymentLinkRequest) -> operations.CreatePaymentLinkResponse:
         r"""Create a payment link"""
         hook_ctx = HookContext(operation_id='createPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreatePaymentLinkRequest, base_url, '/payment/{connection_id}/link', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePaymentLinkRequest, "payment_link", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_payment_link(self, request: operations.GetPaymentLinkRequest) -> operations.GetPaymentLinkResponse:
         r"""Retrieve a payment link"""
         hook_ctx = HookContext(operation_id='getPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentLinkRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_payment_links(self, request: operations.ListPaymentLinksRequest) -> operations.ListPaymentLinksResponse:
         r"""List all payment links"""
         hook_ctx = HookContext(operation_id='listPaymentLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentLinksRequest, base_url, '/payment/{connection_id}/link', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentLinksRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_payment_link(self, request: operations.PatchPaymentLinkRequest) -> operations.PatchPaymentLinkResponse:
         r"""Update a payment link"""
         hook_ctx = HookContext(operation_id='patchPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchPaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPaymentLinkRequest, "payment_link", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_payment_link(self, request: operations.RemovePaymentLinkRequest) -> operations.RemovePaymentLinkResponse:
         r"""Remove a payment link"""
         hook_ctx = HookContext(operation_id='removePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemovePaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_payment_link(self, request: operations.UpdatePaymentLinkRequest) -> operations.UpdatePaymentLinkResponse:
         r"""Update a payment link"""
         hook_ctx = HookContext(operation_id='updatePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePaymentLinkRequest, "payment_link", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/list.py` & `Unified-python-sdk-0.21.4/src/unified_to/list.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_martech_list(self, request: operations.CreateMartechListRequest) -> operations.CreateMartechListResponse:
         r"""Create a list"""
         hook_ctx = HookContext(operation_id='createMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateMartechListRequest, base_url, '/martech/{connection_id}/list', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateMartechListRequest, "marketing_list", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_martech_list(self, request: operations.GetMartechListRequest) -> operations.GetMartechListResponse:
         r"""Retrieve a list"""
         hook_ctx = HookContext(operation_id='getMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetMartechListRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_martech_lists(self, request: operations.ListMartechListsRequest) -> operations.ListMartechListsResponse:
         r"""List all lists"""
         hook_ctx = HookContext(operation_id='listMartechLists', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListMartechListsRequest, base_url, '/martech/{connection_id}/list', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListMartechListsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_martech_list(self, request: operations.PatchMartechListRequest) -> operations.PatchMartechListResponse:
         r"""Update a list"""
         hook_ctx = HookContext(operation_id='patchMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchMartechListRequest, "marketing_list", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_martech_list(self, request: operations.RemoveMartechListRequest) -> operations.RemoveMartechListResponse:
         r"""Remove a list"""
         hook_ctx = HookContext(operation_id='removeMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_martech_list(self, request: operations.UpdateMartechListRequest) -> operations.UpdateMartechListResponse:
         r"""Update a list"""
         hook_ctx = HookContext(operation_id='updateMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateMartechListRequest, "marketing_list", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/location.py` & `Unified-python-sdk-0.21.4/src/unified_to/location.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_commerce_location(self, request: operations.CreateCommerceLocationRequest) -> operations.CreateCommerceLocationResponse:
         r"""Create a location"""
         hook_ctx = HookContext(operation_id='createCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCommerceLocationRequest, base_url, '/commerce/{connection_id}/location', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCommerceLocationRequest, "commerce_location", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_commerce_location(self, request: operations.GetCommerceLocationRequest) -> operations.GetCommerceLocationResponse:
         r"""Retrieve a location"""
         hook_ctx = HookContext(operation_id='getCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCommerceLocationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_commerce_locations(self, request: operations.ListCommerceLocationsRequest) -> operations.ListCommerceLocationsResponse:
         r"""List all locations"""
         hook_ctx = HookContext(operation_id='listCommerceLocations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCommerceLocationsRequest, base_url, '/commerce/{connection_id}/location', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCommerceLocationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_commerce_location(self, request: operations.PatchCommerceLocationRequest) -> operations.PatchCommerceLocationResponse:
         r"""Update a location"""
         hook_ctx = HookContext(operation_id='patchCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCommerceLocationRequest, "commerce_location", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_commerce_location(self, request: operations.RemoveCommerceLocationRequest) -> operations.RemoveCommerceLocationResponse:
         r"""Remove a location"""
         hook_ctx = HookContext(operation_id='removeCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_commerce_location(self, request: operations.UpdateCommerceLocationRequest) -> operations.UpdateCommerceLocationResponse:
         r"""Update a location"""
         hook_ctx = HookContext(operation_id='updateCommerceLocation', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCommerceLocationRequest, base_url, '/commerce/{connection_id}/location/{id}', request)
+        url = utils.generate_url(base_url, '/commerce/{connection_id}/location/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCommerceLocationRequest, "commerce_location", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/login.py` & `Unified-python-sdk-0.21.4/src/unified_to/login.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,22 +17,22 @@
     def get_unified_integration_login(self, request: operations.GetUnifiedIntegrationLoginRequest) -> operations.GetUnifiedIntegrationLoginResponse:
         r"""Sign in a user
         Returns an authentication URL for the specified integration.  Once a successful authentication occurs, the name and email are returned inside a jwt parameter, which is a JSON web token that is base-64 encoded.
         """
         hook_ctx = HookContext(operation_id='getUnifiedIntegrationLogin', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedIntegrationLoginRequest, base_url, '/unified/integration/login/{workspace_id}/{integration_type}', request)
+        url = utils.generate_url(base_url, '/unified/integration/login/{workspace_id}/{integration_type}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUnifiedIntegrationLoginRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'text/plain'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/martech.py` & `Unified-python-sdk-0.21.4/src/unified_to/martech.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_martech_list(self, request: operations.CreateMartechListRequest) -> operations.CreateMartechListResponse:
         r"""Create a list"""
         hook_ctx = HookContext(operation_id='createMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateMartechListRequest, base_url, '/martech/{connection_id}/list', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateMartechListRequest, "marketing_list", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_martech_member(self, request: operations.CreateMartechMemberRequest) -> operations.CreateMartechMemberResponse:
         r"""Create a member"""
         hook_ctx = HookContext(operation_id='createMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateMartechMemberRequest, base_url, '/martech/{connection_id}/member', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateMartechMemberRequest, "marketing_member", False, True, 'json')
@@ -130,22 +130,22 @@
     
     
     def get_martech_list(self, request: operations.GetMartechListRequest) -> operations.GetMartechListResponse:
         r"""Retrieve a list"""
         hook_ctx = HookContext(operation_id='getMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetMartechListRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -185,22 +185,22 @@
     
     
     def get_martech_member(self, request: operations.GetMartechMemberRequest) -> operations.GetMartechMemberResponse:
         r"""Retrieve a member"""
         hook_ctx = HookContext(operation_id='getMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetMartechMemberRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -240,22 +240,22 @@
     
     
     def list_martech_lists(self, request: operations.ListMartechListsRequest) -> operations.ListMartechListsResponse:
         r"""List all lists"""
         hook_ctx = HookContext(operation_id='listMartechLists', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListMartechListsRequest, base_url, '/martech/{connection_id}/list', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListMartechListsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -295,22 +295,22 @@
     
     
     def list_martech_members(self, request: operations.ListMartechMembersRequest) -> operations.ListMartechMembersResponse:
         r"""List all members"""
         hook_ctx = HookContext(operation_id='listMartechMembers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListMartechMembersRequest, base_url, '/martech/{connection_id}/member', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListMartechMembersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -350,15 +350,15 @@
     
     
     def patch_martech_list(self, request: operations.PatchMartechListRequest) -> operations.PatchMartechListResponse:
         r"""Update a list"""
         hook_ctx = HookContext(operation_id='patchMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchMartechListRequest, "marketing_list", False, True, 'json')
@@ -407,15 +407,15 @@
     
     
     def patch_martech_member(self, request: operations.PatchMartechMemberRequest) -> operations.PatchMartechMemberResponse:
         r"""Update a member"""
         hook_ctx = HookContext(operation_id='patchMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchMartechMemberRequest, "marketing_member", False, True, 'json')
@@ -464,15 +464,15 @@
     
     
     def remove_martech_list(self, request: operations.RemoveMartechListRequest) -> operations.RemoveMartechListResponse:
         r"""Remove a list"""
         hook_ctx = HookContext(operation_id='removeMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -518,15 +518,15 @@
     
     
     def remove_martech_member(self, request: operations.RemoveMartechMemberRequest) -> operations.RemoveMartechMemberResponse:
         r"""Remove member"""
         hook_ctx = HookContext(operation_id='removeMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -572,15 +572,15 @@
     
     
     def update_martech_list(self, request: operations.UpdateMartechListRequest) -> operations.UpdateMartechListResponse:
         r"""Update a list"""
         hook_ctx = HookContext(operation_id='updateMartechList', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateMartechListRequest, base_url, '/martech/{connection_id}/list/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/list/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateMartechListRequest, "marketing_list", False, True, 'json')
@@ -629,15 +629,15 @@
     
     
     def update_martech_member(self, request: operations.UpdateMartechMemberRequest) -> operations.UpdateMartechMemberResponse:
         r"""Update a member"""
         hook_ctx = HookContext(operation_id='updateMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateMartechMemberRequest, "marketing_member", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/member.py` & `Unified-python-sdk-0.21.4/src/unified_to/member.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_martech_member(self, request: operations.CreateMartechMemberRequest) -> operations.CreateMartechMemberResponse:
         r"""Create a member"""
         hook_ctx = HookContext(operation_id='createMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateMartechMemberRequest, base_url, '/martech/{connection_id}/member', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateMartechMemberRequest, "marketing_member", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_martech_member(self, request: operations.GetMartechMemberRequest) -> operations.GetMartechMemberResponse:
         r"""Retrieve a member"""
         hook_ctx = HookContext(operation_id='getMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetMartechMemberRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_martech_members(self, request: operations.ListMartechMembersRequest) -> operations.ListMartechMembersResponse:
         r"""List all members"""
         hook_ctx = HookContext(operation_id='listMartechMembers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListMartechMembersRequest, base_url, '/martech/{connection_id}/member', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListMartechMembersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_martech_member(self, request: operations.PatchMartechMemberRequest) -> operations.PatchMartechMemberResponse:
         r"""Update a member"""
         hook_ctx = HookContext(operation_id='patchMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchMartechMemberRequest, "marketing_member", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_martech_member(self, request: operations.RemoveMartechMemberRequest) -> operations.RemoveMartechMemberResponse:
         r"""Remove member"""
         hook_ctx = HookContext(operation_id='removeMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_martech_member(self, request: operations.UpdateMartechMemberRequest) -> operations.UpdateMartechMemberResponse:
         r"""Update a member"""
         hook_ctx = HookContext(operation_id='updateMartechMember', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateMartechMemberRequest, base_url, '/martech/{connection_id}/member/{id}', request)
+        url = utils.generate_url(base_url, '/martech/{connection_id}/member/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateMartechMemberRequest, "marketing_member", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/errors/sdkerror.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/__init__.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createaccountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createatsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcommercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createcrmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createhrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createhrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createhrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createhrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createmartechlist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createmartechmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpassthrough.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpaymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createpaymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createstoragefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createuccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createunifiedconnection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/createunifiedwebhook.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/createunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingorganization.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingorganization.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getaccountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatscompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatscompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getatsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcommercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getcrmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethrispayslip.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethrispayslip.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/gethristimeoff.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/gethristimeoff.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getmartechlist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getmartechmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentpayout.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentpayout.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getpaymentrefund.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getpaymentrefund.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getstoragefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getuccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedapicall.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedapicall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedconnection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedintegrationauth.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedintegrationauth.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedintegrationlogin.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedintegrationlogin.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/getunifiedwebhook.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/getunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingaccounts.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingaccounts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingcontacts.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingcontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountinginvoices.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountinginvoices.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingorganizations.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingorganizations.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingtaxrates.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingtaxrates.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listaccountingtransactions.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listaccountingtransactions.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsactivities.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsactivities.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsapplications.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsapplications.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsapplicationstatuses.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsapplicationstatuses.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatscandidates.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatscandidates.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatscompanies.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatscompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsdocuments.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsdocuments.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsinterviews.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsinterviews.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsjobs.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsjobs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listatsscorecards.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listatsscorecards.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommercecollections.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommercecollections.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommerceinventories.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommerceinventories.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommerceitems.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommerceitems.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcommercelocations.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcommercelocations.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmcompanies.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmcompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmcontacts.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmcontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmdeals.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmdeals.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmevents.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmevents.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmleads.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmleads.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listcrmpipelines.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listcrmpipelines.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listenrichcompanies.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listenrichcompanies.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listenrichpeople.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listenrichpeople.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrisemployees.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrisemployees.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrisgroups.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrisgroups.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhrispayslips.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhrispayslips.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listhristimeoffs.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listhristimeoffs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listmartechlists.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listmartechlists.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listmartechmembers.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listmartechmembers.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpassthroughs.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpassthroughs.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentlinks.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentlinks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentpayments.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentpayments.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentpayouts.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentpayouts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listpaymentrefunds.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listpaymentrefunds.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/liststoragefiles.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/liststoragefiles.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingcustomers.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingcustomers.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingnotes.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingnotes.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listticketingtickets.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listticketingtickets.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listuccalls.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listuccalls.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listuccontacts.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listuccontacts.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedapicalls.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedapicalls.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedconnections.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedconnections.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedintegrations.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedintegrations.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedintegrationworkspaces.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedintegrationworkspaces.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedissues.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedissues.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/listunifiedwebhooks.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/listunifiedwebhooks.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchaccountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchatsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcommercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchcrmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchcrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchhrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchhrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchhrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchhrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchmartechlist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchmartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchmartechmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchmartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpassthrough.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpaymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchpaymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchpaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchstoragefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchstoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchuccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchunifiedconnection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/patchunifiedwebhooktrigger.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/patchunifiedwebhooktrigger.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeaccountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeatsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecommercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removecrmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removecrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removehrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removehrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removehrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removehrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removemartechlist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removemartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removemartechmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removemartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepassthrough.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepaymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removepaymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removepaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removestoragefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removestoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeuccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeunifiedconnection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/removeunifiedwebhook.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/removeunifiedwebhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateaccountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateaccountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateatsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateatsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecommercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecommercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatecrmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatecrmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatehrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatehrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatehrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatehrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatemartechlist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatemartechlist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatemartechmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatemartechmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepassthrough.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepassthrough.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepaymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepaymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatepaymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatepaymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updatestoragefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updatestoragefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateuccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateuccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateunifiedconnection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateunifiedconnection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/operations/updateunifiedwebhooktrigger.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/operations/updateunifiedwebhooktrigger.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/__init__.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingaccount.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingaccount.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingcontactpaymentmethod.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingcontactpaymentmethod.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountinginvoice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountinginvoice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountinglineitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountinglineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingorganization.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingorganization.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtaxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtaxrate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtransaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtransaction.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/accountingtransactionlineitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/accountingtransactionlineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/apicall.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/apicall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsactivity.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsactivity.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsaddress.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsaddress.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsapplication.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsapplication.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsapplicationanswer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsapplicationanswer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscandidate.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscandidate.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atscompensation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atscompensation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsdocument.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsdocument.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsinterview.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsinterview.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsjob.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsjob.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsjobquestion.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsjobquestion.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsscorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsscorecard.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsscorecardquestion.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsscorecardquestion.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atsstatus.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atsstatus.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/atstelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/atstelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commercecollection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commercecollection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceinventory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceinventory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemmedia.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemmedia.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemoption.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemoption.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemprice.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemprice.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commerceitemvariant.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commerceitemvariant.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/commercelocation.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/commercelocation.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/connection.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/connection.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmcontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmcontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmdeal.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmdeal.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmevent.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmevent.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmlead.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmlead.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmpipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmpipeline.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/crmtelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/crmtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichcompany.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichcompany.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichperson.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichperson.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichpersonworkhistory.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichpersonworkhistory.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/enrichtelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/enrichtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisemployee.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisemployee.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrisgroup.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrisgroup.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrispayslip.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrispayslip.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hrispayslipdetail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hrispayslipdetail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hristelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hristelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/hristimeoff.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/hristimeoff.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/integration.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/integration.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/integrationsupport.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/integrationsupport.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/issue.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/issue.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketingemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketinglist.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketinglist.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/marketingmember.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/marketingmember.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentlink.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentlink.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentlinklineitem.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentlinklineitem.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentpayment.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentpayment.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentpayout.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentpayout.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/paymentrefund.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/paymentrefund.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingcontact_billing_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingcontact_billing_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingcontact_shipping_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingcontact_shipping_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_accountingorganization_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_accountingorganization_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_atscandidate_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_atscandidate_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_atscompany_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_atscompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_commercelocation_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_commercelocation_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_connection_auth.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_connection_auth.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_connection_permissions.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_connection_permissions.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmcompany_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmcompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmcontact_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmcontact_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_call.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_call.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_email.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_email.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_meeting.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_meeting.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_note.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_note.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmevent_task.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmevent_task.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_crmlead_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_crmlead_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_enrichcompany_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_enrichcompany_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_enrichperson_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_enrichperson_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_hrisemployee_address.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_hrisemployee_address.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_integrationsupport_webhook_events.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_integrationsupport_webhook_events.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/property_uccall_telephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/property_uccall_telephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/storagefile.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/storagefile.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/storagepermission.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/storagepermission.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingcustomer.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingcustomer.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingnote.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingnote.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingtelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingtelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ticketingticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ticketingticket.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/uccall.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/uccall.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/uccontact.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/uccontact.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/ucemail.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/ucemail.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/uctelephone.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/uctelephone.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/models/shared/webhook.py` & `Unified-python-sdk-0.21.4/src/unified_to/models/shared/webhook.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/note.py` & `Unified-python-sdk-0.21.4/src/unified_to/note.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ticketing_note(self, request: operations.CreateTicketingNoteRequest) -> operations.CreateTicketingNoteResponse:
         r"""Create a note"""
         hook_ctx = HookContext(operation_id='createTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingNoteRequest, "ticketing_note", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ticketing_note(self, request: operations.GetTicketingNoteRequest) -> operations.GetTicketingNoteResponse:
         r"""Retrieve a note"""
         hook_ctx = HookContext(operation_id='getTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingNoteRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ticketing_notes(self, request: operations.ListTicketingNotesRequest) -> operations.ListTicketingNotesResponse:
         r"""List all notes"""
         hook_ctx = HookContext(operation_id='listTicketingNotes', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingNotesRequest, base_url, '/ticketing/{connection_id}/note', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingNotesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ticketing_note(self, request: operations.PatchTicketingNoteRequest) -> operations.PatchTicketingNoteResponse:
         r"""Update a note"""
         hook_ctx = HookContext(operation_id='patchTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingNoteRequest, "ticketing_note", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ticketing_note(self, request: operations.RemoveTicketingNoteRequest) -> operations.RemoveTicketingNoteResponse:
         r"""Remove a note"""
         hook_ctx = HookContext(operation_id='removeTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ticketing_note(self, request: operations.UpdateTicketingNoteRequest) -> operations.UpdateTicketingNoteResponse:
         r"""Update a note"""
         hook_ctx = HookContext(operation_id='updateTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingNoteRequest, "ticketing_note", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/organization.py` & `Unified-python-sdk-0.21.4/src/unified_to/organization.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def get_accounting_organization(self, request: operations.GetAccountingOrganizationRequest) -> operations.GetAccountingOrganizationResponse:
         r"""Retrieve an organization"""
         hook_ctx = HookContext(operation_id='getAccountingOrganization', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingOrganizationRequest, base_url, '/accounting/{connection_id}/organization/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/organization/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingOrganizationRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_accounting_organizations(self, request: operations.ListAccountingOrganizationsRequest) -> operations.ListAccountingOrganizationsResponse:
         r"""List all organizations"""
         hook_ctx = HookContext(operation_id='listAccountingOrganizations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingOrganizationsRequest, base_url, '/accounting/{connection_id}/organization', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/organization', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingOrganizationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/passthrough.py` & `Unified-python-sdk-0.21.4/src/unified_to/passthrough.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_passthrough(self, request: operations.CreatePassthroughRequest) -> operations.CreatePassthroughResponse:
         r"""Passthrough POST"""
         hook_ctx = HookContext(operation_id='createPassthrough', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreatePassthroughRequest, base_url, '/passthrough/{connection_id}/{path}', request)
+        url = utils.generate_url(base_url, '/passthrough/{connection_id}/{path}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePassthroughRequest, "request_body", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def list_passthroughs(self, request: operations.ListPassthroughsRequest) -> operations.ListPassthroughsResponse:
         r"""Passthrough GET"""
         hook_ctx = HookContext(operation_id='listPassthroughs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPassthroughsRequest, base_url, '/passthrough/{connection_id}/{path}', request)
+        url = utils.generate_url(base_url, '/passthrough/{connection_id}/{path}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -127,15 +127,15 @@
     
     
     def patch_passthrough(self, request: operations.PatchPassthroughRequest) -> operations.PatchPassthroughResponse:
         r"""Passthrough PUT"""
         hook_ctx = HookContext(operation_id='patchPassthrough', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchPassthroughRequest, base_url, '/passthrough/{connection_id}/{path}', request)
+        url = utils.generate_url(base_url, '/passthrough/{connection_id}/{path}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPassthroughRequest, "request_body", False, True, 'json')
@@ -184,15 +184,15 @@
     
     
     def remove_passthrough(self, request: operations.RemovePassthroughRequest) -> operations.RemovePassthroughResponse:
         r"""Passthrough DELETE"""
         hook_ctx = HookContext(operation_id='removePassthrough', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemovePassthroughRequest, base_url, '/passthrough/{connection_id}/{path}', request)
+        url = utils.generate_url(base_url, '/passthrough/{connection_id}/{path}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -238,15 +238,15 @@
     
     
     def update_passthrough(self, request: operations.UpdatePassthroughRequest) -> operations.UpdatePassthroughResponse:
         r"""Passthrough PUT"""
         hook_ctx = HookContext(operation_id='updatePassthrough', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePassthroughRequest, base_url, '/passthrough/{connection_id}/{path}', request)
+        url = utils.generate_url(base_url, '/passthrough/{connection_id}/{path}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePassthroughRequest, "request_body", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/payment.py` & `Unified-python-sdk-0.21.4/src/unified_to/payment.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_payment_link(self, request: operations.CreatePaymentLinkRequest) -> operations.CreatePaymentLinkResponse:
         r"""Create a payment link"""
         hook_ctx = HookContext(operation_id='createPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreatePaymentLinkRequest, base_url, '/payment/{connection_id}/link', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePaymentLinkRequest, "payment_link", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_payment_payment(self, request: operations.CreatePaymentPaymentRequest) -> operations.CreatePaymentPaymentResponse:
         r"""Create a payment"""
         hook_ctx = HookContext(operation_id='createPaymentPayment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreatePaymentPaymentRequest, base_url, '/payment/{connection_id}/payment', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePaymentPaymentRequest, "payment_payment", False, True, 'json')
@@ -130,22 +130,22 @@
     
     
     def get_payment_link(self, request: operations.GetPaymentLinkRequest) -> operations.GetPaymentLinkResponse:
         r"""Retrieve a payment link"""
         hook_ctx = HookContext(operation_id='getPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentLinkRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -185,22 +185,22 @@
     
     
     def get_payment_payment(self, request: operations.GetPaymentPaymentRequest) -> operations.GetPaymentPaymentResponse:
         r"""Retrieve a payment"""
         hook_ctx = HookContext(operation_id='getPaymentPayment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentPaymentRequest, base_url, '/payment/{connection_id}/payment/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentPaymentRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -240,22 +240,22 @@
     
     
     def get_payment_payout(self, request: operations.GetPaymentPayoutRequest) -> operations.GetPaymentPayoutResponse:
         r"""Retrieve a payout"""
         hook_ctx = HookContext(operation_id='getPaymentPayout', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentPayoutRequest, base_url, '/payment/{connection_id}/payout/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payout/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentPayoutRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -295,22 +295,22 @@
     
     
     def get_payment_refund(self, request: operations.GetPaymentRefundRequest) -> operations.GetPaymentRefundResponse:
         r"""Retrieve a refund"""
         hook_ctx = HookContext(operation_id='getPaymentRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentRefundRequest, base_url, '/payment/{connection_id}/refund/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/refund/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentRefundRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -350,22 +350,22 @@
     
     
     def list_payment_links(self, request: operations.ListPaymentLinksRequest) -> operations.ListPaymentLinksResponse:
         r"""List all payment links"""
         hook_ctx = HookContext(operation_id='listPaymentLinks', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentLinksRequest, base_url, '/payment/{connection_id}/link', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentLinksRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -405,22 +405,22 @@
     
     
     def list_payment_payments(self, request: operations.ListPaymentPaymentsRequest) -> operations.ListPaymentPaymentsResponse:
         r"""List all payments"""
         hook_ctx = HookContext(operation_id='listPaymentPayments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentPaymentsRequest, base_url, '/payment/{connection_id}/payment', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentPaymentsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -460,22 +460,22 @@
     
     
     def list_payment_payouts(self, request: operations.ListPaymentPayoutsRequest) -> operations.ListPaymentPayoutsResponse:
         r"""List all payouts"""
         hook_ctx = HookContext(operation_id='listPaymentPayouts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentPayoutsRequest, base_url, '/payment/{connection_id}/payout', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payout', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentPayoutsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -515,22 +515,22 @@
     
     
     def list_payment_refunds(self, request: operations.ListPaymentRefundsRequest) -> operations.ListPaymentRefundsResponse:
         r"""List all refunds"""
         hook_ctx = HookContext(operation_id='listPaymentRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentRefundsRequest, base_url, '/payment/{connection_id}/refund', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/refund', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentRefundsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -570,15 +570,15 @@
     
     
     def patch_payment_link(self, request: operations.PatchPaymentLinkRequest) -> operations.PatchPaymentLinkResponse:
         r"""Update a payment link"""
         hook_ctx = HookContext(operation_id='patchPaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchPaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPaymentLinkRequest, "payment_link", False, True, 'json')
@@ -627,15 +627,15 @@
     
     
     def patch_payment_payment(self, request: operations.PatchPaymentPaymentRequest) -> operations.PatchPaymentPaymentResponse:
         r"""Update a payment"""
         hook_ctx = HookContext(operation_id='patchPaymentPayment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchPaymentPaymentRequest, base_url, '/payment/{connection_id}/payment/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchPaymentPaymentRequest, "payment_payment", False, True, 'json')
@@ -684,15 +684,15 @@
     
     
     def remove_payment_link(self, request: operations.RemovePaymentLinkRequest) -> operations.RemovePaymentLinkResponse:
         r"""Remove a payment link"""
         hook_ctx = HookContext(operation_id='removePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemovePaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -738,15 +738,15 @@
     
     
     def remove_payment_payment(self, request: operations.RemovePaymentPaymentRequest) -> operations.RemovePaymentPaymentResponse:
         r"""Remove a payment"""
         hook_ctx = HookContext(operation_id='removePaymentPayment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemovePaymentPaymentRequest, base_url, '/payment/{connection_id}/payment/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -792,15 +792,15 @@
     
     
     def update_payment_link(self, request: operations.UpdatePaymentLinkRequest) -> operations.UpdatePaymentLinkResponse:
         r"""Update a payment link"""
         hook_ctx = HookContext(operation_id='updatePaymentLink', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePaymentLinkRequest, base_url, '/payment/{connection_id}/link/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/link/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePaymentLinkRequest, "payment_link", False, True, 'json')
@@ -849,15 +849,15 @@
     
     
     def update_payment_payment(self, request: operations.UpdatePaymentPaymentRequest) -> operations.UpdatePaymentPaymentResponse:
         r"""Update a payment"""
         hook_ctx = HookContext(operation_id='updatePaymentPayment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdatePaymentPaymentRequest, base_url, '/payment/{connection_id}/payment/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payment/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdatePaymentPaymentRequest, "payment_payment", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/payout.py` & `Unified-python-sdk-0.21.4/src/unified_to/payout.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def get_payment_payout(self, request: operations.GetPaymentPayoutRequest) -> operations.GetPaymentPayoutResponse:
         r"""Retrieve a payout"""
         hook_ctx = HookContext(operation_id='getPaymentPayout', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentPayoutRequest, base_url, '/payment/{connection_id}/payout/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payout/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentPayoutRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_payment_payouts(self, request: operations.ListPaymentPayoutsRequest) -> operations.ListPaymentPayoutsResponse:
         r"""List all payouts"""
         hook_ctx = HookContext(operation_id='listPaymentPayouts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentPayoutsRequest, base_url, '/payment/{connection_id}/payout', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/payout', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentPayoutsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/payslip.py` & `Unified-python-sdk-0.21.4/src/unified_to/payslip.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def get_hris_payslip(self, request: operations.GetHrisPayslipRequest) -> operations.GetHrisPayslipResponse:
         r"""Retrieve a payslip"""
         hook_ctx = HookContext(operation_id='getHrisPayslip', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisPayslipRequest, base_url, '/hris/{connection_id}/payslip/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/payslip/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisPayslipRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_hris_payslips(self, request: operations.ListHrisPayslipsRequest) -> operations.ListHrisPayslipsResponse:
         r"""List all payslip"""
         hook_ctx = HookContext(operation_id='listHrisPayslips', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisPayslipsRequest, base_url, '/hris/{connection_id}/payslip', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/payslip', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisPayslipsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/person.py` & `Unified-python-sdk-0.21.4/src/unified_to/person.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def list_enrich_people(self, request: operations.ListEnrichPeopleRequest) -> operations.ListEnrichPeopleResponse:
         r"""Retrieve enrichment information for a person"""
         hook_ctx = HookContext(operation_id='listEnrichPeople', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListEnrichPeopleRequest, base_url, '/enrich/{connection_id}/person', request)
+        url = utils.generate_url(base_url, '/enrich/{connection_id}/person', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListEnrichPeopleRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/pipeline.py` & `Unified-python-sdk-0.21.4/src/unified_to/pipeline.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_crm_pipeline(self, request: operations.CreateCrmPipelineRequest) -> operations.CreateCrmPipelineResponse:
         r"""Create a pipeline"""
         hook_ctx = HookContext(operation_id='createCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCrmPipelineRequest, "crm_pipeline", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_crm_pipeline(self, request: operations.GetCrmPipelineRequest) -> operations.GetCrmPipelineResponse:
         r"""Retrieve a pipeline"""
         hook_ctx = HookContext(operation_id='getCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetCrmPipelineRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_crm_pipelines(self, request: operations.ListCrmPipelinesRequest) -> operations.ListCrmPipelinesResponse:
         r"""List all pipelines"""
         hook_ctx = HookContext(operation_id='listCrmPipelines', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListCrmPipelinesRequest, base_url, '/crm/{connection_id}/pipeline', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListCrmPipelinesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_crm_pipeline(self, request: operations.PatchCrmPipelineRequest) -> operations.PatchCrmPipelineResponse:
         r"""Update a pipeline"""
         hook_ctx = HookContext(operation_id='patchCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchCrmPipelineRequest, "crm_pipeline", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_crm_pipeline(self, request: operations.RemoveCrmPipelineRequest) -> operations.RemoveCrmPipelineResponse:
         r"""Remove a pipeline"""
         hook_ctx = HookContext(operation_id='removeCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_crm_pipeline(self, request: operations.UpdateCrmPipelineRequest) -> operations.UpdateCrmPipelineResponse:
         r"""Update a pipeline"""
         hook_ctx = HookContext(operation_id='updateCrmPipeline', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCrmPipelineRequest, base_url, '/crm/{connection_id}/pipeline/{id}', request)
+        url = utils.generate_url(base_url, '/crm/{connection_id}/pipeline/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCrmPipelineRequest, "crm_pipeline", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/refund.py` & `Unified-python-sdk-0.21.4/src/unified_to/refund.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def get_payment_refund(self, request: operations.GetPaymentRefundRequest) -> operations.GetPaymentRefundResponse:
         r"""Retrieve a refund"""
         hook_ctx = HookContext(operation_id='getPaymentRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetPaymentRefundRequest, base_url, '/payment/{connection_id}/refund/{id}', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/refund/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetPaymentRefundRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_payment_refunds(self, request: operations.ListPaymentRefundsRequest) -> operations.ListPaymentRefundsResponse:
         r"""List all refunds"""
         hook_ctx = HookContext(operation_id='listPaymentRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListPaymentRefundsRequest, base_url, '/payment/{connection_id}/refund', request)
+        url = utils.generate_url(base_url, '/payment/{connection_id}/refund', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListPaymentRefundsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/scorecard.py` & `Unified-python-sdk-0.21.4/src/unified_to/scorecard.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ats_scorecard(self, request: operations.CreateAtsScorecardRequest) -> operations.CreateAtsScorecardResponse:
         r"""Create a scorecard"""
         hook_ctx = HookContext(operation_id='createAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAtsScorecardRequest, "ats_scorecard", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ats_scorecard(self, request: operations.GetAtsScorecardRequest) -> operations.GetAtsScorecardResponse:
         r"""Retrieve a scorecard"""
         hook_ctx = HookContext(operation_id='getAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAtsScorecardRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ats_scorecards(self, request: operations.ListAtsScorecardsRequest) -> operations.ListAtsScorecardsResponse:
         r"""List all scorecards"""
         hook_ctx = HookContext(operation_id='listAtsScorecards', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAtsScorecardsRequest, base_url, '/ats/{connection_id}/scorecard', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAtsScorecardsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ats_scorecard(self, request: operations.PatchAtsScorecardRequest) -> operations.PatchAtsScorecardResponse:
         r"""Update a scorecard"""
         hook_ctx = HookContext(operation_id='patchAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAtsScorecardRequest, "ats_scorecard", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ats_scorecard(self, request: operations.RemoveAtsScorecardRequest) -> operations.RemoveAtsScorecardResponse:
         r"""Remove a scorecard"""
         hook_ctx = HookContext(operation_id='removeAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ats_scorecard(self, request: operations.UpdateAtsScorecardRequest) -> operations.UpdateAtsScorecardResponse:
         r"""Update a scorecard"""
         hook_ctx = HookContext(operation_id='updateAtsScorecard', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAtsScorecardRequest, base_url, '/ats/{connection_id}/scorecard/{id}', request)
+        url = utils.generate_url(base_url, '/ats/{connection_id}/scorecard/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAtsScorecardRequest, "ats_scorecard", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/sdk.py` & `Unified-python-sdk-0.21.4/src/unified_to/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
         """
         if client is None:
             client = requests_http.Session()
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
+    
 
         self.sdk_configuration = SDKConfiguration(
             client,
             security,
             server_url,
             server_idx,
             retry_config=retry_config
@@ -171,15 +172,15 @@
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.accounting = Accounting(self.sdk_configuration)
         self.account = Account(self.sdk_configuration)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/sdkconfiguration.py` & `Unified-python-sdk-0.21.4/src/unified_to/sdkconfiguration.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,19 +22,21 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = '1.0'
-    sdk_version: str = '0.21.3'
-    gen_version: str = '2.300.0'
-    user_agent: str = 'speakeasy-sdk/python 0.21.3 2.300.0 1.0 Unified-python-sdk'
+    sdk_version: str = '0.21.4'
+    gen_version: str = '2.301.0'
+    user_agent: str = 'speakeasy-sdk/python 0.21.4 2.301.0 1.0 Unified-python-sdk'
     retry_config: Optional[RetryConfig] = None
-    _hooks: Optional[SDKHooks] = None
+
+    def __post_init__(self):
+        self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
             return utils.remove_suffix(self.server_url, '/'), {}
         if self.server_idx is None:
             self.server_idx = 0
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/storage.py` & `Unified-python-sdk-0.21.4/src/unified_to/storage.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_storage_file(self, request: operations.CreateStorageFileRequest) -> operations.CreateStorageFileResponse:
         r"""Create a file"""
         hook_ctx = HookContext(operation_id='createStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateStorageFileRequest, base_url, '/storage/{connection_id}/file', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateStorageFileRequest, "storage_file", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_storage_file(self, request: operations.GetStorageFileRequest) -> operations.GetStorageFileResponse:
         r"""Retrieve a file"""
         hook_ctx = HookContext(operation_id='getStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetStorageFileRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_storage_files(self, request: operations.ListStorageFilesRequest) -> operations.ListStorageFilesResponse:
         r"""List all files"""
         hook_ctx = HookContext(operation_id='listStorageFiles', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListStorageFilesRequest, base_url, '/storage/{connection_id}/file', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListStorageFilesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_storage_file(self, request: operations.PatchStorageFileRequest) -> operations.PatchStorageFileResponse:
         r"""Update a file"""
         hook_ctx = HookContext(operation_id='patchStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchStorageFileRequest, "storage_file", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_storage_file(self, request: operations.RemoveStorageFileRequest) -> operations.RemoveStorageFileResponse:
         r"""Remove a file"""
         hook_ctx = HookContext(operation_id='removeStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_storage_file(self, request: operations.UpdateStorageFileRequest) -> operations.UpdateStorageFileResponse:
         r"""Update a file"""
         hook_ctx = HookContext(operation_id='updateStorageFile', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateStorageFileRequest, base_url, '/storage/{connection_id}/file/{id}', request)
+        url = utils.generate_url(base_url, '/storage/{connection_id}/file/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateStorageFileRequest, "storage_file", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/taxrate.py` & `Unified-python-sdk-0.21.4/src/unified_to/taxrate.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_taxrate(self, request: operations.CreateAccountingTaxrateRequest) -> operations.CreateAccountingTaxrateResponse:
         r"""Create a taxrate"""
         hook_ctx = HookContext(operation_id='createAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_accounting_taxrate(self, request: operations.GetAccountingTaxrateRequest) -> operations.GetAccountingTaxrateResponse:
         r"""Retrieve a taxrate"""
         hook_ctx = HookContext(operation_id='getAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingTaxrateRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_accounting_taxrates(self, request: operations.ListAccountingTaxratesRequest) -> operations.ListAccountingTaxratesResponse:
         r"""List all taxrates"""
         hook_ctx = HookContext(operation_id='listAccountingTaxrates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingTaxratesRequest, base_url, '/accounting/{connection_id}/taxrate', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingTaxratesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_accounting_taxrate(self, request: operations.PatchAccountingTaxrateRequest) -> operations.PatchAccountingTaxrateResponse:
         r"""Update a taxrate"""
         hook_ctx = HookContext(operation_id='patchAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_accounting_taxrate(self, request: operations.RemoveAccountingTaxrateRequest) -> operations.RemoveAccountingTaxrateResponse:
         r"""Remove a taxrate"""
         hook_ctx = HookContext(operation_id='removeAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_accounting_taxrate(self, request: operations.UpdateAccountingTaxrateRequest) -> operations.UpdateAccountingTaxrateResponse:
         r"""Update a taxrate"""
         hook_ctx = HookContext(operation_id='updateAccountingTaxrate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingTaxrateRequest, base_url, '/accounting/{connection_id}/taxrate/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/taxrate/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingTaxrateRequest, "accounting_taxrate", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/ticket.py` & `Unified-python-sdk-0.21.4/src/unified_to/ticket.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ticketing_ticket(self, request: operations.CreateTicketingTicketRequest) -> operations.CreateTicketingTicketResponse:
         r"""Create a ticket"""
         hook_ctx = HookContext(operation_id='createTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_ticketing_ticket(self, request: operations.GetTicketingTicketRequest) -> operations.GetTicketingTicketResponse:
         r"""Retrieve a ticket"""
         hook_ctx = HookContext(operation_id='getTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingTicketRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_ticketing_tickets(self, request: operations.ListTicketingTicketsRequest) -> operations.ListTicketingTicketsResponse:
         r"""List all tickets"""
         hook_ctx = HookContext(operation_id='listTicketingTickets', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingTicketsRequest, base_url, '/ticketing/{connection_id}/ticket', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingTicketsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_ticketing_ticket(self, request: operations.PatchTicketingTicketRequest) -> operations.PatchTicketingTicketResponse:
         r"""Update a ticket"""
         hook_ctx = HookContext(operation_id='patchTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_ticketing_ticket(self, request: operations.RemoveTicketingTicketRequest) -> operations.RemoveTicketingTicketResponse:
         r"""Remove a ticket"""
         hook_ctx = HookContext(operation_id='removeTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_ticketing_ticket(self, request: operations.UpdateTicketingTicketRequest) -> operations.UpdateTicketingTicketResponse:
         r"""Update a ticket"""
         hook_ctx = HookContext(operation_id='updateTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/ticketing.py` & `Unified-python-sdk-0.21.4/src/unified_to/ticketing.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_ticketing_customer(self, request: operations.CreateTicketingCustomerRequest) -> operations.CreateTicketingCustomerResponse:
         r"""Create a customer"""
         hook_ctx = HookContext(operation_id='createTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
@@ -73,15 +73,15 @@
     
     
     def create_ticketing_note(self, request: operations.CreateTicketingNoteRequest) -> operations.CreateTicketingNoteResponse:
         r"""Create a note"""
         hook_ctx = HookContext(operation_id='createTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingNoteRequest, "ticketing_note", False, True, 'json')
@@ -130,15 +130,15 @@
     
     
     def create_ticketing_ticket(self, request: operations.CreateTicketingTicketRequest) -> operations.CreateTicketingTicketResponse:
         r"""Create a ticket"""
         hook_ctx = HookContext(operation_id='createTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
@@ -187,22 +187,22 @@
     
     
     def get_ticketing_customer(self, request: operations.GetTicketingCustomerRequest) -> operations.GetTicketingCustomerResponse:
         r"""Retrieve a customer"""
         hook_ctx = HookContext(operation_id='getTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingCustomerRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -242,22 +242,22 @@
     
     
     def get_ticketing_note(self, request: operations.GetTicketingNoteRequest) -> operations.GetTicketingNoteResponse:
         r"""Retrieve a note"""
         hook_ctx = HookContext(operation_id='getTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingNoteRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -297,22 +297,22 @@
     
     
     def get_ticketing_ticket(self, request: operations.GetTicketingTicketRequest) -> operations.GetTicketingTicketResponse:
         r"""Retrieve a ticket"""
         hook_ctx = HookContext(operation_id='getTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetTicketingTicketRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -352,22 +352,22 @@
     
     
     def list_ticketing_customers(self, request: operations.ListTicketingCustomersRequest) -> operations.ListTicketingCustomersResponse:
         r"""List all customers"""
         hook_ctx = HookContext(operation_id='listTicketingCustomers', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingCustomersRequest, base_url, '/ticketing/{connection_id}/customer', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingCustomersRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -407,22 +407,22 @@
     
     
     def list_ticketing_notes(self, request: operations.ListTicketingNotesRequest) -> operations.ListTicketingNotesResponse:
         r"""List all notes"""
         hook_ctx = HookContext(operation_id='listTicketingNotes', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingNotesRequest, base_url, '/ticketing/{connection_id}/note', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingNotesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -462,22 +462,22 @@
     
     
     def list_ticketing_tickets(self, request: operations.ListTicketingTicketsRequest) -> operations.ListTicketingTicketsResponse:
         r"""List all tickets"""
         hook_ctx = HookContext(operation_id='listTicketingTickets', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListTicketingTicketsRequest, base_url, '/ticketing/{connection_id}/ticket', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListTicketingTicketsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -517,15 +517,15 @@
     
     
     def patch_ticketing_customer(self, request: operations.PatchTicketingCustomerRequest) -> operations.PatchTicketingCustomerResponse:
         r"""Update a customer"""
         hook_ctx = HookContext(operation_id='patchTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
@@ -574,15 +574,15 @@
     
     
     def patch_ticketing_note(self, request: operations.PatchTicketingNoteRequest) -> operations.PatchTicketingNoteResponse:
         r"""Update a note"""
         hook_ctx = HookContext(operation_id='patchTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingNoteRequest, "ticketing_note", False, True, 'json')
@@ -631,15 +631,15 @@
     
     
     def patch_ticketing_ticket(self, request: operations.PatchTicketingTicketRequest) -> operations.PatchTicketingTicketResponse:
         r"""Update a ticket"""
         hook_ctx = HookContext(operation_id='patchTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
@@ -688,15 +688,15 @@
     
     
     def remove_ticketing_customer(self, request: operations.RemoveTicketingCustomerRequest) -> operations.RemoveTicketingCustomerResponse:
         r"""Remove a customer"""
         hook_ctx = HookContext(operation_id='removeTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -742,15 +742,15 @@
     
     
     def remove_ticketing_note(self, request: operations.RemoveTicketingNoteRequest) -> operations.RemoveTicketingNoteResponse:
         r"""Remove a note"""
         hook_ctx = HookContext(operation_id='removeTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -796,15 +796,15 @@
     
     
     def remove_ticketing_ticket(self, request: operations.RemoveTicketingTicketRequest) -> operations.RemoveTicketingTicketResponse:
         r"""Remove a ticket"""
         hook_ctx = HookContext(operation_id='removeTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -850,15 +850,15 @@
     
     
     def update_ticketing_customer(self, request: operations.UpdateTicketingCustomerRequest) -> operations.UpdateTicketingCustomerResponse:
         r"""Update a customer"""
         hook_ctx = HookContext(operation_id='updateTicketingCustomer', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingCustomerRequest, base_url, '/ticketing/{connection_id}/customer/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/customer/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingCustomerRequest, "ticketing_customer", False, True, 'json')
@@ -907,15 +907,15 @@
     
     
     def update_ticketing_note(self, request: operations.UpdateTicketingNoteRequest) -> operations.UpdateTicketingNoteResponse:
         r"""Update a note"""
         hook_ctx = HookContext(operation_id='updateTicketingNote', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingNoteRequest, base_url, '/ticketing/{connection_id}/note/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/note/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingNoteRequest, "ticketing_note", False, True, 'json')
@@ -964,15 +964,15 @@
     
     
     def update_ticketing_ticket(self, request: operations.UpdateTicketingTicketRequest) -> operations.UpdateTicketingTicketResponse:
         r"""Update a ticket"""
         hook_ctx = HookContext(operation_id='updateTicketingTicket', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateTicketingTicketRequest, base_url, '/ticketing/{connection_id}/ticket/{id}', request)
+        url = utils.generate_url(base_url, '/ticketing/{connection_id}/ticket/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateTicketingTicketRequest, "ticketing_ticket", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/timeoff.py` & `Unified-python-sdk-0.21.4/src/unified_to/timeoff.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,22 @@
     
     
     def get_hris_timeoff(self, request: operations.GetHrisTimeoffRequest) -> operations.GetHrisTimeoffResponse:
         r"""Retrieve a timeoff"""
         hook_ctx = HookContext(operation_id='getHrisTimeoff', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetHrisTimeoffRequest, base_url, '/hris/{connection_id}/timeoff/{id}', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/timeoff/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetHrisTimeoffRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -71,22 +71,22 @@
     
     
     def list_hris_timeoffs(self, request: operations.ListHrisTimeoffsRequest) -> operations.ListHrisTimeoffsResponse:
         r"""List all timeoffs"""
         hook_ctx = HookContext(operation_id='listHrisTimeoffs', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListHrisTimeoffsRequest, base_url, '/hris/{connection_id}/timeoff', request)
+        url = utils.generate_url(base_url, '/hris/{connection_id}/timeoff', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListHrisTimeoffsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/transaction.py` & `Unified-python-sdk-0.21.4/src/unified_to/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_accounting_transaction(self, request: operations.CreateAccountingTransactionRequest) -> operations.CreateAccountingTransactionResponse:
         r"""Create a transaction"""
         hook_ctx = HookContext(operation_id='createAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_accounting_transaction(self, request: operations.GetAccountingTransactionRequest) -> operations.GetAccountingTransactionResponse:
         r"""Retrieve a transaction"""
         hook_ctx = HookContext(operation_id='getAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetAccountingTransactionRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_accounting_transactions(self, request: operations.ListAccountingTransactionsRequest) -> operations.ListAccountingTransactionsResponse:
         r"""List all transactions"""
         hook_ctx = HookContext(operation_id='listAccountingTransactions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListAccountingTransactionsRequest, base_url, '/accounting/{connection_id}/transaction', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListAccountingTransactionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,15 +183,15 @@
     
     
     def patch_accounting_transaction(self, request: operations.PatchAccountingTransactionRequest) -> operations.PatchAccountingTransactionResponse:
         r"""Update a transaction"""
         hook_ctx = HookContext(operation_id='patchAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
@@ -240,15 +240,15 @@
     
     
     def remove_accounting_transaction(self, request: operations.RemoveAccountingTransactionRequest) -> operations.RemoveAccountingTransactionResponse:
         r"""Remove a transaction"""
         hook_ctx = HookContext(operation_id='removeAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -294,15 +294,15 @@
     
     
     def update_accounting_transaction(self, request: operations.UpdateAccountingTransactionRequest) -> operations.UpdateAccountingTransactionResponse:
         r"""Update a transaction"""
         hook_ctx = HookContext(operation_id='updateAccountingTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateAccountingTransactionRequest, base_url, '/accounting/{connection_id}/transaction/{id}', request)
+        url = utils.generate_url(base_url, '/accounting/{connection_id}/transaction/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateAccountingTransactionRequest, "accounting_transaction", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/uc.py` & `Unified-python-sdk-0.21.4/src/unified_to/uc.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     
     
     def create_uc_contact(self, request: operations.CreateUcContactRequest) -> operations.CreateUcContactResponse:
         r"""Create a contact"""
         hook_ctx = HookContext(operation_id='createUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.CreateUcContactRequest, base_url, '/uc/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUcContactRequest, "uc_contact", False, True, 'json')
@@ -73,22 +73,22 @@
     
     
     def get_uc_contact(self, request: operations.GetUcContactRequest) -> operations.GetUcContactResponse:
         r"""Retrieve a contact"""
         hook_ctx = HookContext(operation_id='getUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUcContactRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -128,22 +128,22 @@
     
     
     def list_uc_calls(self, request: operations.ListUcCallsRequest) -> operations.ListUcCallsResponse:
         r"""List all calls"""
         hook_ctx = HookContext(operation_id='listUcCalls', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUcCallsRequest, base_url, '/uc/{connection_id}/call', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/call', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUcCallsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -183,22 +183,22 @@
     
     
     def list_uc_contacts(self, request: operations.ListUcContactsRequest) -> operations.ListUcContactsResponse:
         r"""List all contacts"""
         hook_ctx = HookContext(operation_id='listUcContacts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUcContactsRequest, base_url, '/uc/{connection_id}/contact', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUcContactsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -238,15 +238,15 @@
     
     
     def patch_uc_contact(self, request: operations.PatchUcContactRequest) -> operations.PatchUcContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='patchUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchUcContactRequest, "uc_contact", False, True, 'json')
@@ -295,15 +295,15 @@
     
     
     def remove_uc_contact(self, request: operations.RemoveUcContactRequest) -> operations.RemoveUcContactResponse:
         r"""Remove a contact"""
         hook_ctx = HookContext(operation_id='removeUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -349,15 +349,15 @@
     
     
     def update_uc_contact(self, request: operations.UpdateUcContactRequest) -> operations.UpdateUcContactResponse:
         r"""Update a contact"""
         hook_ctx = HookContext(operation_id='updateUcContact', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUcContactRequest, base_url, '/uc/{connection_id}/contact/{id}', request)
+        url = utils.generate_url(base_url, '/uc/{connection_id}/contact/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUcContactRequest, "uc_contact", False, True, 'json')
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/unified.py` & `Unified-python-sdk-0.21.4/src/unified_to/unified.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,15 +85,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUnifiedWebhookRequest, "webhook", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.CreateUnifiedWebhookRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -133,15 +133,15 @@
     
     
     def get_unified_apicall(self, request: operations.GetUnifiedApicallRequest) -> operations.GetUnifiedApicallResponse:
         r"""Retrieve specific API Call by its ID"""
         hook_ctx = HookContext(operation_id='getUnifiedApicall', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedApicallRequest, base_url, '/unified/apicall/{id}', request)
+        url = utils.generate_url(base_url, '/unified/apicall/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -187,15 +187,15 @@
     
     
     def get_unified_connection(self, request: operations.GetUnifiedConnectionRequest) -> operations.GetUnifiedConnectionResponse:
         r"""Retrieve connection"""
         hook_ctx = HookContext(operation_id='getUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -243,22 +243,22 @@
     def get_unified_integration_auth(self, request: operations.GetUnifiedIntegrationAuthRequest) -> operations.GetUnifiedIntegrationAuthResponse:
         r"""Create connection indirectly
         Returns an authorization URL for the specified integration.  Once a successful authorization occurs, a new connection is created.
         """
         hook_ctx = HookContext(operation_id='getUnifiedIntegrationAuth', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedIntegrationAuthRequest, base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
+        url = utils.generate_url(base_url, '/unified/integration/auth/{workspace_id}/{integration_type}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.GetUnifiedIntegrationAuthRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'text/plain'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -297,15 +297,15 @@
     
     
     def get_unified_webhook(self, request: operations.GetUnifiedWebhookRequest) -> operations.GetUnifiedWebhookResponse:
         r"""Retrieve webhook by its ID"""
         hook_ctx = HookContext(operation_id='getUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedWebhookRequest, base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -358,15 +358,15 @@
         url = base_url + '/unified/apicall'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedApicallsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -413,15 +413,15 @@
         url = base_url + '/unified/connection'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedConnectionsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -463,22 +463,22 @@
     def list_unified_integration_workspaces(self, request: operations.ListUnifiedIntegrationWorkspacesRequest) -> operations.ListUnifiedIntegrationWorkspacesResponse:
         r"""Returns all activated integrations in a workspace
         No authentication required as this is to be used by front-end interface
         """
         hook_ctx = HookContext(operation_id='listUnifiedIntegrationWorkspaces', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListUnifiedIntegrationWorkspacesRequest, base_url, '/unified/integration/workspace/{workspace_id}', request)
+        url = utils.generate_url(base_url, '/unified/integration/workspace/{workspace_id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIntegrationWorkspacesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -525,15 +525,15 @@
         url = base_url + '/unified/integration'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIntegrationsRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -580,15 +580,15 @@
         url = base_url + '/unified/issue'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedIssuesRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -635,15 +635,15 @@
         url = base_url + '/unified/webhook'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedWebhooksRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -683,15 +683,15 @@
     
     
     def patch_unified_connection(self, request: operations.PatchUnifiedConnectionRequest) -> operations.PatchUnifiedConnectionResponse:
         r"""Update connection"""
         hook_ctx = HookContext(operation_id='patchUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.PatchUnifiedConnectionRequest, "connection", False, True, 'json')
@@ -740,15 +740,15 @@
     
     
     def patch_unified_webhook_trigger(self, request: operations.PatchUnifiedWebhookTriggerRequest) -> operations.PatchUnifiedWebhookTriggerResponse:
         r"""Trigger webhook"""
         hook_ctx = HookContext(operation_id='patchUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUnifiedWebhookTriggerRequest, base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -794,15 +794,15 @@
     
     
     def remove_unified_connection(self, request: operations.RemoveUnifiedConnectionRequest) -> operations.RemoveUnifiedConnectionResponse:
         r"""Remove connection"""
         hook_ctx = HookContext(operation_id='removeUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -848,15 +848,15 @@
     
     
     def remove_unified_webhook(self, request: operations.RemoveUnifiedWebhookRequest) -> operations.RemoveUnifiedWebhookResponse:
         r"""Remove webhook subscription"""
         hook_ctx = HookContext(operation_id='removeUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUnifiedWebhookRequest, base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -902,15 +902,15 @@
     
     
     def update_unified_connection(self, request: operations.UpdateUnifiedConnectionRequest) -> operations.UpdateUnifiedConnectionResponse:
         r"""Update connection"""
         hook_ctx = HookContext(operation_id='updateUnifiedConnection', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUnifiedConnectionRequest, base_url, '/unified/connection/{id}', request)
+        url = utils.generate_url(base_url, '/unified/connection/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUnifiedConnectionRequest, "connection", False, True, 'json')
@@ -959,15 +959,15 @@
     
     
     def update_unified_webhook_trigger(self, request: operations.UpdateUnifiedWebhookTriggerRequest) -> operations.UpdateUnifiedWebhookTriggerResponse:
         r"""Trigger webhook"""
         hook_ctx = HookContext(operation_id='updateUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUnifiedWebhookTriggerRequest, base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/utils/retries.py` & `Unified-python-sdk-0.21.4/src/unified_to/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/utils/utils.py` & `Unified-python-sdk-0.21.4/src/unified_to/utils/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,16 +5,25 @@
 import re
 import sys
 from dataclasses import Field, fields, is_dataclass, make_dataclass
 from datetime import date, datetime
 from decimal import Decimal
 from email.message import Message
 from enum import Enum
-from typing import (Any, Callable, Dict, List, Optional, Tuple, Union,
-                    get_args, get_origin)
+from typing import (
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    get_args,
+    get_origin,
+)
 from xmlrpc.client import boolean
 from typing_inspect import is_optional_type
 import dateutil.parser
 from dataclasses_json import DataClassJsonMixin
 
 
 def get_security(security: Any) -> Tuple[Dict[str, str], Dict[str, str]]:
@@ -26,470 +35,600 @@
 
     sec_fields: Tuple[Field, ...] = fields(security)
     for sec_field in sec_fields:
         value = getattr(security, sec_field.name)
         if value is None:
             continue
 
-        metadata = sec_field.metadata.get('security')
+        metadata = sec_field.metadata.get("security")
         if metadata is None:
             continue
-        if metadata.get('option'):
+        if metadata.get("option"):
             _parse_security_option(headers, query_params, value)
             return headers, query_params
-        if metadata.get('scheme'):
+        if metadata.get("scheme"):
             # Special case for basic auth which could be a flattened struct
             if metadata.get("sub_type") == "basic" and not is_dataclass(value):
                 _parse_security_scheme(headers, query_params, metadata, security)
             else:
                 _parse_security_scheme(headers, query_params, metadata, value)
 
     return headers, query_params
 
 
-def _parse_security_option(headers: Dict[str, str], query_params: Dict[str, str], option: Any):
+def _parse_security_option(
+    headers: Dict[str, str], query_params: Dict[str, str], option: Any
+):
     opt_fields: Tuple[Field, ...] = fields(option)
     for opt_field in opt_fields:
-        metadata = opt_field.metadata.get('security')
-        if metadata is None or metadata.get('scheme') is None:
+        metadata = opt_field.metadata.get("security")
+        if metadata is None or metadata.get("scheme") is None:
             continue
         _parse_security_scheme(
-            headers, query_params, metadata, getattr(option, opt_field.name))
+            headers, query_params, metadata, getattr(option, opt_field.name)
+        )
 
 
-def _parse_security_scheme(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, scheme: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    scheme: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
     if is_dataclass(scheme):
-        if scheme_type == 'http' and sub_type == 'basic':
+        if scheme_type == "http" and sub_type == "basic":
             _parse_basic_auth_scheme(headers, scheme)
             return
 
         scheme_fields: Tuple[Field, ...] = fields(scheme)
         for scheme_field in scheme_fields:
-            metadata = scheme_field.metadata.get('security')
-            if metadata is None or metadata.get('field_name') is None:
+            metadata = scheme_field.metadata.get("security")
+            if metadata is None or metadata.get("field_name") is None:
                 continue
 
             value = getattr(scheme, scheme_field.name)
 
             _parse_security_scheme_value(
-                headers, query_params, scheme_metadata, metadata, value)
+                headers, query_params, scheme_metadata, metadata, value
+            )
     else:
         _parse_security_scheme_value(
-            headers, query_params, scheme_metadata, scheme_metadata, scheme)
+            headers, query_params, scheme_metadata, scheme_metadata, scheme
+        )
 
 
-def _parse_security_scheme_value(headers: Dict[str, str], query_params: Dict[str, str], scheme_metadata: Dict, security_metadata: Dict, value: Any):
-    scheme_type = scheme_metadata.get('type')
-    sub_type = scheme_metadata.get('sub_type')
+def _parse_security_scheme_value(
+    headers: Dict[str, str],
+    query_params: Dict[str, str],
+    scheme_metadata: Dict,
+    security_metadata: Dict,
+    value: Any,
+):
+    scheme_type = scheme_metadata.get("type")
+    sub_type = scheme_metadata.get("sub_type")
 
-    header_name = str(security_metadata.get('field_name'))
+    header_name = str(security_metadata.get("field_name"))
 
     if scheme_type == "apiKey":
-        if sub_type == 'header':
+        if sub_type == "header":
             headers[header_name] = value
-        elif sub_type == 'query':
+        elif sub_type == "query":
             query_params[header_name] = value
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     elif scheme_type == "openIdConnect":
         headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'oauth2':
-        if sub_type != 'client_credentials':
+    elif scheme_type == "oauth2":
+        if sub_type != "client_credentials":
             headers[header_name] = _apply_bearer(value)
-    elif scheme_type == 'http':
-        if sub_type == 'bearer':
+    elif scheme_type == "http":
+        if sub_type == "bearer":
             headers[header_name] = _apply_bearer(value)
         else:
-            raise Exception('not supported')
+            raise Exception("not supported")
     else:
-        raise Exception('not supported')
+        raise Exception("not supported")
 
 
 def _apply_bearer(token: str) -> str:
-    return token.lower().startswith('bearer ') and token or f'Bearer {token}'
+    return token.lower().startswith("bearer ") and token or f"Bearer {token}"
 
 
 def _parse_basic_auth_scheme(headers: Dict[str, str], scheme: Any):
     username = ""
     password = ""
 
     scheme_fields: Tuple[Field, ...] = fields(scheme)
     for scheme_field in scheme_fields:
-        metadata = scheme_field.metadata.get('security')
-        if metadata is None or metadata.get('field_name') is None:
+        metadata = scheme_field.metadata.get("security")
+        if metadata is None or metadata.get("field_name") is None:
             continue
 
-        field_name = metadata.get('field_name')
+        field_name = metadata.get("field_name")
         value = getattr(scheme, scheme_field.name)
 
-        if field_name == 'username':
+        if field_name == "username":
             username = value
-        if field_name == 'password':
+        if field_name == "password":
             password = value
 
-    data = f'{username}:{password}'.encode()
-    headers['Authorization'] = f'Basic {base64.b64encode(data).decode()}'
+    data = f"{username}:{password}".encode()
+    headers["Authorization"] = f"Basic {base64.b64encode(data).decode()}"
 
 
-def generate_url(clazz: type, server_url: str, path: str, path_params: Any,
-                 gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> str:
-    path_param_fields: Tuple[Field, ...] = fields(clazz)
+def generate_url(
+    server_url: str,
+    path: str,
+    path_params: Any,
+    gbls: Optional[Any] = None,
+) -> str:
+    path_param_values: Dict[str, str] = {}
+
+    globals_already_populated = _populate_path_params(
+        path_params, gbls, path_param_values, []
+    )
+    if gbls is not None:
+        _populate_path_params(gbls, None, path_param_values, globals_already_populated)
+
+    for key, value in path_param_values.items():
+        path = path.replace("{" + key + "}", value, 1)
+
+    return remove_suffix(server_url, "/") + path
+
+
+def _populate_path_params(
+    path_params: Any,
+    gbls: Any,
+    path_param_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    path_param_fields: Tuple[Field, ...] = fields(path_params)
     for field in path_param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        param_metadata = field.metadata.get('path_param')
+        param_metadata = field.metadata.get("path_param")
         if param_metadata is None:
             continue
 
-        param = getattr(
-            path_params, field.name) if path_params is not None else None
-        param = _populate_from_globals(
-            field.name, param, 'pathParam', gbls)
+        param = getattr(path_params, field.name) if path_params is not None else None
+        param, global_found = _populate_from_globals(
+            field.name, param, "path_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
 
         if param is None:
             continue
 
         f_name = param_metadata.get("field_name", field.name)
-        serialization = param_metadata.get('serialization', '')
-        if serialization != '':
+        serialization = param_metadata.get("serialization", "")
+        if serialization != "":
             serialized_params = _get_serialized_params(
-                param_metadata, field.type, f_name, param)
+                param_metadata, field.type, f_name, param
+            )
             for key, value in serialized_params.items():
-                path = path.replace(
-                    '{' + key + '}', value, 1)
+                path_param_values[key] = value
         else:
-            if param_metadata.get('style', 'simple') == 'simple':
+            if param_metadata.get("style", "simple") == "simple":
                 if isinstance(param, List):
                     pp_vals: List[str] = []
                     for pp_val in param:
                         if pp_val is None:
                             continue
                         pp_vals.append(_val_to_string(pp_val))
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif isinstance(param, Dict):
                     pp_vals: List[str] = []
                     for pp_key in param:
                         if param[pp_key] is None:
                             continue
-                        if param_metadata.get('explode'):
-                            pp_vals.append(
-                                f"{pp_key}={_val_to_string(param[pp_key])}")
+                        if param_metadata.get("explode"):
+                            pp_vals.append(f"{pp_key}={_val_to_string(param[pp_key])}")
                         else:
-                            pp_vals.append(
-                                f"{pp_key},{_val_to_string(param[pp_key])}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                            pp_vals.append(f"{pp_key},{_val_to_string(param[pp_key])}")
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 elif not isinstance(param, (str, int, float, complex, bool, Decimal)):
                     pp_vals: List[str] = []
                     param_fields: Tuple[Field, ...] = fields(param)
                     for param_field in param_fields:
-                        param_value_metadata = param_field.metadata.get(
-                            'path_param')
+                        param_value_metadata = param_field.metadata.get("path_param")
                         if not param_value_metadata:
                             continue
 
-                        parm_name = param_value_metadata.get(
-                            'field_name', field.name)
+                        param_name = param_value_metadata.get("field_name", field.name)
 
                         param_field_val = getattr(param, param_field.name)
                         if param_field_val is None:
                             continue
-                        if param_metadata.get('explode'):
+                        if param_metadata.get("explode"):
                             pp_vals.append(
-                                f"{parm_name}={_val_to_string(param_field_val)}")
+                                f"{param_name}={_val_to_string(param_field_val)}"
+                            )
                         else:
                             pp_vals.append(
-                                f"{parm_name},{_val_to_string(param_field_val)}")
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', ",".join(pp_vals), 1)
+                                f"{param_name},{_val_to_string(param_field_val)}"
+                            )
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        ",".join(pp_vals)
+                    )
                 else:
-                    path = path.replace(
-                        '{' + param_metadata.get('field_name', field.name) + '}', _val_to_string(param), 1)
+                    path_param_values[param_metadata.get("field_name", field.name)] = (
+                        _val_to_string(param)
+                    )
 
-    return remove_suffix(server_url, '/') + path
+    return globals_already_populated
 
 
 def is_optional(field):
     return get_origin(field) is Union and type(None) in get_args(field)
 
 
 def template_url(url_with_params: str, params: Dict[str, str]) -> str:
     for key, value in params.items():
-        url_with_params = url_with_params.replace(
-            '{' + key + '}', value)
+        url_with_params = url_with_params.replace("{" + key + "}", value)
 
     return url_with_params
 
 
-def get_query_params(clazz: type, query_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[
-        str, List[str]]:
+def get_query_params(
+    query_params: Any,
+    gbls: Optional[Any] = None,
+) -> Dict[str, List[str]]:
     params: Dict[str, List[str]] = {}
 
-    param_fields: Tuple[Field, ...] = fields(clazz)
+    globals_already_populated = _populate_query_params(query_params, gbls, params, [])
+    if gbls is not None:
+        _populate_query_params(gbls, None, params, globals_already_populated)
+
+    return params
+
+
+def _populate_query_params(
+    query_params: Any,
+    gbls: Any,
+    query_param_values: Dict[str, List[str]],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(query_params)
     for field in param_fields:
-        request_metadata = field.metadata.get('request')
-        if request_metadata is not None:
+        if field.name in skip_fields:
             continue
 
-        metadata = field.metadata.get('query_param')
+        metadata = field.metadata.get("query_param")
         if not metadata:
             continue
 
         param_name = field.name
-        value = getattr(
-            query_params, param_name) if query_params is not None else None
+        value = getattr(query_params, param_name) if query_params is not None else None
 
-        value = _populate_from_globals(param_name, value, 'queryParam', gbls)
+        value, global_found = _populate_from_globals(
+            param_name, value, "query_param", gbls
+        )
+        if global_found:
+            globals_already_populated.append(param_name)
 
         f_name = metadata.get("field_name")
-        serialization = metadata.get('serialization', '')
-        if serialization != '':
+        serialization = metadata.get("serialization", "")
+        if serialization != "":
             serialized_parms = _get_serialized_params(
-                metadata, field.type, f_name, value)
+                metadata, field.type, f_name, value
+            )
             for key, value in serialized_parms.items():
-                if key in params:
-                    params[key].extend(value)
+                if key in query_param_values:
+                    query_param_values[key].extend(value)
                 else:
-                    params[key] = [value]
+                    query_param_values[key] = [value]
         else:
-            style = metadata.get('style', 'form')
-            if style == 'deepObject':
-                params = {**params, **_get_deep_object_query_params(
-                    metadata, f_name, value)}
-            elif style == 'form':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, ",")}
-            elif style == 'pipeDelimited':
-                params = {**params, **_get_delimited_query_params(
-                    metadata, f_name, value, "|")}
+            style = metadata.get("style", "form")
+            if style == "deepObject":
+                _populate_deep_object_query_params(
+                    metadata, f_name, value, query_param_values
+                )
+            elif style == "form":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, ",", query_param_values
+                )
+            elif style == "pipeDelimited":
+                _populate_delimited_query_params(
+                    metadata, f_name, value, "|", query_param_values
+                )
             else:
-                raise Exception('not yet implemented')
-    return params
+                raise Exception("not yet implemented")
 
+    return globals_already_populated
 
-def get_headers(headers_params: Any, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]] = None) -> Dict[str, str]:
-    if headers_params is None:
-        return {}
 
+def get_headers(headers_params: Any, gbls: Optional[Any] = None) -> Dict[str, str]:
     headers: Dict[str, str] = {}
 
-    param_fields: Tuple[Field, ...] = fields(headers_params)
-    for field in param_fields:
-        metadata = field.metadata.get('header')
-        if not metadata:
-            continue
+    globals_already_populated = []
+    if headers_params is not None:
+        globals_already_populated = _populate_headers(headers_params, gbls, headers, [])
+    if gbls is not None:
+        _populate_headers(gbls, None, headers, globals_already_populated)
 
-        value = _populate_from_globals(field.name, getattr(headers_params, field.name), 'header', gbls)
-        value = _serialize_header(metadata.get('explode', False), value)
+    return headers
 
-        if value != '':
-            headers[metadata.get('field_name', field.name)] = value
 
-    return headers
+def _populate_headers(
+    headers_params: Any,
+    gbls: Any,
+    header_values: Dict[str, str],
+    skip_fields: List[str],
+) -> List[str]:
+    globals_already_populated: List[str] = []
+
+    param_fields: Tuple[Field, ...] = fields(headers_params)
+    for field in param_fields:
+        if field.name in skip_fields:
+            continue
 
+        metadata = field.metadata.get("header")
+        if not metadata:
+            continue
 
-def _get_serialized_params(metadata: Dict, field_type: type, field_name: str, obj: Any) -> Dict[str, str]:
+        value, global_found = _populate_from_globals(
+            field.name, getattr(headers_params, field.name), "header", gbls
+        )
+        if global_found:
+            globals_already_populated.append(field.name)
+        value = _serialize_header(metadata.get("explode", False), value)
+
+        if value != "":
+            header_values[metadata.get("field_name", field.name)] = value
+
+    return globals_already_populated
+
+
+def _get_serialized_params(
+    metadata: Dict, field_type: type, field_name: str, obj: Any
+) -> Dict[str, str]:
     params: Dict[str, str] = {}
 
-    serialization = metadata.get('serialization', '')
-    if serialization == 'json':
-        params[metadata.get("field_name", field_name)
-               ] = marshal_json(obj, field_type)
+    serialization = metadata.get("serialization", "")
+    if serialization == "json":
+        params[metadata.get("field_name", field_name)] = marshal_json(obj, field_type)
 
     return params
 
 
-def _get_deep_object_query_params(metadata: Dict, field_name: str, obj: Any) -> Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_deep_object_query_params(
+    metadata: Dict, field_name: str, obj: Any, params: Dict[str, List[str]]
+):
     if obj is None:
-        return params
+        return
 
     if is_dataclass(obj):
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('query_param')
+            obj_param_metadata = obj_field.metadata.get("query_param")
             if not obj_param_metadata:
                 continue
 
             obj_val = getattr(obj, obj_field.name)
             if obj_val is None:
                 continue
 
             if isinstance(obj_val, List):
                 for val in obj_val:
                     if val is None:
                         continue
 
-                    if params.get(
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]') is None:
+                    if (
+                        params.get(
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        )
+                        is None
+                    ):
                         params[
-                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                        ]
+                            f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                        ] = []
 
                     params[
-                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'].append(
-                        _val_to_string(val))
+                        f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                    ].append(_val_to_string(val))
             else:
                 params[
-                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'] = [
-                    _val_to_string(obj_val)]
+                    f'{metadata.get("field_name", field_name)}[{obj_param_metadata.get("field_name", obj_field.name)}]'
+                ] = [_val_to_string(obj_val)]
     elif isinstance(obj, Dict):
         for key, value in obj.items():
             if value is None:
                 continue
 
             if isinstance(value, List):
                 for val in value:
                     if val is None:
                         continue
 
-                    if params.get(f'{metadata.get("field_name", field_name)}[{key}]') is None:
-                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                        ]
-
-                    params[
-                        f'{metadata.get("field_name", field_name)}[{key}]'].append(_val_to_string(val))
+                    if (
+                        params.get(f'{metadata.get("field_name", field_name)}[{key}]')
+                        is None
+                    ):
+                        params[f'{metadata.get("field_name", field_name)}[{key}]'] = []
+
+                    params[f'{metadata.get("field_name", field_name)}[{key}]'].append(
+                        _val_to_string(val)
+                    )
             else:
                 params[f'{metadata.get("field_name", field_name)}[{key}]'] = [
-                    _val_to_string(value)]
-    return params
+                    _val_to_string(value)
+                ]
 
 
 def _get_query_param_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('query_param')
+    obj_param_metadata = obj_field.metadata.get("query_param")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _get_delimited_query_params(metadata: Dict, field_name: str, obj: Any, delimiter: str) -> Dict[
-        str, List[str]]:
-    return _populate_form(field_name, metadata.get("explode", True), obj, _get_query_param_field_name, delimiter)
+def _populate_delimited_query_params(
+    metadata: Dict,
+    field_name: str,
+    obj: Any,
+    delimiter: str,
+    query_param_values: Dict[str, List[str]],
+):
+    _populate_form(
+        field_name,
+        metadata.get("explode", True),
+        obj,
+        _get_query_param_field_name,
+        delimiter,
+        query_param_values,
+    )
 
 
 SERIALIZATION_METHOD_TO_CONTENT_TYPE = {
-    'json': 'application/json',
-    'form': 'application/x-www-form-urlencoded',
-    'multipart': 'multipart/form-data',
-    'raw': 'application/octet-stream',
-    'string': 'text/plain',
+    "json": "application/json",
+    "form": "application/x-www-form-urlencoded",
+    "multipart": "multipart/form-data",
+    "raw": "application/octet-stream",
+    "string": "text/plain",
 }
 
 
-def serialize_request_body(request: Any, request_type: type, request_field_name: str, nullable: bool, optional: bool, serialization_method: str, encoder=None) -> Tuple[
-        Optional[str], Optional[Any], Optional[Any]]:
+def serialize_request_body(
+    request: Any,
+    request_type: type,
+    request_field_name: str,
+    nullable: bool,
+    optional: bool,
+    serialization_method: str,
+    encoder=None,
+) -> Tuple[Optional[str], Optional[Any], Optional[Any]]:
     if request is None:
         if not nullable and optional:
             return None, None, None
 
     if not is_dataclass(request) or not hasattr(request, request_field_name):
-        return serialize_content_type(request_field_name, request_type, SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
-                                      request, encoder)
+        return serialize_content_type(
+            request_field_name,
+            request_type,
+            SERIALIZATION_METHOD_TO_CONTENT_TYPE[serialization_method],
+            request,
+            encoder,
+        )
 
     request_val = getattr(request, request_field_name)
 
     if request_val is None:
         if not nullable and optional:
             return None, None, None
 
     request_fields: Tuple[Field, ...] = fields(request)
     request_metadata = None
 
     for field in request_fields:
         if field.name == request_field_name:
-            request_metadata = field.metadata.get('request')
+            request_metadata = field.metadata.get("request")
             break
 
     if request_metadata is None:
-        raise Exception('invalid request type')
+        raise Exception("invalid request type")
 
-    return serialize_content_type(request_field_name, request_type, request_metadata.get('media_type', 'application/octet-stream'),
-                                  request_val)
+    return serialize_content_type(
+        request_field_name,
+        request_type,
+        request_metadata.get("media_type", "application/octet-stream"),
+        request_val,
+    )
 
 
-def serialize_content_type(field_name: str, request_type: Any, media_type: str, request: Any, encoder=None) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
-    if re.match(r'(application|text)\/.*?\+*json.*', media_type) is not None:
+def serialize_content_type(
+    field_name: str, request_type: Any, media_type: str, request: Any, encoder=None
+) -> Tuple[Optional[str], Optional[Any], Optional[List[List[Any]]]]:
+    if re.match(r"(application|text)\/.*?\+*json.*", media_type) is not None:
         return media_type, marshal_json(request, request_type, encoder), None
-    if re.match(r'multipart\/.*', media_type) is not None:
+    if re.match(r"multipart\/.*", media_type) is not None:
         return serialize_multipart_form(media_type, request)
-    if re.match(r'application\/x-www-form-urlencoded.*', media_type) is not None:
+    if re.match(r"application\/x-www-form-urlencoded.*", media_type) is not None:
         return media_type, serialize_form_data(field_name, request), None
     if isinstance(request, (bytes, bytearray)):
         return media_type, request, None
     if isinstance(request, str):
         return media_type, request, None
 
     raise Exception(
-        f"invalid request body type {type(request)} for mediaType {media_type}")
+        f"invalid request body type {type(request)} for mediaType {media_type}"
+    )
 
 
-def serialize_multipart_form(media_type: str, request: Any) -> Tuple[str, Any, List[List[Any]]]:
+def serialize_multipart_form(
+    media_type: str, request: Any
+) -> Tuple[str, Any, List[List[Any]]]:
     form: List[List[Any]] = []
     request_fields = fields(request)
 
     for field in request_fields:
         val = getattr(request, field.name)
         if val is None:
             continue
 
-        field_metadata = field.metadata.get('multipart_form')
+        field_metadata = field.metadata.get("multipart_form")
         if not field_metadata:
             continue
 
         if field_metadata.get("file") is True:
             file_fields = fields(val)
 
             file_name = ""
             field_name = ""
             content = bytes()
 
             for file_field in file_fields:
-                file_metadata = file_field.metadata.get('multipart_form')
+                file_metadata = file_field.metadata.get("multipart_form")
                 if file_metadata is None:
                     continue
 
                 if file_metadata.get("content") is True:
                     content = getattr(val, file_field.name)
                 else:
-                    field_name = file_metadata.get(
-                        "field_name", file_field.name)
+                    field_name = file_metadata.get("field_name", file_field.name)
                     file_name = getattr(val, file_field.name)
             if field_name == "" or file_name == "" or content == bytes():
-                raise Exception('invalid multipart/form-data file')
+                raise Exception("invalid multipart/form-data file")
 
             form.append([field_name, [file_name, content]])
         elif field_metadata.get("json") is True:
-            to_append = [field_metadata.get("field_name", field.name), [
-                None, marshal_json(val, field.type), "application/json"]]
+            to_append = [
+                field_metadata.get("field_name", field.name),
+                [None, marshal_json(val, field.type), "application/json"],
+            ]
             form.append(to_append)
         else:
-            field_name = field_metadata.get(
-                "field_name", field.name)
+            field_name = field_metadata.get("field_name", field.name)
             if isinstance(val, List):
                 for value in val:
                     if value is None:
                         continue
-                    form.append(
-                        [field_name + "[]", [None, _val_to_string(value)]])
+                    form.append([field_name + "[]", [None, _val_to_string(value)]])
             else:
                 form.append([field_name, [None, _val_to_string(val)]])
     return media_type, None, form
 
 
-def serialize_dict(original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]) -> Dict[
-        str, List[str]]:
+def serialize_dict(
+    original: Dict, explode: bool, field_name, existing: Optional[Dict[str, List[str]]]
+) -> Dict[str, List[str]]:
     if existing is None:
         existing = {}
 
     if explode is True:
         for key, val in original.items():
             if key not in existing:
                 existing[key] = []
@@ -510,215 +649,218 @@
 
     if is_dataclass(data):
         for field in fields(data):
             val = getattr(data, field.name)
             if val is None:
                 continue
 
-            metadata = field.metadata.get('form')
+            metadata = field.metadata.get("form")
             if metadata is None:
                 continue
 
-            field_name = metadata.get('field_name', field.name)
+            field_name = metadata.get("field_name", field.name)
 
-            if metadata.get('json'):
+            if metadata.get("json"):
                 form[field_name] = [marshal_json(val, field.type)]
             else:
-                if metadata.get('style', 'form') == 'form':
-                    form = {**form, **_populate_form(
-                        field_name, metadata.get('explode', True), val, _get_form_field_name, ",")}
+                if metadata.get("style", "form") == "form":
+                    _populate_form(
+                        field_name,
+                        metadata.get("explode", True),
+                        val,
+                        _get_form_field_name,
+                        ",",
+                        form,
+                    )
                 else:
-                    raise Exception(
-                        f'Invalid form style for field {field.name}')
+                    raise Exception(f"Invalid form style for field {field.name}")
     elif isinstance(data, Dict):
         for key, value in data.items():
             form[key] = [_val_to_string(value)]
     else:
-        raise Exception(f'Invalid request body type for field {field_name}')
+        raise Exception(f"Invalid request body type for field {field_name}")
 
     return form
 
 
 def _get_form_field_name(obj_field: Field) -> str:
-    obj_param_metadata = obj_field.metadata.get('form')
+    obj_param_metadata = obj_field.metadata.get("form")
 
     if not obj_param_metadata:
         return ""
 
     return obj_param_metadata.get("field_name", obj_field.name)
 
 
-def _populate_form(field_name: str, explode: boolean, obj: Any, get_field_name_func: Callable, delimiter: str) -> \
-        Dict[str, List[str]]:
-    params: Dict[str, List[str]] = {}
-
+def _populate_form(
+    field_name: str,
+    explode: boolean,
+    obj: Any,
+    get_field_name_func: Callable,
+    delimiter: str,
+    form: Dict[str, List[str]],
+):
     if obj is None:
-        return params
+        return form
 
     if is_dataclass(obj):
         items = []
 
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
             obj_field_name = get_field_name_func(obj_field)
-            if obj_field_name == '':
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                params[obj_field_name] = [_val_to_string(val)]
+                form[obj_field_name] = [_val_to_string(val)]
             else:
-                items.append(
-                    f'{obj_field_name}{delimiter}{_val_to_string(val)}')
+                items.append(f"{obj_field_name}{delimiter}{_val_to_string(val)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, Dict):
         items = []
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                params[key] = [_val_to_string(value)]
+                form[key] = [_val_to_string(value)]
             else:
-                items.append(f'{key}{delimiter}{_val_to_string(value)}')
+                items.append(f"{key}{delimiter}{_val_to_string(value)}")
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(items)]
+            form[field_name] = [delimiter.join(items)]
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             if explode:
-                if not field_name in params:
-                    params[field_name] = []
-                params[field_name].append(_val_to_string(value))
+                if not field_name in form:
+                    form[field_name] = []
+                form[field_name].append(_val_to_string(value))
             else:
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            params[field_name] = [delimiter.join(
-                [str(item) for item in items])]
+            form[field_name] = [delimiter.join([str(item) for item in items])]
     else:
-        params[field_name] = [_val_to_string(obj)]
+        form[field_name] = [_val_to_string(obj)]
 
-    return params
+    return form
 
 
 def _serialize_header(explode: bool, obj: Any) -> str:
     if obj is None:
-        return ''
+        return ""
 
     if is_dataclass(obj):
         items = []
         obj_fields: Tuple[Field, ...] = fields(obj)
         for obj_field in obj_fields:
-            obj_param_metadata = obj_field.metadata.get('header')
+            obj_param_metadata = obj_field.metadata.get("header")
 
             if not obj_param_metadata:
                 continue
 
-            obj_field_name = obj_param_metadata.get(
-                'field_name', obj_field.name)
-            if obj_field_name == '':
+            obj_field_name = obj_param_metadata.get("field_name", obj_field.name)
+            if obj_field_name == "":
                 continue
 
             val = getattr(obj, obj_field.name)
             if val is None:
                 continue
 
             if explode:
-                items.append(
-                    f'{obj_field_name}={_val_to_string(val)}')
+                items.append(f"{obj_field_name}={_val_to_string(val)}")
             else:
                 items.append(obj_field_name)
                 items.append(_val_to_string(val))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     elif isinstance(obj, Dict):
         items = []
 
         for key, value in obj.items():
             if value is None:
                 continue
 
             if explode:
-                items.append(f'{key}={_val_to_string(value)}')
+                items.append(f"{key}={_val_to_string(value)}")
             else:
                 items.append(key)
                 items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join([str(item) for item in items])
+            return ",".join([str(item) for item in items])
     elif isinstance(obj, List):
         items = []
 
         for value in obj:
             if value is None:
                 continue
 
             items.append(_val_to_string(value))
 
         if len(items) > 0:
-            return ','.join(items)
+            return ",".join(items)
     else:
-        return f'{_val_to_string(obj)}'
+        return f"{_val_to_string(obj)}"
 
-    return ''
+    return ""
 
 
 def unmarshal_json(data, typ, decoder=None):
-    unmarshal = make_dataclass('Unmarshal', [('res', typ)],
-                               bases=(DataClassJsonMixin,))
+    unmarshal = make_dataclass("Unmarshal", [("res", typ)], bases=(DataClassJsonMixin,))
     json_dict = json.loads(data)
     try:
         out = unmarshal.from_dict({"res": json_dict})
     except AttributeError as attr_err:
         raise AttributeError(
-            f'unable to unmarshal {data} as {typ} - {attr_err}') from attr_err
+            f"unable to unmarshal {data} as {typ} - {attr_err}"
+        ) from attr_err
 
     return out.res if decoder is None else decoder(out.res)
 
 
 def marshal_json(val, typ, encoder=None):
     if not is_optional_type(typ) and val is None:
-        raise ValueError(
-            f"Could not marshal None into non-optional type: {typ}")
+        raise ValueError(f"Could not marshal None into non-optional type: {typ}")
 
-    marshal = make_dataclass('Marshal', [('res', typ)],
-                             bases=(DataClassJsonMixin,))
+    marshal = make_dataclass("Marshal", [("res", typ)], bases=(DataClassJsonMixin,))
     marshaller = marshal(res=val)
     json_dict = marshaller.to_dict()
     val = json_dict["res"] if encoder is None else encoder(json_dict["res"])
 
-    return json.dumps(val, separators=(',', ':'), sort_keys=True)
+    return json.dumps(val, separators=(",", ":"), sort_keys=True)
 
 
 def match_content_type(content_type: str, pattern: str) -> boolean:
     if pattern in (content_type, "*", "*/*"):
         return True
 
     msg = Message()
-    msg['content-type'] = content_type
+    msg["content-type"] = content_type
     media_type = msg.get_content_type()
 
     if media_type == pattern:
         return True
 
     parts = media_type.split("/")
     if len(parts) == 2:
-        if pattern in (f'{parts[0]}/*', f'*/{parts[1]}'):
+        if pattern in (f"{parts[0]}/*", f"*/{parts[1]}"):
             return True
 
     return False
 
 
 def match_status_codes(status_codes: List[str], status_code: int) -> bool:
     for code in status_codes:
@@ -835,64 +977,84 @@
 
 
 def union_encoder(all_encoders: Dict[str, Callable]):
     def selective_encoder(val: Any):
         if type(val) in all_encoders:
             return all_encoders[type(val)](val)
         return val
+
     return selective_encoder
 
 
 def union_decoder(all_decoders: List[Callable]):
     def selective_decoder(val: Any):
         decoded = val
         for decoder in all_decoders:
             try:
                 decoded = decoder(val)
                 break
             except (TypeError, ValueError):
                 continue
         return decoded
+
     return selective_decoder
 
 
 def get_field_name(name):
     def override(_, _field_name=name):
         return _field_name
 
     return override
 
 
 def _val_to_string(val) -> str:
     if isinstance(val, bool):
         return str(val).lower()
     if isinstance(val, datetime):
-        return str(val.isoformat().replace('+00:00', 'Z'))
+        return str(val.isoformat().replace("+00:00", "Z"))
     if isinstance(val, Enum):
         return str(val.value)
 
     return str(val)
 
 
-def _populate_from_globals(param_name: str, value: Any, param_type: str, gbls: Optional[Dict[str, Dict[str, Dict[str, Any]]]]):
-    if value is None and gbls is not None:
-        if 'parameters' in gbls:
-            if param_type in gbls['parameters']:
-                if param_name in gbls['parameters'][param_type]:
-                    global_value = gbls['parameters'][param_type][param_name]
-                    if global_value is not None:
-                        value = global_value
+def _populate_from_globals(
+    param_name: str, value: Any, param_type: str, gbls: Any
+) -> Tuple[Any, bool]:
+    if gbls is None:
+        return value, False
+
+    global_fields = fields(gbls)
+
+    found = False
+    for field in global_fields:
+        if field.name is not param_name:
+            continue
+
+        found = True
+
+        if value is not None:
+            return value, True
 
-    return value
+        global_value = getattr(gbls, field.name)
+
+        param_metadata = field.metadata.get(param_type)
+        if param_metadata is None:
+            return value, True
+
+        return global_value, True
+
+    return value, found
 
 
 def decoder_with_discriminator(field_name):
     def decode_fx(obj):
-        kls = getattr(sys.modules['sdk.models.shared'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.shared"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `Unified-python-sdk-0.21.3/src/unified_to/webhook.py` & `Unified-python-sdk-0.21.4/src/unified_to/webhook.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUnifiedWebhookRequest, "webhook", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
-        query_params = { **utils.get_query_params(operations.CreateUnifiedWebhookRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -76,15 +76,15 @@
     
     
     def get_unified_webhook(self, request: operations.GetUnifiedWebhookRequest) -> operations.GetUnifiedWebhookResponse:
         r"""Retrieve webhook by its ID"""
         hook_ctx = HookContext(operation_id='getUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUnifiedWebhookRequest, base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -137,15 +137,15 @@
         url = base_url + '/unified/webhook'
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        query_params = { **utils.get_query_params(operations.ListUnifiedWebhooksRequest, request), **query_params }
+        query_params = { **utils.get_query_params(request), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -185,15 +185,15 @@
     
     
     def patch_unified_webhook_trigger(self, request: operations.PatchUnifiedWebhookTriggerRequest) -> operations.PatchUnifiedWebhookTriggerResponse:
         r"""Trigger webhook"""
         hook_ctx = HookContext(operation_id='patchUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PatchUnifiedWebhookTriggerRequest, base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -239,15 +239,15 @@
     
     
     def remove_unified_webhook(self, request: operations.RemoveUnifiedWebhookRequest) -> operations.RemoveUnifiedWebhookResponse:
         r"""Remove webhook subscription"""
         hook_ctx = HookContext(operation_id='removeUnifiedWebhook', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveUnifiedWebhookRequest, base_url, '/unified/webhook/{id}', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
@@ -293,15 +293,15 @@
     
     
     def update_unified_webhook_trigger(self, request: operations.UpdateUnifiedWebhookTriggerRequest) -> operations.UpdateUnifiedWebhookTriggerResponse:
         r"""Trigger webhook"""
         hook_ctx = HookContext(operation_id='updateUnifiedWebhookTrigger', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUnifiedWebhookTriggerRequest, base_url, '/unified/webhook/{id}/trigger', request)
+        url = utils.generate_url(base_url, '/unified/webhook/{id}/trigger', request)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
         headers['Accept'] = 'application/json'
```

