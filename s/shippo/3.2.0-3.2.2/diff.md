# Comparing `tmp/shippo-3.2.0.tar.gz` & `tmp/shippo-3.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shippo-3.2.0.tar", last modified: Thu Apr  4 17:33:55 2024, max compression
+gzip compressed data, was "shippo-3.2.2.tar", last modified: Mon Apr  8 19:04:24 2024, max compression
```

## Comparing `shippo-3.2.0.tar` & `shippo-3.2.2.tar`

### file list

```diff
@@ -1,241 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-04 17:33:55.587271 shippo-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9772 2024-04-04 17:33:47.000000 shippo-3.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 17:33:55.587271 shippo-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1698 2024-04-04 17:33:47.000000 shippo-3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.547271 shippo-3.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/registration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    13636 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/addresses.py
--rw-r--r--   0 runner    (1001) docker     (127)    18874 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/batches.py
--rw-r--r--   0 runner    (1001) docker     (127)    22928 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/carrier_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8145 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/carrier_parcel_templates.py
--rw-r--r--   0 runner    (1001) docker     (127)    10948 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/customs_declarations.py
--rw-r--r--   0 runner    (1001) docker     (127)    10641 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/customs_items.py
--rw-r--r--   0 runner    (1001) docker     (127)    10693 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/manifests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.555271 shippo-3.2.0/src/shippo/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.575271 shippo-3.2.0/src/shippo/models/components/
--rw-r--r--   0 runner    (1001) docker     (127)     9741 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresscompletecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressimporter.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addresspaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressvalidationresults.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/addressvalidationresultsmessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/alcohol.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batch.py
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipmentbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/batchshipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      939 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrieraccountuspscreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/carriers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/cod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/connectexistingownupsaccountrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customerreference.py
--rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclarationcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsdeclarationpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsexporteridentification.py
--rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsinvoicedcharges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customsitempaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/customstaxidentification.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
--rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dangerousgoodsobject.py
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/defaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/departmentnumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/distanceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/dryice.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/errormessage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/instanttransactionrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/insurance.py
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/invoicenumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/labelfiletype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/lineitem.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/lineitembase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liverate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liveratecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/liveratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/location.py
--rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifestcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/manifestpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/objectstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ordercreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/orderpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelextra.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelinsurance.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parcelrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/parceltemplateenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/pickup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/pickupbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ponumber.py
--rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/rate.py
--rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ratemessage.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/ratepaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refund.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refundpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/refundrequestbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/rmanumber.py
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/security.py
--rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupaccountandservicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegrouptype.py
--rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicegroupupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2479 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicelevel.py
--rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/servicelevelenumset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipment.py
--rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentcreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentextra.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shipmentpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccountpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/shippoaccountupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/track.py
--rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatuslocationbase.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/trackingstatussubstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/tracksrequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactioncreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactionpaginatedlist.py
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/transactionstatusenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplateupdaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/components/weightunit.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.575271 shippo-3.2.0/src/shippo/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/badrequestwithdetail.py
--rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/badrequestwitherror.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/src/shippo/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/addshipmentstobatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createliverate.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      715 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createpickup.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createtrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createtransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     1158 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/createuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deletedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      710 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deleteservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/deleteuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getbatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      647 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrierparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcarrierregistrationstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcustomsdeclaration.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getcustomsitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getdefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getmanifest.py
--rw-r--r--   0 runner    (1001) docker     (127)      609 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getorder.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getparcel.py
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getrate.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getrefund.py
--rw-r--r--   0 runner    (1001) docker     (127)      631 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getshipment.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      775 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/gettrack.py
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/gettransaction.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/getuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listaddresses.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcarrieraccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)      987 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcarrierparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      858 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcustomsdeclarations.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listcustomsitems.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listmanifests.py
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listorders.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listparcels.py
--rw-r--r--   0 runner    (1001) docker     (127)      449 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listrefunds.py
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listservicegroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipmentrates.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshipments.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listshippoaccounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listtransactions.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/listuserparceltemplates.py
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/purchasebatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/registercarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/removeshipmentsfrombatch.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updatecarrieraccount.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updatedefaultparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateservicegroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateshippoaccount.py
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/updateuserparceltemplate.py
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/models/operations/validateaddress.py
--rw-r--r--   0 runner    (1001) docker     (127)    10993 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)    10592 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/parcels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4217 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/pickups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11463 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/rates.py
--rw-r--r--   0 runner    (1001) docker     (127)    14821 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/rates_at_checkout.py
--rw-r--r--   0 runner    (1001) docker     (127)     9976 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/refunds.py
--rw-r--r--   0 runner    (1001) docker     (127)    15477 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)    13455 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/service_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    11620 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/shipments.py
--rw-r--r--   0 runner    (1001) docker     (127)    14509 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/shippo_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     9265 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/tracking_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    10557 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/transactions.py
--rw-r--r--   0 runner    (1001) docker     (127)    18149 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/user_parcel_templates.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.587271 shippo-3.2.0/src/shippo/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3764 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    30026 2024-04-04 17:33:47.000000 shippo-3.2.0/src/shippo/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 17:33:55.551271 shippo-3.2.0/src/shippo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16550 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10959 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-04 17:33:55.000000 shippo-3.2.0/src/shippo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-08 19:04:24.101134 shippo-3.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10785 2024-04-08 19:03:54.000000 shippo-3.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 19:04:24.101134 shippo-3.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1743 2024-04-08 19:03:54.000000 shippo-3.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.065134 shippo-3.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1780 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/registration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2455 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14334 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/addresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19782 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/batches.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28886 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/carrier_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8424 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/carrier_parcel_templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11344 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/customs_declarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11037 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/customs_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11229 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/manifests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/components/
+-rw-r--r--   0 runner    (1001) docker     (127)     9957 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8056 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5293 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresscompletecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4225 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressimporter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addresspaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressvalidationresults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/addressvalidationresultsmessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/alcohol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipmentbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/batchshipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2032 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      730 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3924 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountuspscreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5660 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrieraccountwithextrainfo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4001 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/carriers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1728 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/cod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/connectexistingownupsaccountrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customerreference.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11041 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8977 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclarationcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      955 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsdeclarationpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsexporteridentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1560 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsinvoicedcharges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customsitempaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/customstaxidentification.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py
+-rw-r--r--   0 runner    (1001) docker     (127)      667 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dangerousgoodsobject.py
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/defaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/departmentnumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/distanceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/dryice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/errormessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/httpmetadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/instanttransactionrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/insurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/invoicenumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/labelfiletype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4349 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/lineitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/lineitembase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liveratecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/liveratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2566 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/location.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3199 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifestcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/manifestpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/objectstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7201 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5522 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ordercreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/orderpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5447 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1799 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelinsurance.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parcelrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10231 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/parceltemplateenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5867 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/pickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/pickupbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ponumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6894 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/rate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ratemessage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/ratepaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refundpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/refundrequestbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/rmanumber.py
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupaccountandservicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3697 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      754 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegrouptype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4080 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicegroupupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicelevel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41853 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/servicelevelenumset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6868 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3070 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentcreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13950 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentextra.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shipmentpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccountpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      816 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/shippoaccountupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/track.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2391 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1034 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatuslocationbase.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/trackingstatussubstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/tracksrequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactioncreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactionpaginatedlist.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/transactionstatusenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2146 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplateupdaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      254 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/components/weightunit.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      610 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/badrequestwithdetail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/badrequestwitherror.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.089134 shippo-3.2.2/src/shippo/models/internal/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/internal/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/src/shippo/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/addshipmentstobatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1033 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createliverate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createpickup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)      978 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createtrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1246 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createtransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/createuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deletedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deleteservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/deleteuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getbatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrierparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcarrierregistrationstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcustomsdeclaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getcustomsitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getdefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getmanifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getorder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getparcel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      912 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getrefund.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getshipment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      938 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/gettrack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/gettransaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/getuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/initiateoauth2signin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listaddresses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcarrieraccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1293 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcarrierparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcustomsdeclarations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listcustomsitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listmanifests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listorders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1137 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listparcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listrefunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)      752 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listservicegroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipmentrates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listshippoaccounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listtransactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/listuserparceltemplates.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/purchasebatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/registercarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/removeshipmentsfrombatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updatecarrieraccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updatedefaultparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateservicegroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateshippoaccount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/updateuserparceltemplate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/models/operations/validateaddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11126 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/parcels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4474 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/pickups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11648 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/rates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15887 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/rates_at_checkout.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10650 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/refunds.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15308 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14402 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/service_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12156 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/shipments.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/shippo_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/tracking_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11096 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/transactions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19173 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/user_parcel_templates.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.101134 shippo-3.2.2/src/shippo/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32093 2024-04-08 19:03:54.000000 shippo-3.2.2/src/shippo/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 19:04:24.069134 shippo-3.2.2/src/shippo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17805 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11263 2024-04-08 19:04:23.000000 shippo-3.2.2/src/shippo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 19:04:21.000000 shippo-3.2.2/src/shippo.egg-info/top_level.txt
```

### Comparing `shippo-3.2.0/PKG-INFO` & `shippo-3.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.0
+Version: 3.2.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
@@ -64,14 +64,36 @@
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
         s = shippo.Shippo(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
+        ## Debug HTTP Client
+        
+        The Shippo Python SDK returns schema models directly rather than wrapping the response in an envelope along with 
+        additional request/response details (status code, raw json, etc).  However, there are times when the underlying 
+        http information is useful so a 'debug' client is provided.  Using this client, you can retrieve the 
+        `requests.PreparedRequest` and `requests.Response` from the most recent API call.
+        
+        ```python
+        import shippo
+        from shippo.debug import DebugSession
+        
+        debug_session = DebugSession()
+        shippo_sdk = shippo.Shippo(api_key_header="<YOUR_API_KEY_HERE>", client=debug_session)
+        
+        shippo_sdk.addresses.list()
+        
+        # print the previous request http headers
+        print(debug_session.last_request.headers)  
+        # print the previous response status code and raw json
+        print(debug_session.last_response.status_code, debug_session.last_response.text)
+        ```
+        
         ## Documentation
         Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
         
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
@@ -93,14 +115,15 @@
         
         ### [carrier_accounts](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md)
         
         * [list](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#list) - List all carrier accounts
         * [create](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#create) - Create a new carrier account
         * [get](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#get) - Retrieve a carrier account
         * [update](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#update) - Update a carrier account
+        * [initiate_oauth2_signin](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#initiate_oauth2_signin) - Connect an existing carrier account using OAuth 2.0
         * [register](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#register) - Add a Shippo carrier account
         * [get_registration_status](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#get_registration_status) - Get Carrier Registration status
         
         ### [customs_declarations](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md)
         
         * [list](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md#list) - List all customs declarations
         * [create](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md#create) - Create a new customs declaration
```

### Comparing `shippo-3.2.0/README.md` & `shippo-3.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -57,14 +57,36 @@
 
 http_client = requests.Session()
 http_client.headers.update({'x-custom-header': 'someValue'})
 s = shippo.Shippo(client=http_client)
 ```
 <!-- End Custom HTTP Client [http-client] -->
 
+## Debug HTTP Client
+
+The Shippo Python SDK returns schema models directly rather than wrapping the response in an envelope along with 
+additional request/response details (status code, raw json, etc).  However, there are times when the underlying 
+http information is useful so a 'debug' client is provided.  Using this client, you can retrieve the 
+`requests.PreparedRequest` and `requests.Response` from the most recent API call.
+
+```python
+import shippo
+from shippo.debug import DebugSession
+
+debug_session = DebugSession()
+shippo_sdk = shippo.Shippo(api_key_header="<YOUR_API_KEY_HERE>", client=debug_session)
+
+shippo_sdk.addresses.list()
+
+# print the previous request http headers
+print(debug_session.last_request.headers)  
+# print the previous response status code and raw json
+print(debug_session.last_response.status_code, debug_session.last_response.text)
+```
+
 ## Documentation
 Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
 
 <!-- Placeholder for Future Speakeasy SDK Sections -->
 
 <!-- Start Available Resources and Operations [operations] -->
 ## Available Resources and Operations
@@ -86,14 +108,15 @@
 
 ### [carrier_accounts](docs/sdks/carrieraccounts/README.md)
 
 * [list](docs/sdks/carrieraccounts/README.md#list) - List all carrier accounts
 * [create](docs/sdks/carrieraccounts/README.md#create) - Create a new carrier account
 * [get](docs/sdks/carrieraccounts/README.md#get) - Retrieve a carrier account
 * [update](docs/sdks/carrieraccounts/README.md#update) - Update a carrier account
+* [initiate_oauth2_signin](docs/sdks/carrieraccounts/README.md#initiate_oauth2_signin) - Connect an existing carrier account using OAuth 2.0
 * [register](docs/sdks/carrieraccounts/README.md#register) - Add a Shippo carrier account
 * [get_registration_status](docs/sdks/carrieraccounts/README.md#get_registration_status) - Get Carrier Registration status
 
 ### [customs_declarations](docs/sdks/customsdeclarations/README.md)
 
 * [list](docs/sdks/customsdeclarations/README.md#list) - List all customs declarations
 * [create](docs/sdks/customsdeclarations/README.md#create) - Create a new customs declaration
```

### Comparing `shippo-3.2.0/setup.py` & `shippo-3.2.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='shippo',
-    version='3.2.0',
+    version='3.2.2',
     author='Shippo',
     description='Python Client SDK Generated by Speakeasy',
     url='https://github.com/goshippo/shippo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
@@ -40,15 +40,18 @@
         "six>=1.16.0",
         "typing-inspect>=0.9.0",
         "typing_extensions>=4.7.1",
         "urllib3>=1.26.18",
     ],
     extras_require={
         "dev": [
-            "pylint==2.16.2",
+            "httpretty==1.1.4",
+            "pylint==3.1.0",
             "pytest==8.1.1",
         ],
     },
     package_dir={'': 'src'},
     python_requires='>=3.8',
-    package_data={'shippo': ['py.typed']},
+    package_data={
+        'shippo': ['py.typed']
+    },
 )
```

### Comparing `shippo-3.2.0/src/shippo/_hooks/registration.py` & `shippo-3.2.2/src/shippo/_hooks/registration.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 # This file is only ever generated once on the first generation and then is free to be modified.
 # Any hooks you wish to add should be registered in the init_hooks function. Feel free to define them
 # in this file or in separate files in the hooks folder.
 
 
 def add_shippo_token_to_auth_header_if_missing(request: requests.PreparedRequest):
     auth_header = request.headers.get("authorization")
-    if auth_header is not None and auth_header.startswith("ShippoToken") is False:
+    if auth_header is not None and auth_header.startswith("shippo_"):
         request.headers["authorization"] = f"ShippoToken {auth_header}"
 
 
 class ShippoAuthBeforeRequestHook(BeforeRequestHook):
 
     def before_request(
             self, hook_ctx: BeforeRequestContext, request: requests.PreparedRequest
```

### Comparing `shippo-3.2.0/src/shippo/_hooks/sdkhooks.py` & `shippo-3.2.2/src/shippo/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/_hooks/types.py` & `shippo-3.2.2/src/shippo/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/addresses.py` & `shippo-3.2.2/src/shippo/addresses.py`

 * *Files 11% similar despite different names*

```diff
@@ -25,25 +25,29 @@
         hook_ctx = HookContext(operation_id='ListAddresses', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListAddressesRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListAddressesGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/addresses'
+        url = utils.generate_url(base_url, '/addresses', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListAddressesRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -85,27 +89,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateAddress', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateAddressRequest(
             shippo_api_version=shippo_api_version,
             address_create_request=address_create_request,
         )
         
+        _globals = operations.CreateAddressGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/addresses'
+        url = utils.generate_url(base_url, '/addresses', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateAddressRequest, "address_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -147,24 +156,29 @@
         """
         hook_ctx = HookContext(operation_id='GetAddress', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetAddressRequest(
             address_id=address_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetAddressGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetAddressRequest, base_url, '/addresses/{AddressId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/addresses/{AddressId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -206,24 +220,29 @@
         """
         hook_ctx = HookContext(operation_id='ValidateAddress', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ValidateAddressRequest(
             address_id=address_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ValidateAddressGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ValidateAddressRequest, base_url, '/addresses/{AddressId}/validate', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/addresses/{AddressId}/validate', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -253,8 +272,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/batches.py` & `shippo-3.2.2/src/shippo/batches.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,27 +32,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateBatchRequest(
             shippo_api_version=shippo_api_version,
             batch_create_request=batch_create_request,
         )
         
+        _globals = operations.CreateBatchGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/batches'
+        url = utils.generate_url(base_url, '/batches', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateBatchRequest, "batch_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -97,24 +102,29 @@
         """
         hook_ctx = HookContext(operation_id='GetBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetBatchGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetBatchRequest, base_url, '/batches/{BatchId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/batches/{BatchId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -157,27 +167,32 @@
         hook_ctx = HookContext(operation_id='AddShipmentsToBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.AddShipmentsToBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
             request_body=request_body,
         )
         
+        _globals = operations.AddShipmentsToBatchGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.AddShipmentsToBatchRequest, base_url, '/batches/{BatchId}/add_shipments', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/batches/{BatchId}/add_shipments', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.AddShipmentsToBatchRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -222,24 +237,29 @@
         """
         hook_ctx = HookContext(operation_id='PurchaseBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.PurchaseBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.PurchaseBatchGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.PurchaseBatchRequest, base_url, '/batches/{BatchId}/purchase', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/batches/{BatchId}/purchase', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -282,27 +302,32 @@
         hook_ctx = HookContext(operation_id='RemoveShipmentsFromBatch', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RemoveShipmentsFromBatchRequest(
             batch_id=batch_id,
             shippo_api_version=shippo_api_version,
             request_body=request_body,
         )
         
+        _globals = operations.RemoveShipmentsFromBatchGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.RemoveShipmentsFromBatchRequest, base_url, '/batches/{BatchId}/remove_shipments', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/batches/{BatchId}/remove_shipments', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.RemoveShipmentsFromBatchRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -332,8 +357,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/carrier_accounts.py` & `shippo-3.2.2/src/shippo/carrier_accounts.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,25 +24,29 @@
         Returns a list of all carrier accounts connected to your Shippo account. These carrier accounts include both Shippo carrier accounts and your own carrier accounts that you have connected to your Shippo account.
 
         Additionally, you can get information about the service levels associated with each carrier account by passing in the `?service_levels=true` query parameter. <br>
         Using it appends the property `service_levels` to each carrier account. <br>
         By default, if the query parameter is omitted, the `service_levels` property will not be included in the response.
         """
         hook_ctx = HookContext(operation_id='ListCarrierAccounts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.ListCarrierAccountsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/carrier_accounts'
+        url = utils.generate_url(base_url, '/carrier_accounts', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListCarrierAccountsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -84,27 +88,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateCarrierAccountRequest(
             shippo_api_version=shippo_api_version,
             connect_existing_own_ups_account_request=connect_existing_own_ups_account_request,
         )
         
+        _globals = operations.CreateCarrierAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/carrier_accounts'
+        url = utils.generate_url(base_url, '/carrier_accounts', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCarrierAccountRequest, "connect_existing_own_ups_account_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -143,34 +152,39 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, carrier_account_id: str, shippo_api_version: Optional[str] = None) -> components.CarrierAccount:
+    def get(self, carrier_account_id: str, shippo_api_version: Optional[str] = None) -> components.CarrierAccountWithExtraInfo:
         r"""Retrieve a carrier account
         Returns an existing carrier account using an object ID.
         """
         hook_ctx = HookContext(operation_id='GetCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCarrierAccountRequest(
             carrier_account_id=carrier_account_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetCarrierAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/carrier_accounts/{CarrierAccountId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -190,15 +204,15 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccount])
+                out = utils.unmarshal_json(http_res.text, Optional[components.CarrierAccountWithExtraInfo])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
@@ -213,27 +227,32 @@
         hook_ctx = HookContext(operation_id='UpdateCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.UpdateCarrierAccountRequest(
             carrier_account_id=carrier_account_id,
             shippo_api_version=shippo_api_version,
             carrier_account_base=carrier_account_base,
         )
         
+        _globals = operations.UpdateCarrierAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateCarrierAccountRequest, base_url, '/carrier_accounts/{CarrierAccountId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/carrier_accounts/{CarrierAccountId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateCarrierAccountRequest, "carrier_account_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -265,37 +284,128 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
+    def initiate_oauth2_signin(self, carrier_account_object_id: str, redirect_uri: str, state: Optional[str] = None, shippo_api_version: Optional[str] = None) -> operations.InitiateOauth2SigninResponse:
+        r"""Connect an existing carrier account using OAuth 2.0
+        Used by client applications to setup or reconnect an existing carrier account with carriers that support OAuth 2.0
+        """
+        hook_ctx = HookContext(operation_id='InitiateOauth2Signin', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.InitiateOauth2SigninRequest(
+            carrier_account_object_id=carrier_account_object_id,
+            redirect_uri=redirect_uri,
+            state=state,
+            shippo_api_version=shippo_api_version,
+        )
+        
+        _globals = operations.InitiateOauth2SigninGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
+        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
+        
+        url = utils.generate_url(base_url, '/carrier_accounts/{CarrierAccountObjectId}/signin/initiate', request, _globals)
+        
+        if callable(self.sdk_configuration.security):
+            headers, query_params = utils.get_security(self.sdk_configuration.security())
+        else:
+            headers, query_params = utils.get_security(self.sdk_configuration.security)
+        
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
+        headers['user-agent'] = self.sdk_configuration.user_agent
+        client = self.sdk_configuration.client
+        
+        try:
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
+            http_res = client.send(req)
+        except Exception as e:
+            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
+            if e is not None:
+                raise e
+
+        if utils.match_status_codes(['400','401','422','4XX','5XX'], http_res.status_code):
+            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
+            if e is not None:
+                raise e
+            if result is not None:
+                http_res = result
+        else:
+            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
+            
+        
+        
+        res = operations.InitiateOauth2SigninResponse(headers=None)
+        
+        if http_res.status_code == 302:
+            res.headers = http_res.headers
+            
+        elif http_res.status_code == 400:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninResponseBody)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 401:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninCarrierAccountsResponseBody)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code == 422:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, errors.InitiateOauth2SigninCarrierAccountsResponseResponseBody)
+                raise out
+            else:
+                content_type = http_res.headers.get('Content-Type')
+                raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
+        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
+            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
+        else:
+            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
+
+        return res
+
+    
+    
     def register(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.CarrierAccountCanadaPostCreateRequest, components.CarrierAccountChronopostCreateRequest, components.CarrierAccountColissimoCreateRequest, components.CarrierAccountCorreosCreateRequest, components.CarrierAccountDeutschePostCreateRequest, components.CarrierAccountDHLExpressCreateRequest, components.CarrierAccountDpdDeCreateRequest, components.CarrierAccountDPDUKCreateRequest, components.CarrierAccountHermesUKCreateRequest, components.CarrierAccountPosteItalianeCreateRequest, components.CarrierAccountUPSCreateRequest, components.CarrierAccountUSPSCreateRequest]] = None) -> components.CarrierAccount:
         r"""Add a Shippo carrier account
         Adds a Shippo carrier account
         """
         hook_ctx = HookContext(operation_id='RegisterCarrierAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.RegisterCarrierAccountRequest(
             shippo_api_version=shippo_api_version,
             request_body=request_body,
         )
         
+        _globals = operations.RegisterCarrierAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/carrier_accounts/register/new'
+        url = utils.generate_url(base_url, '/carrier_accounts/register/new', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.RegisterCarrierAccountRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -344,25 +454,29 @@
         """
         hook_ctx = HookContext(operation_id='GetCarrierRegistrationStatus', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCarrierRegistrationStatusRequest(
             carrier=carrier,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetCarrierRegistrationStatusGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/carrier_accounts/reg-status'
+        url = utils.generate_url(base_url, '/carrier_accounts/reg-status', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.GetCarrierRegistrationStatusRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -392,8 +506,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/carrier_parcel_templates.py` & `shippo-3.2.2/src/shippo/carrier_parcel_templates.py`

 * *Files 10% similar despite different names*

```diff
@@ -26,25 +26,29 @@
         hook_ctx = HookContext(operation_id='ListCarrierParcelTemplates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListCarrierParcelTemplatesRequest(
             include=include,
             carrier=carrier,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListCarrierParcelTemplatesGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/parcel-templates'
+        url = utils.generate_url(base_url, '/parcel-templates', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListCarrierParcelTemplatesRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -86,24 +90,29 @@
         """
         hook_ctx = HookContext(operation_id='GetCarrierParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCarrierParcelTemplateRequest(
             carrier_parcel_template_token=carrier_parcel_template_token,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetCarrierParcelTemplateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCarrierParcelTemplateRequest, base_url, '/parcel-templates/{CarrierParcelTemplateToken}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/parcel-templates/{CarrierParcelTemplateToken}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -133,8 +142,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/customs_declarations.py` & `shippo-3.2.2/src/shippo/customs_declarations.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,25 +26,29 @@
         hook_ctx = HookContext(operation_id='ListCustomsDeclarations', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListCustomsDeclarationsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListCustomsDeclarationsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/declarations'
+        url = utils.generate_url(base_url, '/customs/declarations', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsDeclarationsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -86,27 +90,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateCustomsDeclarationRequest(
             shippo_api_version=shippo_api_version,
             customs_declaration_create_request=customs_declaration_create_request,
         )
         
+        _globals = operations.CreateCustomsDeclarationGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/declarations'
+        url = utils.generate_url(base_url, '/customs/declarations', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsDeclarationRequest, "customs_declaration_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -149,25 +158,29 @@
         hook_ctx = HookContext(operation_id='GetCustomsDeclaration', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCustomsDeclarationRequest(
             customs_declaration_id=customs_declaration_id,
             page=page,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetCustomsDeclarationGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsDeclarationRequest, base_url, '/customs/declarations/{CustomsDeclarationId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/customs/declarations/{CustomsDeclarationId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsDeclarationRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -197,8 +210,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/customs_items.py` & `shippo-3.2.2/src/shippo/customs_items.py`

 * *Files 6% similar despite different names*

```diff
@@ -25,25 +25,29 @@
         hook_ctx = HookContext(operation_id='ListCustomsItems', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListCustomsItemsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListCustomsItemsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/items'
+        url = utils.generate_url(base_url, '/customs/items', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListCustomsItemsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -85,27 +89,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateCustomsItemRequest(
             shippo_api_version=shippo_api_version,
             customs_item_base=customs_item_base,
         )
         
+        _globals = operations.CreateCustomsItemGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/customs/items'
+        url = utils.generate_url(base_url, '/customs/items', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateCustomsItemRequest, "customs_item_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -148,25 +157,29 @@
         hook_ctx = HookContext(operation_id='GetCustomsItem', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetCustomsItemRequest(
             customs_item_id=customs_item_id,
             page=page,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetCustomsItemGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetCustomsItemRequest, base_url, '/customs/items/{CustomsItemId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/customs/items/{CustomsItemId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.GetCustomsItemRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -196,8 +209,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/manifests.py` & `shippo-3.2.2/src/shippo/manifests.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,25 +31,29 @@
         hook_ctx = HookContext(operation_id='ListManifests', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListManifestsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListManifestsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = utils.generate_url(base_url, '/manifests', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListManifestsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -91,27 +95,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateManifestRequest(
             shippo_api_version=shippo_api_version,
             manifest_create_request=manifest_create_request,
         )
         
+        _globals = operations.CreateManifestGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/manifests'
+        url = utils.generate_url(base_url, '/manifests', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateManifestRequest, "manifest_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -153,24 +162,29 @@
         """
         hook_ctx = HookContext(operation_id='GetManifest', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetManifestRequest(
             manifest_id=manifest_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetManifestGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetManifestRequest, base_url, '/manifests/{ManifestId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/manifests/{ManifestId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -200,8 +214,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/models/components/__init__.py` & `shippo-3.2.2/src/shippo/models/components/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,15 @@
 from .carrieraccountpaginatedlist import *
 from .carrieraccountposteitalianecreaterequest import *
 from .carrieraccountregistrationstatus import *
 from .carrieraccountservicelevel import *
 from .carrieraccountupscreaterequest import *
 from .carrieraccountupscreaterequestparameters import *
 from .carrieraccountuspscreaterequest import *
+from .carrieraccountwithextrainfo import *
 from .carrierparceltemplate import *
 from .carriers import *
 from .cod import *
 from .connectexistingownupsaccountrequest import *
 from .customerreference import *
 from .customsdeclaration import *
 from .customsdeclarationcreaterequest import *
@@ -53,14 +54,15 @@
 from .dangerousgoodsobject import *
 from .defaultparceltemplate import *
 from .defaultparceltemplateupdaterequest import *
 from .departmentnumber import *
 from .distanceunit import *
 from .dryice import *
 from .errormessage import *
+from .httpmetadata import *
 from .instanttransactionrequestbody import *
 from .insurance import *
 from .invoicenumber import *
 from .labelfiletype import *
 from .lineitem import *
 from .lineitembase import *
 from .liverate import *
@@ -119,8 +121,8 @@
 from .upsconnectexistingownaccountparameters import *
 from .userparceltemplate import *
 from .userparceltemplateupdaterequest import *
 from .userparceltemplatewithcarriertemplatecreaterequest import *
 from .userparceltemplatewithoutcarriertemplatecreaterequest import *
 from .weightunit import *
 
-__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
+__all__ = ["Address","AddressCompleteCreateRequest","AddressCreateRequest","AddressImporter","AddressPaginatedList","AddressValidationResults","AddressValidationResultsMessage","Alcohol","AncillaryEndorsement","Attributes","Authentication","B13aFilingOption","Batch","BatchCreateRequest","BatchShipment","BatchShipmentBase","BatchShipmentPaginatedList","BatchStatus","Billing","BuildingLocationType","BuildingType","CarrierAccount","CarrierAccountBase","CarrierAccountCanadaPostCreateParameters","CarrierAccountCanadaPostCreateRequest","CarrierAccountChronopostCreateRequest","CarrierAccountColissimoCreateRequest","CarrierAccountColissimoCreateRequestParameters","CarrierAccountCorreosCreateRequest","CarrierAccountCorreosCreateRequestParameters","CarrierAccountDHLExpressCreateRequest","CarrierAccountDHLExpressCreateRequestParameters","CarrierAccountDPDUKCreateRequest","CarrierAccountDPDUKCreateRequestParameters","CarrierAccountDeutschePostCreateRequest","CarrierAccountDeutschePostCreateRequestParameters","CarrierAccountDpdDeCreateRequest","CarrierAccountDpdDeCreateRequestParameters","CarrierAccountHermesUKCreateRequest","CarrierAccountHermesUKCreateRequestParameters","CarrierAccountPaginatedList","CarrierAccountPosteItalianeCreateRequest","CarrierAccountPosteItalianeCreateRequestParameters","CarrierAccountRegistrationStatus","CarrierAccountServiceLevel","CarrierAccountUPSCreateRequest","CarrierAccountUPSCreateRequestParameters","CarrierAccountUSPSCreateRequest","CarrierAccountUSPSCreateRequestParameters","CarrierAccountWithExtraInfo","CarrierAccountWithExtraInfoStatus","CarrierAccountWithExtraInfoType","CarrierParcelTemplate","Carriers","Cod","Code","ConnectExistingOwnUPSAccountRequest","ContentsType","CustomerReference","CustomsDeclaration","CustomsDeclarationAddressImporter","CustomsDeclarationCreateRequest","CustomsDeclarationCreateRequestB13aFilingOption","CustomsDeclarationCreateRequestContentsType","CustomsDeclarationCreateRequestEelPfc","CustomsDeclarationCreateRequestIncoterm","CustomsDeclarationCreateRequestNonDeliveryOption","CustomsDeclarationPaginatedList","CustomsExporterIdentification","CustomsInvoicedCharges","CustomsItem","CustomsItemBase","CustomsItemPaginatedList","CustomsTaxIdentification","CustomsTaxIdentificationType","DangerousGoodsBiologicalMaterial","DangerousGoodsCode","DangerousGoodsLithiumBatteries","DangerousGoodsObject","DefaultParcelTemplate","DefaultParcelTemplateUpdateRequest","DepartmentNumber","DistanceUnit","DryIce","EelPfc","ErrorMessage","HTTPMetadata","Incoterm","InstantTransactionRequestBody","InstantTransactionRequestBodyLabelFileType","Insurance","InvoiceNumber","LabelFileType","LasershipAttrs","LineItem","LineItemBase","LiveRate","LiveRateCreateRequest","LiveRatePaginatedList","Location","Manifest","ManifestCreateRequest","ManifestPaginatedList","ManifestStatus","Messages","NonDeliveryOption","ObjectInfo","ObjectResults","ObjectState","Order","OrderCreateRequest","OrderCreateRequestOrderStatus","OrderPaginatedList","OrderStatus","Parameters","Parcel","ParcelCreateRequest","ParcelExtra","ParcelInsurance","ParcelInsuranceProvider","ParcelObjectState","ParcelPaginatedList","ParcelRequest","ParcelTemplateAramexAustralia","ParcelTemplateCouriersPlease","ParcelTemplateDHLeCommerce","ParcelTemplateDPDUK","ParcelTemplateFedEx","ParcelTemplateUPS","ParcelTemplateUSPS","PaymentMethod","Pickup","PickupBase","PickupStatus","PoNumber","PreferredDeliveryTimeframe","Provider","Rate","RateMessage","RatePaginatedList","RecipientType","Refund","RefundPaginatedList","RefundRequestBody","RefundStatus","ReturnServiceType","RmaNumber","Security","ServiceGroup","ServiceGroupAccountAndServiceLevel","ServiceGroupCreateRequest","ServiceGroupType","ServiceGroupUpdateRequest","ServiceLevel","ServiceLevelAPCPostal","ServiceLevelAPG","ServiceLevelAirterra","ServiceLevelAramexAustralia","ServiceLevelAsendia","ServiceLevelAustraliaPost","ServiceLevelAxleHire","ServiceLevelBetterTrucks","ServiceLevelCDL","ServiceLevelCanadaPost","ServiceLevelChronopost","ServiceLevelColissimo","ServiceLevelCorreosEspana","ServiceLevelCouriersPlease","ServiceLevelDHLExpress","ServiceLevelDHLGermany","ServiceLevelDHLeCommerce","ServiceLevelDPDDE","ServiceLevelDPDUK","ServiceLevelDeutschePost","ServiceLevelEvriUK","ServiceLevelFedEx","ServiceLevelGLSUS","ServiceLevelGlobegistics","ServiceLevelLSO","ServiceLevelLasership","ServiceLevelMaergo","ServiceLevelMondialRelay","ServiceLevelOnTrac","ServiceLevelParcelforce","ServiceLevelPostItaliane","ServiceLevelPurolator","ServiceLevelRoyalMail","ServiceLevelSendle","ServiceLevelSwyft","ServiceLevelUDS","ServiceLevelUPS","ServiceLevelUSPS","ServiceLevelVeho","ServiceLevelePostGlobal","Shipment","ShipmentCreateRequest","ShipmentExtra","ShipmentPaginatedList","ShipmentStatus","ShippoAccount","ShippoAccountPaginatedList","ShippoAccountUpdateRequest","ShopApp","SignatureConfirmation","Source","Status","Track","TrackingStatus","TrackingStatusEnum","TrackingStatusLocationBase","TrackingStatusSubstatus","TracksRequest","Transaction","TransactionCreateRequest","TransactionMessages","TransactionPaginatedList","TransactionStatusEnum","Type","UPSConnectExistingOwnAccountParameters","UserParcelTemplate","UserParcelTemplateUpdateRequest","UserParcelTemplateWithCarrierTemplateCreateRequest","UserParcelTemplateWithoutCarrierTemplateCreateRequest","WeightUnit"]
```

### Comparing `shippo-3.2.0/src/shippo/models/components/address.py` & `shippo-3.2.2/src/shippo/models/components/address.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addresscompletecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/addresscompletecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addresscreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/addresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addressimporter.py` & `shippo-3.2.2/src/shippo/models/components/addressimporter.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addresspaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/addresspaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addressvalidationresults.py` & `shippo-3.2.2/src/shippo/models/components/addressvalidationresults.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/addressvalidationresultsmessage.py` & `shippo-3.2.2/src/shippo/models/components/addressvalidationresultsmessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/alcohol.py` & `shippo-3.2.2/src/shippo/models/components/alcohol.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/batch.py` & `shippo-3.2.2/src/shippo/models/components/batch.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/batchcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/batchcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/batchshipment.py` & `shippo-3.2.2/src/shippo/models/components/batchshipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/batchshipmentbase.py` & `shippo-3.2.2/src/shippo/models/components/batchshipmentbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/batchshipmentpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/batchshipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/billing.py` & `shippo-3.2.2/src/shippo/models/components/billing.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccount.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountbase.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreateparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountcanadapostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountchronopostcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountchronopostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountcolissimocreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountcolissimocreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountcorreoscreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountcorreoscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountdeutschepostcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountdhlexpresscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountdpddecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountdpddecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountdpdukcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountdpdukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccounthermesukcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccounthermesukcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountpaginatedlist.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from .carrieraccount import CarrierAccount
+from .carrieraccountwithextrainfo import CarrierAccountWithExtraInfo
 from dataclasses_json import Undefined, dataclass_json
 from shippo import utils
 from typing import List, Optional
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CarrierAccountPaginatedList:
     next: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('next'), 'exclude': lambda f: f is None }})
     previous: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('previous'), 'exclude': lambda f: f is None }})
-    results: Optional[List[CarrierAccount]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
+    results: Optional[List[CarrierAccountWithExtraInfo]] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('results'), 'exclude': lambda f: f is None }})
```

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountposteitalianecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountregistrationstatus.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountregistrationstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountservicelevel.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountupscreaterequestparameters.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountupscreaterequestparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrieraccountuspscreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/carrieraccountuspscreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carrierparceltemplate.py` & `shippo-3.2.2/src/shippo/models/components/carrierparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/carriers.py` & `shippo-3.2.2/src/shippo/models/components/carriers.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/cod.py` & `shippo-3.2.2/src/shippo/models/components/cod.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/connectexistingownupsaccountrequest.py` & `shippo-3.2.2/src/shippo/models/components/connectexistingownupsaccountrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customerreference.py` & `shippo-3.2.2/src/shippo/models/components/customerreference.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsdeclaration.py` & `shippo-3.2.2/src/shippo/models/components/customsdeclaration.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsdeclarationcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/customsdeclarationcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsdeclarationpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/customsdeclarationpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsexporteridentification.py` & `shippo-3.2.2/src/shippo/models/components/customsexporteridentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsinvoicedcharges.py` & `shippo-3.2.2/src/shippo/models/components/customsinvoicedcharges.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsitem.py` & `shippo-3.2.2/src/shippo/models/components/customsitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsitembase.py` & `shippo-3.2.2/src/shippo/models/components/customsitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customsitempaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/customsitempaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/customstaxidentification.py` & `shippo-3.2.2/src/shippo/models/components/customstaxidentification.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py` & `shippo-3.2.2/src/shippo/models/components/dangerousgoodsbiologicalmaterial.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/dangerousgoodslithiumbatteries.py` & `shippo-3.2.2/src/shippo/models/components/dangerousgoodslithiumbatteries.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/dangerousgoodsobject.py` & `shippo-3.2.2/src/shippo/models/components/dangerousgoodsobject.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/defaultparceltemplate.py` & `shippo-3.2.2/src/shippo/models/components/defaultparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/defaultparceltemplateupdaterequest.py` & `shippo-3.2.2/src/shippo/models/components/defaultparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/departmentnumber.py` & `shippo-3.2.2/src/shippo/models/components/departmentnumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/dryice.py` & `shippo-3.2.2/src/shippo/models/components/dryice.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/errormessage.py` & `shippo-3.2.2/src/shippo/models/components/errormessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/instanttransactionrequestbody.py` & `shippo-3.2.2/src/shippo/models/components/instanttransactionrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/insurance.py` & `shippo-3.2.2/src/shippo/models/components/insurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/invoicenumber.py` & `shippo-3.2.2/src/shippo/models/components/invoicenumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/labelfiletype.py` & `shippo-3.2.2/src/shippo/models/components/labelfiletype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/lineitem.py` & `shippo-3.2.2/src/shippo/models/components/lineitem.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/lineitembase.py` & `shippo-3.2.2/src/shippo/models/components/lineitembase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/liverate.py` & `shippo-3.2.2/src/shippo/models/components/liverate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/liveratecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/liveratecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/liveratepaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/liveratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/location.py` & `shippo-3.2.2/src/shippo/models/components/location.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/manifest.py` & `shippo-3.2.2/src/shippo/models/components/manifest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/manifestcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/manifestcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/manifestpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/manifestpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/order.py` & `shippo-3.2.2/src/shippo/models/components/order.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/ordercreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/ordercreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/orderpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/orderpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcel.py` & `shippo-3.2.2/src/shippo/models/components/parcel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcelcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/parcelcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcelextra.py` & `shippo-3.2.2/src/shippo/models/components/parcelextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcelinsurance.py` & `shippo-3.2.2/src/shippo/models/components/parcelinsurance.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcelpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/parcelpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parcelrequest.py` & `shippo-3.2.2/src/shippo/models/components/parcelrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/parceltemplateenumset.py` & `shippo-3.2.2/src/shippo/models/components/parceltemplateenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/pickup.py` & `shippo-3.2.2/src/shippo/models/components/pickup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/pickupbase.py` & `shippo-3.2.2/src/shippo/models/components/pickupbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/ponumber.py` & `shippo-3.2.2/src/shippo/models/components/ponumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/rate.py` & `shippo-3.2.2/src/shippo/models/components/rate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/ratemessage.py` & `shippo-3.2.2/src/shippo/models/components/ratemessage.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/ratepaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/ratepaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/refund.py` & `shippo-3.2.2/src/shippo/models/components/refund.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/refundpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/refundpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/refundrequestbody.py` & `shippo-3.2.2/src/shippo/models/components/refundrequestbody.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/rmanumber.py` & `shippo-3.2.2/src/shippo/models/components/rmanumber.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicegroup.py` & `shippo-3.2.2/src/shippo/models/components/servicegroup.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicegroupaccountandservicelevel.py` & `shippo-3.2.2/src/shippo/models/components/servicegroupaccountandservicelevel.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicegroupcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/servicegroupcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicegrouptype.py` & `shippo-3.2.2/src/shippo/models/components/servicegrouptype.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicegroupupdaterequest.py` & `shippo-3.2.2/src/shippo/models/components/servicegroupupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/servicelevel.py` & `shippo-3.2.2/src/shippo/models/components/servicelevel.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     name: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('name'), 'exclude': lambda f: f is None }})
     r"""Name of the Rate's servicelevel, e.g. `International Priority` or `Standard Post`.
     A servicelevel commonly defines the transit time of a Shipment (e.g., Express vs. Standard), along with other properties. 
     These names vary depending on the provider.
     """
     terms: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('terms'), 'exclude': lambda f: f is None }})
     r"""Further clarification of the service."""
-    service_level_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('service_level_token'), 'exclude': lambda f: f is None }})
+    token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('token'), 'exclude': lambda f: f is None }})
     r"""Token of the Rate's servicelevel, e.g. `usps_priority` or `fedex_ground`.
     See <a href=\"#tag/Service-Levels\">servicelevels</a>.
     """
     extended_token: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('extended_token'), 'exclude': lambda f: f is None }})
     r"""Unique, extended version of the Service Level \\"token\\".
     Guaranteed to be unique across all Service Levels, and may help offer insight into the specific Service Level it describes.
     """
```

### Comparing `shippo-3.2.0/src/shippo/models/components/servicelevelenumset.py` & `shippo-3.2.2/src/shippo/models/components/servicelevelenumset.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shipment.py` & `shippo-3.2.2/src/shippo/models/components/shipment.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shipmentcreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/shipmentcreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shipmentextra.py` & `shippo-3.2.2/src/shippo/models/components/shipmentextra.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shipmentpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/shipmentpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shippoaccount.py` & `shippo-3.2.2/src/shippo/models/components/shippoaccount.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shippoaccountpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/shippoaccountpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/shippoaccountupdaterequest.py` & `shippo-3.2.2/src/shippo/models/components/shippoaccountupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/track.py` & `shippo-3.2.2/src/shippo/models/components/track.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/trackingstatus.py` & `shippo-3.2.2/src/shippo/models/components/trackingstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/trackingstatuslocationbase.py` & `shippo-3.2.2/src/shippo/models/components/trackingstatuslocationbase.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/trackingstatussubstatus.py` & `shippo-3.2.2/src/shippo/models/components/trackingstatussubstatus.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/tracksrequest.py` & `shippo-3.2.2/src/shippo/models/components/tracksrequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/transaction.py` & `shippo-3.2.2/src/shippo/models/components/transaction.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/transactioncreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/transactioncreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/transactionpaginatedlist.py` & `shippo-3.2.2/src/shippo/models/components/transactionpaginatedlist.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/upsconnectexistingownaccountparameters.py` & `shippo-3.2.2/src/shippo/models/components/upsconnectexistingownaccountparameters.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/userparceltemplate.py` & `shippo-3.2.2/src/shippo/models/components/userparceltemplate.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/userparceltemplateupdaterequest.py` & `shippo-3.2.2/src/shippo/models/components/userparceltemplateupdaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py` & `shippo-3.2.2/src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/errors/badrequestwithdetail.py` & `shippo-3.2.2/src/shippo/models/errors/badrequestwithdetail.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/errors/badrequestwitherror.py` & `shippo-3.2.2/src/shippo/models/errors/badrequestwitherror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/errors/sdkerror.py` & `shippo-3.2.2/src/shippo/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `shippo-3.2.0/src/shippo/models/operations/addshipmentstobatch.py` & `shippo-3.2.2/src/shippo/models/operations/addshipmentstobatch.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import batchshipmentbase as components_batchshipmentbase
 from typing import List, Optional
 
 
 @dataclasses.dataclass
+class AddShipmentsToBatchGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class AddShipmentsToBatchRequest:
     batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the batch"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     request_body: Optional[List[components_batchshipmentbase.BatchShipmentBase]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Array of shipments to add to the batch"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createaddress.py` & `shippo-3.2.2/src/shippo/models/operations/createaddress.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import addresscreaterequest as components_addresscreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class CreateAddressGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateAddressRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     address_create_request: Optional[components_addresscreaterequest.AddressCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Address details."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createbatch.py` & `shippo-3.2.2/src/shippo/models/operations/createshipment.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import batchcreaterequest as components_batchcreaterequest
+from ...models.components import shipmentcreaterequest as components_shipmentcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateBatchRequest:
+class CreateShipmentGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    batch_create_request: Optional[components_batchcreaterequest.BatchCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Batch details."""
+    
+
+
+
+@dataclasses.dataclass
+class CreateShipmentRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    shipment_create_request: Optional[components_shipmentcreaterequest.ShipmentCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Shipment details and contact info."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createcarrieraccount.py` & `shippo-3.2.2/src/shippo/models/operations/createparcel.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import connectexistingownupsaccountrequest as components_connectexistingownupsaccountrequest
+from ...models.components import parcelrequest as components_parcelrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateCarrierAccountRequest:
+class CreateParcelGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    connect_existing_own_ups_account_request: Optional[components_connectexistingownupsaccountrequest.ConnectExistingOwnUPSAccountRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Examples."""
+    
+
+
+
+@dataclasses.dataclass
+class CreateParcelRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    parcel_request: Optional[components_parcelrequest.ParcelRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Parcel details."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createcustomsdeclaration.py` & `shippo-3.2.2/src/shippo/models/operations/createliverate.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import customsdeclarationcreaterequest as components_customsdeclarationcreaterequest
+from ...models.components import liveratecreaterequest as components_liveratecreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateCustomsDeclarationRequest:
+class CreateLiveRateGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    customs_declaration_create_request: Optional[components_customsdeclarationcreaterequest.CustomsDeclarationCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""CustomsDeclaration details."""
+    
+
+
+
+@dataclasses.dataclass
+class CreateLiveRateRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    live_rate_create_request: Optional[components_liveratecreaterequest.LiveRateCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Generate rates at checkout"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createcustomsitem.py` & `shippo-3.2.2/src/shippo/models/operations/createcustomsitem.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import customsitembase as components_customsitembase
 from typing import Optional
 
 
 @dataclasses.dataclass
+class CreateCustomsItemGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateCustomsItemRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     customs_item_base: Optional[components_customsitembase.CustomsItemBase] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""CustomsItem details."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createliverate.py` & `shippo-3.2.2/src/shippo/models/operations/createbatch.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import liveratecreaterequest as components_liveratecreaterequest
+from ...models.components import batchcreaterequest as components_batchcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateLiveRateRequest:
+class CreateBatchGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    live_rate_create_request: Optional[components_liveratecreaterequest.LiveRateCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Generate rates at checkout"""
+    
+
+
+
+@dataclasses.dataclass
+class CreateBatchRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    batch_create_request: Optional[components_batchcreaterequest.BatchCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Batch details."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createmanifest.py` & `shippo-3.2.2/src/shippo/models/operations/createmanifest.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import manifestcreaterequest as components_manifestcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class CreateManifestGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateManifestRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     manifest_create_request: Optional[components_manifestcreaterequest.ManifestCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Manifest details and contact info."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createorder.py` & `shippo-3.2.2/src/shippo/models/operations/createorder.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import ordercreaterequest as components_ordercreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class CreateOrderGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateOrderRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     order_create_request: Optional[components_ordercreaterequest.OrderCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Order details."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createparcel.py` & `shippo-3.2.2/src/shippo/models/operations/createtrack.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import parcelrequest as components_parcelrequest
+from ...models.components import tracksrequest as components_tracksrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateParcelRequest:
+class CreateTrackGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    parcel_request: Optional[components_parcelrequest.ParcelRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Parcel details."""
+    
+
+
+
+@dataclasses.dataclass
+class CreateTrackRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    tracks_request: Optional[components_tracksrequest.TracksRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createpickup.py` & `shippo-3.2.2/src/shippo/models/operations/createshippoaccount.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import pickupbase as components_pickupbase
+from ...models.components import shippoaccountupdaterequest as components_shippoaccountupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreatePickupRequest:
+class CreateShippoAccountGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    pickup_base: Optional[components_pickupbase.PickupBase] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Shippo’s pickups endpoint allows you to schedule pickups with USPS and DHL Express for eligible shipments that you have already created."""
+    
+
+
+
+@dataclasses.dataclass
+class CreateShippoAccountRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    shippo_account_update_request: Optional[components_shippoaccountupdaterequest.ShippoAccountUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createrefund.py` & `shippo-3.2.2/src/shippo/models/operations/getshippoaccount.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import refundrequestbody as components_refundrequestbody
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateRefundRequest:
+class GetShippoAccountGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetShippoAccountRequest:
+    shippo_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShippoAccountId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the ShippoAccount"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    refund_request_body: Optional[components_refundrequestbody.RefundRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Refund details"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createservicegroup.py` & `shippo-3.2.2/src/shippo/models/operations/createservicegroup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,13 +3,21 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import servicegroupcreaterequest as components_servicegroupcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class CreateServiceGroupGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateServiceGroupRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     service_group_create_request: Optional[components_servicegroupcreaterequest.ServiceGroupCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createshipment.py` & `shippo-3.2.2/src/shippo/models/operations/getrate.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import shipmentcreaterequest as components_shipmentcreaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateShipmentRequest:
+class GetRateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetRateRequest:
+    rate_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'RateId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the rate"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    shipment_create_request: Optional[components_shipmentcreaterequest.ShipmentCreateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Shipment details and contact info."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createtrack.py` & `shippo-3.2.2/src/shippo/models/operations/purchasebatch.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,23 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import tracksrequest as components_tracksrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class CreateTrackRequest:
+class PurchaseBatchGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class PurchaseBatchRequest:
+    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the batch"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    tracks_request: Optional[components_tracksrequest.TracksRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createtransaction.py` & `shippo-3.2.2/src/shippo/models/operations/createtransaction.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 import dataclasses
 from ...models.components import instanttransactionrequestbody as components_instanttransactionrequestbody
 from ...models.components import transactioncreaterequest as components_transactioncreaterequest
 from typing import Optional, Union
 
 
 @dataclasses.dataclass
+class CreateTransactionGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateTransactionRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     request_body: Optional[Union[components_transactioncreaterequest.TransactionCreateRequest, components_instanttransactionrequestbody.InstantTransactionRequestBody]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/createuserparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/createuserparceltemplate.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,13 +4,21 @@
 import dataclasses
 from ...models.components import userparceltemplatewithcarriertemplatecreaterequest as components_userparceltemplatewithcarriertemplatecreaterequest
 from ...models.components import userparceltemplatewithoutcarriertemplatecreaterequest as components_userparceltemplatewithoutcarriertemplatecreaterequest
 from typing import Optional, Union
 
 
 @dataclasses.dataclass
+class CreateUserParcelTemplateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class CreateUserParcelTemplateRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     user_parcel_template_create_request: Optional[Union[components_userparceltemplatewithcarriertemplatecreaterequest.UserParcelTemplateWithCarrierTemplateCreateRequest, components_userparceltemplatewithoutcarriertemplatecreaterequest.UserParcelTemplateWithoutCarrierTemplateCreateRequest]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/deletedefaultparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/deletedefaultparceltemplate.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class DeleteDefaultParcelTemplateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class DeleteDefaultParcelTemplateRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/deleteservicegroup.py` & `shippo-3.2.2/src/shippo/models/operations/listservicegroups.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,19 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DeleteServiceGroupRequest:
-    service_group_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ServiceGroupId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the service group"""
+class ListServiceGroupsGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class DeleteServiceGroupResponse:
-    pass
+class ListServiceGroupsRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/deleteuserparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/getuserparceltemplate.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,19 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class DeleteUserParcelTemplateRequest:
-    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the user parcel template"""
+class GetUserParcelTemplateGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
 
 
 @dataclasses.dataclass
-class DeleteUserParcelTemplateResponse:
-    pass
+class GetUserParcelTemplateRequest:
+    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the user parcel template"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getaddress.py` & `shippo-3.2.2/src/shippo/models/operations/getorder.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetAddressRequest:
-    address_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'AddressId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the address"""
+class GetOrderGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetOrderRequest:
+    order_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'OrderId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the order"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getbatch.py` & `shippo-3.2.2/src/shippo/models/operations/getbatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetBatchGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetBatchRequest:
     batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the batch"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getcarrieraccount.py` & `shippo-3.2.2/src/shippo/models/operations/getmanifest.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetCarrierAccountRequest:
-    carrier_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CarrierAccountId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the carrier account"""
+class GetManifestGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetManifestRequest:
+    manifest_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ManifestId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the manifest to update"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getcarrierparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/getcarrierparceltemplate.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetCarrierParcelTemplateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetCarrierParcelTemplateRequest:
     carrier_parcel_template_token: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CarrierParcelTemplateToken', 'style': 'simple', 'explode': False }})
     r"""The unique string representation of the carrier parcel template"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getcarrierregistrationstatus.py` & `shippo-3.2.2/src/shippo/models/operations/getcarrierregistrationstatus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from enum import Enum
 from typing import Optional
 
+
+@dataclasses.dataclass
+class GetCarrierRegistrationStatusGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
 class Carrier(str, Enum):
     r"""filter by specific carrier"""
     UPS = 'ups'
     USPS = 'usps'
     CANADA_POST = 'canada_post'
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getcustomsdeclaration.py` & `shippo-3.2.2/src/shippo/models/operations/getcustomsdeclaration.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetCustomsDeclarationGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetCustomsDeclarationRequest:
     customs_declaration_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CustomsDeclarationId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the customs declaration"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getcustomsitem.py` & `shippo-3.2.2/src/shippo/models/operations/getcustomsitem.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetCustomsItemGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetCustomsItemRequest:
     customs_item_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CustomsItemId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the customs item"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getmanifest.py` & `shippo-3.2.2/src/shippo/models/operations/removeshipmentsfrombatch.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import Optional
+from typing import List, Optional
 
 
 @dataclasses.dataclass
-class GetManifestRequest:
-    manifest_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ManifestId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the manifest to update"""
+class RemoveShipmentsFromBatchGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
+
+
+@dataclasses.dataclass
+class RemoveShipmentsFromBatchRequest:
+    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the batch"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Array of shipments object ids to remove from the batch"""
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getorder.py` & `shippo-3.2.2/src/shippo/models/operations/getdefaultparceltemplate.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetOrderRequest:
-    order_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'OrderId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the order"""
+class GetDefaultParcelTemplateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetDefaultParcelTemplateRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getparcel.py` & `shippo-3.2.2/src/shippo/models/operations/listuserparceltemplates.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetParcelRequest:
-    parcel_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ParcelId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the parcel"""
+class ListUserParcelTemplatesGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListUserParcelTemplatesRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getrate.py` & `shippo-3.2.2/src/shippo/models/operations/deleteuserparceltemplate.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,27 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetRateRequest:
-    rate_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'RateId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the rate"""
+class DeleteUserParcelTemplateGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
+
+
+@dataclasses.dataclass
+class DeleteUserParcelTemplateRequest:
+    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the user parcel template"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class DeleteUserParcelTemplateResponse:
+    pass
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getrefund.py` & `shippo-3.2.2/src/shippo/models/operations/getrefund.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetRefundGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetRefundRequest:
     refund_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'RefundId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the refund to update"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getshipment.py` & `shippo-3.2.2/src/shippo/models/operations/updatecarrieraccount.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,15 +1,26 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
+from ...models.components import carrieraccountbase as components_carrieraccountbase
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetShipmentRequest:
-    shipment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShipmentId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the shipment to update"""
+class UpdateCarrierAccountGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     
 
+
+
+@dataclasses.dataclass
+class UpdateCarrierAccountRequest:
+    carrier_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CarrierAccountId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the carrier account"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    carrier_account_base: Optional[components_carrieraccountbase.CarrierAccountBase] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Examples."""
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getshippoaccount.py` & `shippo-3.2.2/src/shippo/models/operations/listrefunds.py`

 * *Files 26% similar despite different names*

```diff
@@ -2,14 +2,20 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetShippoAccountRequest:
-    shippo_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShippoAccountId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the ShippoAccount"""
+class ListRefundsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListRefundsRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/gettrack.py` & `shippo-3.2.2/src/shippo/models/operations/getcarrieraccount.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetTrackRequest:
-    tracking_number: str = dataclasses.field(metadata={'path_param': { 'field_name': 'TrackingNumber', 'style': 'simple', 'explode': False }})
-    r"""Tracking number"""
-    carrier: str = dataclasses.field(metadata={'path_param': { 'field_name': 'Carrier', 'style': 'simple', 'explode': False }})
-    r"""Name of the carrier"""
+class GetCarrierAccountGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetCarrierAccountRequest:
+    carrier_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CarrierAccountId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the carrier account"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/gettransaction.py` & `shippo-3.2.2/src/shippo/models/operations/gettransaction.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class GetTransactionGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class GetTransactionRequest:
     transaction_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'TransactionId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the transaction to update"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/getuserparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/validateaddress.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class GetUserParcelTemplateRequest:
-    user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the user parcel template"""
+class ValidateAddressGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ValidateAddressRequest:
+    address_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'AddressId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the address"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listaddresses.py` & `shippo-3.2.2/src/shippo/models/operations/getaddress.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListAddressesRequest:
-    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+class GetAddressGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetAddressRequest:
+    address_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'AddressId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the address"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listcarrieraccounts.py` & `shippo-3.2.2/src/shippo/models/operations/listcarrieraccounts.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,22 +3,30 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import carriers as components_carriers
 from typing import Optional
 
 
 @dataclasses.dataclass
+class ListCarrierAccountsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class ListCarrierAccountsRequest:
     service_levels: Optional[bool] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'service_levels', 'style': 'form', 'explode': True }})
     r"""Appends the property `service_levels` to each returned carrier account"""
     carrier: Optional[components_carriers.Carriers] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'carrier', 'style': 'form', 'explode': True }})
     r"""Filter the response by the specified carrier"""
     account_id: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'account_id', 'style': 'form', 'explode': True }})
     r"""Filter the response by the specified carrier account Id"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+    results: Optional[int] = dataclasses.field(default=5, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
+    r"""The number of results to return per page (max 100, default 5)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listcarrierparceltemplates.py` & `shippo-3.2.2/src/shippo/models/operations/listcarrierparceltemplates.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,22 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
 from enum import Enum
 from typing import Optional
 
+
+@dataclasses.dataclass
+class ListCarrierParcelTemplatesGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
 class Include(str, Enum):
     r"""filter by user or enabled"""
     ALL = 'all'
     USER = 'user'
     ENABLED = 'enabled'
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listcustomsdeclarations.py` & `shippo-3.2.2/src/shippo/models/operations/listshipments.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListCustomsDeclarationsRequest:
+class ListShipmentsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListShipmentsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listcustomsitems.py` & `shippo-3.2.2/src/shippo/models/operations/getshipment.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,16 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListCustomsItemsRequest:
-    page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
-    r"""The page number you want to select"""
-    results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
-    r"""The number of results to return per page (max 100)"""
+class GetShipmentGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetShipmentRequest:
+    shipment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShipmentId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the shipment to update"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listmanifests.py` & `shippo-3.2.2/src/shippo/models/operations/listcustomsdeclarations.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListManifestsRequest:
+class ListCustomsDeclarationsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListCustomsDeclarationsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listorders.py` & `shippo-3.2.2/src/shippo/models/operations/listshipmentrates.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,25 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListOrdersRequest:
+class ListShipmentRatesGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListShipmentRatesRequest:
+    shipment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShipmentId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the shipment to update"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listparcels.py` & `shippo-3.2.2/src/shippo/models/operations/listparcels.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class ListParcelsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class ListParcelsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listshipmentrates.py` & `shippo-3.2.2/src/shippo/models/operations/listorders.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,17 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShipmentRatesRequest:
-    shipment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShipmentId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the shipment to update"""
+class ListOrdersGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListOrdersRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listshipmentratesbycurrencycode.py` & `shippo-3.2.2/src/shippo/models/operations/listshipmentratesbycurrencycode.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
+class ListShipmentRatesByCurrencyCodeGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class ListShipmentRatesByCurrencyCodeRequest:
     shipment_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShipmentId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the shipment to update"""
     currency_code: str = dataclasses.field(default='USD', metadata={'path_param': { 'field_name': 'CurrencyCode', 'style': 'simple', 'explode': False }})
     r"""ISO currency code for the rates"""
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listshipments.py` & `shippo-3.2.2/src/shippo/models/operations/listshippoaccounts.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShipmentsRequest:
+class ListShippoAccountsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListShippoAccountsRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listshippoaccounts.py` & `shippo-3.2.2/src/shippo/models/operations/listaddresses.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,23 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ListShippoAccountsRequest:
+class ListAddressesGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class ListAddressesRequest:
     page: Optional[int] = dataclasses.field(default=1, metadata={'query_param': { 'field_name': 'page', 'style': 'form', 'explode': True }})
     r"""The page number you want to select"""
     results: Optional[int] = dataclasses.field(default=25, metadata={'query_param': { 'field_name': 'results', 'style': 'form', 'explode': True }})
     r"""The number of results to return per page (max 100)"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/listtransactions.py` & `shippo-3.2.2/src/shippo/models/operations/listtransactions.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,14 +4,22 @@
 import dataclasses
 from ...models.components import trackingstatusenum as components_trackingstatusenum
 from ...models.components import transactionstatusenum as components_transactionstatusenum
 from typing import Optional
 
 
 @dataclasses.dataclass
+class ListTransactionsGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class ListTransactionsRequest:
     rate: Optional[str] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'rate', 'style': 'form', 'explode': True }})
     r"""Filter by rate ID"""
     object_status: Optional[components_transactionstatusenum.TransactionStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'object_status', 'style': 'form', 'explode': True }})
     r"""Filter by object status"""
     tracking_status: Optional[components_trackingstatusenum.TrackingStatusEnum] = dataclasses.field(default=None, metadata={'query_param': { 'field_name': 'tracking_status', 'style': 'form', 'explode': True }})
     r"""Filter by tracking status"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/registercarrieraccount.py` & `shippo-3.2.2/src/shippo/models/operations/registercarrieraccount.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,14 +14,22 @@
 from ...models.components import carrieraccountposteitalianecreaterequest as components_carrieraccountposteitalianecreaterequest
 from ...models.components import carrieraccountupscreaterequest as components_carrieraccountupscreaterequest
 from ...models.components import carrieraccountuspscreaterequest as components_carrieraccountuspscreaterequest
 from typing import Optional, Union
 
 
 @dataclasses.dataclass
+class RegisterCarrierAccountGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class RegisterCarrierAccountRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     request_body: Optional[Union[components_carrieraccountcanadapostcreaterequest.CarrierAccountCanadaPostCreateRequest, components_carrieraccountchronopostcreaterequest.CarrierAccountChronopostCreateRequest, components_carrieraccountcolissimocreaterequest.CarrierAccountColissimoCreateRequest, components_carrieraccountcorreoscreaterequest.CarrierAccountCorreosCreateRequest, components_carrieraccountdeutschepostcreaterequest.CarrierAccountDeutschePostCreateRequest, components_carrieraccountdhlexpresscreaterequest.CarrierAccountDHLExpressCreateRequest, components_carrieraccountdpddecreaterequest.CarrierAccountDpdDeCreateRequest, components_carrieraccountdpdukcreaterequest.CarrierAccountDPDUKCreateRequest, components_carrieraccounthermesukcreaterequest.CarrierAccountHermesUKCreateRequest, components_carrieraccountposteitalianecreaterequest.CarrierAccountPosteItalianeCreateRequest, components_carrieraccountupscreaterequest.CarrierAccountUPSCreateRequest, components_carrieraccountuspscreaterequest.CarrierAccountUSPSCreateRequest]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/removeshipmentsfrombatch.py` & `shippo-3.2.2/src/shippo/models/operations/createrefund.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from typing import List, Optional
+from ...models.components import refundrequestbody as components_refundrequestbody
+from typing import Optional
 
 
 @dataclasses.dataclass
-class RemoveShipmentsFromBatchRequest:
-    batch_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'BatchId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the batch"""
+class CreateRefundGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    request_body: Optional[List[str]] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
-    r"""Array of shipments object ids to remove from the batch"""
+    
+
+
+
+@dataclasses.dataclass
+class CreateRefundRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    refund_request_body: Optional[components_refundrequestbody.RefundRequestBody] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    r"""Refund details"""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/updatecarrieraccount.py` & `shippo-3.2.2/src/shippo/models/operations/createcarrieraccount.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,24 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import carrieraccountbase as components_carrieraccountbase
+from ...models.components import connectexistingownupsaccountrequest as components_connectexistingownupsaccountrequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class UpdateCarrierAccountRequest:
-    carrier_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'CarrierAccountId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the carrier account"""
+class CreateCarrierAccountGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    carrier_account_base: Optional[components_carrieraccountbase.CarrierAccountBase] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
+    
+
+
+
+@dataclasses.dataclass
+class CreateCarrierAccountRequest:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    connect_existing_own_ups_account_request: Optional[components_connectexistingownupsaccountrequest.ConnectExistingOwnUPSAccountRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     r"""Examples."""
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/updatedefaultparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/deleteservicegroup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,28 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 from __future__ import annotations
 import dataclasses
-from ...models.components import defaultparceltemplateupdaterequest as components_defaultparceltemplateupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
-class UpdateDefaultParcelTemplateRequest:
+class DeleteServiceGroupGlobals:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
-    default_parcel_template_update_request: Optional[components_defaultparceltemplateupdaterequest.DefaultParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
     
 
+
+
+@dataclasses.dataclass
+class DeleteServiceGroupRequest:
+    service_group_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ServiceGroupId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the service group"""
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class DeleteServiceGroupResponse:
+    pass
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/updateservicegroup.py` & `shippo-3.2.2/src/shippo/models/operations/updateservicegroup.py`

 * *Files 15% similar despite different names*

```diff
@@ -3,13 +3,21 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import servicegroupupdaterequest as components_servicegroupupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class UpdateServiceGroupGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class UpdateServiceGroupRequest:
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     service_group_update_request: Optional[components_servicegroupupdaterequest.ServiceGroupUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/updateshippoaccount.py` & `shippo-3.2.2/src/shippo/models/operations/updateshippoaccount.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import shippoaccountupdaterequest as components_shippoaccountupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class UpdateShippoAccountGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class UpdateShippoAccountRequest:
     shippo_account_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ShippoAccountId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the ShippoAccount"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     shippo_account_update_request: Optional[components_shippoaccountupdaterequest.ShippoAccountUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/updateuserparceltemplate.py` & `shippo-3.2.2/src/shippo/models/operations/updateuserparceltemplate.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from __future__ import annotations
 import dataclasses
 from ...models.components import userparceltemplateupdaterequest as components_userparceltemplateupdaterequest
 from typing import Optional
 
 
 @dataclasses.dataclass
+class UpdateUserParcelTemplateGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
 class UpdateUserParcelTemplateRequest:
     user_parcel_template_object_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'UserParcelTemplateObjectId', 'style': 'simple', 'explode': False }})
     r"""Object ID of the user parcel template"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
     user_parcel_template_update_request: Optional[components_userparceltemplateupdaterequest.UserParcelTemplateUpdateRequest] = dataclasses.field(default=None, metadata={'request': { 'media_type': 'application/json' }})
```

### Comparing `shippo-3.2.0/src/shippo/models/operations/validateaddress.py` & `shippo-3.2.2/src/shippo/models/operations/getparcel.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,22 @@
 
 from __future__ import annotations
 import dataclasses
 from typing import Optional
 
 
 @dataclasses.dataclass
-class ValidateAddressRequest:
-    address_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'AddressId', 'style': 'simple', 'explode': False }})
-    r"""Object ID of the address"""
+class GetParcelGlobals:
+    shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
+    r"""String used to pick a non-default API version to use"""
+    
+
+
+
+@dataclasses.dataclass
+class GetParcelRequest:
+    parcel_id: str = dataclasses.field(metadata={'path_param': { 'field_name': 'ParcelId', 'style': 'simple', 'explode': False }})
+    r"""Object ID of the parcel"""
     shippo_api_version: Optional[str] = dataclasses.field(default=None, metadata={'header': { 'field_name': 'SHIPPO-API-VERSION', 'style': 'simple', 'explode': False }})
     r"""String used to pick a non-default API version to use"""
```

### Comparing `shippo-3.2.0/src/shippo/orders.py` & `shippo-3.2.2/src/shippo/orders.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,25 +36,29 @@
         hook_ctx = HookContext(operation_id='ListOrders', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListOrdersRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListOrdersGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/orders'
+        url = utils.generate_url(base_url, '/orders', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListOrdersRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -96,27 +100,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateOrder', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateOrderRequest(
             shippo_api_version=shippo_api_version,
             order_create_request=order_create_request,
         )
         
+        _globals = operations.CreateOrderGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/orders'
+        url = utils.generate_url(base_url, '/orders', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateOrderRequest, "order_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -158,24 +167,29 @@
         """
         hook_ctx = HookContext(operation_id='GetOrder', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetOrderRequest(
             order_id=order_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetOrderGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetOrderRequest, base_url, '/orders/{OrderId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/orders/{OrderId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -205,8 +219,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/parcels.py` & `shippo-3.2.2/src/shippo/parcels.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,25 +29,29 @@
         hook_ctx = HookContext(operation_id='ListParcels', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListParcelsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListParcelsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/parcels'
+        url = utils.generate_url(base_url, '/parcels', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListParcelsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -89,27 +93,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateParcelRequest(
             shippo_api_version=shippo_api_version,
             parcel_request=parcel_request,
         )
         
+        _globals = operations.CreateParcelGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/parcels'
+        url = utils.generate_url(base_url, '/parcels', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateParcelRequest, "parcel_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -151,24 +160,29 @@
         """
         hook_ctx = HookContext(operation_id='GetParcel', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetParcelRequest(
             parcel_id=parcel_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetParcelGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetParcelRequest, base_url, '/parcels/{ParcelId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/parcels/{ParcelId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -198,8 +212,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/pickups.py` & `shippo-3.2.2/src/shippo/pickups.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,27 +25,32 @@
         """
         hook_ctx = HookContext(operation_id='CreatePickup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreatePickupRequest(
             shippo_api_version=shippo_api_version,
             pickup_base=pickup_base,
         )
         
+        _globals = operations.CreatePickupGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/pickups'
+        url = utils.generate_url(base_url, '/pickups', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreatePickupRequest, "pickup_base", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -75,8 +80,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/rates.py` & `shippo-3.2.2/src/shippo/rates.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,24 +24,29 @@
         """
         hook_ctx = HookContext(operation_id='GetRate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetRateRequest(
             rate_id=rate_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetRateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRateRequest, base_url, '/rates/{RateId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/rates/{RateId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -85,25 +90,29 @@
         request = operations.ListShipmentRatesRequest(
             shipment_id=shipment_id,
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListShipmentRatesGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListShipmentRatesRequest, base_url, '/shipments/{ShipmentId}/rates', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/shipments/{ShipmentId}/rates', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentRatesRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -146,25 +155,29 @@
         When you create a new valid shipment object, Shippo automatically calculates all available rates. Depending on your shipment data, there may be none, one or multiple rates.
 
         By default, the calculated rates will return the price in two currencies under the `amount` and `amount_local` keys, respectively. The `amount` key will contain the price of a rate expressed in the currency that is used in the country from where the parcel originates, and the `amount_local` key will contain the price expressed in the currency that is used in the country the parcel is shipped to. You can request rates with prices expressed in a different currency by adding the currency code to the end of the resource URL. The full list of supported currencies along with their codes can be viewed on <a href=\"http://openexchangerates.org/api/currencies.json\">open exchange rates</a>.
 
         Note: re-requesting the rates with a different currency code will re-queue the shipment (i.e. set the Shipment's `status` to `QUEUED`) and the converted currency rates will only be available when the Shipment's `status` is set to `SUCCESS`.
         """
         hook_ctx = HookContext(operation_id='ListShipmentRatesByCurrencyCode', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.ListShipmentRatesByCurrencyCodeGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.ListShipmentRatesByCurrencyCodeRequest, base_url, '/shipments/{ShipmentId}/rates/{CurrencyCode}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/shipments/{ShipmentId}/rates/{CurrencyCode}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentRatesByCurrencyCodeRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -194,8 +207,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/rates_at_checkout.py` & `shippo-3.2.2/src/shippo/shippo_accounts.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,64 +3,59 @@
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
 from typing import Optional
 
-class RatesAtCheckout:
-    r"""Rates at checkout is a tool for merchants to display up-to-date shipping estimates based on what's in their customers cart and where they’re shipping to.
-    Merchants set up curated shipping options for customers in the checkout flow based on data in the shopping cart. The request must include the **to** address and item information. Optional fields are the **from** address and package information. If the optional fields are not included, the service will use the default address and/or package configured for rates at checkout. The response is a list of shipping options based on the Service Group configuration.
-    (see <a href=\"#tag/Service-Groups\">Service Group configuration</a> for details).
-    <SchemaDefinition schemaRef=\"#/components/schemas/LiveRate\"/>
-
-
-    # Default Parcel Template
-    Assign one of your user parcel templates to be the default used when generating Live Rates. This template will be used by default when generating Live Rates, unless you explicitly provide a parcel in the Live Rates request.
-    <SchemaDefinition schemaRef=\"#/components/schemas/UserParcelTemplate\"/>
+class ShippoAccounts:
+    r"""Shippo Accounts are used by Shippo Platform Accounts to create and manage Managed Shippo Accounts.
+    Managed Shippo Accounts are headless accounts that represent your customers. They are opaque to your end customers, meaning customers do not need to create their own Shippo login or have a billing relationship with Shippo. 
+    They can be used by marketplaces, e-commerce platforms, and third-party logistics providers who want to offer, seamless, built-in shipping functionality to their customers. 
+    <SchemaDefinition schemaRef=\"#/components/schemas/ShippoAccount\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def create(self, shippo_api_version: Optional[str] = None, live_rate_create_request: Optional[components.LiveRateCreateRequest] = None) -> components.LiveRatePaginatedList:
-        r"""Generate a live rates request
-        Initiates a live rates request. Include either the object ID for
-        an existing address record or a fully formed address object when entering
-        an address value. You can also enter the object ID of an existing user parcel
-        template or a fully formed user parcel template object as the parcel value.
+    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ShippoAccountPaginatedList:
+        r"""List all Shippo Accounts
+        Returns a list of Shippo Accounts objects
         """
-        hook_ctx = HookContext(operation_id='CreateLiveRate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateLiveRateRequest(
+        hook_ctx = HookContext(operation_id='ListShippoAccounts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.ListShippoAccountsRequest(
+            page=page,
+            results=results,
             shippo_api_version=shippo_api_version,
-            live_rate_create_request=live_rate_create_request,
+        )
+        
+        _globals = operations.ListShippoAccountsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/live-rates'
+        url = utils.generate_url(base_url, '/shippo-accounts', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateLiveRateRequest, "live_rate_create_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -74,51 +69,60 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.LiveRatePaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccountPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get_default_parcel_template(self, shippo_api_version: Optional[str] = None) -> components.DefaultParcelTemplate:
-        r"""Show current default parcel template
-        Retrieve and display the currently configured default parcel template for live rates.
+    def create(self, shippo_api_version: Optional[str] = None, shippo_account_update_request: Optional[components.ShippoAccountUpdateRequest] = None) -> components.ShippoAccount:
+        r"""Create a Shippo Account
+        Creates a Shippo Account object
         """
-        hook_ctx = HookContext(operation_id='GetDefaultParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetDefaultParcelTemplateRequest(
+        hook_ctx = HookContext(operation_id='CreateShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateShippoAccountRequest(
             shippo_api_version=shippo_api_version,
+            shippo_account_update_request=shippo_account_update_request,
+        )
+        
+        _globals = operations.CreateShippoAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/live-rates/settings/parcel-template'
+        url = utils.generate_url(base_url, '/shippo-accounts', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -132,55 +136,57 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def update_default_parcel_template(self, shippo_api_version: Optional[str] = None, default_parcel_template_update_request: Optional[components.DefaultParcelTemplateUpdateRequest] = None) -> components.DefaultParcelTemplate:
-        r"""Update default parcel template
-        Update the currently configured default parcel template for live rates. The object_id in the request payload should identify the user parcel template to be the new default.
+    def get(self, shippo_account_id: str, shippo_api_version: Optional[str] = None) -> components.ShippoAccount:
+        r"""Retrieve a Shippo Account
+        Returns a Shippo Account using an object ID
         """
-        hook_ctx = HookContext(operation_id='UpdateDefaultParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.UpdateDefaultParcelTemplateRequest(
+        hook_ctx = HookContext(operation_id='GetShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetShippoAccountRequest(
+            shippo_account_id=shippo_account_id,
             shippo_api_version=shippo_api_version,
-            default_parcel_template_update_request=default_parcel_template_update_request,
+        )
+        
+        _globals = operations.GetShippoAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/live-rates/settings/parcel-template'
+        url = utils.generate_url(base_url, '/shippo-accounts/{ShippoAccountId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateDefaultParcelTemplateRequest, "default_parcel_template_update_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
+            req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -194,51 +200,61 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.DefaultParcelTemplate])
+                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def delete_default_parcel_template(self, shippo_api_version: Optional[str] = None) -> operations.DeleteDefaultParcelTemplateResponse:
-        r"""Clear current default parcel template
-        Clears the currently configured default parcel template for live rates.
+    def update(self, shippo_account_id: str, shippo_api_version: Optional[str] = None, shippo_account_update_request: Optional[components.ShippoAccountUpdateRequest] = None) -> components.ShippoAccount:
+        r"""Update a Shippo Account
+        Updates a Shippo Account object
         """
-        hook_ctx = HookContext(operation_id='DeleteDefaultParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.DeleteDefaultParcelTemplateRequest(
+        hook_ctx = HookContext(operation_id='UpdateShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.UpdateShippoAccountRequest(
+            shippo_account_id=shippo_account_id,
             shippo_api_version=shippo_api_version,
+            shippo_account_update_request=shippo_account_update_request,
+        )
+        
+        _globals = operations.UpdateShippoAccountGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/live-rates/settings/parcel-template'
+        url = utils.generate_url(base_url, '/shippo-accounts/{ShippoAccountId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        headers['Accept'] = '*/*'
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
+        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
+            headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
+        headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
-            req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
+            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
             http_res = client.send(req)
         except Exception as e:
             _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
             if e is not None:
                 raise e
 
@@ -249,19 +265,22 @@
             if result is not None:
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
-        res = operations.DeleteDefaultParcelTemplateResponse()
         
-        if http_res.status_code == 204:
-            pass
+        if http_res.status_code == 200:
+            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
+                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
+                return out
+            
+            content_type = http_res.headers.get('Content-Type')
+            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-        return res
+    
 
-
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `shippo-3.2.0/src/shippo/refunds.py` & `shippo-3.2.2/src/shippo/refunds.py`

 * *Files 6% similar despite different names*

```diff
@@ -24,27 +24,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateRefundRequest(
             shippo_api_version=shippo_api_version,
             refund_request_body=refund_request_body,
         )
         
+        _globals = operations.CreateRefundGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/refunds'
+        url = utils.generate_url(base_url, '/refunds', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateRefundRequest, "refund_request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -85,24 +90,29 @@
         Returns a list all refund objects.
         """
         hook_ctx = HookContext(operation_id='ListRefunds', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListRefundsRequest(
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListRefundsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/refunds/'
+        url = utils.generate_url(base_url, '/refunds/', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -144,24 +154,29 @@
         """
         hook_ctx = HookContext(operation_id='GetRefund', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetRefundRequest(
             refund_id=refund_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetRefundGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetRefundRequest, base_url, '/refunds/{RefundId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/refunds/{RefundId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -191,8 +206,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/sdk.py` & `shippo-3.2.2/src/shippo/sdk.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 from .shippo_accounts import ShippoAccounts
 from .tracking_status import TrackingStatus
 from .transactions import Transactions
 from .user_parcel_templates import UserParcelTemplates
 from .utils.retries import RetryConfig
 from shippo import utils
 from shippo._hooks import SDKHooks
-from shippo.models import components
+from shippo.models import components, internal
 from typing import Callable, Dict, Optional, Union
 
 class Shippo:
     r"""Shippo external API.: Use this API to integrate with the Shippo service"""
     addresses: Addresses
     r"""Addresses are the locations a parcel is being shipped **from** and **to**. They represent company and residential places. Among other things, you can use address objects to create shipments, calculate shipping rates, and purchase shipping labels.
     <SchemaDefinition schemaRef=\"#/components/schemas/Address\"/>
@@ -203,44 +203,37 @@
                 return components.Security(api_key_header = api_key_header())
         else:
             security = components.Security(api_key_header = api_key_header)
 
         if server_url is not None:
             if url_params is not None:
                 server_url = utils.template_url(server_url, url_params)
-        global_params = {
-            'parameters': {
-                'queryParam': {
-                },
-                'pathParam': {
-                },
-                'header': {
-                    'shippo_api_version': shippo_api_version,
-                },
-            },
-        }
+    
+        _globals = internal.Globals(
+            shippo_api_version=shippo_api_version,
+        )
 
         self.sdk_configuration = SDKConfiguration(
             client,
+            _globals,
             security,
             server_url,
             server_idx,
-            global_params,
             retry_config=retry_config
         )
 
         hooks = SDKHooks()
 
         current_server_url, *_ = self.sdk_configuration.get_server_details()
         server_url, self.sdk_configuration.client = hooks.sdk_init(current_server_url, self.sdk_configuration.client)
         if current_server_url != server_url:
             self.sdk_configuration.server_url = server_url
 
         # pylint: disable=protected-access
-        self.sdk_configuration._hooks = hooks
+        self.sdk_configuration.__dict__['_hooks'] = hooks
 
         self._init_sdks()
 
 
     def _init_sdks(self):
         self.addresses = Addresses(self.sdk_configuration)
         self.batches = Batches(self.sdk_configuration)
```

### Comparing `shippo-3.2.0/src/shippo/sdkconfiguration.py` & `shippo-3.2.2/src/shippo/sdkconfiguration.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,40 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 
 import requests as requests_http
 from ._hooks import SDKHooks
 from .utils import utils
 from .utils.retries import RetryConfig
-from dataclasses import dataclass, field
-from shippo.models import components
-from typing import Any, Callable, Dict, Optional, Tuple, Union
+from dataclasses import dataclass
+from shippo.models import components, internal
+from typing import Callable, Dict, Optional, Tuple, Union
 
 
 SERVERS = [
     'https://api.goshippo.com',
 ]
 """Contains the list of servers available to the SDK"""
 
 @dataclass
 class SDKConfiguration:
     client: requests_http.Session
+    globals: internal.Globals
     security: Union[components.Security,Callable[[], components.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
-    globals: Dict[str, Dict[str, Dict[str, Any]]] = field(default_factory=Dict)
     language: str = 'python'
     openapi_doc_version: str = '2018-02-08'
-    sdk_version: str = '3.2.0'
-    gen_version: str = '2.298.2'
-    user_agent: str = 'speakeasy-sdk/python 3.2.0 2.298.2 2018-02-08 shippo'
+    sdk_version: str = '3.2.2'
+    gen_version: str = '2.301.0'
+    user_agent: str = 'speakeasy-sdk/python 3.2.2 2.301.0 2018-02-08 shippo'
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

### Comparing `shippo-3.2.0/src/shippo/service_groups.py` & `shippo-3.2.2/src/shippo/service_groups.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,24 +24,29 @@
         Returns a list of service group objects.
         """
         hook_ctx = HookContext(operation_id='ListServiceGroups', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListServiceGroupsRequest(
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListServiceGroupsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/service-groups'
+        url = utils.generate_url(base_url, '/service-groups', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -83,27 +88,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateServiceGroupRequest(
             shippo_api_version=shippo_api_version,
             service_group_create_request=service_group_create_request,
         )
         
+        _globals = operations.CreateServiceGroupGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/service-groups'
+        url = utils.generate_url(base_url, '/service-groups', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateServiceGroupRequest, "service_group_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -145,27 +155,32 @@
         """
         hook_ctx = HookContext(operation_id='UpdateServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.UpdateServiceGroupRequest(
             shippo_api_version=shippo_api_version,
             service_group_update_request=service_group_update_request,
         )
         
+        _globals = operations.UpdateServiceGroupGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/service-groups'
+        url = utils.generate_url(base_url, '/service-groups', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateServiceGroupRequest, "service_group_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -207,24 +222,29 @@
         """
         hook_ctx = HookContext(operation_id='DeleteServiceGroup', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteServiceGroupRequest(
             service_group_id=service_group_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.DeleteServiceGroupGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteServiceGroupRequest, base_url, '/service-groups/{ServiceGroupId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/service-groups/{ServiceGroupId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -252,8 +272,9 @@
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
         return res
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/shipments.py` & `shippo-3.2.2/src/shippo/shipments.py`

 * *Files 3% similar despite different names*

```diff
@@ -46,25 +46,29 @@
         hook_ctx = HookContext(operation_id='ListShipments', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListShipmentsRequest(
             page=page,
             results=results,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListShipmentsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/shipments'
+        url = utils.generate_url(base_url, '/shipments', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListShipmentsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -106,27 +110,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateShipment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateShipmentRequest(
             shippo_api_version=shippo_api_version,
             shipment_create_request=shipment_create_request,
         )
         
+        _globals = operations.CreateShipmentGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/shipments'
+        url = utils.generate_url(base_url, '/shipments', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateShipmentRequest, "shipment_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -168,24 +177,29 @@
         """
         hook_ctx = HookContext(operation_id='GetShipment', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetShipmentRequest(
             shipment_id=shipment_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetShipmentGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetShipmentRequest, base_url, '/shipments/{ShipmentId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/shipments/{ShipmentId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -215,8 +229,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/shippo_accounts.py` & `shippo-3.2.2/src/shippo/transactions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,51 +1,47 @@
 """Code generated by Speakeasy (https://speakeasyapi.dev). DO NOT EDIT."""
 
 import requests as requests_http
 from .sdkconfiguration import SDKConfiguration
 from shippo import utils
 from shippo._hooks import AfterErrorContext, AfterSuccessContext, BeforeRequestContext, HookContext
 from shippo.models import components, errors, operations
-from typing import Optional
+from typing import Optional, Union
 
-class ShippoAccounts:
-    r"""Shippo Accounts are used by Shippo Platform Accounts to create and manage Managed Shippo Accounts.
-    Managed Shippo Accounts are headless accounts that represent your customers. They are opaque to your end customers, meaning customers do not need to create their own Shippo login or have a billing relationship with Shippo. 
-    They can be used by marketplaces, e-commerce platforms, and third-party logistics providers who want to offer, seamless, built-in shipping functionality to their customers. 
-    <SchemaDefinition schemaRef=\"#/components/schemas/ShippoAccount\"/>
+class Transactions:
+    r"""A transaction is the purchase of a shipping label from a shipping provider for a specific service. You can print purchased labels and used them to ship a parcel with a carrier, such as USPS or FedEx.
+    <SchemaDefinition schemaRef=\"#/components/schemas/Transaction\"/>
     """
     sdk_configuration: SDKConfiguration
 
     def __init__(self, sdk_config: SDKConfiguration) -> None:
         self.sdk_configuration = sdk_config
         
     
     
-    def list(self, page: Optional[int] = None, results: Optional[int] = None, shippo_api_version: Optional[str] = None) -> components.ShippoAccountPaginatedList:
-        r"""List all Shippo Accounts
-        Returns a list of Shippo Accounts objects
+    def list(self, request: operations.ListTransactionsRequest) -> components.TransactionPaginatedList:
+        r"""List all shipping labels
+        Returns a list of all transaction objects.
         """
-        hook_ctx = HookContext(operation_id='ListShippoAccounts', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.ListShippoAccountsRequest(
-            page=page,
-            results=results,
-            shippo_api_version=shippo_api_version,
+        hook_ctx = HookContext(operation_id='ListTransactions', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        _globals = operations.ListTransactionsGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/shippo-accounts'
+        url = utils.generate_url(base_url, '/transactions', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        query_params = { **utils.get_query_params(operations.ListShippoAccountsRequest, request, self.sdk_configuration.globals), **query_params }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -65,49 +61,54 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccountPaginatedList])
+                out = utils.unmarshal_json(http_res.text, Optional[components.TransactionPaginatedList])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def create(self, shippo_api_version: Optional[str] = None, shippo_account_update_request: Optional[components.ShippoAccountUpdateRequest] = None) -> components.ShippoAccount:
-        r"""Create a Shippo Account
-        Creates a Shippo Account object
+    def create(self, shippo_api_version: Optional[str] = None, request_body: Optional[Union[components.TransactionCreateRequest, components.InstantTransactionRequestBody]] = None) -> components.Transaction:
+        r"""Create a shipping label
+        Creates a new transaction object and purchases the shipping label using a rate object that has previously been created. <br> OR <br> Creates a new transaction object and purchases the shipping label instantly using shipment details, an existing carrier account, and an existing service level token.
         """
-        hook_ctx = HookContext(operation_id='CreateShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.CreateShippoAccountRequest(
+        hook_ctx = HookContext(operation_id='CreateTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.CreateTransactionRequest(
             shippo_api_version=shippo_api_version,
-            shippo_account_update_request=shippo_account_update_request,
+            request_body=request_body,
+        )
+        
+        _globals = operations.CreateTransactionGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
         )
         
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/shippo-accounts'
+        url = utils.generate_url(base_url, '/transactions', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
+        headers = { **utils.get_headers(request, _globals), **headers }
+        req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTransactionRequest, "request_body", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -125,48 +126,53 @@
                 http_res = result
         else:
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
-        if http_res.status_code == 200:
+        if http_res.status_code == 201:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
     
-    def get(self, shippo_account_id: str, shippo_api_version: Optional[str] = None) -> components.ShippoAccount:
-        r"""Retrieve a Shippo Account
-        Returns a Shippo Account using an object ID
+    def get(self, transaction_id: str, shippo_api_version: Optional[str] = None) -> components.Transaction:
+        r"""Retrieve a shipping label
+        Returns an existing transaction using an object ID.
         """
-        hook_ctx = HookContext(operation_id='GetShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.GetShippoAccountRequest(
-            shippo_account_id=shippo_account_id,
+        hook_ctx = HookContext(operation_id='GetTransaction', oauth2_scopes=[], security_source=self.sdk_configuration.security)
+        request = operations.GetTransactionRequest(
+            transaction_id=transaction_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetTransactionGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/transactions/{TransactionId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -186,81 +192,19 @@
             http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
             
         
         
         
         if http_res.status_code == 200:
             if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
+                out = utils.unmarshal_json(http_res.text, Optional[components.Transaction])
                 return out
             
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
     
-    
-    def update(self, shippo_account_id: str, shippo_api_version: Optional[str] = None, shippo_account_update_request: Optional[components.ShippoAccountUpdateRequest] = None) -> components.ShippoAccount:
-        r"""Update a Shippo Account
-        Updates a Shippo Account object
-        """
-        hook_ctx = HookContext(operation_id='UpdateShippoAccount', oauth2_scopes=[], security_source=self.sdk_configuration.security)
-        request = operations.UpdateShippoAccountRequest(
-            shippo_account_id=shippo_account_id,
-            shippo_api_version=shippo_api_version,
-            shippo_account_update_request=shippo_account_update_request,
-        )
-        
-        base_url = utils.template_url(*self.sdk_configuration.get_server_details())
-        
-        url = utils.generate_url(operations.UpdateShippoAccountRequest, base_url, '/shippo-accounts/{ShippoAccountId}', request, self.sdk_configuration.globals)
-        
-        if callable(self.sdk_configuration.security):
-            headers, query_params = utils.get_security(self.sdk_configuration.security())
-        else:
-            headers, query_params = utils.get_security(self.sdk_configuration.security)
-        
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
-        req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateShippoAccountRequest, "shippo_account_update_request", False, True, 'json')
-        if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
-            headers['content-type'] = req_content_type
-        headers['Accept'] = 'application/json'
-        headers['user-agent'] = self.sdk_configuration.user_agent
-        client = self.sdk_configuration.client
-        
-        try:
-            req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
-            req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
-            http_res = client.send(req)
-        except Exception as e:
-            _, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), None, e)
-            if e is not None:
-                raise e
-
-        if utils.match_status_codes(['4XX','5XX'], http_res.status_code):
-            result, e = self.sdk_configuration.get_hooks().after_error(AfterErrorContext(hook_ctx), http_res, None)
-            if e is not None:
-                raise e
-            if result is not None:
-                http_res = result
-        else:
-            http_res = self.sdk_configuration.get_hooks().after_success(AfterSuccessContext(hook_ctx), http_res)
-            
-        
-        
-        
-        if http_res.status_code == 200:
-            if utils.match_content_type(http_res.headers.get('Content-Type') or '', 'application/json'):                
-                out = utils.unmarshal_json(http_res.text, Optional[components.ShippoAccount])
-                return out
-            
-            content_type = http_res.headers.get('Content-Type')
-            raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
-        elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
-            raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
-        else:
-            raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-
```

### Comparing `shippo-3.2.0/src/shippo/tracking_status.py` & `shippo-3.2.2/src/shippo/tracking_status.py`

 * *Files 7% similar despite different names*

```diff
@@ -33,27 +33,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateTrackRequest(
             shippo_api_version=shippo_api_version,
             tracks_request=tracks_request,
         )
         
+        _globals = operations.CreateTrackGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/tracks'
+        url = utils.generate_url(base_url, '/tracks', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateTrackRequest, "tracks_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -103,24 +108,29 @@
         hook_ctx = HookContext(operation_id='GetTrack', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetTrackRequest(
             tracking_number=tracking_number,
             carrier=carrier,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetTrackGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetTrackRequest, base_url, '/tracks/{Carrier}/{TrackingNumber}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/tracks/{Carrier}/{TrackingNumber}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -157,8 +167,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/user_parcel_templates.py` & `shippo-3.2.2/src/shippo/user_parcel_templates.py`

 * *Files 8% similar despite different names*

```diff
@@ -28,24 +28,29 @@
         Returns a list all of all user parcel template objects.
         """
         hook_ctx = HookContext(operation_id='ListUserParcelTemplates', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.ListUserParcelTemplatesRequest(
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.ListUserParcelTemplatesGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/user-parcel-templates'
+        url = utils.generate_url(base_url, '/user-parcel-templates', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -93,27 +98,32 @@
         """
         hook_ctx = HookContext(operation_id='CreateUserParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.CreateUserParcelTemplateRequest(
             shippo_api_version=shippo_api_version,
             user_parcel_template_create_request=user_parcel_template_create_request,
         )
         
+        _globals = operations.CreateUserParcelTemplateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = base_url + '/user-parcel-templates'
+        url = utils.generate_url(base_url, '/user-parcel-templates', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.CreateUserParcelTemplateRequest, "user_parcel_template_create_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('POST', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -155,24 +165,29 @@
         """
         hook_ctx = HookContext(operation_id='DeleteUserParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.DeleteUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.DeleteUserParcelTemplateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.DeleteUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = '*/*'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('DELETE', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -213,24 +228,29 @@
         """
         hook_ctx = HookContext(operation_id='GetUserParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.GetUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
         )
         
+        _globals = operations.GetUserParcelTemplateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.GetUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('GET', url, params=query_params, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -273,27 +293,32 @@
         hook_ctx = HookContext(operation_id='UpdateUserParcelTemplate', oauth2_scopes=[], security_source=self.sdk_configuration.security)
         request = operations.UpdateUserParcelTemplateRequest(
             user_parcel_template_object_id=user_parcel_template_object_id,
             shippo_api_version=shippo_api_version,
             user_parcel_template_update_request=user_parcel_template_update_request,
         )
         
+        _globals = operations.UpdateUserParcelTemplateGlobals(
+            shippo_api_version=self.sdk_configuration.globals.shippo_api_version,
+        )
+        
         base_url = utils.template_url(*self.sdk_configuration.get_server_details())
         
-        url = utils.generate_url(operations.UpdateUserParcelTemplateRequest, base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, self.sdk_configuration.globals)
+        url = utils.generate_url(base_url, '/user-parcel-templates/{UserParcelTemplateObjectId}', request, _globals)
         
         if callable(self.sdk_configuration.security):
             headers, query_params = utils.get_security(self.sdk_configuration.security())
         else:
             headers, query_params = utils.get_security(self.sdk_configuration.security)
         
-        headers = { **utils.get_headers(request, self.sdk_configuration.globals), **headers }
+        headers = { **utils.get_headers(request, _globals), **headers }
         req_content_type, data, form = utils.serialize_request_body(request, operations.UpdateUserParcelTemplateRequest, "user_parcel_template_update_request", False, True, 'json')
         if req_content_type is not None and req_content_type not in ('multipart/form-data', 'multipart/mixed'):
             headers['content-type'] = req_content_type
+        query_params = { **utils.get_query_params(request, _globals), **query_params }
         headers['Accept'] = 'application/json'
         headers['user-agent'] = self.sdk_configuration.user_agent
         client = self.sdk_configuration.client
         
         try:
             req = client.prepare_request(requests_http.Request('PUT', url, params=query_params, data=data, files=form, headers=headers))
             req = self.sdk_configuration.get_hooks().before_request(BeforeRequestContext(hook_ctx), req)
@@ -323,8 +348,9 @@
             content_type = http_res.headers.get('Content-Type')
             raise errors.SDKError(f'unknown content-type received: {content_type}', http_res.status_code, http_res.text, http_res)
         elif http_res.status_code >= 400 and http_res.status_code < 500 or http_res.status_code >= 500 and http_res.status_code < 600:
             raise errors.SDKError('API error occurred', http_res.status_code, http_res.text, http_res)
         else:
             raise errors.SDKError('unknown status code received', http_res.status_code, http_res.text, http_res)
 
-    
+    
+
```

### Comparing `shippo-3.2.0/src/shippo/utils/retries.py` & `shippo-3.2.2/src/shippo/utils/retries.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,11 +110,10 @@
             if now - start > max_elapsed_time:
                 if isinstance(exception, TemporaryError):
                     return exception.response
 
                 raise
             sleep = ((initial_interval/1000) *
                      exponent**retries + random.uniform(0, 1))
-            if sleep > max_interval/1000:
-                sleep = max_interval/1000
+            sleep = min(sleep, max_interval / 1000)
             time.sleep(sleep)
             retries += 1
```

### Comparing `shippo-3.2.0/src/shippo/utils/utils.py` & `shippo-3.2.2/src/shippo/utils/utils.py`

 * *Files 12% similar despite different names*

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
-        kls = getattr(sys.modules['sdk.models.components'], obj[field_name])
+        kls = getattr(sys.modules["sdk.models.components"], obj[field_name])
         return unmarshal_json(json.dumps(obj), kls)
+
     return decode_fx
 
 
 def remove_suffix(input_string, suffix):
     if suffix and input_string.endswith(suffix):
-        return input_string[:-len(suffix)]
+        return input_string[: -len(suffix)]
     return input_string
```

### Comparing `shippo-3.2.0/src/shippo.egg-info/PKG-INFO` & `shippo-3.2.2/src/shippo.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shippo
-Version: 3.2.0
+Version: 3.2.2
 Summary: Python Client SDK Generated by Speakeasy
 Home-page: https://github.com/goshippo/shippo-python-sdk.git
 Author: Shippo
 License: UNKNOWN
 Description: # <img src="https://docs.goshippo.com/images/Logo.png" width="30" alt="Shippo logo"> Shippo Python SDK 
         
         Shippo is a shipping API that connects you with [multiple shipping carriers](https://goshippo.com/carriers) (such as USPS, UPS, DHL, Canada Post, Australia Post, and many others) through one interface.
@@ -64,14 +64,36 @@
         
         http_client = requests.Session()
         http_client.headers.update({'x-custom-header': 'someValue'})
         s = shippo.Shippo(client=http_client)
         ```
         <!-- End Custom HTTP Client [http-client] -->
         
+        ## Debug HTTP Client
+        
+        The Shippo Python SDK returns schema models directly rather than wrapping the response in an envelope along with 
+        additional request/response details (status code, raw json, etc).  However, there are times when the underlying 
+        http information is useful so a 'debug' client is provided.  Using this client, you can retrieve the 
+        `requests.PreparedRequest` and `requests.Response` from the most recent API call.
+        
+        ```python
+        import shippo
+        from shippo.debug import DebugSession
+        
+        debug_session = DebugSession()
+        shippo_sdk = shippo.Shippo(api_key_header="<YOUR_API_KEY_HERE>", client=debug_session)
+        
+        shippo_sdk.addresses.list()
+        
+        # print the previous request http headers
+        print(debug_session.last_request.headers)  
+        # print the previous response status code and raw json
+        print(debug_session.last_response.status_code, debug_session.last_response.text)
+        ```
+        
         ## Documentation
         Review our full guides and references at [https://docs.goshippo.com/](https://docs.goshippo.com/).
         
         <!-- Placeholder for Future Speakeasy SDK Sections -->
         
         <!-- Start Available Resources and Operations [operations] -->
         ## Available Resources and Operations
@@ -93,14 +115,15 @@
         
         ### [carrier_accounts](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md)
         
         * [list](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#list) - List all carrier accounts
         * [create](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#create) - Create a new carrier account
         * [get](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#get) - Retrieve a carrier account
         * [update](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#update) - Update a carrier account
+        * [initiate_oauth2_signin](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#initiate_oauth2_signin) - Connect an existing carrier account using OAuth 2.0
         * [register](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#register) - Add a Shippo carrier account
         * [get_registration_status](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/carrieraccounts/README.md#get_registration_status) - Get Carrier Registration status
         
         ### [customs_declarations](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md)
         
         * [list](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md#list) - List all customs declarations
         * [create](https://github.com/goshippo/shippo-python-sdk/blob/master/docs/sdks/customsdeclarations/README.md#create) - Create a new customs declaration
```

### Comparing `shippo-3.2.0/src/shippo.egg-info/SOURCES.txt` & `shippo-3.2.2/src/shippo.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 src/shippo/__init__.py
 src/shippo/addresses.py
 src/shippo/batches.py
 src/shippo/carrier_accounts.py
 src/shippo/carrier_parcel_templates.py
 src/shippo/customs_declarations.py
 src/shippo/customs_items.py
+src/shippo/debug.py
 src/shippo/manifests.py
 src/shippo/orders.py
 src/shippo/parcels.py
 src/shippo/pickups.py
 src/shippo/rates.py
 src/shippo/rates_at_checkout.py
 src/shippo/refunds.py
@@ -63,14 +64,15 @@
 src/shippo/models/components/carrieraccountpaginatedlist.py
 src/shippo/models/components/carrieraccountposteitalianecreaterequest.py
 src/shippo/models/components/carrieraccountregistrationstatus.py
 src/shippo/models/components/carrieraccountservicelevel.py
 src/shippo/models/components/carrieraccountupscreaterequest.py
 src/shippo/models/components/carrieraccountupscreaterequestparameters.py
 src/shippo/models/components/carrieraccountuspscreaterequest.py
+src/shippo/models/components/carrieraccountwithextrainfo.py
 src/shippo/models/components/carrierparceltemplate.py
 src/shippo/models/components/carriers.py
 src/shippo/models/components/cod.py
 src/shippo/models/components/connectexistingownupsaccountrequest.py
 src/shippo/models/components/customerreference.py
 src/shippo/models/components/customsdeclaration.py
 src/shippo/models/components/customsdeclarationcreaterequest.py
@@ -86,14 +88,15 @@
 src/shippo/models/components/dangerousgoodsobject.py
 src/shippo/models/components/defaultparceltemplate.py
 src/shippo/models/components/defaultparceltemplateupdaterequest.py
 src/shippo/models/components/departmentnumber.py
 src/shippo/models/components/distanceunit.py
 src/shippo/models/components/dryice.py
 src/shippo/models/components/errormessage.py
+src/shippo/models/components/httpmetadata.py
 src/shippo/models/components/instanttransactionrequestbody.py
 src/shippo/models/components/insurance.py
 src/shippo/models/components/invoicenumber.py
 src/shippo/models/components/labelfiletype.py
 src/shippo/models/components/lineitem.py
 src/shippo/models/components/lineitembase.py
 src/shippo/models/components/liverate.py
@@ -154,15 +157,18 @@
 src/shippo/models/components/userparceltemplateupdaterequest.py
 src/shippo/models/components/userparceltemplatewithcarriertemplatecreaterequest.py
 src/shippo/models/components/userparceltemplatewithoutcarriertemplatecreaterequest.py
 src/shippo/models/components/weightunit.py
 src/shippo/models/errors/__init__.py
 src/shippo/models/errors/badrequestwithdetail.py
 src/shippo/models/errors/badrequestwitherror.py
+src/shippo/models/errors/initiateoauth2signin.py
 src/shippo/models/errors/sdkerror.py
+src/shippo/models/internal/__init__.py
+src/shippo/models/internal/globals.py
 src/shippo/models/operations/__init__.py
 src/shippo/models/operations/addshipmentstobatch.py
 src/shippo/models/operations/createaddress.py
 src/shippo/models/operations/createbatch.py
 src/shippo/models/operations/createcarrieraccount.py
 src/shippo/models/operations/createcustomsdeclaration.py
 src/shippo/models/operations/createcustomsitem.py
@@ -195,14 +201,15 @@
 src/shippo/models/operations/getrate.py
 src/shippo/models/operations/getrefund.py
 src/shippo/models/operations/getshipment.py
 src/shippo/models/operations/getshippoaccount.py
 src/shippo/models/operations/gettrack.py
 src/shippo/models/operations/gettransaction.py
 src/shippo/models/operations/getuserparceltemplate.py
+src/shippo/models/operations/initiateoauth2signin.py
 src/shippo/models/operations/listaddresses.py
 src/shippo/models/operations/listcarrieraccounts.py
 src/shippo/models/operations/listcarrierparceltemplates.py
 src/shippo/models/operations/listcustomsdeclarations.py
 src/shippo/models/operations/listcustomsitems.py
 src/shippo/models/operations/listmanifests.py
 src/shippo/models/operations/listorders.py
```

