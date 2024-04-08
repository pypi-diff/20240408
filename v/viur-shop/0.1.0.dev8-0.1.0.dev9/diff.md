# Comparing `tmp/viur-shop-0.1.0.dev8.tar.gz` & `tmp/viur-shop-0.1.0.dev9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "viur-shop-0.1.0.dev8.tar", last modified: Thu Mar 14 00:56:30 2024, max compression
+gzip compressed data, was "viur-shop-0.1.0.dev9.tar", last modified: Mon Mar 25 13:16:11 2024, max compression
```

## Comparing `viur-shop-0.1.0.dev8.tar` & `viur-shop-0.1.0.dev9.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.489757 viur-shop-0.1.0.dev8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.489757 viur-shop-0.1.0.dev8/src/viur/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.489757 viur-shop-0.1.0.dev8/src/viur/shop/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.489757 viur-shop-0.1.0.dev8/src/viur/shop/data/
--rw-r--r--   0 runner    (1001) docker     (127)     1337 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/data/translations.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/globals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.493757 viur-shop-0.1.0.dev8/src/viur/shop/modules/
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/address.py
--rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/discount.py
--rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/discount_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/shipping.py
--rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/shipping_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/modules/vat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.493757 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/amazon_pay.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/paypal_plus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_card.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_ideal.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_paypal.py
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_sofort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.493757 viur-shop-0.1.0.dev8/src/viur/shop/services/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/services/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/services/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/shop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/article.py
--rw-r--r--   0 runner    (1001) docker     (127)     8170 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/cart.py
--rw-r--r--   0 runner    (1001) docker     (127)     3936 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/discount.py
--rw-r--r--   0 runner    (1001) docker     (127)     7370 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/discount_condition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/shipping.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/shipping_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/shipping_precondition.py
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/skeletons/vat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/src/viur/shop/types/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/data.py
--rw-r--r--   0 runner    (1001) docker     (127)    11451 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/dc_scope.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     8267 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/price.py
--rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/types/response.py
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-14 00:56:26.000000 viur-shop-0.1.0.dev8/src/viur/shop/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-14 00:56:30.497757 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-14 00:56:30.000000 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-14 00:56:30.000000 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-14 00:56:30.000000 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-14 00:56:30.000000 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-14 00:56:30.000000 viur-shop-0.1.0.dev8/src/viur_shop.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.807650 viur-shop-0.1.0.dev9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-25 13:16:11.807650 viur-shop-0.1.0.dev9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-03-25 13:16:11.807650 viur-shop-0.1.0.dev9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.795650 viur-shop-0.1.0.dev9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.795650 viur-shop-0.1.0.dev9/src/viur/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.799650 viur-shop-0.1.0.dev9/src/viur/shop/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.799650 viur-shop-0.1.0.dev9/src/viur/shop/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    25925 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/data/translations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/globals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.799650 viur-shop-0.1.0.dev9/src/viur/shop/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1659 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2187 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12861 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20444 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8921 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/discount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7119 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/discount_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13034 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/shipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      389 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/shipping_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      363 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/modules/vat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.803650 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/amazon_pay.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/paypal_plus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8360 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_card.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_ideal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_paypal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_sofort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.803650 viur-shop-0.1.0.dev9/src/viur/shop/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/services/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/services/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5931 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/shop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.803650 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1905 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/article.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7399 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/cart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/discount.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6596 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/discount_condition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2198 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/shipping.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/shipping_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/shipping_precondition.py
+-rw-r--r--   0 runner    (1001) docker     (127)      549 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/skeletons/vat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.803650 viur-shop-0.1.0.dev9/src/viur/shop/types/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11552 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/dc_scope.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1502 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8025 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/price.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1684 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/types/response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-03-25 13:16:06.000000 viur-shop-0.1.0.dev9/src/viur/shop/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-25 13:16:11.807650 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-03-25 13:16:11.000000 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1889 2024-03-25 13:16:11.000000 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-25 13:16:11.000000 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-25 13:16:11.000000 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2024-03-25 13:16:11.000000 viur-shop-0.1.0.dev9/src/viur_shop.egg-info/top_level.txt
```

### Comparing `viur-shop-0.1.0.dev8/LICENSE` & `viur-shop-0.1.0.dev9/LICENSE`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/PKG-INFO` & `viur-shop-0.1.0.dev9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-shop
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A ViUR-shop
 Home-page: https://github.com/viur-framework/viur-shop
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Development Status :: 1 - Planning
@@ -13,25 +13,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: viur-toolkit>=0.1.0.dev3
+Requires-Dist: viur-toolkit>=0.1.0.dev4
 Provides-Extra: unzer
 Requires-Dist: unzer~=1.0.0.dev4; extra == "unzer"
 
 <div align="center">
     <h1>viur-shop (WIP)</h1>
     <a href="https://pypi.org/project/viur-shop/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-shop">
     </a>
-    <a href="https://www.npmjs.com/package/@viur/viur-shop-client">
-        <img alt="Badge showing current NPM version" title="PyPI" src="https://img.shields.io/npm/v/@viur/viur-shop-client">
-    </a>
     <a href="LICENSE">
         <img src="https://img.shields.io/github/license/viur-framework/viur-shop" alt="Badge displaying the license" title="License badge">
     </a>
     <br>
     On the way to becoming a <a href="https://www.viur.dev">ViUR</a> shop plugin.
 </div>
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: viur-shop Version: 0.1.0.dev8 Summary: A ViUR-shop
+Metadata-Version: 2.1 Name: viur-shop Version: 0.1.0.dev9 Summary: A ViUR-shop
 Home-page: https://github.com/viur-framework/viur-shop Author: Sven Eberth
 Author-email: se@mausbrand.de Maintainer: Sven Eberth Maintainer-email:
 se@mausbrand.de Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: viur-toolkit>=0.1.0.dev3 Provides-Extra: unzer Requires-
+LICENSE Requires-Dist: viur-toolkit>=0.1.0.dev4 Provides-Extra: unzer Requires-
 Dist: unzer~=1.0.0.dev4; extra == "unzer"
                          ************ vviiuurr--sshhoopp ((WWIIPP)) ************
- _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _N_P_M_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e
-                            _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
+      _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
                   On the way to becoming a _V_i_U_R shop plugin.
```

### Comparing `viur-shop-0.1.0.dev8/setup.cfg` & `viur-shop-0.1.0.dev9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 	Topic :: Software Development :: Libraries :: Python Modules
 
 [options]
 python_requires = >=3.10
 package_dir = 
 	= src
 install_requires = 
-	viur-toolkit>=0.1.0.dev3
+	viur-toolkit>=0.1.0.dev4
 
 [options.extras_require]
 unzer = unzer~=1.0.0.dev4
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/abstract.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/abstract.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/address.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/address.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,29 @@
 import typing as t
 
 from viur.core import current, db
 from viur.core.prototypes import List
+from viur.core.prototypes.skelmodule import DEFAULT_ORDER_TYPE
 from viur.core.skeleton import SkeletonInstance
 from .abstract import ShopModuleAbstract
 from ..globals import SHOP_LOGGER
+from viur.core.prototypes.skelmodule import ORDER_TYPE
 
 logger = SHOP_LOGGER.getChild(__name__)
 
 
 class Address(ShopModuleAbstract, List):
     kindName = "shop_address"
 
+    default_order: DEFAULT_ORDER_TYPE = (  #
+        # TODO: https://github.com/viur-framework/viur-core/pull/1109
+        ("firstname", db.SortOrder.Ascending)  # ,
+        # ("lastname", db.SortOrder.Ascending),
+    )
+
     def adminInfo(self) -> dict:
         admin_info = super().adminInfo()
         admin_info["icon"] = "person-vcard"
         return admin_info
 
     def canAdd(self) -> bool:
         return True
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/api.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/api.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/cart.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/cart.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/discount.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/discount.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/discount_condition.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/discount_condition.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/modules/order.py` & `viur-shop-0.1.0.dev9/src/viur/shop/modules/order.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/abstract.py` & `viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/abstract.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import abc
 import typing as t
 
-from viur.core import Module
+from viur.core import Module, translate
 from viur.core.prototypes.instanced_module import InstancedModule
 from viur.core.skeleton import SkeletonInstance
 from ..types import ClientError
 
 if t.TYPE_CHECKING:
     from ..shop import Shop
 
@@ -16,17 +16,22 @@
 
 class PaymentProviderAbstract(InstancedModule, Module, abc.ABC):
     shop: "Shop" = None
 
     @property
     @abc.abstractmethod
     def name(self) -> str:
-        """Define the name of the payment provider"""
+        """Define the internal name of the payment provider"""
         ...
 
+    @property
+    def title(self) -> translate:
+        """Define the external title of the payment provider"""
+        return translate(f"viur.shop.payment_provider.{self.name}", self.name)
+
     def can_checkout(
         self,
         order_skel: SkeletonInstance,
     ) -> list[ClientError]:
         """Check if a checkout process can be started
 
         An empty list means not error,
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/amazon_pay.py` & `viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/amazon_pay.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/paypal_plus.py` & `viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/paypal_plus.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/payment_providers/unzer_abstract.py` & `viur-shop-0.1.0.dev9/src/viur/shop/payment_providers/unzer_abstract.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/services/events.py` & `viur-shop-0.1.0.dev9/src/viur/shop/services/events.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/services/hooks.py` & `viur-shop-0.1.0.dev9/src/viur/shop/services/hooks.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/shop.py` & `viur-shop-0.1.0.dev9/src/viur/shop/shop.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/address.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/address.py`

 * *Files 23% similar despite different names*

```diff
@@ -8,74 +8,67 @@
 
 
 # TODO: should these bones required or will this be handled in a editSkel?
 
 class AddressSkel(Skeleton):  # STATE: Complete (as in model)
     kindName = "shop_address"
 
+    name = StringBone(
+        descr="Name",
+        compute=Compute(
+            lambda skel: f'{skel["salutation"]} {skel["firstname"]} {skel["lastname"]}'.strip(),
+            ComputeInterval(ComputeMethod.OnWrite),
+        )
+    )
+
     customer_type = SelectBone(
-        descr="customer_type",
         values=CustomerType,
     )
 
     salutation = SelectBone(
-        descr="salutation",
         values=Salutation,
     )
 
     company_name = StringBone(
-        descr="company_name",
     )
 
     firstname = StringBone(
-        descr="firstname",
     )
 
     lastname = StringBone(
-        descr="lastname",
     )
 
     street_name = StringBone(
-        descr="street_name",
     )
 
     street_number = StringBone(
-        descr="street_number",
     )
 
     address_addition = StringBone(
-        descr="address_addition",
     )
 
     zip_code = StringBone(
-        descr="zip_code",
     )
 
     city = StringBone(
-        descr="city",
     )
 
     country = SelectCountryBone(
-        descr="country",
     )
 
     customer = RelationalBone(
-        descr="customer",
         kind="user",
     )
 
     is_default = BooleanBone(
-        descr="is_default",
     )
 
     address_type = SelectBone(
-        descr="address_type",
         values=AddressType,
     )
 
     cloned_from = RelationalBone(
-        descr="cloned_from",
         kind="shop_address",
-        module="shop.address",
+        module="shop/address",
         readOnly=True,  # set by the system
         consistency=RelationalConsistency.Ignore,
     )
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/article.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/article.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,77 +14,76 @@
 
     All members in this abstract skeleton has to be prefixed with `shop_` to
     avoid name collisions with bones in the project skeleton
     """
 
     @property
     @abc.abstractmethod
-    def shop_name(self):
+    def shop_name(self) -> StringBone | TextBone:
         """Name of the article in the shop"""
         ...
 
     @property
     @abc.abstractmethod
-    def shop_description(self):
+    def shop_description(self) -> TextBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_price_retail(self):
+    def shop_price_retail(self) -> NumericBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_price_recommended(self):
+    def shop_price_recommended(self) -> NumericBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_availability(self):
+    def shop_availability(self) -> SelectBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_listed(self) -> bool:
+    def shop_listed(self) -> BooleanBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_image(self):
+    def shop_image(self) -> FileBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_art_no_or_gtin(self):
+    def shop_art_no_or_gtin(self) -> StringBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_vat(self):
+    def shop_vat(self) -> RelationalBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_shipping(self):
+    def shop_shipping(self) -> RelationalBone:
         ...
 
     @property
     @abc.abstractmethod
-    def shop_is_weee(self) -> bool:
+    def shop_is_weee(self) -> BooleanBone:
         """Waste Electrical and Electronic Equipment Directive (WEEE Directive)"""
         ...
 
     @property
     @abc.abstractmethod
-    def shop_is_low_price(self) -> bool:
+    def shop_is_low_price(self) -> BooleanBone:
         """shop_price_retail != shop_price_recommended"""
         ...
 
     @property
     def shop_price_(self) -> Price:
         return Price.get_or_create(self)
 
     shop_price = RawBone(  # FIXME: JsonBone doesn't work (https://github.com/viur-framework/viur-core/issues/1092)
-        descr="price",
         compute=Compute(lambda skel: skel.shop_price_.to_dict(), ComputeInterval(ComputeMethod.Always))
     )
     shop_price.type = JsonBone.type
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/cart.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/cart.py`

 * *Files 11% similar despite different names*

```diff
@@ -75,101 +75,89 @@
     ]
 
 
 class CartNodeSkel(TreeSkel):  # STATE: Complete (as in model)
     kindName = "shop_cart_node"
 
     is_root_node = BooleanBone(
-        descr="Is root node?",
         readOnly=True,
     )
 
     total = NumericBone(
-        descr="Total",
         precision=2,
         compute=Compute(
             TotalFactory("total", lambda child: child.price_.current, True),
             ComputeInterval(ComputeMethod.Always),
         ),
     )
 
     vat_total = NumericBone(
-        descr="Total",
         precision=2,
         compute=Compute(
             TotalFactory("vat_total", lambda child: child.price_.vat_value, True),
             ComputeInterval(ComputeMethod.Always),
         ),
     )
 
     vat_rate = RelationalBone(
-        descr="Vat Rate",
         kind="shop_vat",
         module="shop/vat",
         compute=Compute(get_vat_rate_for_node, ComputeInterval(ComputeMethod.Always)),
         refKeys=["key", "name", "rate"],
         multiple=True,
     )
 
     total_quantity = NumericBone(
-        descr="Total quantity",
         precision=0,
         compute=Compute(
             TotalFactory("total_quantity", lambda child: 1, True),
             ComputeInterval(ComputeMethod.Always)
         ),
         defaultValue=0,
     )
 
     shipping_address = RelationalBone(
-        descr="shipping_address",
         kind="shop_address",
         module="shop/shop_address",
         refKeys=[
             "key", "name", "customer_type", "salutation", "company_name",
             "firstname", "lastname", "street_name", "street_number",
             "address_addition", "zip_code", "city", "country",
             "is_default", "address_type",
         ],
     )
 
     customer_comment = TextBone(
-        descr="customer_comment",
         validHtml=None,
     )
 
     name = StringBone(
-        descr="name",
     )
 
     cart_type = SelectBone(
-        descr="cart_type",
         values=CartType,
     )
 
     shipping = RelationalBone(
-        descr="shipping",
         kind="shop_shipping",
         module="shop/shipping",
     )
     """Versand bei Warenkorb der einer Bestellung zugehört"""
 
     discount = RelationalBone(
-        descr="discount",
         kind="shop_discount",
         module="shop/discount",
         refKeys=["key", "name", "discount_type", "absolute", "percentage"],
     )
 
 
 class CartItemSkel(TreeSkel):  # STATE: Complete (as in model)
     kindName = "shop_cart_leaf"
 
     article = RelationalBone(
-        descr="article",
         kind="...",  # will be set in Shop._set_kind_names()
         # FIXME: What's necessary here?
         parentKeys=["key", "parententry", "article"],
         refKeys=[
             "shop_name", "shop_description",
             "shop_price_retail", "shop_price_recommended",
             "shop_availability", "shop_listed",
@@ -178,79 +166,65 @@
             "shop_is_weee", "shop_is_low_price",
             "shop_price_current",
         ],
         consistency=RelationalConsistency.CascadeDeletion,
     )
 
     quantity = NumericBone(
-        descr="quantity",
         min=0,
         defaultValue=0,
     )
 
     project_data = JsonBone(
-        descr="Custom project data",
     )
 
     # --- Bones to store a frozen copy of the article values: -----------------
 
     shop_name = StringBone(
-        descr="shop_name",
     )
 
     shop_description = TextBone(
-        descr="shop_description",
     )
 
     shop_price_retail = NumericBone(
-        descr="Verkaufspreis",
     )
 
     shop_price_recommended = NumericBone(
-        descr="UVP",
     )
 
     shop_availability = SelectBone(
-        descr="shop_availability",
         values=ArticleAvailability,
     )
 
     shop_listed = BooleanBone(
-        descr="shop_listed",
     )
 
     shop_image = FileBone(
-        descr="Produktbild",
     )
 
     shop_art_no_or_gtin = StringBone(
-        descr="Artikelnummer",
     )
 
     shop_vat = RelationalBone(
-        descr="Steuersatz",
         kind="shop_vat",
-        module="shop.vat",
+        module="shop/vat",
         refKeys=["key", "name", "rate"],
         consistency=RelationalConsistency.PreventDeletion,
     )
 
     shop_shipping = RelationalBone(
-        descr="Versandkosten",
         kind="shop_shipping_config",
-        module="shop.shipping_config",
+        module="shop/shipping_config",
         consistency=RelationalConsistency.SetNull,
     )
 
     shop_is_weee = BooleanBone(
-        descr="Elektro",
     )
 
     shop_is_low_price = BooleanBone(
-        descr="shop_is_low_price",
     )
 
     @property
     def article_skel(self):
         return self["article"]["dest"]
 
     @property
@@ -268,15 +242,14 @@
         return skel
 
     @property
     def price_(self) -> Price:
         return Price.get_or_create(self)
 
     price = RawBone(  # FIXME: JsonBone doesn't work (https://github.com/viur-framework/viur-core/issues/1092)
-        descr="price",
         compute=Compute(lambda skel: skel.price_.to_dict(), ComputeInterval(ComputeMethod.Always))
     )
     price.type = JsonBone.type
 
     @classmethod
     def toDB(cls, skelValues: SkeletonInstance, update_relations: bool = True, **kwargs) -> db.Key:
         return super().toDB(skelValues, update_relations, **kwargs)
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/discount_condition.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/discount_condition.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             )]
             if skel["code_type"] == CodeType.INDIVIDUAL and not skel["individual_codes_prefix"]
             else []
         ),
     ]
 
     name = StringBone(
-        descr="name",
         compute=Compute(
             fn=lambda skel: str({
                 key: "..." if key == "scope_article" else (value.isoformat() if isinstance(value, dt) else value)
                 for key, value in skel.items(True)
                 if value and value != getattr(skel, key).defaultValue and key not in dir(Skeleton)
             }),
             interval=ComputeInterval(
@@ -52,213 +51,190 @@
         ),
         params={
             "category": "1 – General",
         },
     )
 
     description = TextBone(
-        descr="description",
         validHtml=None,
         params={
             "category": "1 – General",
         },
     )
 
     code_type = SelectBone(
-        descr="code_type",
         required=True,
         values=CodeType,
         defaultValue=CodeType.NONE,
         params={
             "category": "1 – General",
         },
     )
 
     application_domain = SelectBone(
-        descr="application_domain",
         required=True,
         values=ApplicationDomain,
         defaultValue=ApplicationDomain.ALL,
         params={
             "category": "1 – General",
         },
     )
     """Anwendungsbereich"""
 
     quantity_volume = NumericBone(
-        descr="quantity_volume",
         required=True,
         defaultValue=-1,  # Unlimited
         min=-1,
         getEmptyValueFunc=lambda: None,
         params={
             "category": "1 – General",
             "tooltip": "-1 ^= unlimited",
         },
     )
 
     quantity_used = NumericBone(
-        descr="quantity_used",
         defaultValue=0,
         min=0,
         params={
             "category": "1 – General",
         },
     )
     """Wie oft wurde der code Bereits verwendet?"""
 
     individual_codes_amount = NumericBone(
-        descr="individual_codes_amount",
         min=1,
         params={
             "category": "1 – General",
             "visibleIf": 'code_type == "individual"'
         },
         defaultValue=0,
     )
 
     scope_code = StringBone(
-        descr="code",
         # TODO: limit charset
         params={
             "category": "2 – Scope",
             "visibleIf": 'code_type == "universal"'
         },
         unique=UniqueValue(UniqueLockMethod.SameValue, False, "Code exist already"),  # TODO
     )
 
     individual_codes_prefix = StringBone(
-        descr="individual_codes_prefix",
         # TODO: limit charset
         params={
             "category": "2 – Scope",
             "visibleIf": 'code_type == "individual"'
         },
         unique=UniqueValue(UniqueLockMethod.SameValue, False, "Value already taken"),
     )
 
     scope_minimum_order_value = NumericBone(
-        descr="scope_minimum_order_value",
         required=True,
         min=0,
         defaultValue=0,
         getEmptyValueFunc=lambda: None,
         # TODO: UnitBone / CurrencyBone
         params={
             "category": "2 – Scope",
         },
     )
 
     scope_date_start = DateBone(
-        descr="scope_date_start",
         params={
             "category": "2 – Scope",
         },
     )
 
     scope_date_end = DateBone(
-        descr="scope_date_end",
         params={
             "category": "2 – Scope",
         },
     )
 
     scope_language = SelectBone(
-        descr="scope_language",
         values=conf.i18n.available_languages,
         params={
             "category": "2 – Scope",
         },
         # TODO: multiple=True, ???
     )
 
     scope_country = SelectCountryBone(
-        descr="scope_country",
         params={
             "category": "2 – Scope",
         },
         # TODO: multiple=True, ???
     )
 
     scope_minimum_quantity = NumericBone(
-        descr="scope_minimum_quantity",
         required=True,
         min=0,
         defaultValue=0,
         getEmptyValueFunc=lambda: None,
         params={
             "category": "2 – Scope",
         },
     )
     """Minimale Anzahl
 
     für Staffelrabatte (in Kombination mit application_domain) für Artikel oder kompletten Warenkorb"""
 
     scope_customer_group = SelectBone(
-        descr="scope_customer_group",
         required=True,
         values=CustomerGroup,
         defaultValue=CustomerGroup.ALL,
         params={
             "category": "2 – Scope",
         },
     )
 
     scope_combinable_other_discount = BooleanBone(
-        descr="scope_combinable_other_discount",
         params={
             "category": "2 – Scope",
         },
     )
     """Kombinierbar mit anderen Rabatten"""
 
     scope_combinable_low_price = BooleanBone(
-        descr="scope_combinable_low_price",
         params={
             "category": "2 – Scope",
         },
     )
     """Kombinierbar
 
     prüfen mit shop_is_low_price"""
 
     scope_article = RelationalBone(
-        descr="scope_article",
         kind="...",  # will be set in Shop._set_kind_names()
         consistency=RelationalConsistency.PreventDeletion,
         params={
             "category": "2 – Scope",
             "visibleIf": 'application_domain == "article"'
         },
         refKeys=["name", "shop_name", "shop_*"],
         format="$(dest.shop_name) | $(dest.shop_shop_art_no_or_gtin) | $(dest.shop_price_retail) €",
     )
 
     is_subcode = BooleanBone(
-        descr="is_subcode",
         compute=Compute(
             fn=lambda skel: skel["parent_code"] is not None,
             interval=ComputeInterval(
                 method=ComputeMethod.OnWrite,
             ),
         ),
         params={
             "category": "2 – Scope",
             "visibleIf": 'code_type == "individual"'
         },
         readOnly=True,
     )
 
     parent_code = RelationalBone(
-        descr="parent_code",
         kind="shop_discount_condition",
-        module="shop.discount_condition",
+        module="shop/discount_condition",
         consistency=RelationalConsistency.PreventDeletion,
         params={
             "category": "2 – Scope",
             "visibleIf": 'code_type == "individual"'
         },
         readOnly=True,
     )
-
-
-print(f"{DiscountConditionSkel.scope_article.refKeys = }")
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/shipping_config.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/shipping_config.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,17 +8,15 @@
 logger = SHOP_LOGGER.getChild(__name__)
 
 
 class ShippingConfigSkel(Skeleton):  # STATE: Complete (as in model)
     kindName = "shop_shipping_config"
 
     name = StringBone(
-        descr="name",
     )
 
     shipping_skel = RelationalBone(
-        descr="shipping_skel",
         kind="shop_shipping",
-        module="shop.shipping",
+        module="shop/shipping",
         using=ShippingPreconditionRelSkel,
         multiple=True,
     )
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/skeletons/vat.py` & `viur-shop-0.1.0.dev9/src/viur/shop/skeletons/vat.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,19 +9,17 @@
 
 class VatSkel(Skeleton):  # STATE: Complete (as in model)
     kindName = "shop_vat"
 
     # TODO: add descr bone?!
 
     name = StringBone(
-        descr="name",
         compute=Compute(lambda skel: f'{skel["rate"]} %')
     )
 
     rate = NumericBone(
-        descr="rate",
         required=True,
         precision=2,
         min=0,
         getEmptyValueFunc=lambda: None,
         # TODO: UnitBone / PercentageBone
     )
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/__init__.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/__init__.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/dc_scope.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/dc_scope.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,14 +131,15 @@
 
         # We need the full skel with all bones (otherwise the refSkel would be to large)
         condition_skel_cls: t.Type[Skeleton] = skeletonByKind(discount_skel.condition.kind)
         for condition in discount_skel["condition"]:
             condition_skel: SkeletonInstance = condition_skel_cls()  # noqa
             if not condition_skel.fromDB(condition["dest"]["key"]):
                 logger.warning(f'Broken relation {condition=} in {discount_skel["key"]}?!')
+                raise InvalidStateError(f'Broken relation {condition=} in {discount_skel["key"]}?!')
                 self.condition_skels.append(None)  # TODO
                 self.condition_validator_instances.append(None)  # TODO
                 continue
             cv = ConditionValidator()(cart_skel=cart_skel, discount_skel=discount_skel, condition_skel=condition_skel,
                                       code=code)
             self.condition_skels.append(condition_skel)
             self.condition_validator_instances.append(cv)
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/enums.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/enums.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/exceptions.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/exceptions.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/price.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/price.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import functools
 import typing as t  # noqa
 
 from viur import toolkit
-from viur.core import current
+from viur.core import current, utils
 from viur.core.skeleton import SkeletonInstance
 from .enums import ConditionOperator, DiscountType
 from ..globals import SHOP_INSTANCE, SHOP_LOGGER
 
 logger = SHOP_LOGGER.getChild(__name__)
 
 
@@ -81,15 +81,15 @@
         best_discount = None
         article_price = self.retail or 0.0  # FIXME: how to handle None prices?
         if not article_price:
             return None
         for skel in SHOP_INSTANCE.get().discount.current_automatically_discounts:
             # TODO: if can apply (article range, lang, ...)
             price = self.apply_discount(skel, article_price)
-            if best_discount is None or price < best_discount[1]:
+            if best_discount is None or price < best_discount[0]:
                 best_discount = price, skel
         return best_discount
 
     def choose_best_discount_set(self) -> tuple[float, list[SkeletonInstance]]:
         """
         Find the best set of applyable discounts for this article.
 
@@ -142,34 +142,23 @@
 
     @property
     def vat_value(self) -> float:
         """Calculate the vat value based on current price and vat rate"""
         return toolkit.round_decimal(self.vat_rate * self.current, 2)
 
     def to_dict(self):
-        _current = self.current
-
+        from viur.shop.types import ExtendedCustomJsonEncoder
         return {
             attr_name: getattr(self, attr_name)
             for attr_name, attr_value in vars(self.__class__).items()
             if isinstance(attr_value, (property, functools.cached_property))
-        } | {  # TODO: must be JSON serializable for vi renderer
-            # "cart_discounts": self.cart_discounts,
-            # "article_discount": self.article_discount,
-        }
-
-        return {
-            "retail": self.retail,
-            "recommended": self.recommended,
-            "current": _current,
-            "saved": self.saved,
-            "saved_percentage": self.saved_percentage,
+        } | utils.json.loads(utils.json.dumps({  # must be JSON serializable for vi renderer
             "cart_discounts": self.cart_discounts,
             "article_discount": self.article_discount,
-        }
+        }, cls=ExtendedCustomJsonEncoder))
 
     @staticmethod
     def apply_discount(
         discount_skel: SkeletonInstance,
         article_price: float
     ):
         """Apply a given discount on the given price and return the new price"""
```

### Comparing `viur-shop-0.1.0.dev8/src/viur/shop/types/response.py` & `viur-shop-0.1.0.dev9/src/viur/shop/types/response.py`

 * *Files identical despite different names*

### Comparing `viur-shop-0.1.0.dev8/src/viur_shop.egg-info/PKG-INFO` & `viur-shop-0.1.0.dev9/src/viur_shop.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: viur-shop
-Version: 0.1.0.dev8
+Version: 0.1.0.dev9
 Summary: A ViUR-shop
 Home-page: https://github.com/viur-framework/viur-shop
 Author: Sven Eberth
 Author-email: se@mausbrand.de
 Maintainer: Sven Eberth
 Maintainer-email: se@mausbrand.de
 Classifier: Development Status :: 1 - Planning
@@ -13,25 +13,22 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: viur-toolkit>=0.1.0.dev3
+Requires-Dist: viur-toolkit>=0.1.0.dev4
 Provides-Extra: unzer
 Requires-Dist: unzer~=1.0.0.dev4; extra == "unzer"
 
 <div align="center">
     <h1>viur-shop (WIP)</h1>
     <a href="https://pypi.org/project/viur-shop/">
         <img alt="Badge showing current PyPI version" title="PyPI" src="https://img.shields.io/pypi/v/viur-shop">
     </a>
-    <a href="https://www.npmjs.com/package/@viur/viur-shop-client">
-        <img alt="Badge showing current NPM version" title="PyPI" src="https://img.shields.io/npm/v/@viur/viur-shop-client">
-    </a>
     <a href="LICENSE">
         <img src="https://img.shields.io/github/license/viur-framework/viur-shop" alt="Badge displaying the license" title="License badge">
     </a>
     <br>
     On the way to becoming a <a href="https://www.viur.dev">ViUR</a> shop plugin.
 </div>
```

#### html2text {}

```diff
@@ -1,15 +1,14 @@
-Metadata-Version: 2.1 Name: viur-shop Version: 0.1.0.dev8 Summary: A ViUR-shop
+Metadata-Version: 2.1 Name: viur-shop Version: 0.1.0.dev9 Summary: A ViUR-shop
 Home-page: https://github.com/viur-framework/viur-shop Author: Sven Eberth
 Author-email: se@mausbrand.de Maintainer: Sven Eberth Maintainer-email:
 se@mausbrand.de Classifier: Development Status :: 1 - Planning Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.10 Description-Content-Type: text/markdown License-File:
-LICENSE Requires-Dist: viur-toolkit>=0.1.0.dev3 Provides-Extra: unzer Requires-
+LICENSE Requires-Dist: viur-toolkit>=0.1.0.dev4 Provides-Extra: unzer Requires-
 Dist: unzer~=1.0.0.dev4; extra == "unzer"
                          ************ vviiuurr--sshhoopp ((WWIIPP)) ************
- _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _N_P_M_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e
-                            _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
+      _[_B_a_d_g_e_ _s_h_o_w_i_n_g_ _c_u_r_r_e_n_t_ _P_y_P_I_ _v_e_r_s_i_o_n_]_[_B_a_d_g_e_ _d_i_s_p_l_a_y_i_n_g_ _t_h_e_ _l_i_c_e_n_s_e_]
                   On the way to becoming a _V_i_U_R shop plugin.
```

### Comparing `viur-shop-0.1.0.dev8/src/viur_shop.egg-info/SOURCES.txt` & `viur-shop-0.1.0.dev9/src/viur_shop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

